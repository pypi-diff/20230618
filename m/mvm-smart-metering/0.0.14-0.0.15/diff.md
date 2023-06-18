# Comparing `tmp/mvm_smart_metering-0.0.14.tar.gz` & `tmp/mvm_smart_metering-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvm_smart_metering-0.0.14.tar", max compression
+gzip compressed data, was "mvm_smart_metering-0.0.15.tar", max compression
```

## Comparing `mvm_smart_metering-0.0.14.tar` & `mvm_smart_metering-0.0.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      286 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/README.md
--rw-r--r--   0        0        0       78 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/mvm_smart_meter/__init__.py
--rw-r--r--   0        0        0    16148 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/mvm_smart_meter/smart_meter.py
--rw-r--r--   0        0        0      501 2023-06-10 10:28:46.619204 mvm_smart_metering-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.14/setup.py
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-06-18 17:51:41.670975 mvm_smart_metering-0.0.15/README.md
+-rw-r--r--   0        0        0       78 2023-06-18 17:51:41.670975 mvm_smart_metering-0.0.15/mvm_smart_meter/__init__.py
+-rw-r--r--   0        0        0    17043 2023-06-18 17:51:41.670975 mvm_smart_metering-0.0.15/mvm_smart_meter/smart_meter.py
+-rw-r--r--   0        0        0      501 2023-06-18 17:51:41.674975 mvm_smart_metering-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.15/setup.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 mvm_smart_metering-0.0.15/PKG-INFO
```

### Comparing `mvm_smart_metering-0.0.14/mvm_smart_meter/smart_meter.py` & `mvm_smart_metering-0.0.15/mvm_smart_meter/smart_meter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,41 @@
 from webdriver_manager.firefox import GeckoDriverManager
 from selenium.webdriver.firefox.service import Service
 from selenium.webdriver.firefox.options import Options
 import pandas
 import io
 
 
+class GuidNotFoundException(Exception):
+    """
+    Exception raised when the GUID is not found in a URL.
+
+    :param message: Custom error message describing the exception. Defaults to "Guid not found in URL".
+    :type message: str
+    :param url: URL where the GUID was not found. Defaults to None.
+    :type url: str
+
+    :ivar message: Custom error message describing the exception.
+    :ivar url: URL where the GUID was not found.
+    """
+
+    def __init__(self, message="Guid not found in URL", url=None):
+        """
+        Initialize a GuidNotFoundException instance.
+
+        :param message: Custom error message. Defaults to "Guid not found in URL".
+        :type message: str
+        :param url: URL where the GUID was not found. Defaults to None.
+        :type url: str
+        """
+        self.message = message
+        self.url = url
+        super().__init__(f"{self.message}: {url}")
+
+
 class Smart_meter:
     """All the main function to gather date from the smart metering site is gathered here"""
 
     def __init__(self, username: str, password: str):
         self.options = Options()
         self.options.add_argument("--headless")
 
@@ -112,30 +139,30 @@
         """The smart metering site is on a external site, this function gets thoose links into a list."""
         custumer_meters_url = f"https://eloszto.mvmemaszhalozat.hu/sap/opu/odata/sap/ZGW_UGYFELSZOLGALAT_SRV/Felhelyek(Vevo='{self.custumer_number}',Id='{self.customer_id}')/Okosmero"
         querystring = {"sap-client": "112", "sap-language": "HU"}
         r = self.s.get(custumer_meters_url, headers=self.headers, params=querystring)
         r_list = r.json()["d"]["results"]
         self.meter_ids = r.json()["d"]["results"]
         self.smart_meter_links = []
-        print(r_list)
+
         for link in r_list:
-  
-            if link["URL"].find("guid=&") == -1:
-                split_url = link["URL"].split("?")
-                query_string = split_url[1]
-
-                query_string_list = query_string.split("&")
-
-                query_dict = {"url": split_url[0], "meter_id": link["FogyMeroAzon"]}
-  
-                for item in query_string_list:
-                    key, value = item.split("=")
-                    query_dict[key] = value
-    
-                self.smart_meter_links.append(query_dict)
+            if link["URL"].find("guid=&") != -1:
+                raise GuidNotFoundException(url=link)
+            split_url = link["URL"].split("?")
+            query_string = split_url[1]
+
+            query_string_list = query_string.split("&")
+
+            query_dict = {"url": split_url[0], "meter_id": link["FogyMeroAzon"]}
+
+            for item in query_string_list:
+                key, value = item.split("=")
+                query_dict[key] = value
+
+            self.smart_meter_links.append(query_dict)
 
     def get_cookies_smart_meter_site(self):
         """Get cookies from the main site.Need to find a workaround as requestium uses old version of selenium."""
         # TODO get around without using selenium
 
         self.smart_meter_url = f"{self.smart_meter_links[0]['url']}"
         # print(f"Smart meter link : {smart_meter_url}")
```

### Comparing `mvm_smart_metering-0.0.14/setup.py` & `mvm_smart_metering-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'python-dotenv==1.0.0',
  'requestium==0.2.1',
  'requests>=2.28.2,<3.0.0',
  'webdriver-manager>=3.8.5,<4.0.0']
 
 setup_kwargs = {
     'name': 'mvm-smart-metering',
-    'version': '0.0.14',
+    'version': '0.0.15',
     'description': 'Script for scraping mvm smart meter data',
     'long_description': '# MVM Smart Metering\nThis is a automation tool for collecting load curve from mvm smart metering site\n\n---\n\nInstallation:\n\n```bash\npip install mvm-smart-metering\n```\n\nor\n\n```bash\npoetry add mvm-smart-metering\n```\n\n\n\n[Documantion](https://ktomi96.github.io/mvm_smart_metering/)\n\n---\n\n\n\n\n',
     'author': 'ktomi96',
     'author_email': 'kokai.tamas.96@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mvm_smart_metering-0.0.14/PKG-INFO` & `mvm_smart_metering-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvm-smart-metering
-Version: 0.0.14
+Version: 0.0.15
 Summary: Script for scraping mvm smart meter data
 Author: ktomi96
 Author-email: kokai.tamas.96@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
```

