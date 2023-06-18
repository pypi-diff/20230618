# Comparing `tmp/pycargoebuild-0.6.3.tar.gz` & `tmp/pycargoebuild-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycargoebuild-0.6.3.tar", last modified: Sun Apr  2 19:08:14 2023, max compression
+gzip compressed data, was "pycargoebuild-0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pycargoebuild-0.6.3.tar` & `pycargoebuild-0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1081 2022-11-09 09:31:36.847189 pycargoebuild-0.6.3/LICENSE
--rw-r--r--   0        0        0     2304 2022-12-11 16:55:26.062005 pycargoebuild-0.6.3/README.rst
--rw-r--r--   0        0        0       82 2023-04-02 18:56:53.659562 pycargoebuild-0.6.3/pycargoebuild/__init__.py
--rw-r--r--   0        0        0     8502 2023-02-06 04:04:07.821645 pycargoebuild-0.6.3/pycargoebuild/__main__.py
--rw-r--r--   0        0        0     3159 2023-02-06 04:03:59.321434 pycargoebuild-0.6.3/pycargoebuild/cargo.py
--rw-r--r--   0        0        0     6727 2023-04-02 18:47:07.951678 pycargoebuild-0.6.3/pycargoebuild/ebuild.py
--rw-r--r--   0        0        0     2272 2023-02-06 04:03:59.321434 pycargoebuild-0.6.3/pycargoebuild/fetch.py
--rw-r--r--   0        0        0     4645 2022-11-25 16:23:06.667384 pycargoebuild-0.6.3/pycargoebuild/format.py
--rw-r--r--   0        0        0     3541 2022-11-22 19:20:48.996065 pycargoebuild-0.6.3/pycargoebuild/license.py
--rw-r--r--   0        0        0     1126 2022-11-13 11:10:20.163896 pycargoebuild-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 pycargoebuild-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-11-09 09:31:36.847189 pycargoebuild-0.7/LICENSE
+-rw-r--r--   0        0        0     2304 2022-12-11 16:55:26.062005 pycargoebuild-0.7/README.rst
+-rw-r--r--   0        0        0       80 2023-06-18 14:57:52.100741 pycargoebuild-0.7/pycargoebuild/__init__.py
+-rw-r--r--   0        0        0     8525 2023-06-18 14:25:48.715463 pycargoebuild-0.7/pycargoebuild/__main__.py
+-rw-r--r--   0        0        0     3253 2023-06-18 14:37:33.218459 pycargoebuild-0.7/pycargoebuild/cargo.py
+-rw-r--r--   0        0        0     6899 2023-06-18 14:43:47.326364 pycargoebuild-0.7/pycargoebuild/ebuild.py
+-rw-r--r--   0        0        0     2272 2023-02-06 04:03:59.321434 pycargoebuild-0.7/pycargoebuild/fetch.py
+-rw-r--r--   0        0        0     4645 2022-11-25 16:23:06.667384 pycargoebuild-0.7/pycargoebuild/format.py
+-rw-r--r--   0        0        0     3541 2022-11-22 19:20:48.996065 pycargoebuild-0.7/pycargoebuild/license.py
+-rw-r--r--   0        0        0     1126 2022-11-13 11:10:20.163896 pycargoebuild-0.7/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 pycargoebuild-0.7/PKG-INFO
```

### Comparing `pycargoebuild-0.6.3/LICENSE` & `pycargoebuild-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.6.3/README.rst` & `pycargoebuild-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.6.3/pycargoebuild/__main__.py` & `pycargoebuild-0.7/pycargoebuild/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,27 +150,28 @@
         if not args.force and outfile.exists():
             print(f"{outfile} exists already, pass -f to overwrite it",
                   file=sys.stderr)
             return 1
 
     fetch_crates(crates)
     verify_crates(crates, distdir=args.distdir)
-    crate_files = [args.distdir / crate.filename for crate in crates]
 
     if args.input is not None:
         ebuild = update_ebuild(args.input.read(),
                                pkg_meta,
-                               crate_files,
+                               crates,
+                               distdir=args.distdir,
                                crate_license=not args.no_license)
         logging.warning(
             "The in-place mode updates CRATES and crate LICENSE+= variables "
             "only, other metadata is left unchanged")
     else:
         ebuild = get_ebuild(pkg_meta,
-                            crate_files,
+                            crates,
+                            distdir=args.distdir,
                             crate_license=not args.no_license)
 
     try:
         with tempfile.NamedTemporaryFile(mode="w",
                                          encoding="utf-8",
                                          dir=outfile.parent,
                                          delete=False) as outf:
```

### Comparing `pycargoebuild-0.6.3/pycargoebuild/cargo.py` & `pycargoebuild-0.7/pycargoebuild/cargo.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
         return f"{self.name}-{self.version}.crate"
 
     @property
     def crates_io_url(self) -> str:
         return (f"https://crates.io/api/v1/crates/{self.name}/{self.version}/"
                 "download")
 
+    @property
+    def crate_entry(self) -> str:
+        return f"{self.name}@{self.version}"
+
 
 class PackageMetadata(typing.NamedTuple):
     name: str
     version: str
     license: typing.Optional[str] = None
     license_file: typing.Optional[str] = None
     description: typing.Optional[str] = None
```

### Comparing `pycargoebuild-0.6.3/pycargoebuild/ebuild.py` & `pycargoebuild-0.7/pycargoebuild/ebuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from functools import partial
 from pathlib import Path
 
 import license_expression
 
 from pycargoebuild import __version__
-from pycargoebuild.cargo import PackageMetadata, get_package_metadata
+from pycargoebuild.cargo import Crate, PackageMetadata, get_package_metadata
 from pycargoebuild.format import format_license_var
 from pycargoebuild.license import spdx_to_ebuild
 
 
 EBUILD_TEMPLATE_START = """\
 # Copyright {year} Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
@@ -27,15 +27,15 @@
 CRATES="{crates}"
 
 inherit cargo
 
 DESCRIPTION="{description}"
 HOMEPAGE="{homepage}"
 SRC_URI="
-\t$(cargo_crate_uris)
+\t${{CARGO_CRATE_URIS}}
 "
 
 LICENSE="{pkg_license}"
 """
 
 EBUILD_TEMPLATE_CRATE_LICENSE = """\
 # Dependent crate licenses
@@ -44,22 +44,22 @@
 
 EBUILD_TEMPLATE_END = """\
 SLOT="0"
 KEYWORDS="~amd64"
 """
 
 
-def get_CRATES(crate_files: typing.Iterable[Path]) -> str:
+def get_CRATES(crates: typing.Iterable[Crate]) -> str:
     """
     Return the value of CRATES for the given crate list
     """
-    if not crate_files:
+    if not crates:
         return ""
     return ("\n" +
-            "\n".join(f"\t{p.name[:-6]}" for p in sorted(crate_files)) +
+            "\n".join(sorted(f"\t{c.crate_entry}" for c in crates)) +
             "\n")
 
 
 def get_package_LICENSE(pkg_meta: PackageMetadata) -> str:
     """
     Get the value of package's LICENSE string
     """
@@ -140,29 +140,31 @@
 def url_dquote_escape(value: str) -> str:
     """URL-encode whitespace and special chars to use in bash double-quotes"""
     return DQUOTE_SPECIAL_PLUS_WS_RE.sub(
         lambda x: urllib.parse.quote_plus(x.group(0)), value)
 
 
 def get_ebuild(pkg_meta: PackageMetadata,
-               crate_files: typing.Iterable[Path],
+               crates: typing.Iterable[Crate],
+               distdir: Path,
                *,
                crate_license: bool = True,
                ) -> str:
     """
     Get ebuild contents for passed contents of Cargo.toml and Cargo.lock.
     """
 
     template = EBUILD_TEMPLATE_START
     if crate_license:
         template += EBUILD_TEMPLATE_CRATE_LICENSE
     template += EBUILD_TEMPLATE_END
 
+    crate_files = [distdir / crate.filename for crate in crates]
     return template.format(
-        crates=get_CRATES(crate_files),
+        crates=get_CRATES(crates),
         crate_licenses=get_crate_LICENSE(crate_files),
         description=bash_dquote_escape(collapse_whitespace(
             pkg_meta.description or "")),
         homepage=url_dquote_escape(pkg_meta.homepage or ""),
         pkg_license=get_package_LICENSE(pkg_meta),
         prog_version=__version__,
         year=datetime.date.today().year)
@@ -192,23 +194,25 @@
         if self.count != expected:
             raise RuntimeError(
                 f"{desc} matched {self.count} times, {expected} expected")
 
 
 def update_ebuild(ebuild: str,
                   pkg_meta: PackageMetadata,
-                  crate_files: typing.Iterable[Path],
+                  crates: typing.Iterable[Crate],
+                  distdir: Path,
                   *,
                   crate_license: bool = True,
                   ) -> str:
     """
     Update the CRATES and LICENSE in an existing ebuild
     """
 
-    crates_repl = CountingSubst(partial(get_CRATES, crate_files))
+    crate_files = [distdir / crate.filename for crate in crates]
+    crates_repl = CountingSubst(partial(get_CRATES, crates))
     crate_license_repl = CountingSubst(partial(get_crate_LICENSE, crate_files))
 
     ebuild = CRATE_LICENSE_RE.sub(crate_license_repl,
                                   CRATES_RE.sub(crates_repl, ebuild))
 
     crates_repl.assert_count("CRATES=", 1)
     crate_license_repl.assert_count(
```

### Comparing `pycargoebuild-0.6.3/pycargoebuild/fetch.py` & `pycargoebuild-0.7/pycargoebuild/fetch.py`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.6.3/pycargoebuild/format.py` & `pycargoebuild-0.7/pycargoebuild/format.py`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.6.3/pycargoebuild/license.py` & `pycargoebuild-0.7/pycargoebuild/license.py`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.6.3/pyproject.toml` & `pycargoebuild-0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycargoebuild-0.6.3/PKG-INFO` & `pycargoebuild-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycargoebuild
-Version: 0.6.3
+Version: 0.7
 Summary: A generator for Rust/Cargo ebuilds written in Python
 Author-email: Michał Górny <mgorny@gentoo.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: license_expression
 Requires-Dist: tomli >= 1.2.3; python_version < '3.11'
```

