# Comparing `tmp/autopyre-0.0.7.tar.gz` & `tmp/autopyre-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.7.tar", last modified: Sun Jun 18 14:00:53 2023, max compression
+gzip compressed data, was "autopyre-0.0.8.tar", last modified: Sun Jun 18 14:50:35 2023, max compression
```

## Comparing `autopyre-0.0.7.tar` & `autopyre-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:00:53.123075 autopyre-0.0.7/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.7/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:00:53.122012 autopyre-0.0.7/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.7/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:00:53.120051 autopyre-0.0.7/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 14:00:53.000000 autopyre-0.0.7/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191748 2023-06-18 14:00:36.000000 autopyre-0.0.7/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 14:00:53.123297 autopyre-0.0.7/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 14:00:07.000000 autopyre-0.0.7/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:50:35.924500 autopyre-0.0.8/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.8/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:50:35.922359 autopyre-0.0.8/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.8/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:50:35.920190 autopyre-0.0.8/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   191843 2023-06-18 14:50:06.000000 autopyre-0.0.8/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 14:50:35.942019 autopyre-0.0.8/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 14:00:07.000000 autopyre-0.0.8/setup.py
```

### Comparing `autopyre-0.0.7/LICENSE` & `autopyre-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.7/PKG-INFO` & `autopyre-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.7/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.8/autopyre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.7/autopyre.py` & `autopyre-0.0.8/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -906,15 +906,18 @@
         fixed = indentation + '# ' + target.lstrip('# \t')
 
         self.source[result['line'] - 1] = fixed
 
     def fix_e267(self, result):
         line_index = result['line'] - 1
         target = self.source[line_index]
-        offset = result['column']- 1
+        if self.options.aggressive >= 3:
+            offset = target.index('#')
+        else: 
+            offset = result['column']- 1
         comment = target[offset:].rstrip()
         self.source[line_index] = target[:offset].rstrip()
         
         # 현재 줄이나 윗 줄에 줄 잇기의 형태가 존재하면 따로 수정x
         if ((line_index == 0 and check_continuous_line(self.source[line_index], '')) or
             (line_index > 0 and check_continuous_line(self.source[line_index],
                                                     self.source[line_index - 1]))):
@@ -1918,14 +1921,15 @@
 def find_importing_files(project_path, target_file):
     target_file_name = os.path.splitext(os.path.basename(target_file))[0]
     importing_files = set()
     target_file_path = get_file_path(project_path, target_file)
     
     for root, dirs, files in os.walk(project_path):
         for file_name in files:
+            
             file_path = os.path.join(root, file_name)
             if file_name.endswith('.py') and file_path != target_file_path:
                 
                 # iuput 파일이 import되고 있는 경우
                 if is_file_imported(file_path, target_file_name): 
                     importing_files.add(file_path)
     
@@ -1939,31 +1943,33 @@
 # 보안 적용 - 
 # 적절한 자원 반환 - with문 내의 코드에 예외가 발생하더라도 항상 파일 닫기가 보장 
 # 예외 처리 - try-except : 사용자가 syntax 에러가 있는 소스 코드에 대해 작명 컨벤션을 적용할 경우
 def is_file_imported(file_path, target_file):
     with open(file_path, 'r', errors='ignore') as file:
         source_code = file.read()
     tree = None
+    
     try:
         tree = ast.parse(source_code)
     except SyntaxError:
         return False
     
     for node in ast.walk(tree):
         if isinstance(node, ast.Import):
+            
             for alias in node.names:
                 imported_module = alias.name
-                print('imported_module : ', imported_module)
-                print('target_file : ', target_file)
                 if target_file == imported_module or '.' + target_file in imported_module:
                     return True
         elif isinstance(node, ast.ImportFrom):
+            if node.module is None: 
+                pass
             if node.module == target_file or '.' + target_file in node.module:
                 return True
-
+    
     return False
 
 
 # 추가한 부분 - 김위성 - 식별자, 참조되는 식별자를 모두 저장
 def analyze_file(file_path):
     with open(file_path, 'r', errors='ignore') as file:
         source_code = file.read()
@@ -2046,15 +2052,15 @@
 
         library_path = get_library_path(project_path, import_path)
         
         if library_path is None: continue
         if library_path.startswith(project_path):
 
             library_paths.append(library_path)
-        
+    # print("library_paths", library_paths)
     return library_paths
 
 
 # 추가한 부분 - 김위성 - input 파일의 경로를 가져온다.
 def get_file_path(project_path, file_name):
     for root, _, files in os.walk(project_path):
         for file in files:
@@ -2654,16 +2660,14 @@
     """Key for sorting PEP8 results.
 
     Global fixes should be done first. This is important for things like
     indentation.
 
     """
     priority = [
-        # 우선 순위에 인라인 주석을 추가해 이름 변경으로 인한 행 위치 변경 방지
-        'e267',
         # 먼저 바꿔줘야 import로 인한 라인 브레이킹 문제가 없어진다.
         # 추가한 부분 - 김위성 - 클래스 이름
         'w701',
         # 추가한 부분 - 김위성 - 함수 이름
         'w702',
         # Fix multiline colon-based before semicolon based.
         'e701',
@@ -2677,14 +2681,16 @@
         'e262'
     ]
     middle_index = 10000
     lowest_priority = [
         # We need to shorten lines last since the logical fixer can get in a
         # loop, which causes us to exit early.
         'e501',
+        # 인라인 주석을 추가해 이름 변경으로 인한 행 위치 변경 방지
+        'e267'
     ]
     key = pep8_result['id'].lower()
     try:
         return priority.index(key)
     except ValueError:
         try:
             return middle_index + lowest_priority.index(key) + 1
```

### Comparing `autopyre-0.0.7/setup.py` & `autopyre-0.0.8/setup.py`

 * *Files identical despite different names*

