# Comparing `tmp/ansar-encode-0.1.78.tar.gz` & `tmp/ansar-encode-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-encode-0.1.78.tar", last modified: Mon Jun 12 06:34:35 2023, max compression
+gzip compressed data, was "ansar-encode-0.1.79.tar", last modified: Sun Jun 18 03:36:28 2023, max compression
```

## Comparing `ansar-encode-0.1.78.tar` & `ansar-encode-0.1.79.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/LICENSE
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      309 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     1971 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    12104 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/command/show_release.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     4943 2023-06-12 06:34:32.000000 ansar-encode-0.1.78/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37139 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16843 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11271 2023-05-22 09:25:36.000000 ansar-encode-0.1.78/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19680 2023-05-22 09:46:06.000000 ansar-encode-0.1.78/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33766 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10956 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6335 2023-06-12 06:19:56.000000 ansar-encode-0.1.78/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1814 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2023-04-19 07:09:52.000000 ansar-encode-0.1.78/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-12 06:34:35.356512 ansar-encode-0.1.78/src/ansar_encode.egg-info/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-06-12 06:34:35.000000 ansar-encode-0.1.78/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:14.000000 ansar-encode-0.1.79/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1484 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar-encode-0.1.79/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      311 2023-06-18 03:22:42.000000 ansar-encode-0.1.79/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1983 2023-06-18 03:18:21.000000 ansar-encode-0.1.79/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.778816 ansar-encode-0.1.79/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.778816 ansar-encode-0.1.79/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12110 2023-06-18 03:18:22.000000 ansar-encode-0.1.79/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4961 2023-06-18 03:36:25.000000 ansar-encode-0.1.79/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37157 2023-06-18 03:22:16.000000 ansar-encode-0.1.79/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    16861 2023-06-18 03:22:16.000000 ansar-encode-0.1.79/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11277 2023-06-18 03:20:47.000000 ansar-encode-0.1.79/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19686 2023-06-18 03:20:48.000000 ansar-encode-0.1.79/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3737 2023-06-18 03:22:17.000000 ansar-encode-0.1.79/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33784 2023-06-18 03:22:17.000000 ansar-encode-0.1.79/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10974 2023-06-18 03:22:17.000000 ansar-encode-0.1.79/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3340 2023-06-18 03:20:51.000000 ansar-encode-0.1.79/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6353 2023-06-18 03:22:18.000000 ansar-encode-0.1.79/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1820 2023-06-18 03:20:53.000000 ansar-encode-0.1.79/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11523 2023-06-18 03:20:54.000000 ansar-encode-0.1.79/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2023-06-18 03:36:28.782816 ansar-encode-0.1.79/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1484 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      642 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2023-06-18 03:36:28.000000 ansar-encode-0.1.79/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar-encode-0.1.78/LICENSE` & `ansar-encode-0.1.79/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Author: Scott Woods <scott.suzuki@gmail.com>
+Author: Scott Woods <scott.18.ansar@gmail.com.com>
 MIT License
 
-Copyright (c) 2017-2022
+Copyright (c) 2017-2023 Scott Woods
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/PKG-INFO` & `ansar-encode-0.1.79/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.78
+Version: 0.1.79
 Summary: Persistence of complex application data
 Author: Scott Woods
-Author-email: Scott Woods <scott.suzuki@gmail.com>
+Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ansar-encode-0.1.78/README.md` & `ansar-encode-0.1.79/README.md`

 * *Files identical despite different names*

### Comparing `ansar-encode-0.1.78/setup.py` & `ansar-encode-0.1.79/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Standard PyPi packaging.
 # Build materials and push to pypi.org.
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 import sys
 import setuptools
 import re
 
 #
 #
 VERSION_PATTERN = re.compile(r'([0-9]+)\.([0-9]+)\.([0-9]+)')
@@ -43,15 +43,15 @@
 	"python-dateutil>=2.8.1",
 ]
 
 setuptools.setup(
 	name=PACKAGE,
 	version=VERSION,
 	author="Scott Woods",
-	author_email="scott.suzuki@gmail.com",
+	author_email="scott.18.ansar@gmail.com.com",
 	description=DESCRIPTION,
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	# url="https://gitlab.com/scott.ansar/ansar-encode",
 	project_urls={
 		"Documentation": DOC_LINK,
 	},
```

### Comparing `ansar-encode-0.1.78/src/ansar/command/show_release.py` & `ansar-encode-0.1.79/src/ansar/command/show_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
 # Copyright (c) 2022 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/__init__.py` & `ansar-encode-0.1.79/src/ansar/encode/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
 Repo: git@github.com:mr-ansar/ansar-encode.git
 Branch: main
-Commit: 9b1b58561ae82d48307c62377790e60ab3773aa3
-Version: 0.1.77 (2023-06-12@18:34:32+NZST)
+Commit: df86792c81859d23fa9c0345405b3806544ee3ec
+Version: 0.1.78 (2023-06-18@15:36:25+NZST)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/codec.py` & `ansar-encode-0.1.79/src/ansar/encode/codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/convert.py` & `ansar-encode-0.1.79/src/ansar/encode/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/file.py` & `ansar-encode-0.1.79/src/ansar/encode/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/folder.py` & `ansar-encode-0.1.79/src/ansar/encode/folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/json.py` & `ansar-encode-0.1.79/src/ansar/encode/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/message.py` & `ansar-encode-0.1.79/src/ansar/encode/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/portable.py` & `ansar-encode-0.1.79/src/ansar/encode/portable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/release.py` & `ansar-encode-0.1.79/src/ansar/encode/release.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/runtime.py` & `ansar-encode-0.1.79/src/ansar/encode/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/version.py` & `ansar-encode-0.1.79/src/ansar/encode/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar/encode/xml.py` & `ansar-encode-0.1.79/src/ansar/encode/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.suzuki@gmail.com>
+# Author: Scott Woods <scott.18.ansar@gmail.com.com>
 # MIT License
 #
-# Copyright (c) 2017-2022 Scott Woods
+# Copyright (c) 2017-2023 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `ansar-encode-0.1.78/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.79/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.78
+Version: 0.1.79
 Summary: Persistence of complex application data
 Author: Scott Woods
-Author-email: Scott Woods <scott.suzuki@gmail.com>
+Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `ansar-encode-0.1.78/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.79/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

