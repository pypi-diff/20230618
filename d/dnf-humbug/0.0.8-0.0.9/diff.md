# Comparing `tmp/dnf_humbug-0.0.8-py3-none-any.whl.zip` & `tmp/dnf_humbug-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5700 bytes, number of entries: 8
--rw-r--r--  2.0 unx       87 b- defN 22-Nov-26 12:20 dnf_humbug/__init__.py
--rw-r--r--  2.0 unx       87 b- defN 22-Nov-26 12:20 dnf_humbug/__main__.py
--rw-r--r--  2.0 unx     9749 b- defN 22-Nov-26 21:57 dnf_humbug/app.py
--rw-r--r--  2.0 unx     1724 b- defN 22-Nov-26 21:58 dnf_humbug-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-26 21:58 dnf_humbug-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 22-Nov-26 21:58 dnf_humbug-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 22-Nov-26 21:58 dnf_humbug-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      636 b- defN 22-Nov-26 21:58 dnf_humbug-0.0.8.dist-info/RECORD
-8 files, 12437 bytes uncompressed, 4582 bytes compressed:  63.2%
+Zip file size: 5911 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       87 b- defN 22-Nov-26 22:35 dnf_humbug/__init__.py
+-rw-r--r--  2.0 unx       87 b- defN 22-Nov-26 22:35 dnf_humbug/__main__.py
+-rw-r--r--  2.0 unx    10319 b- defN 22-Nov-27 16:16 dnf_humbug/app.py
+-rw-r--r--  2.0 unx     1724 b- defN 22-Nov-27 16:17 dnf_humbug-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Nov-27 16:17 dnf_humbug-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-27 16:17 dnf_humbug-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 22-Nov-27 16:17 dnf_humbug-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      637 b- defN 22-Nov-27 16:17 dnf_humbug-0.0.9.dist-info/RECORD
+8 files, 13008 bytes uncompressed, 4793 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dnf_humbug/__main__.py
 Comment: 
 
 Filename: dnf_humbug/app.py
 Comment: 
 
-Filename: dnf_humbug-0.0.8.dist-info/METADATA
+Filename: dnf_humbug-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: dnf_humbug-0.0.8.dist-info/WHEEL
+Filename: dnf_humbug-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: dnf_humbug-0.0.8.dist-info/entry_points.txt
+Filename: dnf_humbug-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: dnf_humbug-0.0.8.dist-info/top_level.txt
+Filename: dnf_humbug-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dnf_humbug-0.0.8.dist-info/RECORD
+Filename: dnf_humbug-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dnf_humbug/app.py

```diff
@@ -60,40 +60,43 @@
 @dataclass
 class Package:
     """Package that we may want to remove."""
 
     name: str
     needed_by: int
     info: str
-    has_binaries: bool
+    binaries: int
     _pkg: Any
     _rdepends: List[Any]
 
     def __repr__(self) -> str:
         return self.name
 
     def __str__(self) -> str:
         return self.name
 
+def pkg_binaries(pkg) -> int:
+    binaries = sum(["bin/" in s for s in pkg.files])
+    return binaries
+
 
 def filter_packages(packages: List[Pkg], depends, rdepends):
     result = []
     for i, pkg in enumerate(packages):
         if pkg.reason == "user":
-            has_binaries = any("bin/" in s for s in pkg.files)
             # rdepends can have multiple (duplicate) entries, deduplicate first.
             unique_deps = set(rdepends[i])
             needed_by = len(unique_deps)
             _rdepends = [str(packages[n]) for n in unique_deps]
 
             p = Package(
                 name=str(pkg),
                 needed_by=needed_by,
                 info=pkg.summary,
-                has_binaries=has_binaries,
+                binaries=pkg_binaries(pkg),
                 _pkg=pkg,
                 _rdepends=_rdepends,
             )
             result.append(p)
     return result
 
 
@@ -162,30 +165,36 @@
         filtered = filter_packages(packages, depends, rdepends)
         for pkg in filtered:
             self.pkgs[pkg.name] = pkg
 
         await self.re_sort_display()
 
     async def re_sort_display(self, column: int = -1):
+        """As we cannot sort the data without re-adding it, this re-adds the
+        data."""
         self.clear()
         rows = [
-            (pkg.name, pkg.has_binaries, pkg.needed_by) for pkg in self.pkgs.values()
+            (pkg.name, pkg_binaries(pkg._pkg), pkg.needed_by) for pkg in self.pkgs.values()
         ]
 
         if column == -1:
             # Sort by name first
             rows.sort(key=itemgetter(0))
             # Then re-sort by dependencies
             rows.sort(key=itemgetter(2), reverse=True)
             # And finally sort by binaries
             rows.sort(key=itemgetter(1), reverse=True)
         else:
-            rows.sort(key=itemgetter(column), reverse=True)
+            # We sort column 0 by name, the rest we sort decreasing
+            reverse = column > 0
+            rows.sort(key=itemgetter(column), reverse=reverse)
 
         for row in rows:
+            # All columns must be the same data-type, so cast it to string
+            # first.
             self.add_row(row[0], str(row[1]), str(row[2]))
         await self.send_row_changed()
 
 
 class InfoDisplay(TextLog):
     """Widget of the information pane."""
 
@@ -238,42 +247,45 @@
         overflow-y: scroll;
         overflow: auto;
     }
     """
 
     BINDINGS = [
         ("d", "toggle_dark", "Toggle dark mode"),
-        ("i", "show_info", "Show description"),
-        ("f", "show_files", "Show files"),
-        ("m", "mark_unwanted", "Mark as unwanted"),
+        ("m", "mark_unwanted", "Toggle (un)wanted"),
+        ("i", "show_info", "Show package description"),
+        ("f", "show_files", "Show package files"),
         ("escape", "exit_app", "Time to escape"),
     ]
 
     def on_list_display_row_changed(self, message: ListDisplay.RowChanged) -> None:
         """Recieves RowChanged events from ListDisplay class."""
         self.query_one(InfoDisplay).clear()
         self.query_one(InfoDisplay).write(message.package.info)
         self.query_one(InfoDisplay).write("")
         self.query_one(InfoDisplay).write(message.package._pkg.description)
+        name = str(message.package._pkg)
         deps = Markdown(
-            "### Packages that need this:\n" + "  \n".join(message.package._rdepends)
+            f"### Packages that need {name}\n    " +  " ".join(message.package._rdepends)
         )
         self.query_one("#extra").update(deps)
 
     def on_mount(self, event: events.Mount) -> None:
+        self.title = "dnf....humbug"
+        self.sub_title = "List of packages DNF thinks you want."
         self.unwanted = set()
 
     def compose(self) -> ComposeResult:
         """Create child widgets for that App."""
         yield Header()
         display = ListDisplay(id="list", classes="box")
         display.focus()
         yield display
         yield Static(
-            Markdown("### Marked these as unwanted"), id="Unwanted", classes="box"
+            Markdown("### Final command line"), id="Unwanted", classes="box"
         )
         yield InfoDisplay(id="info", classes="box")
         yield Static("", id="extra", classes="box")
         yield Footer()
 
     def action_toggle_dark(self) -> None:
         """An action to toggle dark mode."""
@@ -307,15 +319,15 @@
         table.focus()
         pkg = table.current_package._pkg
         if pkg in self.unwanted:
             self.unwanted.remove(pkg)
         else:
             self.unwanted.add(pkg)
         names = sorted(pkg.name for pkg in self.unwanted)
-        untext = "\n".join(names)
+        untext = Markdown("### Final command line\n" + "    dnf mark remove\n     " + "\n     ".join(names))
         self.query_one("#Unwanted").update(untext)
 
     def action_exit_app(self):
         """When we want out."""
         names = (pkg.name for pkg in self.unwanted)
         output = " ".join(sorted(names))
         if output:
```

## Comparing `dnf_humbug-0.0.8.dist-info/METADATA` & `dnf_humbug-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnf-humbug
-Version: 0.0.8
+Version: 0.0.9
 Summary: List and sort user-installed files according to dnf
 License: GPL-2.0-or-later
 Description-Content-Type: text/markdown
 Requires-Dist: textual
 
 # dnf-humbug
```

