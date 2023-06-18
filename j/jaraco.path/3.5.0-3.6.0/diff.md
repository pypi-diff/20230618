# Comparing `tmp/jaraco.path-3.5.0.tar.gz` & `tmp/jaraco.path-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.path-3.5.0.tar", last modified: Sun Apr  9 22:27:02 2023, max compression
+gzip compressed data, was "jaraco.path-3.6.0.tar", last modified: Sun Jun 18 21:20:13 2023, max compression
```

## Comparing `jaraco.path-3.5.0.tar` & `jaraco.path-3.6.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.477495 jaraco.path-3.5.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/jaraco/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/jaraco.path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 22:27:02.000000 jaraco.path-3.5.0/jaraco.path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 22:27:02.481495 jaraco.path-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-09 22:26:43.000000 jaraco.path-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/jaraco/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/jaraco.path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/tox.ini
```

### Comparing `jaraco.path-3.5.0/.github/workflows/main.yml` & `jaraco.path-3.6.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -100,14 +103,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `jaraco.path-3.5.0/CHANGES.rst` & `jaraco.path-3.6.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v3.6.0
+======
+
+Added support for ``Symlink``s for the tree maker (``build``).
+
 v3.5.0
 ======
 
 Introduced ``Recording`` object and ``TreeMaker`` protocol,
 with ``build()`` now explicitly accepting any ``TreeMaker``.
 
 v3.4.1
```

### Comparing `jaraco.path-3.5.0/LICENSE` & `jaraco.path-3.6.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.path-3.5.0/PKG-INFO` & `jaraco.path-3.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.path
-Version: 3.5.0
+Version: 3.6.0
 Summary: miscellaneous path functions
 Home-page: https://github.com/jaraco/jaraco.path
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,16 +24,16 @@
    :target: https://github.com/jaraco/jaraco.path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Hidden File Detection
 ---------------------
```

### Comparing `jaraco.path-3.5.0/README.rst` & `jaraco.path-3.6.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
    :target: https://github.com/jaraco/jaraco.path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Hidden File Detection
 ---------------------
```

### Comparing `jaraco.path-3.5.0/docs/conf.py` & `jaraco.path-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.5.0/jaraco/path.py` & `jaraco.path-3.6.0/jaraco/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -280,15 +280,21 @@
 def is_hidden_Darwin(path):
     Foundation = importlib.import_module('Foundation')
     url = Foundation.NSURL.fileURLWithPath_(path)
     res = url.getResourceValue_forKey_error_(None, Foundation.NSURLIsHiddenKey, None)
     return res[1]
 
 
-FilesSpec = Dict[str, Union[str, bytes, 'FilesSpec']]  # type: ignore
+class Symlink(str):
+    """
+    A string indicating the target of a symlink.
+    """
+
+
+FilesSpec = Dict[str, Union[str, bytes, Symlink, 'FilesSpec']]  # type: ignore
 
 
 @runtime_checkable
 class TreeMaker(Protocol):
     def __truediv__(self, *args, **kwargs):
         ...  # pragma: no cover
 
@@ -297,14 +303,17 @@
 
     def write_text(self, content, **kwargs):
         ...  # pragma: no cover
 
     def write_bytes(self, content):
         ...  # pragma: no cover
 
+    def symlink_to(self, target):
+        ...  # pragma: no cover
+
 
 def _ensure_tree_maker(obj: Union[str, TreeMaker]) -> TreeMaker:
     return obj if isinstance(obj, TreeMaker) else pathlib.Path(obj)  # type: ignore
 
 
 def build(
     spec: FilesSpec,
@@ -320,20 +329,24 @@
     ...     'README.txt': "A README file",
     ...     "foo": {
     ...         "__init__.py": "",
     ...         "bar": {
     ...             "__init__.py": "",
     ...         },
     ...         "baz.py": "# Some code",
-    ...     }
+    ...         "bar.py": Symlink("baz.py"),
+    ...     },
+    ...     "bing": Symlink("foo"),
     ... }
     >>> target = getfixture('tmp_path')
     >>> build(spec, target)
     >>> target.joinpath('foo/baz.py').read_text(encoding='utf-8')
     '# Some code'
+    >>> target.joinpath('bing/bar.py').read_text(encoding='utf-8')
+    '# Some code'
     """
     for name, contents in spec.items():
         create(contents, _ensure_tree_maker(prefix) / name)
 
 
 @functools.singledispatch
 def create(content: Union[str, bytes, FilesSpec], path):
@@ -347,14 +360,19 @@
 
 
 @create.register
 def _(content: str, path):
     path.write_text(content, encoding='utf-8')
 
 
+@create.register
+def _(content: Symlink, path):
+    path.symlink_to(content)
+
+
 class Recording:
     """
     A TreeMaker object that records everything that would be written.
 
     >>> r = Recording()
     >>> build({'foo': {'foo1.txt': 'yes'}, 'bar.txt': 'abc'}, r)
     >>> r.record
@@ -371,7 +389,10 @@
     def write_text(self, content, **kwargs):
         self.record.append(str(self.loc))
 
     write_bytes = write_text
 
     def mkdir(self, **kwargs):
         return
+
+    def symlink_to(self, target):
+        pass
```

### Comparing `jaraco.path-3.5.0/jaraco.path.egg-info/PKG-INFO` & `jaraco.path-3.6.0/jaraco.path.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.path
-Version: 3.5.0
+Version: 3.6.0
 Summary: miscellaneous path functions
 Home-page: https://github.com/jaraco/jaraco.path
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,16 +24,16 @@
    :target: https://github.com/jaraco/jaraco.path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Hidden File Detection
 ---------------------
```

### Comparing `jaraco.path-3.5.0/pytest.ini` & `jaraco.path-3.6.0/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 addopts=--doctest-modules
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `jaraco.path-3.5.0/setup.cfg` & `jaraco.path-3.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,21 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	jaraco.windows; platform_system == "Windows"
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
```

### Comparing `jaraco.path-3.5.0/tests/test_path.py` & `jaraco.path-3.6.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.5.0/tox.ini` & `jaraco.path-3.6.0/tox.ini`

 * *Files identical despite different names*

