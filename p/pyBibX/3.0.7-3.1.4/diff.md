# Comparing `tmp/pyBibX-3.0.7.tar.gz` & `tmp/pyBibX-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-3.0.7.tar", last modified: Fri Jun 16 00:09:11 2023, max compression
+gzip compressed data, was "dist\pyBibX-3.1.4.tar", last modified: Sat Jun 17 22:08:49 2023, max compression
```

## Comparing `pyBibX-3.0.7.tar` & `pyBibX-3.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:09:11.000000 pyBibX-3.0.7/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.0.7/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     9608 2023-06-16 00:09:11.000000 pyBibX-3.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 00:09:10.000000 pyBibX-3.0.7/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.7/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:09:10.000000 pyBibX-3.0.7/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.0.7/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   265635 2023-06-16 00:07:38.000000 pyBibX-3.0.7/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:09:11.000000 pyBibX-3.0.7/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.0.7/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:09:10.000000 pyBibX-3.0.7/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-06-16 00:09:09.000000 pyBibX-3.0.7/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-06-16 00:09:09.000000 pyBibX-3.0.7/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:09:09.000000 pyBibX-3.0.7/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-06-16 00:09:09.000000 pyBibX-3.0.7/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-16 00:09:09.000000 pyBibX-3.0.7/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-16 00:09:09.000000 pyBibX-3.0.7/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-16 00:09:11.000000 pyBibX-3.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-06-16 00:08:26.000000 pyBibX-3.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:08:49.000000 pyBibX-3.1.4/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.1.4/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-06-17 22:08:49.000000 pyBibX-3.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 22:08:48.000000 pyBibX-3.1.4/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.4/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:08:48.000000 pyBibX-3.1.4/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.1.4/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   265929 2023-06-17 22:06:18.000000 pyBibX-3.1.4/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:08:49.000000 pyBibX-3.1.4/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.4/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:08:48.000000 pyBibX-3.1.4/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-06-17 22:08:47.000000 pyBibX-3.1.4/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-06-17 22:08:47.000000 pyBibX-3.1.4/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 22:08:47.000000 pyBibX-3.1.4/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-06-17 22:08:47.000000 pyBibX-3.1.4/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 22:08:47.000000 pyBibX-3.1.4/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-17 22:08:47.000000 pyBibX-3.1.4/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-17 22:08:49.000000 pyBibX-3.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-06-17 22:07:45.000000 pyBibX-3.1.4/setup.py
```

### Comparing `pyBibX-3.0.7/LICENSE` & `pyBibX-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/PKG-INFO` & `pyBibX-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.0.7
+Version: 3.1.4
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.0.7/README.md` & `pyBibX-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/pbx.py` & `pyBibX-3.1.4/pyBibX/base/pbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from wordcloud import WordCloud                           
 
 ############################################################################
 
 # pbx Class
 class pbx_probe():
     def __init__(self, file_bib, db = 'scopus', del_duplicated = True):
-        self.data_base         =  db
         self.institution_names =  [ 
                                     'acad', 'academy', 'ctr', 'center', 'centre', 'chuo kikuu', 'cient', 'coll', 'college', 'conservatory', 
                                     'egyetemi', 'escola', 'education', 'escuela', 'eyunivesithi', 'fac', 'faculdade', 'facultad', 'fakultet', 
                                     'fakultät', 'fdn', 'fundacion', 'foundation', 'gradevinski', 'higher', 'hsch', 'hochschule', 'hgsk', 
                                     'hogeschool',  'háskóli', 'högskola', 'ibmec', 'inivèsite', 'ist', 'istituto', 'institutional', 'int', 'inst', 
                                     'institut', 'institute', 'institute of technology',  'inyuvesi', 'iskola', 'iunivesite', 'jaamacad', "jami'a", 
                                     'kolej', 'koulu', 'kulanui', 'lab.', 'lab', 'labs', 'laborat', 'mahadum', 'med', 'medicine', 'medical', 
@@ -1238,68 +1237,73 @@
         c_count_ = [0]*len(c_year_)
         for i in range(0, len(c_year)):
             c_count_[c_year_.index(c_year[i])] = c_count_[c_year_.index(c_year[i])] + c_count[i]
         return c_year_, c_count_
     
     # Function: Get Countries
     def __get_countries(self):
-        if   (self.data_base == 'scopus' or self.data_base == 'pubmed'):
+        if ('affiliation' in self.data.columns and 'affiliations' in self.data.columns and 'affiliation_' in self.data.columns):
             df = self.data['affiliation']
-            df = df.str.lower()
-        elif (self.data_base == 'wos'):
+            df = pd.Series(np.zeros(self.data.shape[0]))
+            for i in range(0, self.data.shape[0]):
+                if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
+                    df[i] = self.data.loc[i, 'affiliation']
+                elif (self.data.loc[i, 'source'].lower() == 'wos'):
+                    df[i] = self.data.loc[i, 'affiliation_']
+        elif ('affiliation' in self.data.columns and 'affiliations' in self.data.columns):
+            df = self.data['affiliation']
+        elif ('affiliation' in self.data.columns and 'affiliation_' in self.data.columns):
             df = self.data['affiliation_']
-            df = df.str.replace(' USA',            ' United States of America',   case = False, regex = True)
-            df = df.str.replace('ENGLAND',         'United Kingdom',              case = False, regex = True)
-            df = df.str.replace('Antigua & Barbu', 'Antigua and Barbuda',         case = False, regex = True)
-            df = df.str.replace('Bosnia & Herceg', 'Bosnia and Herzegovina',      case = False, regex = True)
-            df = df.str.replace('Cent Afr Republ', 'Central African Republic',    case = False, regex = True)
-            df = df.str.replace('Dominican Rep',   'Dominican Republic',          case = False, regex = True)
-            df = df.str.replace('Equat Guinea',    'Equatorial Guinea',           case = False, regex = True)
-            df = df.str.replace('Fr Austr Lands',  'French Southern Territories', case = False, regex = True)
-            df = df.str.replace('Fr Polynesia',    'French Polynesia',            case = False, regex = True)
-            df = df.str.replace('Malagasy Republ', 'Madagascar',                  case = False, regex = True)
-            df = df.str.replace('Mongol Peo Rep',  'Mongolia',                    case = False, regex = True)
-            df = df.str.replace('Neth Antilles',   'Saint Martin',                case = False, regex = True)
-            df = df.str.replace('North Ireland',   'Ireland',                     case = False, regex = True)
-            df = df.str.replace('Peoples R China', 'China',                       case = False, regex = True)
-            df = df.str.replace('Rep of Georgia',  'Georgia',                     case = False, regex = True)
-            df = df.str.replace('Sao Tome E Prin', 'Sao Tome and Principe',       case = False, regex = True)
-            df = df.str.replace('St Kitts & Nevi', 'Saint Kitts and Nevis',       case = False, regex = True)
-            df = df.str.replace('Trinid & Tobago', 'Trinidad and Tobago',         case = False, regex = True)
-            df = df.str.replace('U Arab Emirates', 'United Arab Emirates',        case = False, regex = True)
-            df = df.str.lower()
-            for i in range(0, len(self.aut)):
-                for j in range(0, len(self.aut[i])):
-                    df = df.str.replace(self.aut[i][j], self.aut[i][j].replace('.', ''), regex = True)
+        df = df.str.replace(' USA',            ' United States of America',   case = False, regex = True)
+        df = df.str.replace('ENGLAND',         'United Kingdom',              case = False, regex = True)
+        df = df.str.replace('Antigua & Barbu', 'Antigua and Barbuda',         case = False, regex = True)
+        df = df.str.replace('Bosnia & Herceg', 'Bosnia and Herzegovina',      case = False, regex = True)
+        df = df.str.replace('Cent Afr Republ', 'Central African Republic',    case = False, regex = True)
+        df = df.str.replace('Dominican Rep',   'Dominican Republic',          case = False, regex = True)
+        df = df.str.replace('Equat Guinea',    'Equatorial Guinea',           case = False, regex = True)
+        df = df.str.replace('Fr Austr Lands',  'French Southern Territories', case = False, regex = True)
+        df = df.str.replace('Fr Polynesia',    'French Polynesia',            case = False, regex = True)
+        df = df.str.replace('Malagasy Republ', 'Madagascar',                  case = False, regex = True)
+        df = df.str.replace('Mongol Peo Rep',  'Mongolia',                    case = False, regex = True)
+        df = df.str.replace('Neth Antilles',   'Saint Martin',                case = False, regex = True)
+        df = df.str.replace('North Ireland',   'Ireland',                     case = False, regex = True)
+        df = df.str.replace('Peoples R China', 'China',                       case = False, regex = True)
+        df = df.str.replace('Rep of Georgia',  'Georgia',                     case = False, regex = True)
+        df = df.str.replace('Sao Tome E Prin', 'Sao Tome and Principe',       case = False, regex = True)
+        df = df.str.replace('St Kitts & Nevi', 'Saint Kitts and Nevis',       case = False, regex = True)
+        df = df.str.replace('Trinid & Tobago', 'Trinidad and Tobago',         case = False, regex = True)
+        df = df.str.replace('U Arab Emirates', 'United Arab Emirates',        case = False, regex = True)
+        df = df.str.lower()
+        for i in range(0, len(self.aut)):
+            for j in range(0, len(self.aut[i])):
+                df = df.str.replace(self.aut[i][j], self.aut[i][j].replace('.', ''), regex = True)
         ctrs = [[] for i in range(0, df.shape[0])]
-        if (self.data_base == 'scopus'):
-            for i in range(0, df.shape[0]):
+        for i in range(0, self.data.shape[0]):
+            if (self.data.loc[i, 'source'].lower() == 'scopus'):
                 affiliations = str(df[i]).strip().split(';')
                 for affiliation in affiliations:
                     for country in self.country_names:
                         if (country.lower() in affiliation.lower()):
                             ctrs[i].append(country)
                             break
-        if (self.data_base == 'pubmed'):
-            for i in range(0, df.shape[0]):
+            if (self.data.loc[i, 'source'].lower()  == 'pubmed'):
                 affiliations = str(df[i]).strip().split(',')
                 for affiliation in affiliations:
                     for country in self.country_names:
                         if (country.lower() in affiliation.lower()):
                             ctrs[i].append(country)
                             break
-        elif (self.data_base == 'wos'):
-           for i in range(0, df.shape[0]): 
-               affiliations = str(df[i]).strip().split('.')[:-1]
-               for affiliation in affiliations:
-                    for j in range(0, len(self.aut[i])):
-                        for country in self.country_names:
-                            if (country.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') in affiliation.lower()):
-                                ctrs[i].append(country)
-                                break
+            if (self.data.loc[i, 'source'].lower()  == 'wos'):
+                affiliations = str(df[i]).strip().split('.')[:-1]
+                for affiliation in affiliations:
+                     for j in range(0, len(self.aut[i])):
+                         for country in self.country_names:
+                             if (country.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') in affiliation.lower()):
+                                 ctrs[i].append(country)
+                                 break
         for i in range(0, len(ctrs)):
             while len(self.aut[i]) > len(ctrs[i]):
                 if (len(ctrs[i]) == 0):
                     ctrs[i].append('UNKNOW')
                 ctrs[i].append(ctrs[i][-1])
             if (len(ctrs[i]) == 0):
                 ctrs[i].append('UNKNOW')
@@ -1307,97 +1311,83 @@
         u_ctrs = list(set(u_ctrs))
         if (len(u_ctrs[0]) == 0):
             u_ctrs = u_ctrs[1:]
         return ctrs, u_ctrs
   
     # Function: Get Institutions
     def __get_institutions(self):
-        if   (self.data_base == 'scopus' or self.data_base == 'pubmed'):
+        if ('affiliation' in self.data.columns and 'affiliations' in self.data.columns and 'affiliation_' in self.data.columns):
+            df = self.data['affiliation']
+            df = pd.Series(np.zeros(self.data.shape[0]))
+            for i in range(0, self.data.shape[0]):
+                if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
+                    df[i] = self.data.loc[i, 'affiliation']
+                elif (self.data.loc[i, 'source'].lower() == 'wos'):
+                    df[i] = self.data.loc[i, 'affiliation_']
+        elif ('affiliation' in self.data.columns and 'affiliations' in self.data.columns):
             df = self.data['affiliation']
             df = df.str.lower()
-        elif (self.data_base == 'wos'):
+        elif ('affiliation' in self.data.columns and 'affiliation_' in self.data.columns):
             df = self.data['affiliation_']
             df = df.str.lower()
-            for i in range(0, len(self.aut)):
-                for j in range(0, len(self.aut[i])):
-                    df = df.str.replace(self.aut[i][j], self.aut[i][j].replace('.', ''), regex = True)
+        for i in range(0, len(self.aut)):
+            for j in range(0, len(self.aut[i])):
+                df = df.str.replace(self.aut[i][j], self.aut[i][j].replace('.', ''), regex = True)
         inst  = [[] for i in range(0, df.shape[0])]
         inst_ = [[] for i in range(0, df.shape[0])]
-        if  (self.data_base == 'scopus'):
-            for i in range(0, df.shape[0]):
+        for i in range(0, df.shape[0]):
+            if  (self.data.loc[i, 'source'].lower() == 'scopus'):
                 affiliations = str(df[i]).split(';')
                 for affiliation in affiliations:
                     for institution in self.institution_names:
                         if (institution.lower() in affiliation.lower()):
                             if (affiliation.strip() not in inst[i]):
                                 inst[i].append(affiliation.strip())
                             break
-            for i in range(0, len(inst)):
-                for j in range(0, len(inst[i])):
-                    item = inst[i][j].split(',')
-                    for institution in self.institution_names:
-                        idx = [k for k in range(0, len(item)) if institution in item[k].lower()]
-                        if (len(idx) > 0):
-                            institution_name = item[idx[0]]
-                            institution_name = ' '.join(institution_name.split())
-                            inst_[i].append(institution_name)
-                            break
-        if  (self.data_base == 'pubmed'):
-            for i in range(0, df.shape[0]):
+            if  (self.data.loc[i, 'source'].lower() == 'pubmed'):
                 affiliations = str(df[i]).split(',')
                 for affiliation in affiliations:
                     for institution in self.institution_names:
                         if (institution.lower() in affiliation.lower()):
                             if (affiliation.strip() not in inst[i]):
                                 inst[i].append(affiliation.strip())
                             break
-            for i in range(0, len(inst)):
-                for j in range(0, len(inst[i])):
-                    item = inst[i][j].split(',')
-                    for institution in self.institution_names:
-                        idx = [k for k in range(0, len(item)) if institution in item[k].lower()]
-                        if (len(idx) > 0):
-                            institution_name = item[idx[0]]
-                            institution_name = ' '.join(institution_name.split())
-                            inst_[i].append(institution_name)
-                            break
-        elif (self.data_base == 'wos'):
-            for i in range(0, df.shape[0]): 
-               df[i]        = df[i].replace('(corresponding author),',',')
-               affiliations = str(df[i]).strip().split('.')[:-1]
-               for affiliation in affiliations:
-                    for j in range(0, len(self.aut[i])):
-                        for institution in self.institution_names:
-                            if (institution.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') in affiliation.lower()):
-                                if (affiliation.strip() not in inst[i]):
-                                    inst[i].append(affiliation.strip().replace('\&', 'and'))
-                                break  
-                            elif (institution.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') not in affiliation.lower()):
-                                if (',' in self.aut[i][j]):
-                                    name_parts = self.aut[i][j].lower().replace('.', '').split(', ')
-                                    last_name  = name_parts[0]
-                                    initials   = [part[0] for part in name_parts[1:]]
-                                else:
-                                    name_parts  = self.aut[i][j].split()
-                                    initials    = name_parts[0][0]
-                                    last_name   = name_parts[-1]
-                                if (last_name in affiliation.lower() and  all(initial in affiliation.lower() for initial in initials)):
-                                    if (affiliation.strip() not in inst[i]):
-                                        inst[i].append(affiliation.strip().replace('\&', 'and'))
-                                    break 
-            for i in range(0, len(inst)):
-                for j in range(0, len(inst[i])):
-                    item = inst[i][j].split(',')
-                    for institution in self.institution_names:
-                        idx = [k for k in range(0, len(item)) if institution in item[k].lower()]
-                        if (len(idx) > 0):
-                            institution_name = item[idx[0]]
-                            institution_name = ' '.join(institution_name.split())
-                            inst_[i].append(institution_name)
-                            break
+            if (self.data.loc[i, 'source'].lower() == 'wos'):
+                df[i]        = df[i].replace('(corresponding author),',',')
+                affiliations = str(df[i]).strip().split('.')[:-1]
+                for affiliation in affiliations:
+                     for j in range(0, len(self.aut[i])):
+                         for institution in self.institution_names:
+                             if (institution.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') in affiliation.lower()):
+                                 if (affiliation.strip() not in inst[i]):
+                                     inst[i].append(affiliation.strip().replace('\&', 'and'))
+                                 break  
+                             elif (institution.lower() in affiliation.lower() and self.aut[i][j].lower().replace('.', '') not in affiliation.lower()):
+                                 if (',' in self.aut[i][j]):
+                                     name_parts = self.aut[i][j].lower().replace('.', '').split(', ')
+                                     last_name  = name_parts[0]
+                                     initials   = [part[0] for part in name_parts[1:]]
+                                 else:
+                                     name_parts  = self.aut[i][j].split()
+                                     initials    = name_parts[0][0]
+                                     last_name   = name_parts[-1]
+                                 if (last_name in affiliation.lower() and  all(initial in affiliation.lower() for initial in initials)):
+                                     if (affiliation.strip() not in inst[i]):
+                                         inst[i].append(affiliation.strip().replace('\&', 'and'))
+                                     break 
+        for i in range(0, len(inst)):
+            for j in range(0, len(inst[i])):
+                item = inst[i][j].split(',')
+                for institution in self.institution_names:
+                    idx = [k for k in range(0, len(item)) if institution in item[k].lower()]
+                    if (len(idx) > 0):
+                        institution_name = item[idx[0]]
+                        institution_name = ' '.join(institution_name.split())
+                        inst_[i].append(institution_name)
+                        break
         for i in range(0, len(inst_)):
             while len(self.aut[i]) > len(inst_[i]):
                 if (len(inst_[i]) == 0):
                     inst_[i].append('UNKNOW')
                 inst_[i].append(inst_[i][-1])
             if (len(inst_[i]) == 0):
                 inst_[i].append('UNKNOW')
@@ -2699,20 +2689,24 @@
             for j in range(0, len(self.ref[i])):
                 try:
                     k = self.u_ref.index(self.ref[i][j])
                     self.matrix_r.iloc[i, k] = self.matrix_r.iloc[i, k] + 1
                 except:
                     pass      
         self.labels_r = ['r_'+str(i) for i in range(0, self.matrix_r.shape[1])]
-        if   (self.data_base == 'scopus'):
-            keys = self.data['title'].tolist()
-            keys = [item.lower().replace('[','').replace(']','') for item in keys]
-        elif (self.data_base == 'wos'):
-            keys = self.data['doi'].tolist()
-            keys = [item.lower() for item in keys]
+        keys_1 = self.data['title'].tolist()
+        keys_1 = [item.lower().replace('[','').replace(']','') for item in keys_1]
+        keys_2 = self.data['doi'].tolist()
+        keys_2 = [item.lower() for item in keys_2]
+        keys   = [[] for item in keys_1]
+        for i in range(0, self.data.shape[0]):   
+            if   (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
+                keys[i] = keys_1[i]
+            elif (self.data.loc[i, 'source'].lower() == 'wos'):
+                keys[i] = keys_2[i]
         insd_r = []
         insd_t = []
         corp   = []
         if (len(self.u_ref) > 0):
             corp.append(self.u_ref[0].lower())
             for i in range(1, len(self.u_ref)):
                 corp[-1] = corp[-1]+' '+self.u_ref[i].lower()
@@ -4016,15 +4010,15 @@
         fig    = go.Figure(data = [trace], layout = layout)
         fig.show()
         return self
  
 ############################################################################
 
     # Function: Abstractive Text Summarization # Model Name List = https://huggingface.co/models?pipeline_tag=summarization&sort=downloads&search=pegasus
-    def summarize_abst_peg(self, article_ids = [], model_name = 'google/pegasus-xsum'):
+    def summarize_abst_peg(self, article_ids = [], model_name = 'google/pegasus-xsum', min_L = 100, max_L = 150):
         abstracts = self.data['abstract']
         corpus    = []
         if (len(article_ids) == 0):
             article_ids = [i for i in range(0, abstracts.shape[0])]
         else:
             article_ids = [int(item) for item in article_ids]
         for i in range(0, abstracts.shape[0]):
@@ -4033,17 +4027,17 @@
         if (len(corpus) > 0):
             print('')
             print('Total Number of Valid Abstracts: ', len(corpus))
             print('')
             corpus    = ' '.join(corpus)
             tokenizer = PegasusTokenizer.from_pretrained(model_name)
             pegasus   = PegasusForConditionalGeneration.from_pretrained(model_name)
-            tokens    = tokenizer(corpus, truncation = True, padding = 'longest', return_tensors = 'pt')
-            summary   = pegasus.generate(**tokens) # max_new_tokens = 1024, max_length = 1024, 
-            summary   = tokenizer.decode(summary[0])
+            tokens    = tokenizer.encode(corpus, return_tensors = 'pt', max_length = max_L, truncation = True)
+            summary   = pegasus.generate(tokens, min_length = min_L, max_length = max_L, length_penalty = 2.0, num_beams = 4, early_stopping = True)
+            summary   = tokenizer.decode(summary[0], skip_special_tokens = True)
         else:
             summary   = 'No abstracts were found in the selected set of documents'
         return summary
     
     # Function: Abstractive Text Summarization
     def summarize_abst_chatgpt(self, article_ids = [], join_articles = False, api_key = 'your_api_key_here', query = 'from the following scientific abstracts, summarize the main information in a single paragraph using around 250 words', model = 'text-davinci-003', max_tokens = 250, n = 1, temperature = 0.8):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
```

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Chinese.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Greek.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Hebrew.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Japanese.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Korean.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Slovak.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Thai.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX/base/stws/Stopwords-Ukrainian.txt` & `pyBibX-3.1.4/pyBibX/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/pyBibX.egg-info/PKG-INFO` & `pyBibX-3.1.4/pyBibX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.0.7
+Version: 3.1.4
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.0.7/pyBibX.egg-info/SOURCES.txt` & `pyBibX-3.1.4/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.0.7/setup.py` & `pyBibX-3.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='3.0.7',
+    version='3.1.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

