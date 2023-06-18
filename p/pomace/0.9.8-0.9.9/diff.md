# Comparing `tmp/pomace-0.9.8.tar.gz` & `tmp/pomace-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomace-0.9.8.tar", max compression
+gzip compressed data, was "pomace-0.9.9.tar", max compression
```

## Comparing `pomace-0.9.8.tar` & `pomace-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1088 2020-05-10 20:24:32.000000 pomace-0.9.8/LICENSE.md
--rw-r--r--   0        0        0     1535 2021-08-08 17:57:21.587237 pomace-0.9.8/README.md
--rw-r--r--   0        0        0      303 2021-11-16 12:40:42.131290 pomace-0.9.8/pomace/__init__.py
--rw-r--r--   0        0        0      157 2021-11-16 12:40:42.131802 pomace-0.9.8/pomace/__main__.py
--rw-r--r--   0        0        0     1224 2021-11-16 12:40:42.132229 pomace-0.9.8/pomace/api.py
--rw-r--r--   0        0        0     4605 2022-01-29 20:22:23.999804 pomace-0.9.8/pomace/browser.py
--rw-r--r--   0        0        0     6665 2022-01-29 19:35:08.232426 pomace-0.9.8/pomace/cli.py
--rw-r--r--   0        0        0      659 2022-01-29 18:53:02.456662 pomace-0.9.8/pomace/compat.py
--rw-r--r--   0        0        0     2637 2022-01-29 20:12:45.001745 pomace-0.9.8/pomace/config.py
--rw-r--r--   0        0        0     4411 2022-01-29 02:57:01.489417 pomace-0.9.8/pomace/enums.py
--rw-r--r--   0        0        0    17310 2022-01-29 20:15:42.909208 pomace-0.9.8/pomace/models.py
--rw-r--r--   0        0        0      694 2021-08-17 18:49:15.841792 pomace-0.9.8/pomace/patched.py
--rw-r--r--   0        0        0     4913 2022-01-29 02:57:01.490806 pomace-0.9.8/pomace/prompts.py
--rw-r--r--   0        0        0      961 2022-01-28 19:06:49.579955 pomace-0.9.8/pomace/server.py
--rw-r--r--   0        0        0     2679 2022-01-29 20:38:07.809440 pomace-0.9.8/pomace/shared.py
--rw-r--r--   0        0        0       34 2020-05-10 20:24:32.000000 pomace-0.9.8/pomace/tests/__init__.py
--rw-r--r--   0        0        0     1876 2021-03-25 15:10:16.930632 pomace-0.9.8/pomace/tests/cassettes/it_computes_values_based_on_the_html.yaml
--rw-r--r--   0        0        0     1166 2021-04-09 23:24:48.583000 pomace-0.9.8/pomace/tests/conftest.py
--rw-r--r--   0        0        0     1020 2022-01-29 18:53:02.458464 pomace-0.9.8/pomace/tests/test_browser.py
--rw-r--r--   0        0        0     1085 2021-04-11 00:45:47.743734 pomace-0.9.8/pomace/tests/test_enums.py
--rw-r--r--   0        0        0     8043 2021-08-17 18:49:15.842154 pomace-0.9.8/pomace/tests/test_models.py
--rw-r--r--   0        0        0     1132 2021-01-28 23:02:04.795722 pomace-0.9.8/pomace/tests/test_prompts.py
--rw-r--r--   0        0        0     6024 2022-01-28 19:06:49.580651 pomace-0.9.8/pomace/tests/test_types.py
--rw-r--r--   0        0        0     6138 2022-01-29 18:53:02.459147 pomace-0.9.8/pomace/types.py
--rw-r--r--   0        0        0     3685 2022-01-29 20:22:56.302220 pomace-0.9.8/pomace/utils.py
--rw-r--r--   0        0        0     2404 2022-01-29 19:37:25.020745 pomace-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2936 2022-01-29 20:40:53.675754 pomace-0.9.8/setup.py
--rw-r--r--   0        0        0     3354 2022-01-29 20:40:53.676234 pomace-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2020-10-23 18:26:14.199957 pomace-0.9.9/LICENSE.md
+-rw-r--r--   0        0        0     1535 2021-08-03 15:58:50.946848 pomace-0.9.9/README.md
+-rw-r--r--   0        0        0      303 2021-10-11 02:49:30.886927 pomace-0.9.9/pomace/__init__.py
+-rw-r--r--   0        0        0      157 2021-10-11 02:49:30.887575 pomace-0.9.9/pomace/__main__.py
+-rw-r--r--   0        0        0     1224 2021-10-11 02:49:30.889006 pomace-0.9.9/pomace/api.py
+-rw-r--r--   0        0        0     4667 2022-01-29 23:36:58.457916 pomace-0.9.9/pomace/browser.py
+-rw-r--r--   0        0        0     6665 2021-10-11 02:49:30.890617 pomace-0.9.9/pomace/cli.py
+-rw-r--r--   0        0        0      659 2022-01-29 21:57:19.960357 pomace-0.9.9/pomace/compat.py
+-rw-r--r--   0        0        0     2637 2022-01-29 21:57:19.960758 pomace-0.9.9/pomace/config.py
+-rw-r--r--   0        0        0     4674 2022-01-29 23:32:41.857399 pomace-0.9.9/pomace/enums.py
+-rw-r--r--   0        0        0    17295 2022-01-29 22:56:11.512212 pomace-0.9.9/pomace/models.py
+-rw-r--r--   0        0        0      694 2021-08-19 21:52:43.673613 pomace-0.9.9/pomace/patched.py
+-rw-r--r--   0        0        0     4913 2022-01-28 23:22:04.076192 pomace-0.9.9/pomace/prompts.py
+-rw-r--r--   0        0        0      961 2022-01-28 22:59:44.194349 pomace-0.9.9/pomace/server.py
+-rw-r--r--   0        0        0     2961 2022-01-29 23:37:27.121261 pomace-0.9.9/pomace/shared.py
+-rw-r--r--   0        0        0       34 2020-10-23 18:26:14.203745 pomace-0.9.9/pomace/tests/__init__.py
+-rw-r--r--   0        0        0     1876 2021-03-27 18:36:49.315623 pomace-0.9.9/pomace/tests/cassettes/it_computes_values_based_on_the_html.yaml
+-rw-r--r--   0        0        0     1166 2021-08-19 22:18:49.940371 pomace-0.9.9/pomace/tests/conftest.py
+-rw-r--r--   0        0        0     1020 2022-01-29 21:57:19.962193 pomace-0.9.9/pomace/tests/test_browser.py
+-rw-r--r--   0        0        0     1085 2021-04-12 23:00:15.149422 pomace-0.9.9/pomace/tests/test_enums.py
+-rw-r--r--   0        0        0     8043 2021-08-19 21:52:43.674091 pomace-0.9.9/pomace/tests/test_models.py
+-rw-r--r--   0        0        0     1132 2020-12-27 05:55:58.687666 pomace-0.9.9/pomace/tests/test_prompts.py
+-rw-r--r--   0        0        0     6024 2022-01-28 22:59:44.194980 pomace-0.9.9/pomace/tests/test_types.py
+-rw-r--r--   0        0        0     6138 2022-01-29 21:57:19.962529 pomace-0.9.9/pomace/types.py
+-rw-r--r--   0        0        0     3685 2022-01-29 21:57:19.962849 pomace-0.9.9/pomace/utils.py
+-rw-r--r--   0        0        0     2404 2022-01-29 23:36:31.131122 pomace-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2936 2022-01-29 23:39:38.573680 pomace-0.9.9/setup.py
+-rw-r--r--   0        0        0     3354 2022-01-29 23:39:38.573979 pomace-0.9.9/PKG-INFO
```

### Comparing `pomace-0.9.8/LICENSE.md` & `pomace-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/README.md` & `pomace-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/api.py` & `pomace-0.9.9/pomace/api.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/browser.py` & `pomace-0.9.9/pomace/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
         log.debug(f"Saving last browser URL: {url}")
         settings.url = url
 
 
 def save_size(browser: GenericBrowser):
     if isinstance(browser, PlaywrightBrowser):
         page = browser.contexts[0].pages[0]
+        # TODO: Figure out how to get the window size instead
         size: dict = page.viewport_size  # type: ignore
     else:
         size = browser.driver.get_window_size()
 
     if size != (settings.browser.width, settings.browser.height):
         log.debug(f"Saving last browser size: {size}")
         settings.browser.width = size["width"]
```

### Comparing `pomace-0.9.8/pomace/cli.py` & `pomace-0.9.9/pomace/cli.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/compat.py` & `pomace-0.9.9/pomace/compat.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/config.py` & `pomace-0.9.9/pomace/config.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/enums.py` & `pomace-0.9.9/pomace/enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,17 +35,22 @@
 
         return getattr(shared.browser, f"find_by_{self.value}")
 
     def find(self, value) -> GenericElement:
         if self is self.ARIA_LABEL:
             value = f'[aria-label="{value}"]'
         elif isinstance(shared.browser, PlaywrightBrowser):
-            if self is not self.CSS:
+            if self is self.TEXT:
+                value = f"text={value!r}"
+            elif self is self.PARTIAL_TEXT:
+                value = f"text={value}"
+            elif self in [self.ID]:
                 value = f"{self.value}={value}"
-
+            elif self not in [self.CSS, self.XPATH]:
+                value = f"[{self.value}={value!r}]"
         return self.finder(value)
 
 
 class Verb(Enum):
     CLICK = "click"
     FILL = "fill"
     SELECT = "select"
```

### Comparing `pomace-0.9.8/pomace/models.py` & `pomace-0.9.9/pomace/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,27 +438,27 @@
                 return action
 
         return object.__getattribute__(self, value)
 
     def __contains__(self, value):
         return value in self.text
 
-    def perform(self, name: str, value: str = "", _logger=None) -> Tuple["Page", bool]:
-        _logger = _logger or log
+    def perform(self, name: str, value: str = "", _log=None) -> Tuple["Page", bool]:
+        _log = _log or log
         action = getattr(self, name)
         if action.verb in {"fill", "select"}:
             if not value:
                 value = settings.get_secret(action.name) or prompts.named_value(
                     action.name
                 )
                 settings.update_secret(action.name, value)
-            _logger.info(f"{action.humanized} with {value!r}")
+            _log.info(f"{action.humanized} with {value!r}")
             page = action(value, _page=self)
         else:
-            _logger.info(f"{action.humanized}")
+            _log.info(f"{action.humanized}")
             page = action(_page=self)
         return page, page != self
 
     def clean(self, *, force: bool = False) -> int:
         count = self.locators.clean(self, force=force)
 
         unused_actions = []
```

### Comparing `pomace-0.9.8/pomace/patched.py` & `pomace-0.9.9/pomace/patched.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/prompts.py` & `pomace-0.9.9/pomace/prompts.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/server.py` & `pomace-0.9.9/pomace/server.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/shared.py` & `pomace-0.9.9/pomace/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     @property
     def page(self) -> Page:
         # Raises an AttributeError for non-Playwright browsers
         return browser.contexts[0].pages[0]
 
     @property
     def url(self) -> str:
+        if browser is None:
+            return ""
+
         if isinstance(browser, PlaywrightBrowser):
             self.page.bring_to_front()
             return self.page.url
 
         return browser.url
 
     @property
@@ -83,9 +86,17 @@
             ActionChains(browser.driver)
             .key_down(modifier)
             .send_keys(key)
             .key_up(modifier)
             .perform
         )
 
+    @staticmethod
+    def clear_cookies():
+        log.info("Clearing cookies")
+        if isinstance(browser, PlaywrightBrowser):
+            browser.contexts[0].clear_cookies()
+        else:
+            browser.cookies.delete()
+
 
 client = _Client()
```

### Comparing `pomace-0.9.8/pomace/tests/cassettes/it_computes_values_based_on_the_html.yaml` & `pomace-0.9.9/pomace/tests/cassettes/it_computes_values_based_on_the_html.yaml`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/tests/conftest.py` & `pomace-0.9.9/pomace/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/tests/test_browser.py` & `pomace-0.9.9/pomace/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/tests/test_enums.py` & `pomace-0.9.9/pomace/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/tests/test_models.py` & `pomace-0.9.9/pomace/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/tests/test_prompts.py` & `pomace-0.9.9/pomace/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/tests/test_types.py` & `pomace-0.9.9/pomace/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/types.py` & `pomace-0.9.9/pomace/types.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pomace/utils.py` & `pomace-0.9.9/pomace/utils.py`

 * *Files identical despite different names*

### Comparing `pomace-0.9.8/pyproject.toml` & `pomace-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "pomace"
-version = "0.9.8"
+version = "0.9.9"
 description = "Dynamic page objects for browser automation."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `pomace-0.9.8/setup.py` & `pomace-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 {':platform_machine != "armv7l"': ['playwright>=1.18,<2.0']}
 
 entry_points = \
 {'console_scripts': ['pomace = pomace.cli:application.run']}
 
 setup_kwargs = {
     'name': 'pomace',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Dynamic page objects for browser automation.',
     'long_description': "# Pomace\n\nDynamic page objects for browser automation.\n\n[![Unix Build Status](https://img.shields.io/github/workflow/status/jacebrowning/pomace/main?label=unix)](https://github.com/jacebrowning/pomace/actions?query=branch%3Amain)\n[![Windows Build Status](https://img.shields.io/appveyor/ci/jacebrowning/pomace/main.svg?label=window)](https://ci.appveyor.com/project/jacebrowning/pomace)\n[![Coverage Status](https://img.shields.io/codecov/c/gh/jacebrowning/pomace)](https://codecov.io/gh/jacebrowning/pomace)\n[![PyPI Version](https://img.shields.io/pypi/v/pomace.svg)](https://pypi.org/project/pomace)\n[![PyPI License](https://img.shields.io/pypi/l/pomace.svg)](https://pypi.org/project/pomace)\n\n## Quick Start\n\nOpen **Terminal.app** in macOS and paste:\n\n```shell\npython3 -m pip install --upgrade pomace && python3 -m pomace run\n```\n\nor if you have Homebrew:\n\n```shell\nbrew install pipx; pipx run --no-cache pomace run\n```\n\n## Full Demo\n\nIf you're planning to run Pomace multiple times, install it with [pipx](https://pipxproject.github.io/pipx/) first:\n\n```shell\npipx install pomace\n```\n\nor get the latest version:\n\n```shell\npipx upgrade pomace\n```\n\nThen download some site models:\n\n```shell\npomace clone https://github.com/jacebrowning/pomace-twitter.com\n```\n\nAnd launch the application:\n\n```shell\npomace run twitter.com\n```\n\n# Usage\n\nInstall this library directly into an activated virtual environment:\n\n```shell\npip install pomace\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```shell\npoetry add pomace\n```\n",
     'author': 'Jace Browning',
     'author_email': 'jacebrowning@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/pomace',
```

### Comparing `pomace-0.9.8/PKG-INFO` & `pomace-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomace
-Version: 0.9.8
+Version: 0.9.9
 Summary: Dynamic page objects for browser automation.
 Home-page: https://pypi.org/project/pomace
 License: MIT
 Keywords: browser automation,page object model,selenium,splinter
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
```

