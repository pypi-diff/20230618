# Comparing `tmp/docleaf-0.4.0-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.5.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1081228 bytes, number of entries: 10
--rw-r--r--  4.6 unx     6708 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     3836 b- defN 23-Jun-14 16:33 docleaf/copied.py
--rw-r--r--  4.6 unx     3709 b- defN 23-Jun-14 16:33 docleaf/domains.py
--rw-r--r--  4.6 unx    18910 b- defN 23-Jun-14 16:33 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jun-14 16:33 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-14 16:33 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3051520 b- defN 23-Jun-14 16:33 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      775 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/RECORD
-10 files, 3089226 bytes uncompressed, 1079922 bytes compressed:  65.0%
+Zip file size: 1074984 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     6823 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3573 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     3836 b- defN 23-Jun-18 17:03 docleaf/copied.py
+-rw-r--r--  4.6 unx     3709 b- defN 23-Jun-18 17:03 docleaf/domains.py
+-rw-r--r--  4.6 unx    20597 b- defN 23-Jun-18 17:03 docleaf/doxygen.py
+-rw-r--r--  4.6 unx       99 b- defN 23-Jun-18 17:03 docleaf/errors.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-18 17:03 docleaf/__init__.py
+-rwxr-xr-x  4.6 unx  3031040 b- defN 23-Jun-18 17:03 docleaf/backend.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      775 b- defN 23-Jun-18 17:03 docleaf-0.5.0.dist-info/RECORD
+10 files, 3070548 bytes uncompressed, 1073678 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: docleaf-0.4.0.dist-info/METADATA
+Filename: docleaf-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.4.0.dist-info/WHEEL
+Filename: docleaf-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.4.0.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.5.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: docleaf/copied.py
 Comment: 
 
 Filename: docleaf/domains.py
 Comment: 
@@ -21,11 +21,11 @@
 
 Filename: docleaf/__init__.py
 Comment: 
 
 Filename: docleaf/backend.cp39-win_amd64.pyd
 Comment: 
 
-Filename: docleaf-0.4.0.dist-info/RECORD
+Filename: docleaf-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docleaf/doxygen.py

```diff
@@ -112,15 +112,16 @@
             "literal": as_list(nodes.literal),
             "literal_block": as_list(nodes.literal_block),
             "literal_strong": as_list(sphinx.addnodes.literal_strong),
             "note": as_list(nodes.note),
             "only": as_list(sphinx.addnodes.only),
             "paragraph": as_list(nodes.paragraph),
             "raw": as_list(nodes.raw),
-            "reference": as_list(nodes.reference),
+            "internal_reference": self.build_internal_reference,
+            "external_reference": as_list(nodes.reference),
             "restructured_text_block": self.build_restructured_text_block,
             "restructured_text_inline": self.build_restructured_text_inline,
             "row": as_list(nodes.row),
             "rubric": as_list(nodes.rubric),
             "strong": as_list(nodes.strong),
             "see_also": as_list(sphinx.addnodes.seealso),
             "table": as_list(nodes.table),
@@ -149,14 +150,25 @@
             attributes["declaration"],
             attributes.get("location"),
             self.build_target(**attributes["target"]),
             self.directive_arguments,
             children,
         )
 
+    def build_internal_reference(self, *children, **attributes):
+        reference = sphinx.addnodes.pending_xref(
+            *children,
+            reftype="ref",
+            refdomain="std",
+            refexplicit=True,
+            refid=attributes["refid"],
+            reftarget=attributes["refid"],
+        )
+        return [reference]
+
     def build_restructured_text_block(self, *children, **attributes):
         text = textwrap.dedent(children[0])
 
         # Inspired by autodoc.py in Sphinx
         rst = StringList()
         for line in text.split("\n"):
             rst.append(line, "<docleaf>")
@@ -211,14 +223,53 @@
         return node_builder("", *children, **node.attributes)
     elif node.call_as == "args":
         return node_builder(*children, **node.attributes)
     else:
         raise DocleafError("Call As not implemented: " + node.call_as)
 
 
+class Project:
+    def __init__(self, root, xml):
+        self._root = root
+        self._xml = xml
+
+    def root(self):
+        return self._root
+
+    def xml(self):
+        return self._xml
+
+    def get(projects, name: str):
+        # For each 'try' block we need to catch KeyError and TypeError (if project is a string) so we catch everything
+        # as there isn't much else that could go wrong
+
+        try:
+            data = projects[name]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find a project called '{name}' defined in the docleaf_projects config variable"
+            )
+
+        try:
+            root = data["root"]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find the 'root' entry in the data for '{name}' project defined in the docleaf_projects config variable"
+            )
+
+        try:
+            xml = data["xml"]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find the 'xml' entry in the data for '{name}' project defined in the docleaf_projects config variable"
+            )
+
+        return Project(root, xml)
+
+
 class BaseDirective(Directive):
     def get_directive_args(self) -> list:
         # Must match order in docutils.parsers.rst.Directive.__init__
         return [
             self.name,
             self.arguments,
             self.options,
@@ -239,25 +290,25 @@
     option_spec = {
         "project": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
         project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = self.app.config.docleaf_projects[project_name]
+        project = Project.get(self.app.config.docleaf_projects, project_name)
 
         skip_settings = get_skip_settings(self.app, self.options)
         context = backend.Context(
-            project["root"],
+            project.root(),
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_class(name, project["xml"], context, tracked_cache)
+        node_list = backend.render_class(name, project.xml(), context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class StructDirective(BaseDirective):
@@ -268,24 +319,24 @@
     option_spec = {
         "project": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
         project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = self.app.config.docleaf_projects[project_name]
+        project = Project.get(self.app.config.docleaf_projects, project_name)
         skip_settings = get_skip_settings(self.app, self.options)
         context = backend.Context(
-            project["root"],
+            project.root(),
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_struct(name, project["xml"], context, tracked_cache)
+        node_list = backend.render_struct(name, project.xml(), context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class EnumDirective(BaseDirective):
@@ -297,25 +348,25 @@
         "project": directives.unchanged,
         "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
         project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = self.app.config.docleaf_projects[project_name]
+        project = Project.get(self.app.config.docleaf_projects, project_name)
         skip_settings = get_skip_settings(self.app, self.options)
 
         context = backend.Context(
-            project["root"],
+            project.root(),
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_enum(name, project["xml"], context, tracked_cache)
+        node_list = backend.render_enum(name, project.xml(), context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class FunctionDirective(BaseDirective):
@@ -327,25 +378,25 @@
         "project": directives.unchanged,
         "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
         project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = self.app.config.docleaf_projects[project_name]
+        project = Project.get(self.app.config.docleaf_projects, project_name)
         skip_settings = get_skip_settings(self.app, self.options)
 
         context = backend.Context(
-            project["root"],
+            project.root(),
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_function(name, project["xml"], context, tracked_cache)
+        node_list = backend.render_function(name, project.xml(), context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class GroupDirective(BaseDirective):
@@ -359,29 +410,29 @@
         "inner": directives.flag,  # TODO: Implement
         "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
         project_name = self.options.get("project", self.app.config.docleaf_default_project)
-        project = self.app.config.docleaf_projects[project_name]
+        project = Project.get(self.app.config.docleaf_projects, project_name)
 
         skip_settings = get_skip_settings(self.app, self.options)
         content_only = "content-only" in self.options
         inner_group = "inner" in self.options
         context = backend.Context(
-            project["root"],
+            project.root(),
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
         node_list = backend.render_group(
             name,
-            project["xml"],
+            project.xml(),
             context,
             content_only,
             inner_group,
             tracked_cache,
         )
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
```

## Comparing `docleaf-0.4.0.dist-info/METADATA` & `docleaf-0.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,<6,!=5.0.0
 License-File: LICENSE.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Keywords: sphinx,doxygen
 Author-email: Michael Jones <michael.jones@docleaf.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
-Project-URL: repository, https://github.com/docleaf-labs/docleaf
 Project-URL: homepage, https://docleaf.io
+Project-URL: repository, https://github.com/docleaf-labs/docleaf
+Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
 
 <h1 align="center">
   Docleaf
 </h1>
 
 <p align="center">
    Your technical docs, beautifully integrated
@@ -36,14 +36,15 @@
 
 For further information please email: [support@docleaf.io](mailto:support@docleaf.io)
 
 ## Features
 
 - Custom directives allowing you to target various parts of C and C++ code bases.
 - Integration with Sphinx C and C++ domains to support easily linking to your generated output.
+- Hash-based content checks, as well as timestamp checks, to minimize incremental build times after a Doxygen run.
 - Integration with the `sphinx.ext.linkcode` extension to support links to source code locations in a GitHub
   repository.
 
 ## Installation
 
 Docleaf can be installed from [PyPI](https://pypi.org/project/docleaf/):
 
@@ -195,10 +196,10 @@
   Time (mean ± σ):     389.658 s ±  5.271 s    [User: 1839.366 s, System: 24.895 s]
   Range (min … max):   379.093 s … 394.315 s    10 runs
 ```
 
 ## History
 
 Docleaf is written and maintained by the creator of the [Breathe](https://github.com/breathe-doc/breathe) project.
-It was created to resolve some of the performance and memory consumption issues with Breathe by re-writing the code
+It was created to resolve some of the performance and memory consumption issues with Breathe by rewriting the code
 base to use Rust. The user experience is designed to match and improve on Breathe.
```

## Comparing `docleaf-0.4.0.dist-info/license_files/LICENSE.md` & `docleaf-0.5.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

