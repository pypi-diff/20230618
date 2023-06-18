# Comparing `tmp/get_pypi_latest_version-0.0.8-py3-none-any.whl.zip` & `tmp/get_pypi_latest_version-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9521 bytes, number of entries: 8
--rw-r--r--  2.0 unx      131 b- defN 23-Apr-03 10:46 get_pypi_latest_version/__init__.py
--rw-r--r--  2.0 unx     6354 b- defN 23-Apr-03 10:46 get_pypi_latest_version/main.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-03 10:46 get_pypi_latest_version-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3900 b- defN 23-Apr-03 10:46 get_pypi_latest_version-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 10:46 get_pypi_latest_version-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-03 10:46 get_pypi_latest_version-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 23-Apr-03 10:46 get_pypi_latest_version-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      757 b- defN 23-Apr-03 10:46 get_pypi_latest_version-0.0.8.dist-info/RECORD
-8 files, 22694 bytes uncompressed, 8169 bytes compressed:  64.0%
+Zip file size: 9532 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      131 b- defN 23-Apr-03 10:50 get_pypi_latest_version/__init__.py
+-rw-r--r--  2.0 unx     6372 b- defN 23-Apr-03 10:50 get_pypi_latest_version/main.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-03 10:50 get_pypi_latest_version-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3900 b- defN 23-Apr-03 10:50 get_pypi_latest_version-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-03 10:50 get_pypi_latest_version-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-03 10:50 get_pypi_latest_version-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Apr-03 10:50 get_pypi_latest_version-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      757 b- defN 23-Apr-03 10:50 get_pypi_latest_version-0.0.9.dist-info/RECORD
+8 files, 22712 bytes uncompressed, 8180 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: get_pypi_latest_version/__init__.py
 Comment: 
 
 Filename: get_pypi_latest_version/main.py
 Comment: 
 
-Filename: get_pypi_latest_version-0.0.8.dist-info/LICENSE
+Filename: get_pypi_latest_version-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: get_pypi_latest_version-0.0.8.dist-info/METADATA
+Filename: get_pypi_latest_version-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: get_pypi_latest_version-0.0.8.dist-info/WHEEL
+Filename: get_pypi_latest_version-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: get_pypi_latest_version-0.0.8.dist-info/entry_points.txt
+Filename: get_pypi_latest_version-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: get_pypi_latest_version-0.0.8.dist-info/top_level.txt
+Filename: get_pypi_latest_version-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: get_pypi_latest_version-0.0.8.dist-info/RECORD
+Filename: get_pypi_latest_version-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## get_pypi_latest_version/__init__.py

```diff
@@ -1,5 +1,5 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 from .main import GetPyPiLatestVersion
-version = '0.0.8'
+version = '0.0.9'
```

## get_pypi_latest_version/main.py

```diff
@@ -22,18 +22,18 @@
 
     def __call__(self, package_name: str,
                  return_all_versions: bool = False) -> Union[str, Tuple[str, List]]:
         """
 
         Args:
             package_name (str): The name of the package you want to get the latest version.
-            return_all_versions (bool, optional): Whether to return all release versions. Default is False.
+            return_all_versions (bool, optional): Whether to return all release versions. Default is :code:`False` .
 
         Returns:
-            Union[str, Tuple[str, List]]: the latest version. When :code:`return_all_versions=False` , Return Tuple: latest_version_str, all_release_list
+            Union[str, Tuple[str, List]]: the latest version. When :code:`return_all_versions=True` , Return Tuple: :code:`[latest_version_str, all_release_list]`
         """
 
         all_versions_web = self.get_by_spider_web(package_name)
         latest_ver_web = all_versions_web[0]
 
         latest_ver_pip = self.get_by_pip_index(package_name)
```

## Comparing `get_pypi_latest_version-0.0.8.dist-info/LICENSE` & `get_pypi_latest_version-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `get_pypi_latest_version-0.0.8.dist-info/METADATA` & `get_pypi_latest_version-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-pypi-latest-version
-Version: 0.0.8
+Version: 0.0.9
 Summary: Get the latest version of the specified python package name in the pypi.
 Home-page: https://github.com/SWHL/GetPyPiLatestVersion
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Download-URL: https://github.com/SWHL/GetPyPiLatestVersion.git
 Project-URL: Documentation, https://getpypilatestversion.readthedocs.io/
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: get-pypi-latest-version Version: 0.0.8 Summary: Get
+Metadata-Version: 2.1 Name: get-pypi-latest-version Version: 0.0.9 Summary: Get
 the latest version of the specified python package name in the pypi. Home-page:
 https://github.com/SWHL/GetPyPiLatestVersion Author: SWHL Author-email:
 liekkaskono@163.com License: Apache-2.0 Download-URL: https://github.com/SWHL/
 GetPyPiLatestVersion.git Project-URL: Documentation, https://
 getpypilatestversion.readthedocs.io/ Project-URL: Source, https://github.com/
 SWHL/GetPyPiLatestVersion Project-URL: Changelog, https://github.com/SWHL/
 GetPyPiLatestVersion#change-log Keywords: pypi,latest_version Platform: Any
```

## Comparing `get_pypi_latest_version-0.0.8.dist-info/RECORD` & `get_pypi_latest_version-0.0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-get_pypi_latest_version/__init__.py,sha256=XFwpTwdReqsHk_L9xt_5K304C0nZZ_6k3dajBg8b_co,131
-get_pypi_latest_version/main.py,sha256=8A4YrRBtprqqfPqjPS_6FlSVP6gMLwLdYerZb8kvejI,6354
-get_pypi_latest_version-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-get_pypi_latest_version-0.0.8.dist-info/METADATA,sha256=E9hc29k2Tb-OAOXhtOCp37c6Sm8kXAU3RiTd1c2Q_Gk,3900
-get_pypi_latest_version-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-get_pypi_latest_version-0.0.8.dist-info/entry_points.txt,sha256=hfo8xeebLSlmooOwKEe-WQtgg835zhoc3NA1TGah6tQ,79
-get_pypi_latest_version-0.0.8.dist-info/top_level.txt,sha256=5FRVVAg90ctJx_87ddGU68bhUS86YJovWM9O4j_PfOU,24
-get_pypi_latest_version-0.0.8.dist-info/RECORD,,
+get_pypi_latest_version/__init__.py,sha256=jtaDvg0BDkn0AoRfjawj1J3-xFSxXVudxyrjwRA09o0,131
+get_pypi_latest_version/main.py,sha256=P9iv9DfUvgkajjQdFWK3DuGkwKLTCmnN-va49utR6Ak,6372
+get_pypi_latest_version-0.0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+get_pypi_latest_version-0.0.9.dist-info/METADATA,sha256=SSuioYiIRja9jYM5ThnOTqRDDZXj6QQJCmhCh5tWEkE,3900
+get_pypi_latest_version-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+get_pypi_latest_version-0.0.9.dist-info/entry_points.txt,sha256=hfo8xeebLSlmooOwKEe-WQtgg835zhoc3NA1TGah6tQ,79
+get_pypi_latest_version-0.0.9.dist-info/top_level.txt,sha256=5FRVVAg90ctJx_87ddGU68bhUS86YJovWM9O4j_PfOU,24
+get_pypi_latest_version-0.0.9.dist-info/RECORD,,
```

