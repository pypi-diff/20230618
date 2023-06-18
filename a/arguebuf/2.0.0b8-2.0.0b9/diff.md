# Comparing `tmp/arguebuf-2.0.0b8.tar.gz` & `tmp/arguebuf-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguebuf-2.0.0b8.tar", max compression
+gzip compressed data, was "arguebuf-2.0.0b9.tar", max compression
```

## Comparing `arguebuf-2.0.0b8.tar` & `arguebuf-2.0.0b9.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1067 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/LICENSE
--rw-r--r--   0        0        0     1590 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/README.md
--rw-r--r--   0        0        0      998 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/__init__.py
--rw-r--r--   0        0        0        0 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/__init__.py
--rw-r--r--   0        0        0       29 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/__main__.py
--rw-r--r--   0        0        0      284 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/app.py
--rw-r--r--   0        0        0     6098 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/graph.py
--rw-r--r--   0        0        0     2032 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/model.py
--rw-r--r--   0        0        0     1315 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/text.py
--rw-r--r--   0        0        0     2377 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/cli/translator.py
--rw-r--r--   0        0        0       50 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/__init__.py
--rw-r--r--   0        0        0     1295 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/analyst.py
--rw-r--r--   0        0        0     6354 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/edge.py
--rw-r--r--   0        0        0    49429 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/graph.py
--rw-r--r--   0        0        0     1224 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/metadata.py
--rw-r--r--   0        0        0    28976 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/node.py
--rw-r--r--   0        0        0     2465 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/participant.py
--rw-r--r--   0        0        0     1852 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/reference.py
--rw-r--r--   0        0        0     2203 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/models/resource.py
--rw-r--r--   0        0        0        0 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/py.typed
--rw-r--r--   0        0        0        0 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/__init__.py
--rw-r--r--   0        0        0      639 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/aif.py
--rw-r--r--   0        0        0     3123 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/aml.py
--rw-r--r--   0        0        0      496 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/argdown_json.py
--rw-r--r--   0        0        0     5671 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/graphviz.py
--rw-r--r--   0        0        0     1863 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/ova.py
--rw-r--r--   0        0        0      646 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/schema/sadface.py
--rw-r--r--   0        0        0        0 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/services/__init__.py
--rw-r--r--   0        0        0      623 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/services/dt.py
--rw-r--r--   0        0        0     1927 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/services/traversal.py
--rw-r--r--   0        0        0     3335 2023-01-11 19:54:55.767222 arguebuf-2.0.0b8/arguebuf/services/utils.py
--rw-r--r--   0        0        0     1483 2023-01-11 19:55:20.791276 arguebuf-2.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 arguebuf-2.0.0b8/setup.py
--rw-r--r--   0        0        0     3107 1970-01-01 00:00:00.000000 arguebuf-2.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/LICENSE
+-rw-r--r--   0        0        0     1590 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/README.md
+-rw-r--r--   0        0        0     1030 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/__init__.py
+-rw-r--r--   0        0        0       29 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/__main__.py
+-rw-r--r--   0        0        0      284 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/app.py
+-rw-r--r--   0        0        0     6098 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/graph.py
+-rw-r--r--   0        0        0     2032 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/model.py
+-rw-r--r--   0        0        0     1315 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/text.py
+-rw-r--r--   0        0        0     2377 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/cli/translator.py
+-rw-r--r--   0        0        0       50 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/__init__.py
+-rw-r--r--   0        0        0     1295 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/analyst.py
+-rw-r--r--   0        0        0     6354 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/edge.py
+-rw-r--r--   0        0        0    49429 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/graph.py
+-rw-r--r--   0        0        0     1224 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/metadata.py
+-rw-r--r--   0        0        0    28976 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/node.py
+-rw-r--r--   0        0        0     2465 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/participant.py
+-rw-r--r--   0        0        0     1852 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/reference.py
+-rw-r--r--   0        0        0     2203 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/models/resource.py
+-rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/py.typed
+-rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/__init__.py
+-rw-r--r--   0        0        0      639 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/aif.py
+-rw-r--r--   0        0        0     3123 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/aml.py
+-rw-r--r--   0        0        0      496 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/argdown_json.py
+-rw-r--r--   0        0        0     5670 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/graphviz.py
+-rw-r--r--   0        0        0     4301 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/microtexts.py
+-rw-r--r--   0        0        0     1863 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/ova.py
+-rw-r--r--   0        0        0      646 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/schema/sadface.py
+-rw-r--r--   0        0        0        0 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/__init__.py
+-rw-r--r--   0        0        0      623 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/dt.py
+-rw-r--r--   0        0        0     1927 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/traversal.py
+-rw-r--r--   0        0        0     3335 2023-01-19 14:45:04.068391 arguebuf-2.0.0b9/arguebuf/services/utils.py
+-rw-r--r--   0        0        0     1506 2023-01-19 14:45:31.688577 arguebuf-2.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 arguebuf-2.0.0b9/setup.py
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 arguebuf-2.0.0b9/PKG-INFO
```

### Comparing `arguebuf-2.0.0b8/LICENSE` & `arguebuf-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/README.md` & `arguebuf-2.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/__init__.py` & `arguebuf-2.0.0b9/arguebuf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     Scheme,
     SchemeNode,
     Support,
 )
 from .models.participant import Participant
 from .models.reference import Reference
 from .models.resource import Resource
-from .schema.graphviz import export as to_gv
-from .schema.graphviz import render
+from .schema.graphviz import render, to_gv
+from .schema.microtexts import from_microtexts
 from .services import traversal
 from .services.utils import uuid
 
 __all__ = (
     "Userdata",
     "Analyst",
     "Edge",
@@ -41,10 +41,11 @@
     "Participant",
     "Reference",
     "Resource",
     "to_gv",
     "render",
     "uuid",
     "traversal",
+    "from_microtexts",
 )
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `arguebuf-2.0.0b8/arguebuf/cli/graph.py` & `arguebuf-2.0.0b9/arguebuf/cli/graph.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/cli/model.py` & `arguebuf-2.0.0b9/arguebuf/cli/model.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/cli/text.py` & `arguebuf-2.0.0b9/arguebuf/cli/text.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/cli/translator.py` & `arguebuf-2.0.0b9/arguebuf/cli/translator.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/analyst.py` & `arguebuf-2.0.0b9/arguebuf/models/analyst.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/edge.py` & `arguebuf-2.0.0b9/arguebuf/models/edge.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/graph.py` & `arguebuf-2.0.0b9/arguebuf/models/graph.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/metadata.py` & `arguebuf-2.0.0b9/arguebuf/models/metadata.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/node.py` & `arguebuf-2.0.0b9/arguebuf/models/node.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/participant.py` & `arguebuf-2.0.0b9/arguebuf/models/participant.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/reference.py` & `arguebuf-2.0.0b9/arguebuf/models/reference.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/models/resource.py` & `arguebuf-2.0.0b9/arguebuf/models/resource.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/schema/aif.py` & `arguebuf-2.0.0b9/arguebuf/schema/aif.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/schema/aml.py` & `arguebuf-2.0.0b9/arguebuf/schema/aml.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/schema/graphviz.py` & `arguebuf-2.0.0b9/arguebuf/schema/graphviz.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class EdgeStyle(Enum):
     BEZIER = "curved"
     STRAIGHT = "line"
     STEP = "ortho"
 
 
-def export(
+def to_gv(
     graph: Graph,
     nodesep: t.Optional[float] = None,
     ranksep: t.Optional[float] = None,
     wrap_col: t.Optional[int] = None,
     margin: t.Optional[t.Tuple[float, float]] = None,
     font_name: t.Optional[str] = None,
     font_size: t.Optional[float] = None,
```

### Comparing `arguebuf-2.0.0b8/arguebuf/schema/ova.py` & `arguebuf-2.0.0b9/arguebuf/schema/ova.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/schema/sadface.py` & `arguebuf-2.0.0b9/arguebuf/schema/sadface.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/services/dt.py` & `arguebuf-2.0.0b9/arguebuf/services/dt.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/services/traversal.py` & `arguebuf-2.0.0b9/arguebuf/services/traversal.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/arguebuf/services/utils.py` & `arguebuf-2.0.0b9/arguebuf/services/utils.py`

 * *Files identical despite different names*

### Comparing `arguebuf-2.0.0b8/pyproject.toml` & `arguebuf-2.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [tool.poetry]
 name = "arguebuf"
-version = "2.0.0b8"
+version = "2.0.0b9"
 description = "A library for loading argument graphs in various formats (e.g., AIF)."
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arguebuf-python"
 documentation = "https://arguebuf.readthedocs.io/en/latest"
 
 [tool.poetry.scripts]
 arguebuf = "arguebuf.cli.app:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-arg-services = "^1.0.4"
+arg-services = "^1.0.8"
 networkx = ">=2.8.8, <4.0"
 pendulum = "^2.1.2"
 graphviz = "^0.20.1"
 lxml = "^4.9.2"
 sphinx = { version = "^5.0.0", optional = true }
 furo = { version = "^2022.12.7", optional = true }
 myst-parser = { version = "^0.18.1", optional = true }
 sphinx-autoapi = { version = "^2.0.0", optional = true }
-autodocsumm = { version = "^0.2.9", optional = true }
+autodocsumm = { version = "^0.2.10", optional = true }
 typer = { version = "^0.7.0", extras = ["all"], optional = true }
 deepl = { version = "^1.12.0", optional = true }
 pygraphviz = { version = "^1.10", optional = true }
 multimethod = { version = "^1.9.1", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-datadir = "^1.3.1"
 pytest-cov = "^4.0.0"
 deepdiff = { extras = ["murmur"], version = "^6.0.0" }
+lxml-stubs = "^0.4.0"
 
 [tool.poetry.extras]
 docs = ["sphinx", "furo", "myst-parser", "sphinx-autoapi", "autodocsumm"]
 cli = ["typer", "deepl", "multimethod"]
 graphviz = ["pygraphviz"]
 
 [build-system]
```

### Comparing `arguebuf-2.0.0b8/setup.py` & `arguebuf-2.0.0b9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,37 +8,37 @@
  'arguebuf.schema',
  'arguebuf.services']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['arg-services>=1.0.4,<2.0.0',
+['arg-services>=1.0.8,<2.0.0',
  'graphviz>=0.20.1,<0.21.0',
  'lxml>=4.9.2,<5.0.0',
  'networkx>=2.8.8,<4.0',
  'pendulum>=2.1.2,<3.0.0']
 
 extras_require = \
 {'cli': ['typer[all]>=0.7.0,<0.8.0',
          'deepl>=1.12.0,<2.0.0',
          'multimethod>=1.9.1,<2.0.0'],
  'docs': ['sphinx>=5.0.0,<6.0.0',
           'furo>=2022.12.7,<2023.0.0',
           'myst-parser>=0.18.1,<0.19.0',
           'sphinx-autoapi>=2.0.0,<3.0.0',
-          'autodocsumm>=0.2.9,<0.3.0'],
+          'autodocsumm>=0.2.10,<0.3.0'],
  'graphviz': ['pygraphviz>=1.10,<2.0']}
 
 entry_points = \
 {'console_scripts': ['arguebuf = arguebuf.cli.app:cli']}
 
 setup_kwargs = {
     'name': 'arguebuf',
-    'version': '2.0.0b8',
+    'version': '2.0.0b9',
     'description': 'A library for loading argument graphs in various formats (e.g., AIF).',
     'long_description': '# Arguebuf\n\nArguebuf is a format for serializing argument graphs and specified using Protobuf.\nThe complete specification and documentation is available at the [Buf Schema Registry](https://buf.build/recap/arg-services/docs/main:arg_services.graph.v1).\nWhile Protobuf automatically generates native code for all major programming languages (including Python), we created a custom implementation that provides some additional benefits, including:\n\n- The ability to import existing formats like [AIF](http://www.argumentinterchange.org), [SADFace](https://github.com/Open-Argumentation/SADFace), and a few others.\n- Export of Arguebuf graphs to AIF, [NetworkX](https://networkx.org), and [Graphviz](https://graphviz.org).\n- Integration with the popular NLP library [spaCy](http://spacy.io).\n- Various helper methods to programmatically manipulate/create argument graphs.\n- More pythonic interfaces than the regular code generated by `protoc`.\n\nYou can easily install the library from [PyPI](https://pypi.org/project/arguebuf/) using pip. The documentation is hosted on [ReadTheDocs](https://arguebuf.readthedocs.io/en/latest/)\n\n## Command Line Interface (CLI)\n\nWe also offer some tools to simplify dealing with structured argument graphs.\nAmong others, it is possible to convert graphs between different formats, translate them, and render images using graphviz.\nTo use it, install the `cli` extras when installing the package.\nWhen using `pip`, this can be accomplished with\n\n`pip install arguebuf[cli]`\n\nAfterwards, you can execute it by calling `arguebuf`, for example:\n\n`arguebuf --help`\n',
     'author': 'Mirko Lenz',
     'author_email': 'info@mirko-lenz.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://recap.uni-trier.de',
```

### Comparing `arguebuf-2.0.0b8/PKG-INFO` & `arguebuf-2.0.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: arguebuf
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: A library for loading argument graphs in various formats (e.g., AIF).
 Home-page: https://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
 Provides-Extra: docs
 Provides-Extra: graphviz
-Requires-Dist: arg-services (>=1.0.4,<2.0.0)
-Requires-Dist: autodocsumm (>=0.2.9,<0.3.0) ; extra == "docs"
+Requires-Dist: arg-services (>=1.0.8,<2.0.0)
+Requires-Dist: autodocsumm (>=0.2.10,<0.3.0) ; extra == "docs"
 Requires-Dist: deepl (>=1.12.0,<2.0.0) ; extra == "cli"
 Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: multimethod (>=1.9.1,<2.0.0) ; extra == "cli"
 Requires-Dist: myst-parser (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: networkx (>=2.8.8,<4.0)
```

