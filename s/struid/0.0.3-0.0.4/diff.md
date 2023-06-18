# Comparing `tmp/struid-0.0.3.tar.gz` & `tmp/struid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struid-0.0.3.tar", last modified: Sat Jun 17 14:58:07 2023, max compression
+gzip compressed data, was "struid-0.0.4.tar", last modified: Sun Jun 18 08:13:03 2023, max compression
```

## Comparing `struid-0.0.3.tar` & `struid-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/
--rw-rw-r--   0 antisol   (1000) antisol   (1000)       48 2023-06-17 14:00:47.000000 struid-0.0.3/LICENSE
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     2268 2023-06-17 14:58:07.577257 struid-0.0.3/PKG-INFO
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     1668 2023-06-17 14:26:52.000000 struid-0.0.3/README.md
--rw-rw-r--   0 antisol   (1000) antisol   (1000)      659 2023-06-17 14:56:57.000000 struid-0.0.3/pyproject.toml
--rw-rw-r--   0 antisol   (1000) antisol   (1000)       38 2023-06-17 14:58:07.577257 struid-0.0.3/setup.cfg
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/src/
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/src/struid/
--rw-rw-r--   0 antisol   (1000) antisol   (1000)       40 2023-06-17 14:30:48.000000 struid-0.0.3/src/struid/__init__.py
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     5912 2023-06-04 13:45:59.000000 struid-0.0.3/src/struid/struid.py
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/src/struid.egg-info/
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     2268 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/PKG-INFO
--rw-rw-r--   0 antisol   (1000) antisol   (1000)      212 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/SOURCES.txt
--rw-rw-r--   0 antisol   (1000) antisol   (1000)        1 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/dependency_links.txt
--rw-rw-r--   0 antisol   (1000) antisol   (1000)        7 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/top_level.txt
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-18 08:13:03.573569 struid-0.0.4/
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)       48 2023-06-17 14:00:47.000000 struid-0.0.4/LICENSE
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     2618 2023-06-18 08:13:03.573569 struid-0.0.4/PKG-INFO
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     2018 2023-06-18 08:09:45.000000 struid-0.0.4/README.md
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)      701 2023-06-18 08:12:54.000000 struid-0.0.4/pyproject.toml
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)       38 2023-06-18 08:13:03.573569 struid-0.0.4/setup.cfg
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-18 08:13:03.549569 struid-0.0.4/src/
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-18 08:13:03.573569 struid-0.0.4/src/struid/
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)       64 2023-06-18 05:58:58.000000 struid-0.0.4/src/struid/__init__.py
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     7252 2023-06-18 06:07:17.000000 struid-0.0.4/src/struid/struid.py
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-18 08:13:03.573569 struid-0.0.4/src/struid.egg-info/
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     2618 2023-06-18 08:13:03.000000 struid-0.0.4/src/struid.egg-info/PKG-INFO
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)      212 2023-06-18 08:13:03.000000 struid-0.0.4/src/struid.egg-info/SOURCES.txt
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)        1 2023-06-18 08:13:03.000000 struid-0.0.4/src/struid.egg-info/dependency_links.txt
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)        7 2023-06-18 08:13:03.000000 struid-0.0.4/src/struid.egg-info/top_level.txt
```

### Comparing `struid-0.0.3/PKG-INFO` & `struid-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struid
-Version: 0.0.3
+Version: 0.0.4
 Summary: Struid - 'Stringy-UUID', an enhanced UUID package
 Author-email: Dale Magee <struid@antisol.org>
 Project-URL: Homepage, https://gitlab.com/AntiSol/struid
 Project-URL: Bug Tracker, https://gitlab.com/AntiSol/struid/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -19,43 +19,52 @@
 BSD 3-clause License
 
 # What is it?
 
 The Struid is an extension of python's UUID class which is intended to be more "pythonic" than the builtin UUID.
 
 In particular, the struid makes it easy to compare with a string or integer value, e.g:
-```
+```python
 > a = Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a == 'deadbeef-d00f-d00f-d00f-c0ffeedecade'
 True
 > a == 295990755078525382164994183696159263454
 True
 ```
 
+Struid also has convenience helpers to make it backwards-compatible with the regular uuid library:
+```python
+>from struid import UUID, uuid4
+>uuid4().shortstr()
+'💤🎝🐆🕏🍛🐃🐉🎧💿🎻🏐💊💡'
+>UUID('💤🎝🐆🕏🍛🐃🐉🎧💿🎻🏐💊💡')
+UUID('fe2fdb50-9280-461e-aa46-1b3e06718995')
+```
+
 # What else can it do?
 
 Struids also have a new shortstr() method, which allows you to compactify your string representations of UUID values down using extended unicode characters (emojis, or any characters you choose)
  
 e.g:
-```
+```python
 > a = Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a.shortstr()
 '🌨🚩💵👤🚡ᚮ🕓💣🐙😝🕴🕤ᛦ'
 ```
 
 And you can also instantiate a struid from a shortstr, or compare with one:
-```
+```python
 > Struid('🌨🚩💵👤🚡ᚮ🕓💣🐙😝🕴🕤ᛦ')
 Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 ```
 
-You can change the available characters shortstr() can use by setting SHORTSTR_DIGITS, e.g:
-```
+You can change the available characters shortstr() can use by calling struid.set_digits(), e.g:
+```python
 > import struid
-> struid.SHORTSTR_DIGITS = "0123456789AbCdEf"
+> struid.set_digits("0123456789AbCdEf")
 > a=Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a.shortstr()
 'dEAdbEEfd00fd00fd00fC0ffEEdECAdE'
 ```
 (note that changing the available characters affects the shortstr for all guids, 
  so if you e.g save shortstrings to a file and then change character sets, 
  the shortstrings in the file will no longer match)
```

### Comparing `struid-0.0.3/README.md` & `struid-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,43 +3,52 @@
 BSD 3-clause License
 
 # What is it?
 
 The Struid is an extension of python's UUID class which is intended to be more "pythonic" than the builtin UUID.
 
 In particular, the struid makes it easy to compare with a string or integer value, e.g:
-```
+```python
 > a = Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a == 'deadbeef-d00f-d00f-d00f-c0ffeedecade'
 True
 > a == 295990755078525382164994183696159263454
 True
 ```
 
+Struid also has convenience helpers to make it backwards-compatible with the regular uuid library:
+```python
+>from struid import UUID, uuid4
+>uuid4().shortstr()
+'💤🎝🐆🕏🍛🐃🐉🎧💿🎻🏐💊💡'
+>UUID('💤🎝🐆🕏🍛🐃🐉🎧💿🎻🏐💊💡')
+UUID('fe2fdb50-9280-461e-aa46-1b3e06718995')
+```
+
 # What else can it do?
 
 Struids also have a new shortstr() method, which allows you to compactify your string representations of UUID values down using extended unicode characters (emojis, or any characters you choose)
  
 e.g:
-```
+```python
 > a = Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a.shortstr()
 '🌨🚩💵👤🚡ᚮ🕓💣🐙😝🕴🕤ᛦ'
 ```
 
 And you can also instantiate a struid from a shortstr, or compare with one:
-```
+```python
 > Struid('🌨🚩💵👤🚡ᚮ🕓💣🐙😝🕴🕤ᛦ')
 Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 ```
 
-You can change the available characters shortstr() can use by setting SHORTSTR_DIGITS, e.g:
-```
+You can change the available characters shortstr() can use by calling struid.set_digits(), e.g:
+```python
 > import struid
-> struid.SHORTSTR_DIGITS = "0123456789AbCdEf"
+> struid.set_digits("0123456789AbCdEf")
 > a=Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a.shortstr()
 'dEAdbEEfd00fd00fd00fC0ffEEdECAdE'
 ```
 (note that changing the available characters affects the shortstr for all guids, 
  so if you e.g save shortstrings to a file and then change character sets, 
  the shortstrings in the file will no longer match)
```

### Comparing `struid-0.0.3/pyproject.toml` & `struid-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "struid"
-version = "0.0.3"
+version = "0.0.4" # Generated Sun 18 Jun 2023 18:12:54 AEST
 authors = [
   { name="Dale Magee", email="struid@antisol.org" },
 ]
 description = "Struid - 'Stringy-UUID', an enhanced UUID package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `struid-0.0.3/src/struid/struid.py` & `struid-0.0.4/src/struid/struid.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,23 +26,66 @@
 	#(8704,8959), # math operators
 	#(9728,9983), # misc symbols
 	#(10241,10495), # braille
 	#(77824,78894), # heiroglyphs
 	
 ]
 
-# populate digits with unicode characters
-for start, end in unicode_ranges:
-	for i in range(start,end+1):		# emojis start at 128512 - 128591
-		SHORTSTR_DIGITS += chr(i)
+def default_shortstr_digits() -> str:
+	"""
+	Returns the default set of shortstr digits as a string
+	"""
+	ret = ""
+	for start, end in unicode_ranges:
+		for i in range(start,end+1):		# emojis start at 128512 - 128591
+			ret += chr(i)
+	return ret
 
 def set_digits(new_digits:str):
+	"""
+	Sets the digits used by shortstr, determining the number base used
+	
+	i.e setting the shortstr digits to "01" would give you binary,
+	 or setting it to '01234567890ABCDEF' will give you hexadecimal.
+	 
+	You must not include both uppercase and lowercase of any character in
+	 the list of digits - struid is built to be case-insensitive (like UUID)
+	"""
 	global SHORTSTR_DIGITS
+	
+	# enforce string
+	new_digits = str(new_digits)
+	
+	# validate: you can't include:
+	# - the same character twice
+	# - both upper and lowercase of the same char
+	for idx in range(0,len(new_digits)):
+		thischar = new_digits[idx]
+		if new_digits.rfind(thischar) != idx:
+			raise ValueError("You cannot include the same character more than once in new_digits")
+		if thischar.lower() != thischar.upper(): # character has upper and lowercase
+			if new_digits.lower().rfind(thischar.lower()) != idx:
+				raise ValueError("You cannot include both uppercase and lowercase of the same character in new_digits")
+	
 	SHORTSTR_DIGITS = new_digits
 
+def get_digits() -> str:
+	"""
+	Returns the list of digits that can be used by shortstr.
+	use set_digits to change this.
+	"""
+	return SHORTSTR_DIGITS
+
+def reset_digits():
+	set_digits(default_shortstr_digits())
+	
+# load the default
+reset_digits()
+
+
 def arb_base(num:int, base:int) -> list:
 	# convert number n to arbitrary base
 	# from https://stackoverflow.com/a/28666223
 	if num == 0:
 		return [0]
 	digits = []
 	while num:
@@ -50,14 +93,15 @@
 		num //= base
 	return digits[::-1]
 
 def from_arb_base(digit: str, digits:str=None) -> int:
 	"""
 	convert an arbitrary-base digit into an integer
 	digits must be a string containing allowed digits, lowest-highest value
+	if the provided digit isn't in the list, will return 0
 	"""
 	if digits is None: digits = SHORTSTR_DIGITS
 	ret = max(str(digits).find(str(digit)),0)
 	return ret
 	
 
 class Struid(UUID_Real):
```

### Comparing `struid-0.0.3/src/struid.egg-info/PKG-INFO` & `struid-0.0.4/src/struid.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struid
-Version: 0.0.3
+Version: 0.0.4
 Summary: Struid - 'Stringy-UUID', an enhanced UUID package
 Author-email: Dale Magee <struid@antisol.org>
 Project-URL: Homepage, https://gitlab.com/AntiSol/struid
 Project-URL: Bug Tracker, https://gitlab.com/AntiSol/struid/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -19,43 +19,52 @@
 BSD 3-clause License
 
 # What is it?
 
 The Struid is an extension of python's UUID class which is intended to be more "pythonic" than the builtin UUID.
 
 In particular, the struid makes it easy to compare with a string or integer value, e.g:
-```
+```python
 > a = Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a == 'deadbeef-d00f-d00f-d00f-c0ffeedecade'
 True
 > a == 295990755078525382164994183696159263454
 True
 ```
 
+Struid also has convenience helpers to make it backwards-compatible with the regular uuid library:
+```python
+>from struid import UUID, uuid4
+>uuid4().shortstr()
+'💤🎝🐆🕏🍛🐃🐉🎧💿🎻🏐💊💡'
+>UUID('💤🎝🐆🕏🍛🐃🐉🎧💿🎻🏐💊💡')
+UUID('fe2fdb50-9280-461e-aa46-1b3e06718995')
+```
+
 # What else can it do?
 
 Struids also have a new shortstr() method, which allows you to compactify your string representations of UUID values down using extended unicode characters (emojis, or any characters you choose)
  
 e.g:
-```
+```python
 > a = Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a.shortstr()
 '🌨🚩💵👤🚡ᚮ🕓💣🐙😝🕴🕤ᛦ'
 ```
 
 And you can also instantiate a struid from a shortstr, or compare with one:
-```
+```python
 > Struid('🌨🚩💵👤🚡ᚮ🕓💣🐙😝🕴🕤ᛦ')
 Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 ```
 
-You can change the available characters shortstr() can use by setting SHORTSTR_DIGITS, e.g:
-```
+You can change the available characters shortstr() can use by calling struid.set_digits(), e.g:
+```python
 > import struid
-> struid.SHORTSTR_DIGITS = "0123456789AbCdEf"
+> struid.set_digits("0123456789AbCdEf")
 > a=Struid('deadbeef-d00f-d00f-d00f-c0ffeedecade')
 > a.shortstr()
 'dEAdbEEfd00fd00fd00fC0ffEEdECAdE'
 ```
 (note that changing the available characters affects the shortstr for all guids, 
  so if you e.g save shortstrings to a file and then change character sets, 
  the shortstrings in the file will no longer match)
```

