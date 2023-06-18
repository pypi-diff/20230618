# Comparing `tmp/tcia_utils-1.4.1.tar.gz` & `tmp/tcia_utils-1.5.tar.gz`

## Comparing `tcia_utils-1.4.1.tar` & `tcia_utils-1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    51403 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/LICENSE
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    58523 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.5/LICENSE
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.5/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tcia_utils-1.5/pyproject.toml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tcia_utils-1.5/PKG-INFO
```

### Comparing `tcia_utils-1.4.1/src/tcia_utils/datacite.py` & `tcia_utils-1.5/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4.1/src/tcia_utils/nbia.py` & `tcia_utils-1.5/src/tcia_utils/nbia.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 import numpy as np
 from ipywidgets import interact
 
 class StopExecution(Exception):
     def _render_traceback_(self):
         pass
 
-token_exp_time = datetime.now()
-nlst_token_exp_time = datetime.now()
-
 _log = logging.getLogger(__name__)
 logging.basicConfig(
     format='%(asctime)s:%(levelname)s:%(message)s'
     , level=logging.INFO
 )
 
 class Criteria(Enum):
@@ -77,37 +74,44 @@
         if api_url == "":
             if endpoint in searchEndpoints:
                 # Using "Search" API (no login required): https://wiki.cancerimagingarchive.net/x/fILTB
                 base_url = "https://services.cancerimagingarchive.net/nbia-api/services/v1/"
             if endpoint in advancedEndpoints:
                 # Using "Advanced" API (login required): https://wiki.cancerimagingarchive.net/x/YoATBg
                 # check if valid token exists, use anonymous login if not
-                if datetime.now() > token_exp_time:
-                    _log.info("Accessing Advanced API anonymously. To access restricted data use nbia.getToken() with your credentials.")
+                if 'token_exp_time' not in globals():
                     getToken(user = "nbia_guest")
+                    _log.info("Accessing Advanced API anonymously. To access restricted data use nbia.getToken() with your credentials.")
+                if 'token_exp_time' in globals() and datetime.now() > token_exp_time:
+                    refreshToken()
+                    _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
                 base_url = "https://services.cancerimagingarchive.net/nbia-api/services/"
         elif api_url == "nlst":
             if endpoint in searchEndpoints:
                 # Using "Search" API with NLST server (no login required): https://wiki.cancerimagingarchive.net/x/fILTB
                 base_url = "https://nlst.cancerimagingarchive.net/nbia-api/services/v1/"
             if endpoint in advancedEndpoints:
                 # Using "Advanced" API docs (login required): https://wiki.cancerimagingarchive.net/x/YoATBg
                 # Checking to see if a valid NLST authentication token exists
-                if datetime.now() > nlst_token_exp_time:
+                if 'nlst_token_exp_time' not in globals():
                     getToken(user = "nbia_guest", api_url = "nlst")
-                base_url = "https://nlst.cancerimagingarchive.net/nbia-api/services/"
+                if 'nlst_token_exp_time' in globals() and datetime.now() > nlst_token_exp_time:
+                    refreshToken(api_url = "nlst")
+                base_url = "https://nlst.cancerimagingarchive.net/nbia-api/services/"                
         elif api_url == "restricted":
             if endpoint in searchEndpoints:
                 # Using "Search with Authentication" API (login required): https://wiki.cancerimagingarchive.net/x/X4ATBg
                 # Checking to see if a valid authentication token exists
-                if datetime.now() < token_exp_time:
-                    base_url = "https://services.cancerimagingarchive.net/nbia-api/services/v2/"
-                else:
-                    _log.error("Your security token for accessing the Restricted API is expired or does not exist. Create one using getToken().")
+                if 'token_exp_time' not in globals():
+                    _log.error("Error using token for accessing the Restricted API. Create one using getToken().")
                     raise StopExecution
+                if 'token_exp_time' in globals() and datetime.now() > token_exp_time:
+                    refreshToken()
+                    _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
+                base_url = "https://services.cancerimagingarchive.net/nbia-api/services/v2/"
             if endpoint in advancedEndpoints:
                 _log.error(
                     f'"{api_url}" is an invalid api_url for the Advanced API endpoint: {endpoint}\n'
                     "Remove the api_url parameter unless you are querying the National Lung Screening Trial collection.\n"
                     "Use api_url = \"nlst\" to query the National Lung Screening Trial collection."
                 )
                 raise StopExecution
@@ -135,15 +139,15 @@
 # Provides interactive prompts for user/pw if they're not specified as parameters
 # Use getToken() for querying restricted collections with "Search API"
 # Use getToken(api_url = "nlst") for "Advanced API" queries of National Lung Screening Trial
 # Sets expiration time for tokens (2 hours from creation)
 
 def getToken(user = "", pw = "", api_url = ""): 
 
-    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers
+    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token
 
     # token URLs
     if api_url == "nlst":
         token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
     else:
         token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
 
@@ -167,34 +171,126 @@
         'username' : userName,
         'password': passWord
         }
         
         data = requests.post(token_url, data = params)
         data.raise_for_status()
         access_token = data.json()["access_token"]
+        refresh_token = data.json()["refresh_token"]
+        expires_in = data.json()["expires_in"]
         # track expiration status/time (2 hours from creation)
         current_time = datetime.now()
         if api_url == "nlst":
-            nlst_token_exp_time = current_time + timedelta(hours=2)
+            nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
             nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
             _log.info(f'Success - Token saved to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
         else:
-            token_exp_time = current_time + timedelta(hours=2)
+            token_exp_time = current_time + timedelta(seconds=expires_in)
             api_call_headers = {'Authorization': 'Bearer ' + access_token}
             _log.info(f'Success - Token saved to api_call_headers variable and expires at {token_exp_time}')
     # handle errors
     except requests.exceptions.HTTPError as errh:
         _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
     except requests.exceptions.ConnectionError as errc:
         _log.error(f"Connection Error: {data.status_code}")
     except requests.exceptions.Timeout as errt:
         _log.error(f"Timeout Error: {data.status_code}")
     except requests.exceptions.RequestException as err:
         _log.error(f"Request Error: {data.status_code}")
 
+####### refreshToken()
+# Refreshes security token to extend access time for APIs that require authorization
+# Must first use getToken() to create a token
+
+def refreshToken(api_url = ""): 
+
+    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers
+
+    try:
+        refresh_token
+    except NameError:
+        _log.error("Error refreshing token for accessing the Restricted API. Create one using getToken().")
+        raise StopExecution
+    else:
+
+        # token URLs
+        if api_url == "nlst":
+            token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
+        else:
+            token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
+
+        # refresh token request
+        try:
+            params = {
+            'client_id': 'nbiaRestAPIClient',
+            'client_secret' : 'ItsBetweenUAndMe',
+            'grant_type': 'refresh_token',
+            'refresh_token' : refresh_token,
+            }
+            
+            # obtain new access token
+            data = requests.post(token_url, data = params)
+            data.raise_for_status()
+            access_token = data.json()["access_token"]
+            expires_in = data.json()["expires_in"]
+            # track expiration status/time (2 hours from creation)
+            current_time = datetime.now()
+            if api_url == "nlst":
+                nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
+                nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
+                _log.info(f'Success - Token refreshed to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
+            else:
+                token_exp_time = current_time + timedelta(seconds=expires_in)
+                api_call_headers = {'Authorization': 'Bearer ' + access_token}
+                _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
+        # handle errors
+        except requests.exceptions.HTTPError as errh:
+            _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
+        except requests.exceptions.ConnectionError as errc:
+            _log.error(f"Connection Error: {data.status_code}")
+        except requests.exceptions.Timeout as errt:
+            _log.error(f"Timeout Error: {data.status_code}")
+        except requests.exceptions.RequestException as err:
+            _log.error(f"Request Error: {data.status_code}")
+            
+####### logoutToken()
+# Logs out of a security token for APIs that require authorization
+# Must first use getToken() to create a token
+
+def logoutToken(api_url = ""): 
+
+    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token
+
+    # determine which server the token was created on
+    if api_url == "nlst" and 'nlst_api_call_headers' in globals():
+        url = "https://nlst.cancerimagingarchive.net/nbia-api/logout"
+        api_call_headers = nlst_api_call_headers
+    elif api_url != "nlst" and 'api_call_headers' in globals():
+        url = "https://services.cancerimagingarchive.net/nbia-api/logout"
+    else: 
+        _log.error("Error: You haven't created a token yet, or have already logged out.")
+        raise StopExecution
+
+    try:
+        _log.info(f'Logging out of... {url}')
+        data = requests.get(url, headers = api_call_headers)
+        _log.info(f'{data.text}')
+        # remove variables holding token details
+        del token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token
+
+    # handle errors
+    except requests.exceptions.HTTPError as errh:
+        _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
+    except requests.exceptions.ConnectionError as errc:
+        _log.error(f"Connection Error: {data.status_code}")
+    except requests.exceptions.Timeout as errt:
+        _log.error(f"Timeout Error: {data.status_code}")
+    except requests.exceptions.RequestException as err:
+        _log.error(f"Request Error: {data.status_code}")
+
 ####### makeCredentialFile()
 # Create a credential file to use with NBIA Data Retriever
 # Provides interactive prompts for user/pw if they're not specified as parameters
 # Documentation at https://wiki.cancerimagingarchive.net/x/2QKPBQ
 
 def makeCredentialFile(user = "", pw = ""):
 
@@ -261,14 +357,15 @@
         _log.error(errh)
     except requests.exceptions.ConnectionError as errc:
         _log.error(errc)
     except requests.exceptions.Timeout as errt:
         _log.error(errt)
     except requests.exceptions.RequestException as err:
         _log.error(err)
+    
 
 ####### getCollections function
 # Gets a list of collections from a specified api_url
 
 def getCollections(api_url = "",
                    format = ""):
 
@@ -952,14 +1049,75 @@
 
     # create options dict to construct URL
     options = {}
     options['SeriesUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
     return data
+    
+####### getSegRefSeries function (Advanced)
+# Gets DICOM tag metadata for a given SEG/RTSTRUCT series UID (scan)
+# and then look up the series UID they were derived from
+
+def getSegRefSeries(uid):
+    # get dicom tags for the series as a dataframe
+    df = getDicomTags(uid, format="df")
+
+    if df is not None:
+        # Find the row where element = "(0008,0060) Modality"
+        findModality = df['element'] == '(0008,0060)'
+        modality = df.loc[findModality, 'data'].item()
+
+        if modality == "RTSTRUCT":
+            # Locate "RT Referenced Series Sequence >>(3006,0014)"
+            # and "Series Instance UID >>>(0020,000E)" in the dataframe
+            refElements = (df['element'] == '>>(3006,0014)') & (df['element'].shift(-1) == '>>>(0020,000E)')
+
+            if refElements.any():
+                # Get the index for end of segmentation sequence
+                index = df.index[refElements].item()
+
+                # Retrieve the value of "Series Instance UID" from the next row
+                refSeriesUid = df.loc[index + 1, 'data']
+                return refSeriesUid
+            
+            else:
+                print("Segmentation doesn't contain a reference series UID.")
+                refSeriesUid = "N/A"
+                return refSeriesUid
+
+        elif modality == "SEG":
+            # Locate ">(0008,114A) End Referenced Instance Sequence"
+            # and ">(0020,000E) Series Instance UID" in the dataframe
+            refElements = (df['element'] == '>(0008,114A)') & (df['element'].shift(-1) == '>(0020,000E)')
+
+            if refElements.any():
+                # Get the index for end of segmentation sequence
+                index = df.index[refElements].item()
+
+                # Retrieve the value of "Series Instance UID" from the next row
+                refSeriesUid = df.loc[index + 1, 'data']
+                return refSeriesUid
+            
+            else:
+                print("Segmentation doesn't contain a reference series UID.")
+                refSeriesUid = "N/A"
+                return refSeriesUid
+
+        else:
+            print("Segmentation series must be RTSTRUCT or SEG modality.")
+            refSeriesUid = "N/A"
+            return refSeriesUid
+
+    else:
+        print("Segmentation series UID not found:", uid)
+        refSeriesUid = "N/A"
+        return refSeriesUid
+
+
 
 ####### getDoiMetadata function
 # Gets a list of Collections or Series associated with a DOI
 # Requires a DOI URL and specification of Collection or Series UID output
 # Result includes whether the data are 3rd party analyses or not
 # Formats output as JSON by default with options for "df" (dataframe) and "csv"
```

### Comparing `tcia_utils-1.4.1/src/tcia_utils/pathdb.py` & `tcia_utils-1.5/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4.1/.gitignore` & `tcia_utils-1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4.1/LICENSE` & `tcia_utils-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4.1/README.md` & `tcia_utils-1.5/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4.1/pyproject.toml` & `tcia_utils-1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.4.1"
+version = "1.5"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.4.1/PKG-INFO` & `tcia_utils-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.4.1
+Version: 1.5
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

