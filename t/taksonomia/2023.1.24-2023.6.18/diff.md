# Comparing `tmp/taksonomia-2023.1.24.tar.gz` & `tmp/taksonomia-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taksonomia-2023.1.24.tar", last modified: Tue Jan 24 22:12:55 2023, max compression
+gzip compressed data, was "taksonomia-2023.6.18.tar", last modified: Sun Jun 18 11:57:53 2023, max compression
```

## Comparing `taksonomia-2023.1.24.tar` & `taksonomia-2023.6.18.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-24 22:12:55.266590 taksonomia-2023.1.24/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 taksonomia-2023.1.24/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)     2787 2023-01-24 22:12:55.266445 taksonomia-2023.1.24/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1736 2023-01-22 12:52:11.000000 taksonomia-2023.1.24/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     2749 2023-01-24 22:03:01.000000 taksonomia-2023.1.24/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-01-24 22:12:55.266627 taksonomia-2023.1.24/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-24 22:12:55.263507 taksonomia-2023.1.24/taksonomia/
--rw-r--r--   0 ruth       (501) staff       (20)     2533 2023-01-24 22:09:50.000000 taksonomia-2023.1.24/taksonomia/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-09-09 18:52:08.000000 taksonomia-2023.1.24/taksonomia/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     9765 2022-09-18 20:13:00.000000 taksonomia-2023.1.24/taksonomia/anglify.py
--rw-r--r--   0 ruth       (501) staff       (20)     4408 2023-01-24 22:01:53.000000 taksonomia-2023.1.24/taksonomia/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     4299 2022-09-12 16:21:43.000000 taksonomia-2023.1.24/taksonomia/machine.py
--rw-r--r--   0 ruth       (501) staff       (20)    14642 2023-01-24 21:56:35.000000 taksonomia-2023.1.24/taksonomia/taksonomia.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-24 22:12:55.265323 taksonomia-2023.1.24/taksonomia.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2787 2023-01-24 22:12:55.000000 taksonomia-2023.1.24/taksonomia.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      454 2023-01-24 22:12:55.000000 taksonomia-2023.1.24/taksonomia.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-01-24 22:12:55.000000 taksonomia-2023.1.24/taksonomia.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       51 2023-01-24 22:12:55.000000 taksonomia-2023.1.24/taksonomia.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      162 2023-01-24 22:12:55.000000 taksonomia-2023.1.24/taksonomia.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       11 2023-01-24 22:12:55.000000 taksonomia-2023.1.24/taksonomia.egg-info/top_level.txt
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-24 22:12:55.266272 taksonomia-2023.1.24/test/
--rw-r--r--   0 ruth       (501) staff       (20)     1242 2022-09-18 20:18:32.000000 taksonomia-2023.1.24/test/test_anglify.py
--rw-r--r--   0 ruth       (501) staff       (20)     7099 2022-12-23 10:29:26.000000 taksonomia-2023.1.24/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      284 2022-09-12 16:25:14.000000 taksonomia-2023.1.24/test/test_machine.py
--rw-r--r--   0 ruth       (501) staff       (20)     4172 2022-09-21 15:45:09.000000 taksonomia-2023.1.24/test/test_taksonomia.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 11:57:53.575039 taksonomia-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 taksonomia-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)     3283 2023-06-18 11:57:53.574898 taksonomia-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2181 2023-03-14 22:45:49.000000 taksonomia-2023.6.18/README.md
+-rw-r--r--   0 ruth       (501) staff       (20)     2804 2023-06-18 11:29:35.000000 taksonomia-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 11:57:53.575076 taksonomia-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 11:57:53.571107 taksonomia-2023.6.18/taksonomia/
+-rw-r--r--   0 ruth       (501) staff       (20)     2543 2023-06-18 11:54:39.000000 taksonomia-2023.6.18/taksonomia/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2022-09-09 18:52:08.000000 taksonomia-2023.6.18/taksonomia/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     9765 2022-09-18 20:13:00.000000 taksonomia-2023.6.18/taksonomia/anglify.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4431 2023-06-18 11:44:53.000000 taksonomia-2023.6.18/taksonomia/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4299 2022-09-12 16:21:43.000000 taksonomia-2023.6.18/taksonomia/machine.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14757 2023-06-18 11:45:16.000000 taksonomia-2023.6.18/taksonomia/taksonomia.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 11:57:53.573368 taksonomia-2023.6.18/taksonomia.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3283 2023-06-18 11:57:53.000000 taksonomia-2023.6.18/taksonomia.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      454 2023-06-18 11:57:53.000000 taksonomia-2023.6.18/taksonomia.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 11:57:53.000000 taksonomia-2023.6.18/taksonomia.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       51 2023-06-18 11:57:53.000000 taksonomia-2023.6.18/taksonomia.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      162 2023-06-18 11:57:53.000000 taksonomia-2023.6.18/taksonomia.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       11 2023-06-18 11:57:53.000000 taksonomia-2023.6.18/taksonomia.egg-info/top_level.txt
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 11:57:53.574737 taksonomia-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     1242 2022-09-18 20:18:32.000000 taksonomia-2023.6.18/test/test_anglify.py
+-rw-r--r--   0 ruth       (501) staff       (20)     7109 2023-06-18 11:46:56.000000 taksonomia-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      284 2022-09-12 16:25:14.000000 taksonomia-2023.6.18/test/test_machine.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4182 2023-06-18 11:46:21.000000 taksonomia-2023.6.18/test/test_taksonomia.py
```

### Comparing `taksonomia-2023.1.24/LICENSE` & `taksonomia-2023.6.18/LICENSE`

 * *Files identical despite different names*

### Comparing `taksonomia-2023.1.24/PKG-INFO` & `taksonomia-2023.6.18/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: taksonomia
-Version: 2023.1.24
+Version: 2023.6.18
 Summary: Taxonomy (Finnish: taksonomia) of a folder tree, guided by conventions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/taksonomia
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/taksonomia
 Project-URL: Documentation, https://codes.dilettant.life/docs/taksonomia
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/taksonomia
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/taksonomia
 Keywords: developer-tools,fingerprints,validation,verification,sbom,taxonomy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Taksonomia
@@ -37,25 +38,32 @@
 
 ## Documentation
 
 User and developer [documentation of taksonomia](https://codes.dilettant.life/docs/taksonomia/).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of taksonomia](https://todo.sr.ht/~sthagen/taksonomia).
+Any feature requests or bug reports shall go to the [todos of taksonomia](https://todo.sr.ht/~sthagen/taksonomia).
 
 ## Primary Source repository
 
 The main source of `taksonomia` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `taksonomia` are:
 
 * [on codeberg](https://codeberg.org/sthagen/taksonomia) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/taksonomia) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `taksonomia-2023.1.24/pyproject.toml` & `taksonomia-2023.6.18/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taksonomia"
-version = "2023.1.24"
+version = "2023.6.18"
 description = "Taxonomy (Finnish: taksonomia) of a folder tree, guided by conventions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "fingerprints", "validation", "verification", "sbom", "taxonomy"]
 dependencies = [
     "PyYAML >= 6.0",
     "lxml >= 4.9.2",
-    "msgspec >= 0.12.0",
-    "psutil >= 5.9.4",
+    "msgspec >= 0.16.0",
+    "psutil >= 5.9.5",
     "py-cpuinfo >= 9.0.0",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "types-jmespath", "ruff"]
 
@@ -43,15 +44,15 @@
 [tool.setuptools.packages.find]
 include = ["taksonomia"]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
```

### Comparing `taksonomia-2023.1.24/taksonomia/__init__.py` & `taksonomia-2023.6.18/taksonomia/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime as dti
 import logging
 import os
 import pathlib
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.1.24+parent.7515eaa5'
-# [[[end]]] (checksum: c9429f943a3fc72cb5a26502723a9fef)
+__version__ = '2023.6.18+parent.a8561973'
+# [[[end]]] (checksum: 403d4b77cdd1dbbd3a56d736185c108d)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_ALIAS = 'taksonomia'
 APP_ENV = 'TAKSONOMIA'
 APP_NAME = 'Taxonomy (Finnish: taksonomia) of a folder tree, guided by conventions.'
@@ -19,15 +19,15 @@
 COMMA = ','
 DEBUG = bool(os.getenv(f'{APP_ENV}_DEBUG', ''))
 DEFAULT_CONFIG_NAME = '.taksonomia.json'
 DEFAULT_LF_ONLY = 'YES'
 ENCODING = 'utf-8'
 ENCODING_ERRORS_POLICY = 'ignore'
 KNOWN_FORMATS = ('json', 'xml', 'yaml')
-KNOWN_KEY_FUNCTIONS = ('elf', 'md5')
+KNOWN_KEY_FUNCTIONS = ('blake2', 'elf', 'md5')
 QUIET = False
 STRICT = bool(os.getenv(f'{APP_ENV}_STRICT', ''))
 TS_FORMAT = '%Y-%m-%d %H:%M:%S.%f +00:00'
 VERBOSE = bool(os.getenv(f'{APP_ENV}_VERBOSE', ''))
 VERSION_INFO = __version_info__
 
 log = logging.getLogger()  # Module level logger is sufficient
```

### Comparing `taksonomia-2023.1.24/taksonomia/anglify.py` & `taksonomia-2023.6.18/taksonomia/anglify.py`

 * *Files identical despite different names*

### Comparing `taksonomia-2023.1.24/taksonomia/cli.py` & `taksonomia-2023.6.18/taksonomia/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         default='',
         help='comma separated list of values to exclude paths\ncontaining the substring (default: empty string)',
     )
     parser.add_argument(
         '--key-function',
         '-k',
         dest='key_function',
-        default='elf',
-        help='key function (elf, md5) for branches and leaves\n(default: elf) use md5 for larger taxonomies',
+        default='blake2',
+        help='key function (blake2, elf, md5) for branches and leaves\n(default: blake2) use elf only for very small taxonomies',
     )
     parser.add_argument(
         '--out-path',
         '-o',
         dest='out_path',
         default=sys.stdout,
         help='output file path (stem) for taxonomy (default: STDOUT)',
```

### Comparing `taksonomia-2023.1.24/taksonomia/machine.py` & `taksonomia-2023.6.18/taksonomia/machine.py`

 * *Files identical despite different names*

### Comparing `taksonomia-2023.1.24/taksonomia/taksonomia.py` & `taksonomia-2023.6.18/taksonomia/taksonomia.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,17 @@
         text = str(path)
         return bool(self.excludes) and any(exclude in text for exclude in self.excludes)
 
     def key(self, path_str: str) -> str:
         """Hashing function for the path keys."""
         if self.key_function == 'elf':
             return str(elf_hash(path_str.encode(ENCODING)))
-        return hashlib.md5(path_str.encode(ENCODING)).hexdigest()  # nosec B324
+        elif self.key_function == 'md5':
+            return hashlib.md5(path_str.encode(ENCODING)).hexdigest()  # nosec B324
+        return hashlib.blake2b(path_str.encode(ENCODING)).hexdigest()
 
     def add_branch(self, path: pathlib.Path) -> None:
         """Add a folder (sub tree) entry."""
         if self.ignore(path):
             return
 
         st = path.stat()
```

### Comparing `taksonomia-2023.1.24/taksonomia.egg-info/PKG-INFO` & `taksonomia-2023.6.18/taksonomia.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: taksonomia
-Version: 2023.1.24
+Version: 2023.6.18
 Summary: Taxonomy (Finnish: taksonomia) of a folder tree, guided by conventions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/taksonomia
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/taksonomia
 Project-URL: Documentation, https://codes.dilettant.life/docs/taksonomia
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/taksonomia
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/taksonomia
 Keywords: developer-tools,fingerprints,validation,verification,sbom,taxonomy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Taksonomia
@@ -37,25 +38,32 @@
 
 ## Documentation
 
 User and developer [documentation of taksonomia](https://codes.dilettant.life/docs/taksonomia/).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of taksonomia](https://todo.sr.ht/~sthagen/taksonomia).
+Any feature requests or bug reports shall go to the [todos of taksonomia](https://todo.sr.ht/~sthagen/taksonomia).
 
 ## Primary Source repository
 
 The main source of `taksonomia` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `taksonomia` are:
 
 * [on codeberg](https://codeberg.org/sthagen/taksonomia) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/taksonomia) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `taksonomia-2023.1.24/test/test_anglify.py` & `taksonomia-2023.6.18/test/test_anglify.py`

 * *Files identical despite different names*

### Comparing `taksonomia-2023.1.24/test/test_cli.py` & `taksonomia-2023.6.18/test/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,11 +187,11 @@
 def test_main_unknown_key_function(capsys):
     with pytest.raises(SystemExit) as err:
         cli.main(['test/fixtures/basic/', '-k', 'unknown-key-function'])
     assert err.value.code == 2
     out, err = capsys.readouterr()
     assert 'usage: taksonomia [-h] [--tree-root TREE_ROOT] [--excludes EXCLUDES]' in err
     assert (
-        "taksonomia: error: requested key function unknown-key-function for branches and leaves not in ('elf', 'md5')"
+        "taksonomia: error: requested key function unknown-key-function for branches and leaves not in ('blake2', 'elf', 'md5')"
         in err
     )
     assert not out
```

### Comparing `taksonomia-2023.1.24/test/test_taksonomia.py` & `taksonomia-2023.6.18/test/test_taksonomia.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     message = '"Unsupported hash algorithm requested - foo is not in (\'sha512\', \'sha256\')"'
     with pytest.raises(KeyError, match=re.escape(message)):
         taxonomy.hash_file(folder / 'empty.txt', 'foo')
 
 
 def test_taxonomy_hash_file_bad_key_function():
     folder = pathlib.Path('test', 'fixtures', 'corner')
-    message = r"key function unknown not in ('elf', 'md5')"
+    message = r"key function unknown not in ('blake2', 'elf', 'md5')"
     with pytest.raises(ValueError, match=re.escape(message)):
         Taxonomy(folder, 'me,too', key_function='unknown')
 
 
 def test_taxonomy_repr():
     folder = pathlib.Path('test', 'fixtures', 'corner')
     taxonomy = Taxonomy(folder, 'me,too')
```

