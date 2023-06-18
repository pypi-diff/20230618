# Comparing `tmp/magicwall-0.0.1.tar.gz` & `tmp/magicwall-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicwall-0.0.1.tar", max compression
+gzip compressed data, was "magicwall-0.0.2.tar", max compression
```

## Comparing `magicwall-0.0.1.tar` & `magicwall-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,13 @@
--rw-r--r--   0        0        0     5121 2022-10-31 15:47:06.221205 magicwall-0.0.1/README.md
--rw-r--r--   0        0        0       45 2022-10-31 16:45:47.083734 magicwall-0.0.1/magicwall/__init__.py
--rw-r--r--   0        0        0     1261 2022-10-31 16:44:30.390658 magicwall-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5893 1970-01-01 00:00:00.000000 magicwall-0.0.1/setup.py
--rw-r--r--   0        0        0     5695 1970-01-01 00:00:00.000000 magicwall-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5121 2022-10-31 15:47:06.221205 magicwall-0.0.2/Readme.md
+-rw-r--r--   0        0        0       45 2023-05-22 06:01:44.639872 magicwall-0.0.2/magicwall/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-18 12:57:55.403215 magicwall-0.0.2/magicwall/common.py
+-rw-r--r--   0        0        0     1437 2023-06-18 12:57:55.403215 magicwall-0.0.2/magicwall/magicwall_api.py
+-rwxr-xr-x   0        0        0    14248 2023-06-18 13:50:08.843120 magicwall-0.0.2/magicwall/server.py
+-rw-r--r--   0        0        0    21604 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/DragDropTouch.js
+-rw-r--r--   0        0        0     5119 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/hilite-solarized-light.css
+-rw-r--r--   0        0        0     1785 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/magicwall.css
+-rw-r--r--   0        0        0    16993 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/magicwall.js
+-rw-r--r--   0        0        0     3600 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/static/unknown.png
+-rw-r--r--   0        0        0     1095 2023-05-22 06:01:44.640872 magicwall-0.0.2/magicwall/templates/magicwall.html
+-rw-r--r--   0        0        0     2132 2023-06-18 13:52:12.703419 magicwall-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5986 1970-01-01 00:00:00.000000 magicwall-0.0.2/PKG-INFO
```

### Comparing `magicwall-0.0.1/README.md` & `magicwall-0.0.2/Readme.md`

 * *Files identical despite different names*

### Comparing `magicwall-0.0.1/setup.py` & `magicwall-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,196 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: magicwall
+Version: 0.0.2
+Summary: This is the magic wall (magicwall.io)
+Home-page: https://projects.om-office.de/frans/magicwall.io
+Author: Frans Fürst
+Author-email: frans.fuerst+gitlab@protonmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
+Requires-Dist: checkmk-dev-tools (>=0.1.12,<0.2.0)
+Requires-Dist: exifread (>=3.0.0,<4.0.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://projects.om-office.de/frans/magicwall.io
+Description-Content-Type: text/markdown
 
-packages = \
-['magicwall']
+# magicwall.io
 
-package_data = \
-{'': ['*']}
+View, share, compose, edit visual, textual and acustical content and apply
+arbitraty effects on it.
+
+Consider magicwall a combination of file sharing, content presentation, blogging
+and programmable playground. Create your own wall by just navigating to it, add
+content by dropping or pasting files and arbitrary data from outside, arrange it
+spacially and write code which can be applied to any of that content.
+
+Other people you shared the link to your wall with can copy its content using
+the drag&drop or copy&paste mechanism or by using Git to clone the whole wall
+content.
+
+Use it: [magicwall.io](https://magicwall.io)
+
+Have your own:
+```
+git clone https://projects.om-office.de/frans/magicwall.io
+```
+
+Have Python3.7+ and `flask` installed and run
+```
+magicwall.io/magicwall.py
+```
+
+Or use a Docker container:
+```
+magicwall.io/run-server
+```
+
+Visit the [locally created site](http://localhost:8006)
+
+
+##  Milestone 1
+
+Requirements for basic usage as simple blogging system and for concept
+demonstration.
+
+* [x] <magicwall.io> registered and used with https
+* [x] Previews of files get turned into HTML elements
+* [x] Visualization works (geometry)
+* [x] Create element from dropping a filter element, text or images
+* [x] Drag/drop of element inside wall area moves it
+* [x] Drag/drop of element outside wall area copies as file
+* [x] Drag/drop of element on remove field removes it
+* [x] Pictures get displayed
+* [x] Basic Markdown text formatting works
+* [x] Basic file info on mouse hover
+* [ ] Drag/drop works on mobile
+* [ ] Basic text editing
+* [ ] Basic "filter" work (e.g. b/w for images and running python)
+* [ ] Auto-update (-> collab mode)
+* [ ] Pasting of text, image data or image files works as dropping
+* [ ] Multiple elements can be dropped/pasted at once
+
+
+##  Milestone 2
+
+* [ ] User / access permission control
+* [ ] Arbitrary files can be added for sharing
+* [ ] CTRL+drag&drop copies
+* [ ] Resize elments
+* [ ] Caching mechanism
+* [ ] Square-select multiple items
+
+
+## Future
+
+* Fullscreen / slideshow mode
+* Undo-stack
+* Config-YAML
+* Filter-Hub
+* Search
+* Offline use
+* Git support
+* Editor
+* Links
+* Copy / Paste between sites
+* Video
+* Live-Update (Weather)
+* Support for folders -> Tree
+* Tree-Structure (allows entering)
+* Filter chaining/stacking
+
+
+## Use cases
+
+* Picture gallery
+* Blogging
+* Mind mapping
+* Algorithm demonstration / education (-> Jupyter)
+* File exchange
+* Note taking
+
+
+## Magic ideas
+
+* Simple auto optimize images (contrast, etc)
+* Simple BW images
+* Configurable Image with roation, cropping, color improvement, vignetting
+* Files to animation
+* SVG background
+* Auto align by date
+* fetch URL -> return generated HTML
+
+
+## License
+
+For all code contained in this repository the rules of GPLv3 apply unless
+otherwise noted. That means that you can do what you want with the source
+code as long as you make the files with their original copyright notice
+and all modifications available.
+
+See [GNU / GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) for details.
+
+
+## Contributing
+
+Before contributing consider installing a pre-commit which runs some static
+checks, code cleaners and unit tests:
+
+```
+ln -s ../../.git-pre-commit .git/hooks/pre-commit
+```
+This `pre-commit` just runs `./qualitygate`, which you can also run manually.
+
+
+## Paradigms
+
+* each site can be seen as a filesystem folder managed and visualized by
+  magicwall.io. I.e. applying an arbitrary folder should give nice results
+  magically.
+
+
+## Random ideas
+
+* Visual Filter (looks like polaroid filter and can be moved over arbitrary elements)
+* Transformer filter
+
+
+## Technical challenges
+
+Feel free to help me with each of those questions
+
+* how to recursively stack drop areas
+* how to keep instances across browsers in sync, see
+    - https://developer.mozilla.org/en-US/docs/Web/API/Background_Synchronization_API
+    - https://stackoverflow.com/questions/55700655/store-data-offline-and-sync-once-online-using-react-native-and-redux-store
+
+
+## Read this
+
+* my [to-go scribble](https://notes.om-office.de/tGG_sJgTThut6-v8F72xYQ#)
+
+* https://stackoverflow.com/questions/57014217/putting-an-image-from-flask-to-an-html5-canvas
+* https://stackoverflow.com/questions/10929941/make-drag-and-drop-uploader-in-flask
+* https://codepen.io/anatomic/pen/DJgrvq
+* https://stackoverflow.com/questions/4288253/html5-canvas-100-width-height-of-viewport
+
+* [Dropzone](https://www.dropzone.dev/js/)
+
+* https://www.reddit.com/r/Python/comments/60gl8w/drag_and_drop_files_with_html5_and_flask/
+* http://hundredminutehack.blogspot.com/2017/03/drag-and-drop-files-with-html5-and-flask.html
+
+* https://www.javascripttutorial.net/web-apis/javascript-drag-and-drop/
+* https://stackoverflow.com/questions/10261989/html5-javascript-drag-and-drop-file-from-external-window-windows-explorer
+* https://stackoverflow.com/questions/21339924/drop-event-not-firing-in-chrome
+* https://stackoverflow.com/questions/2438320/html5-dragover-drop-how-get-current-x-y-coordinates
+* https://stackoverflow.com/questions/2075337/uncaught-referenceerror-is-not-defined
+* https://github.com/gokercebeci/droparea
 
-setup_kwargs = {
-    'name': 'magicwall',
-    'version': '0.0.1',
-    'description': 'This is the magic wall (magicwall.io)',
-    'long_description': '# magicwall.io\n\nView, share, compose, edit visual, textual and acustical content and apply\narbitraty effects on it.\n\nConsider magicwall a combination of file sharing, content presentation, blogging\nand programmable playground. Create your own wall by just navigating to it, add\ncontent by dropping or pasting files and arbitrary data from outside, arrange it\nspacially and write code which can be applied to any of that content.\n\nOther people you shared the link to your wall with can copy its content using\nthe drag&drop or copy&paste mechanism or by using Git to clone the whole wall\ncontent.\n\nUse it: [magicwall.io](https://magicwall.io)\n\nHave your own:\n```\ngit clone https://projects.om-office.de/frans/magicwall.io\n```\n\nHave Python3.7+ and `flask` installed and run\n```\nmagicwall.io/magicwall.py\n```\n\nOr use a Docker container:\n```\nmagicwall.io/run-server\n```\n\nVisit the [locally created site](http://localhost:8006)\n\n\n##  Milestone 1\n\nRequirements for basic usage as simple blogging system and for concept\ndemonstration.\n\n* [x] <magicwall.io> registered and used with https\n* [x] Previews of files get turned into HTML elements\n* [x] Visualization works (geometry)\n* [x] Create element from dropping a filter element, text or images\n* [x] Drag/drop of element inside wall area moves it\n* [x] Drag/drop of element outside wall area copies as file\n* [x] Drag/drop of element on remove field removes it\n* [x] Pictures get displayed\n* [x] Basic Markdown text formatting works\n* [x] Basic file info on mouse hover\n* [ ] Drag/drop works on mobile\n* [ ] Basic text editing\n* [ ] Basic "filter" work (e.g. b/w for images and running python)\n* [ ] Auto-update (-> collab mode)\n* [ ] Pasting of text, image data or image files works as dropping\n* [ ] Multiple elements can be dropped/pasted at once\n\n\n##  Milestone 2\n\n* [ ] User / access permission control\n* [ ] Arbitrary files can be added for sharing\n* [ ] CTRL+drag&drop copies\n* [ ] Resize elments\n* [ ] Caching mechanism\n* [ ] Square-select multiple items\n\n\n## Future\n\n* Fullscreen / slideshow mode\n* Undo-stack\n* Config-YAML\n* Filter-Hub\n* Search\n* Offline use\n* Git support\n* Editor\n* Links\n* Copy / Paste between sites\n* Video\n* Live-Update (Weather)\n* Support for folders -> Tree\n* Tree-Structure (allows entering)\n* Filter chaining/stacking\n\n\n## Use cases\n\n* Picture gallery\n* Blogging\n* Mind mapping\n* Algorithm demonstration / education (-> Jupyter)\n* File exchange\n* Note taking\n\n\n## Magic ideas\n\n* Simple auto optimize images (contrast, etc)\n* Simple BW images\n* Configurable Image with roation, cropping, color improvement, vignetting\n* Files to animation\n* SVG background\n* Auto align by date\n* fetch URL -> return generated HTML\n\n\n## License\n\nFor all code contained in this repository the rules of GPLv3 apply unless\notherwise noted. That means that you can do what you want with the source\ncode as long as you make the files with their original copyright notice\nand all modifications available.\n\nSee [GNU / GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) for details.\n\n\n## Contributing\n\nBefore contributing consider installing a pre-commit which runs some static\nchecks, code cleaners and unit tests:\n\n```\nln -s ../../.git-pre-commit .git/hooks/pre-commit\n```\nThis `pre-commit` just runs `./qualitygate`, which you can also run manually.\n\n\n## Paradigms\n\n* each site can be seen as a filesystem folder managed and visualized by\n  magicwall.io. I.e. applying an arbitrary folder should give nice results\n  magically.\n\n\n## Random ideas\n\n* Visual Filter (looks like polaroid filter and can be moved over arbitrary elements)\n* Transformer filter\n\n\n## Technical challenges\n\nFeel free to help me with each of those questions\n\n* how to recursively stack drop areas\n* how to keep instances across browsers in sync, see\n    - https://developer.mozilla.org/en-US/docs/Web/API/Background_Synchronization_API\n    - https://stackoverflow.com/questions/55700655/store-data-offline-and-sync-once-online-using-react-native-and-redux-store\n\n\n## Read this\n\n* my [to-go scribble](https://notes.om-office.de/tGG_sJgTThut6-v8F72xYQ#)\n\n* https://stackoverflow.com/questions/57014217/putting-an-image-from-flask-to-an-html5-canvas\n* https://stackoverflow.com/questions/10929941/make-drag-and-drop-uploader-in-flask\n* https://codepen.io/anatomic/pen/DJgrvq\n* https://stackoverflow.com/questions/4288253/html5-canvas-100-width-height-of-viewport\n\n* [Dropzone](https://www.dropzone.dev/js/)\n\n* https://www.reddit.com/r/Python/comments/60gl8w/drag_and_drop_files_with_html5_and_flask/\n* http://hundredminutehack.blogspot.com/2017/03/drag-and-drop-files-with-html5-and-flask.html\n\n* https://www.javascripttutorial.net/web-apis/javascript-drag-and-drop/\n* https://stackoverflow.com/questions/10261989/html5-javascript-drag-and-drop-file-from-external-window-windows-explorer\n* https://stackoverflow.com/questions/21339924/drop-event-not-firing-in-chrome\n* https://stackoverflow.com/questions/2438320/html5-dragover-drop-how-get-current-x-y-coordinates\n* https://stackoverflow.com/questions/2075337/uncaught-referenceerror-is-not-defined\n* https://github.com/gokercebeci/droparea\n\n\n',
-    'author': 'Frans Fürst',
-    'author_email': 'frans.fuerst+gitlab@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://projects.om-office.de/frans/magicwall.io',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<3.11',
-}
 
 
-setup(**setup_kwargs)
```

