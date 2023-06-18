# Comparing `tmp/autopyre-0.0.5.tar.gz` & `tmp/autopyre-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.5.tar", last modified: Sun Jun 18 12:54:38 2023, max compression
+gzip compressed data, was "autopyre-0.0.6.tar", last modified: Sun Jun 18 13:53:03 2023, max compression
```

## Comparing `autopyre-0.0.5.tar` & `autopyre-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:54:38.898283 autopyre-0.0.5/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.5/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 12:54:38.897501 autopyre-0.0.5/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.5/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:54:38.894724 autopyre-0.0.5/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       34 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191821 2023-06-18 12:53:59.000000 autopyre-0.0.5/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 12:54:38.904288 autopyre-0.0.5/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2064 2023-06-18 12:54:20.000000 autopyre-0.0.5/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 13:53:03.950159 autopyre-0.0.6/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.6/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 13:53:03.949713 autopyre-0.0.6/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.6/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 13:53:03.948906 autopyre-0.0.6/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   191634 2023-06-18 13:53:01.000000 autopyre-0.0.6/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 13:53:03.950301 autopyre-0.0.6/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 13:13:06.000000 autopyre-0.0.6/setup.py
```

### Comparing `autopyre-0.0.5/LICENSE` & `autopyre-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.5/PKG-INFO` & `autopyre-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
-Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
+Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `autopyre-0.0.5/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.6/autopyre.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
-Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
+Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `autopyre-0.0.5/autopyre.py` & `autopyre-0.0.6/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -1887,17 +1887,16 @@
     if match:
         return match.group(1)
     return None
 
 
 # 추가한 부분 - 김위성 - 프로젝트의 경로
 def get_project_path():
-    script_path = os.path.abspath(__file__)
-    project_path = os.path.dirname(os.path.dirname(script_path))
-    return project_path
+    return os.path.dirname(os.path.abspath(__file__))
+
 
 
 # 추가한 부분 - 김위성 - import 하고 있는 파일과 해당 파일의 모든 식별자와 참조되는 식별자
 def find_all_identifiers(project_path, target_file):
     identifiers = set()
     referenced = set()
     
@@ -1921,14 +1920,15 @@
     importing_files = set()
     target_file_path = get_file_path(project_path, target_file)
     
     for root, dirs, files in os.walk(project_path):
         for file_name in files:
             file_path = os.path.join(root, file_name)
             if file_name.endswith('.py') and file_path != target_file_path:
+                
                 # iuput 파일이 import되고 있는 경우
                 if is_file_imported(file_path, target_file_name): 
                     importing_files.add(file_path)
     
     # iuput 파일이 import하는 파일(라이브러리)의 경우
     import_path = get_import_paths(project_path, target_file)
     importing_files.update(import_path)
@@ -1938,30 +1938,27 @@
 # 추가한 부분 - 김위성 - 프로젝트내의 어떤 파일이 input파일을 import하는지 여부
 # 보안 적용 - 
 # 적절한 자원 반환 - with문 내의 코드에 예외가 발생하더라도 항상 파일 닫기가 보장 
 # 예외 처리 - try-except : 사용자가 syntax 에러가 있는 소스 코드에 대해 작명 컨벤션을 적용할 경우
 def is_file_imported(file_path, target_file):
     with open(file_path, 'r', errors='ignore') as file:
         source_code = file.read()
-    print(file_path, target_file)
     tree = None
     try:
         tree = ast.parse(source_code)
     except SyntaxError:
         return False
     
     for node in ast.walk(tree):
         if isinstance(node, ast.Import):
             for alias in node.names:
                 imported_module = alias.name
-                print(target_file, imported_module)
                 if target_file == imported_module or '.' + target_file in imported_module:
                     return True
         elif isinstance(node, ast.ImportFrom):
-            print(node.module, target_file)
             if node.module == target_file or '.' + target_file in node.module:
                 return True
 
     return False
 
 
 # 추가한 부분 - 김위성 - 식별자, 참조되는 식별자를 모두 저장
@@ -2057,15 +2054,15 @@
 
 # 추가한 부분 - 김위성 - input 파일의 경로를 가져온다.
 def get_file_path(project_path, file_name):
     for root, _, files in os.walk(project_path):
         for file in files:
             if file == file_name:
                 return os.path.join(root, file)
-
+    
     return None
 
 
 # 추가한 부분 - 김위성 - cst를 활용한 클래스 이름 변경 클래스
 class ClassNameTransformer(cst.CSTTransformer):
     def __init__(self, rename_pairs):
         self.rename_pairs = rename_pairs
```

### Comparing `autopyre-0.0.5/setup.py` & `autopyre-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import io
 
 from setuptools import setup
 
 # read the contents of your README file
 
 INSTALL_REQUIRES = (
-    ['tomli; python_version < "3.11"']
+    ['pyrestyle >= 0.0.4', 'tomli; python_version < "3.11"']
 )
 
 
 def version():
     """Return version string."""
     with io.open('autopyre.py') as input_file:
         for line in input_file:
@@ -28,15 +28,15 @@
         version=version(),
         description='A tool that automatically formats Python code to conform '
                     'to the PEP 8 style guide and This project based on autopep8',
         long_description=readme.read(),
         license='MIT',
         author='Hideo Hattori, 2023-1-OPPS1-CGS-08',
         author_email='kys00919@gmail.com',
-        url='https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08',
+        url='https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Console',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             'Programming Language :: Python',
```

