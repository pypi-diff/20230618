# Comparing `tmp/math_calculator-1.0.0.tar.gz` & `tmp/math_calculator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_calculator-1.0.0.tar", last modified: Sun Jun 18 18:18:57 2023, max compression
+gzip compressed data, was "math_calculator-1.0.1.tar", last modified: Sun Jun 18 19:24:21 2023, max compression
```

## Comparing `math_calculator-1.0.0.tar` & `math_calculator-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:18:57.188307 math_calculator-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-18 18:18:56.000000 math_calculator-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-18 18:18:57.188307 math_calculator-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-06-18 18:18:56.000000 math_calculator-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 18:18:57.188307 math_calculator-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-06-18 18:18:56.000000 math_calculator-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:18:57.184307 math_calculator-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:18:57.186307 math_calculator-1.0.0/src/math_calculator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-18 18:18:56.000000 math_calculator-1.0.0/src/math_calculator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-06-18 18:18:56.000000 math_calculator-1.0.0/src/math_calculator/calculator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:18:57.187307 math_calculator-1.0.0/src/math_calculator/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-18 18:18:56.000000 math_calculator-1.0.0/src/math_calculator/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-06-18 18:18:56.000000 math_calculator-1.0.0/src/math_calculator/tests/test_calculator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 18:18:57.187307 math_calculator-1.0.0/src/math_calculator.egg-info/
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-18 18:18:57.000000 math_calculator-1.0.0/src/math_calculator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-18 18:18:57.000000 math_calculator-1.0.0/src/math_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 18:18:57.000000 math_calculator-1.0.0/src/math_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-18 18:18:57.000000 math_calculator-1.0.0/src/math_calculator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-18 18:18:57.000000 math_calculator-1.0.0/src/math_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 19:24:21.916082 math_calculator-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-18 19:24:20.000000 math_calculator-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-18 19:24:21.916082 math_calculator-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-06-18 19:24:20.000000 math_calculator-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 19:24:21.916082 math_calculator-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      838 2023-06-18 19:24:20.000000 math_calculator-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 19:24:21.914082 math_calculator-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 19:24:21.914082 math_calculator-1.0.1/src/math_calculator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-18 19:24:20.000000 math_calculator-1.0.1/src/math_calculator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-06-18 19:24:20.000000 math_calculator-1.0.1/src/math_calculator/calculator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 19:24:21.916082 math_calculator-1.0.1/src/math_calculator/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-18 19:24:20.000000 math_calculator-1.0.1/src/math_calculator/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-06-18 19:24:20.000000 math_calculator-1.0.1/src/math_calculator/tests/test_calculator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 19:24:21.915082 math_calculator-1.0.1/src/math_calculator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-18 19:24:21.000000 math_calculator-1.0.1/src/math_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-18 19:24:21.000000 math_calculator-1.0.1/src/math_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 19:24:21.000000 math_calculator-1.0.1/src/math_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-18 19:24:21.000000 math_calculator-1.0.1/src/math_calculator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-18 19:24:21.000000 math_calculator-1.0.1/src/math_calculator.egg-info/top_level.txt
```

### Comparing `math_calculator-1.0.0/LICENSE` & `math_calculator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `math_calculator-1.0.0/PKG-INFO` & `math_calculator-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: math_calculator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple math calculator package
 Home-page: https://gitlab.com/hassen_mnejja/math_calculator
-Author: Your Name
+Author: Hassen Mnejja
 Author-email: hassenmnejja1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `math_calculator-1.0.0/README.md` & `math_calculator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `math_calculator-1.0.0/setup.py` & `math_calculator-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='math_calculator',
-    version='1.0.0',
-    author='Your Name',
+    version='1.0.1',
+    author='Hassen Mnejja',
     author_email='hassenmnejja1@gmail.com',
     description='A simple math calculator package',
     long_description='A package that provides basic math calculations',
     url='https://gitlab.com/hassen_mnejja/math_calculator',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
```

### Comparing `math_calculator-1.0.0/src/math_calculator/calculator.py` & `math_calculator-1.0.1/src/math_calculator/calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import emoji
 
 def add(x, y):
     """Add two numbers with an emoji."""
     result = x + y
-    return emoji.emojize(":heavy_plus_sign:") + " " + str(result)
+    return emoji.emojize(":plus:") + " " + str(result)
 
 def subtract(x, y):
     """Subtract two numbers with an emoji."""
     result = x - y
-    return emoji.emojize(":heavy_minus_sign:") + " " + str(result)
+    return emoji.emojize(":minus:") + " " + str(result)
 
 def multiply(x, y):
     """Multiply two numbers with an emoji."""
     result = x * y
-    return emoji.emojize(":heavy_multiplication_x:") + " " + str(result)
+    return emoji.emojize(":multiply:") + " " + str(result)
 
 def divide(x, y):
     """Divide two numbers with an emoji."""
     if y != 0:
         result = x / y
-        return emoji.emojize(":heavy_division_sign:") + " " + str(result)
+        return emoji.emojize(":divide:") + " " + str(result)
     else:
         raise ZeroDivisionError("Cannot divide by zero.")
```

### Comparing `math_calculator-1.0.0/src/math_calculator/tests/test_calculator.py` & `math_calculator-1.0.1/src/math_calculator/tests/test_calculator.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from math_calculator.calculator import add, subtract, multiply, divide
 import emoji
 
 class CalculatorTest(unittest.TestCase):
 
     def test_add(self):
         result = add(3, 5)
-        expected = emoji.emojize(":heavy_plus_sign:") + " 8"
+        expected = emoji.emojize(":plus:") + " 8"
         self.assertEqual(result, expected)
 
     def test_subtract(self):
         result = subtract(10, 4)
-        expected = emoji.emojize(":heavy_minus_sign:") + " 6"
+        expected = emoji.emojize(":minus:") + " 6"
         self.assertEqual(result, expected)
 
     def test_multiply(self):
         result = multiply(2, 3)
-        expected = emoji.emojize(":heavy_multiplication_x:") + " 6"
+        expected = emoji.emojize(":multiply:") + " 6"
         self.assertEqual(result, expected)
 
     def test_divide(self):
         result = divide(10, 2)
-        expected = emoji.emojize(":heavy_division_sign:") + " 5.0"
+        expected = emoji.emojize(":divide:") + " 5.0"
         self.assertEqual(result, expected)
 
     def test_divide_by_zero(self):
         with self.assertRaises(ZeroDivisionError):
             divide(10, 0)
 
 if __name__ == '__main__':
```

### Comparing `math_calculator-1.0.0/src/math_calculator.egg-info/PKG-INFO` & `math_calculator-1.0.1/src/math_calculator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: math-calculator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple math calculator package
 Home-page: https://gitlab.com/hassen_mnejja/math_calculator
-Author: Your Name
+Author: Hassen Mnejja
 Author-email: hassenmnejja1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

