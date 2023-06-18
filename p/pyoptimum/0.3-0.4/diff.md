# Comparing `tmp/pyoptimum-0.3.tar.gz` & `tmp/pyoptimum-0.4.tar.gz`

## Comparing `pyoptimum-0.3.tar` & `pyoptimum-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pyoptimum-0.3/.readthedocs.yaml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.3/requirements.txt
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyoptimum-0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pyoptimum-0.3/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/Makefile
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/conf.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/make.bat
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/requirements.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/src/modules.rst
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 pyoptimum-0.3/doc/src/quickstart.rst
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 pyoptimum-0.3/src/pyoptimum/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyoptimum-0.3/tests/__init__.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pyoptimum-0.3/tests/test_basic.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyoptimum-0.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyoptimum-0.3/LICENSE
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 pyoptimum-0.3/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyoptimum-0.3/pyproject.toml
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyoptimum-0.3/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pyoptimum-0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.4/requirements.txt
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyoptimum-0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pyoptimum-0.4/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/Makefile
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/conf.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/requirements.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/src/modules.rst
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/src/quickstart.rst
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 pyoptimum-0.4/src/pyoptimum/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyoptimum-0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pyoptimum-0.4/tests/test_basic.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyoptimum-0.4/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyoptimum-0.4/LICENSE
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 pyoptimum-0.4/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyoptimum-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyoptimum-0.4/PKG-INFO
```

### Comparing `pyoptimum-0.3/.readthedocs.yaml` & `pyoptimum-0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/.github/workflows/python-publish.yml` & `pyoptimum-0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/.github/workflows/python-test.yml` & `pyoptimum-0.4/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/doc/Makefile` & `pyoptimum-0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/doc/conf.py` & `pyoptimum-0.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/doc/index.rst` & `pyoptimum-0.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/doc/make.bat` & `pyoptimum-0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/doc/src/quickstart.rst` & `pyoptimum-0.4/doc/src/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/src/pyoptimum/__init__.py` & `pyoptimum-0.4/src/pyoptimum/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,26 +13,36 @@
 
 
 class Client:
     """
     Client object to facilitate connection to the
     `optimize.vicbee.net <https:optimize.vicbee.net>`_ optimization api
 
+    Calls will be made to a URL of the form:
+
+    ``base_url/api/prefix/entry_point``
+
+    in which ``entry_point`` is set in :meth:`pyoptimum.Client.call`.
+
     :param username: the username
     :param password: the password
     :param token: an authentication token
     :param auto_token_renewal: whether to automatically renew an expired token
     :param base_url: the api base url
+    :param api: the target api
+    :param prefix: the target api prefix
     """
 
     def __init__(self,
                  username: Optional[str] = None, password: Optional[str] = None,
                  token: Optional[str] = None,
                  auto_token_renewal: Optional[bool] = True,
-                 base_url: Optional[str] = 'https://optimize.vicbee.net/api'):
+                 base_url: Optional[str] = 'https://optimize.vicbee.net',
+                 api: Optional[str] = 'optimize',
+                 prefix: Optional[str] = 'api'):
 
         # username and password
         self.username = username
         self.password = password
 
         # token
         self.token = token
@@ -45,15 +55,16 @@
                                      "have not been provided.")
 
         # base url
         self.base_url = base_url
         # make sure base_url does not have trailing /
         while self.base_url[-1] == '/':
             self.base_url = self.base_url[:-1]
-
+        # add api prefix
+        self.base_url = f'{self.base_url}/{api}/{prefix}'
 
         # initialize detail
         self.detail = None
 
     def get_token(self) -> None:
         """
         Retrieve authentication token
@@ -63,15 +74,15 @@
                                        'utf-8')).decode('utf-8')
         headers = {
             'Content-type': 'application/json',
             'Accept': 'application/json',
             'Authorization': 'Basic ' + basic
         }
 
-        response = requests.get(self.base_url + '/get_token', headers=headers)
+        response = requests.get(f'{self.base_url}/get_token', headers=headers)
         self.detail = None
 
         if response.ok:
 
             self.token = response.json().get('token')
 
         else:
@@ -90,21 +101,25 @@
         if self.token is None and not self.auto_token_renewal:
             raise PyOptimumException('No token available. Call get_token first')
 
         elif self.auto_token_renewal:
             # try renewing token
             self.get_token()
 
+        # make sure entry point does not start with a slash
+        while entry_point and entry_point[0] == '/':
+            entry_point = entry_point[1:]
+
         # See https://github.com/psf/requests/issues/6014
         headers = {
             'Content-type': 'application/json',
             'Accept': 'application/json',
             'X-Api-Key': self.token
         }
-        response = requests.post(self.base_url + '/' + entry_point,
+        response = requests.post(f'{self.base_url}/{entry_point}',
                                  data=json.dumps(data),
                                  headers=headers)
 
         if response.ok:
 
             self.detail = None
             return response.json()
```

### Comparing `pyoptimum-0.3/.gitignore` & `pyoptimum-0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/LICENSE` & `pyoptimum-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.3/pyproject.toml` & `pyoptimum-0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyoptimum"
-version = "0.3"
+version = "0.4"
 authors = [
     { name = "Mauricio C. de Oliveira", email = "mcdeoliveira@duck.com" }
 ]
 description = "Python library for optimize.vicbee.net optimize api"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords=["Optimization", "Porfolio Optimization"]
 requires-python = ">3.7"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Other Audience",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
 ]
 
 dependencies = [
     "requests",
     "typing-extensions"
 ]
```

### Comparing `pyoptimum-0.3/PKG-INFO` & `pyoptimum-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptimum
-Version: 0.3
+Version: 0.4
 Summary: Python library for optimize.vicbee.net optimize api
 Project-URL: Homepage, https://github.com/mcdeoliveira/pyoptimum
 Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
 License: MIT License
         
         Copyright (c) 2019 Mauricio de Oliveira
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Keywords: Optimization,Porfolio Optimization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >3.7
 Requires-Dist: requests
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # PyOptimum
```

