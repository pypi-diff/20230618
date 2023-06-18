# Comparing `tmp/nprompter-3.8.0.tar.gz` & `tmp/nprompter-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nprompter-3.8.0.tar", max compression
+gzip compressed data, was "nprompter-3.9.0.tar", max compression
```

## Comparing `nprompter-3.8.0.tar` & `nprompter-3.9.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0       56 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/__init__.py
--rw-r--r--   0        0        0     3736 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/__main__.py
--rw-r--r--   0        0        0        0 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/api/__init__.py
--rw-r--r--   0        0        0     2092 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/api/notion_client.py
--rw-r--r--   0        0        0        0 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/cli/__init__.py
--rw-r--r--   0        0        0      144 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/cli/defaults.py
--rw-r--r--   0        0        0      907 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/cli/helpers.py
--rw-r--r--   0        0        0        0 2023-04-09 12:47:46.587272 nprompter-3.8.0/nprompter/processing/__init__.py
--rw-r--r--   0        0        0     8049 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/processing/processor.py
--rw-r--r--   0        0        0        0 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/__init__.py
--rw-r--r--   0        0        0    31041 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/android-chrome-192x192.png
--rw-r--r--   0        0        0   128229 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/android-chrome-512x512.png
--rw-r--r--   0        0        0    29064 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/apple-touch-icon.png
--rw-r--r--   0        0        0      845 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/favicon-16x16.png
--rw-r--r--   0        0        0     2274 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/favicon.ico
--rw-r--r--   0        0        0      263 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/assets/site.webmanifest
--rw-r--r--   0        0        0      512 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/nprompter.toml
--rw-r--r--   0        0        0     1223 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/base.html
--rw-r--r--   0        0        0      365 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/index.html
--rw-r--r--   0        0        0     4512 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/nprompter.css
--rw-r--r--   0        0        0      172 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/script.html
--rw-r--r--   0        0        0     6750 2023-04-09 12:47:46.591272 nprompter-3.8.0/nprompter/web/templates/script.js
--rw-r--r--   0        0        0     1379 2023-04-09 12:47:46.591272 nprompter-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     1008 2023-04-09 12:48:27.488654 nprompter-3.8.0/setup.py
--rw-r--r--   0        0        0      688 2023-04-09 12:48:27.488926 nprompter-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/__init__.py
+-rw-r--r--   0        0        0     3736 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/api/__init__.py
+-rw-r--r--   0        0        0     2092 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/api/notion_client.py
+-rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/cli/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/cli/defaults.py
+-rw-r--r--   0        0        0      907 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/cli/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/processing/__init__.py
+-rw-r--r--   0        0        0     8053 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/processing/processor.py
+-rw-r--r--   0        0        0        0 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/__init__.py
+-rw-r--r--   0        0        0    31041 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/android-chrome-192x192.png
+-rw-r--r--   0        0        0   128229 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7204 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/app.js
+-rw-r--r--   0        0        0    29064 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/apple-touch-icon.png
+-rw-r--r--   0        0        0      845 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/favicon-16x16.png
+-rw-r--r--   0        0        0     2274 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/favicon.ico
+-rw-r--r--   0        0        0      263 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/assets/site.webmanifest
+-rw-r--r--   0        0        0      512 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/nprompter.toml
+-rw-r--r--   0        0        0     1265 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/base.html
+-rw-r--r--   0        0        0      365 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/index.html
+-rw-r--r--   0        0        0     4512 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/nprompter.css
+-rw-r--r--   0        0        0      172 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/script.html
+-rw-r--r--   0        0        0     1435 2023-06-18 07:25:18.963411 nprompter-3.9.0/nprompter/web/templates/settings.js
+-rw-r--r--   0        0        0     1379 2023-06-18 07:25:18.967411 nprompter-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1008 2023-06-18 07:26:03.383093 nprompter-3.9.0/setup.py
+-rw-r--r--   0        0        0      688 2023-06-18 07:26:03.383386 nprompter-3.9.0/PKG-INFO
```

### Comparing `nprompter-3.8.0/nprompter/__main__.py` & `nprompter-3.9.0/nprompter/__main__.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/api/notion_client.py` & `nprompter-3.9.0/nprompter/api/notion_client.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/cli/helpers.py` & `nprompter-3.9.0/nprompter/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/processing/processor.py` & `nprompter-3.9.0/nprompter/processing/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         self.configuration = configuration or {}
         self.custom_css = []
 
     def prepare_folder(self, configuration: Dict):
         if not self.output_folder.exists():
             self.output_folder.mkdir(parents=True)
 
-        js_template = self.env.get_template("script.js")
+        js_template = self.env.get_template("settings.js")
         css_template = self.env.get_template("nprompter.css")
 
-        with open(self.output_folder / "script.js", "w", encoding="utf8") as writeable:
+        with open(self.output_folder / "settings.js", "w", encoding="utf8") as writeable:
             writeable.write(js_template.render(**configuration))
 
         with open(self.output_folder / "nprompter.css", "w", encoding="utf8") as writeable:
             writeable.write(css_template.render(**configuration))
 
         shutil.copytree(self.assets_folder, self.output_folder, dirs_exist_ok=True)
```

### Comparing `nprompter-3.8.0/nprompter/web/assets/android-chrome-192x192.png` & `nprompter-3.9.0/nprompter/web/assets/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/assets/android-chrome-512x512.png` & `nprompter-3.9.0/nprompter/web/assets/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/assets/apple-touch-icon.png` & `nprompter-3.9.0/nprompter/web/assets/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/assets/favicon-16x16.png` & `nprompter-3.9.0/nprompter/web/assets/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/assets/favicon-32x32.png` & `nprompter-3.9.0/nprompter/web/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/assets/favicon.ico` & `nprompter-3.9.0/nprompter/web/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/nprompter.toml` & `nprompter-3.9.0/nprompter/web/nprompter.toml`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/templates/base.html` & `nprompter-3.9.0/nprompter/web/templates/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -23,10 +23,11 @@
             <div class="modal-bg modal-exit"></div>
             <div class="modal-container">
                 <h2>Help - v{{ version }}</h2>
                 <ul id="help"></ul>
             </div>
         </div>
         <div id="snackbar" class="mirror mirrored">Some text some message..</div>
-        <script src="/script.js"></script>
+        <script src="/settings.js"></script>
+        <script src="/app.js"></script>
     </body>
 </html>
```

### Comparing `nprompter-3.8.0/nprompter/web/templates/nprompter.css` & `nprompter-3.9.0/nprompter/web/templates/nprompter.css`

 * *Files identical despite different names*

### Comparing `nprompter-3.8.0/nprompter/web/templates/script.js` & `nprompter-3.9.0/nprompter/web/assets/app.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,68 +1,22 @@
 const content = document.getElementById('content')
 const mirrorElements = Array.from(document.getElementsByClassName('mirror'))
 const modal = document.getElementById('modal')
 const elem = document.documentElement;
 const snackbar = document.getElementById("snackbar");
-const manualScrollAmount = 40;
-const fontSizeIncrease = {
-    {
-        font.size_increment
-    }
-};
-const paddingSizeIncrease = {
-    {
-        screen.padding.increment
-    }
-};
-const maxScrollSpeed = {
-    {
-        screen.scroll.max_speed
-    }
-};
-const scrollSpeedIncrease = {
-    {
-        screen.scroll.speed_increment
-    }
-};
-const maxPadding = {
-    {
-        screen.padding.max_value
-    }
-};
-const maxFontSize = {
-    {
-        font.max_size
-    }
-};
-const minLineHeight = 0.1;
-const lineHeightIncrement = {
-    {
-        font.line_height_increment
-    }
-};
-const snackbarTimeout = 500;
-let lineHeight = {
-    {
-        font.line_height
-    }
-};
-let fontSize = parseInt(getComputedStyle(content).fontSize);
-let paddingSize = parseInt(getComputedStyle(content).paddingLeft);
+let isScrolling = false
 let scrollTimer = 0;
 let snackbarTimer = -1;
-let isScrolling = false;
-let scrollSpeed = {
-    {
-        screen.scroll.speed
-    }
-};
-
 
 document.addEventListener('keydown', logKey);
+setFontSize(getSetting("fontSize"))
+setPadding(getSetting("paddingSize"))
+setLineHeight(getSetting("lineHeight"))
+
+
 
 function logKey(e) {
     const keyCode = e.keyCode;
     if (handleKeyCode(keyCode)) {
         e.preventDefault();
     }
 }
@@ -85,65 +39,89 @@
 
 function scrollToTop() {
     window.scrollTo(0, 0)
     return "Scrolled to top"
 }
 
 function decreaseSpeed() {
-    scrollSpeed = Math.min(maxScrollSpeed, scrollSpeed + scrollSpeedIncrease)
+    const scrollSpeed = Math.min(maxScrollSpeed, getSetting("scrollSpeed") + scrollSpeedIncrease);
+    saveSetting("scrollSpeed", scrollSpeed)
     return `Scroll speed: ${scrollSpeed}`
 }
 
 function increaseSpeed() {
-    scrollSpeed = Math.max(0, scrollSpeed - scrollSpeedIncrease)
+    const scrollSpeed = Math.max(0, getSetting("scrollSpeed") - scrollSpeedIncrease)
+    saveSetting("scrollSpeed", scrollSpeed)
     return `Scroll speed: ${scrollSpeed}`
 }
 
-function decreaseFontSize() {
-    fontSize = Math.max(0, fontSize - fontSizeIncrease);
-    content.style.fontSize = fontSize + "px"
-    return `Font size: ${fontSize}`
+function setLineHeight(lineHeight) {
+    content.style.lineHeight = lineHeight + "em"
 }
 
 function increaseLineHeight() {
-    lineHeight = lineHeight + lineHeightIncrement;
-    content.style.lineHeight = lineHeight + "em"
-    return `Line height: ${lineHeight}`
+    const newLineHeight = getSetting("lineHeight") + lineHeightIncrement
+    setLineHeight(newLineHeight)
+    saveSetting("lineHeight", newLineHeight)
+    return `Line height: ${newLineHeight}`
 }
 
 function decreaseLineHeight() {
-    lineHeight = Math.max(minLineHeight, lineHeight - lineHeightIncrement);
-    content.style.lineHeight = lineHeight + "em"
-    return `Line height: ${lineHeight}`
+    const currentLineHeight = getSetting("lineHeight")
+    const newLineHeight = Math.max(minLineHeight, currentLineHeight - lineHeightIncrement);
+    setLineHeight(newLineHeight)
+    saveSetting("lineHeight", newLineHeight)
+    return `Line height: ${newLineHeight}`
 }
 
 function mirrorScreen() {
     mirrorElements.forEach(function(element) {
         element.classList.toggle('mirrored')
     })
 }
 
-function decreasePadding() {
-    paddingSize = Math.max(0, paddingSize - paddingSizeIncrease);
+function setPadding(paddingSize) {
     content.style.paddingLeft = paddingSize + "px"
     content.style.paddingRight = paddingSize + "px"
-    return `Padding size: ${paddingSize}`
+}
+
+function decreasePadding() {
+    const currentPadding = getSetting("paddingSize")
+    const newPaddingSize = Math.max(0, currentPadding - paddingSizeIncrease);
+    setPadding(newPaddingSize)
+    saveSetting("paddingSize", newPaddingSize)
+    return `Padding size: ${newPaddingSize}`
 }
 
 function increasePadding() {
-    paddingSize = Math.min(maxPadding, paddingSize + paddingSizeIncrease);
-    content.style.paddingLeft = paddingSize + "px"
-    content.style.paddingRight = paddingSize + "px"
-    return `Padding size: ${paddingSize}`
+    const currentPadding = getSetting("paddingSize")
+    const newPadding = Math.min(maxPadding, currentPadding + paddingSizeIncrease);
+    setPadding(newPadding)
+    saveSetting("paddingSize", newPadding)
+    return `Padding size: ${newPadding}`
 }
 
-function increaseFontSize() {
-    fontSize = Math.min(maxFontSize, fontSize + fontSizeIncrease);
+function setFontSize(fontSize) {
     content.style.fontSize = fontSize + "px"
-    return `Font size: ${fontSize}`
+}
+
+function increaseFontSize() {
+    const currentFontSize = getSetting("fontSize")
+    const newFontSize = Math.min(maxFontSize, currentFontSize + fontSizeIncrease);
+    setFontSize(newFontSize)
+    saveSetting("fontSize", newFontSize)
+    return `Font size: ${newFontSize}`
+}
+
+function decreaseFontSize() {
+    const currentFontSize = getSetting("fontSize")
+    const newFontSize = Math.max(0, currentFontSize - fontSizeIncrease);
+    setFontSize(newFontSize)
+    saveSetting("fontSize", newFontSize)
+    return `Font size: ${newFontSize}`
 }
 
 function debugInfo() {
     const properties = new Map([
         ["Font size", fontSize],
         ["Padding size", paddingSize],
         ["Scroll speed", scrollSpeed]
@@ -159,37 +137,35 @@
         colors.push(red)
         colors.push(black)
     })
     console.log(propertyList.join(' '), ...colors)
 }
 
 const controls = {
-    27: [scrollToTop, "Scroll to top", 'escape'],
-    32: [toggleScrolling, "Start scroll", 'space'],
-    37: [decreaseSpeed, "Decrease speed", '→'],
-    39: [increaseSpeed, "Increase speed", '←'],
-    68: [decreaseFontSize, "Decrease font size", 'D'],
-    70: [openFullscreen, "Fullscreen", 'f'],
-    72: [toggleModalWindow, "Help", 'h'],
-    73: [debugInfo, "Show debug info to the console", 'i'],
-    77: [mirrorScreen, "Mirror screen", 'm'],
-    79: [decreasePadding, "Decrease padding", 'o'],
-    80: [increasePadding, "Increase padding", 'p'],
-    81: [decreaseLineHeight, "Decrease padding", 'q'],
-    87: [increaseLineHeight, "Increase padding", 'w'],
-    85: [increaseFontSize, "Increase font size", 'u']
-}
-
-const urlParams = new URLSearchParams(window.location.search);
-if (urlParams.get('presenterMode')) {
-    controls[116] = [toggleScrolling, "Scroll", 'F5']
-    controls[34] = [increaseSpeed, "Scroll", 'F5']
-    controls[33] = [decreaseSpeed, "Scroll", 'F5']
-    controls[27] = [scrollUpManually, "Scroll", 'F5']
-    controls[66] = [scrollDownManually, "Scroll", 'F5']
+    // Normal controls
+    27: [scrollUpManually, "Manual scroll up", "ESC"], // Esc key
+    32: [toggleScrolling, "Start scroll", 'space'], // Space key
+    37: [decreaseSpeed, "Decrease speed", '→'], // Right arrow
+    39: [increaseSpeed, "Increase speed", '←'], // Left arrow
+    68: [decreaseFontSize, "Decrease font size", 'D'], // D key
+    70: [openFullscreen, "Fullscreen", 'f'], // F key
+    72: [toggleModalWindow, "Help", 'h'], // H key
+    73: [debugInfo, "Show debug info to the console", 'i'], // I key
+    77: [mirrorScreen, "Mirror screen", 'm'], // M key
+    79: [decreasePadding, "Decrease padding", 'o'], // O key
+    80: [increasePadding, "Increase padding", 'p'], // P key
+    81: [decreaseLineHeight, "Decrease padding", 'q'], // Q key
+    87: [increaseLineHeight, "Increase padding", 'w'], // W key
+    88: [scrollToTop, "Scroll to top", 'x'], // X key
+    85: [increaseFontSize, "Increase font size", 'u'], // U key
+    // Presenter mode controls
+    116: [toggleScrolling, "Toggle scrolling", 'F5'], // F5 key
+    34: [increaseSpeed, "Increase speed", 'PageDown'], // PageDown key
+    33: [decreaseSpeed, "Decrease speed", 'PageUp'], // PageUp key
+    66: [scrollDownManually, "Scroll down manually", 'B'] // B key
 }
 
 function handleKeyCode(keyCode) {
     let handled = true;
     if (keyCode in controls) {
         const [action, docs, key] = controls[keyCode]
         const result = action()
@@ -208,15 +184,15 @@
 
 function scrollDownManually() {
     window.scrollBy(0, manualScrollAmount);
 }
 
 function pageScroll() {
     window.scrollBy(0, 1); // horizontal and vertical scroll increments
-    scrollTimer = setTimeout(pageScroll, scrollSpeed);
+    scrollTimer = setTimeout(pageScroll, getSetting("scrollSpeed"));
 }
 
 function toggleScrolling() {
     if (isScrolling === false) {
         pageScroll()
         isScrolling = true;
         return "Scrolling started"
```

### Comparing `nprompter-3.8.0/pyproject.toml` & `nprompter-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nprompter"
-version = "3.8.0"
+version = "3.9.0"
 description = "A web based teleprompter that uses Notion as a storage backend"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 nprompter = 'nprompter.__main__:app'
```

### Comparing `nprompter-3.8.0/setup.py` & `nprompter-3.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'typer>=0.4.1,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['nprompter = nprompter.__main__:app']}
 
 setup_kwargs = {
     'name': 'nprompter',
-    'version': '3.8.0',
+    'version': '3.9.0',
     'description': 'A web based teleprompter that uses Notion as a storage backend',
     'long_description': None,
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nprompter-3.8.0/PKG-INFO` & `nprompter-3.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nprompter
-Version: 3.8.0
+Version: 3.9.0
 Summary: A web based teleprompter that uses Notion as a storage backend
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

