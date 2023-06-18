# Comparing `tmp/bophono-0.1.2.tar.gz` & `tmp/bophono-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bophono-0.1.2.tar", last modified: Sat Jan 14 15:47:21 2023, max compression
+gzip compressed data, was "bophono-0.2.0.tar", last modified: Sun Jun 18 07:03:22 2023, max compression
```

## Comparing `bophono-0.1.2.tar` & `bophono-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 eroux     (1000) eroux     (1000)        0 2023-01-14 15:47:21.000000 bophono-0.1.2/
--rw-r--r--   0 eroux     (1000) eroux     (1000)     3532 2023-01-14 15:47:21.000000 bophono-0.1.2/PKG-INFO
--rw-r--r--   0 eroux     (1000) eroux     (1000)     2173 2023-01-14 15:35:46.000000 bophono-0.1.2/README.md
-drwxr-xr-x   0 eroux     (1000) eroux     (1000)        0 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono/
--rw-r--r--   0 eroux     (1000) eroux     (1000)     8561 2019-10-27 17:36:57.000000 bophono-0.1.2/bophono/PhonStateCAT.py
--rw-r--r--   0 eroux     (1000) eroux     (1000)     3480 2022-09-18 14:04:33.000000 bophono-0.1.2/bophono/PhonStateKVP.py
--rw-r--r--   0 eroux     (1000) eroux     (1000)    17975 2022-01-10 09:45:36.000000 bophono-0.1.2/bophono/PhonStateMST.py
--rw-r--r--   0 eroux     (1000) eroux     (1000)    16954 2021-04-20 18:45:33.000000 bophono-0.1.2/bophono/PhonStateMSTP.py
--rw-r--r--   0 eroux     (1000) eroux     (1000)     5273 2023-01-14 15:34:38.000000 bophono-0.1.2/bophono/UnicodeToApi.py
--rw-r--r--   0 eroux     (1000) eroux     (1000)      153 2023-01-14 15:46:48.000000 bophono-0.1.2/bophono/__init__.py
--rw-r--r--   0 eroux     (1000) eroux     (1000)     3103 2023-01-14 15:46:37.000000 bophono-0.1.2/bophono/apitochinese.py
-drwxr-xr-x   0 eroux     (1000) eroux     (1000)        0 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono/data/
--rw-r--r--   0 eroux     (1000) eroux     (1000)     1902 2019-10-27 17:36:57.000000 bophono-0.1.2/bophono/data/README.md
-drwxr-xr-x   0 eroux     (1000) eroux     (1000)        0 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono/data/chinese/
--rw-r--r--   0 eroux     (1000) eroux     (1000)     4857 2019-10-27 17:36:57.000000 bophono-0.1.2/bophono/data/chinese/chinese_trad.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)      847 2019-10-27 17:36:57.000000 bophono-0.1.2/bophono/data/chinese/exception.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)    13122 2019-10-27 17:36:57.000000 bophono-0.1.2/bophono/data/chinese/zhuyin.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)     2922 2022-01-03 10:35:27.000000 bophono-0.1.2/bophono/data/ends.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)     4922 2022-09-18 14:00:56.000000 bophono-0.1.2/bophono/data/exceptions-kvp.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)     6348 2022-09-18 14:08:46.000000 bophono-0.1.2/bophono/data/exceptions.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)     3890 2022-09-18 14:04:47.000000 bophono-0.1.2/bophono/data/roots.csv
--rw-r--r--   0 eroux     (1000) eroux     (1000)     6269 2021-10-10 14:21:41.000000 bophono-0.1.2/bophono/sdtrie.py
-drwxr-xr-x   0 eroux     (1000) eroux     (1000)        0 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono.egg-info/
--rw-r--r--   0 eroux     (1000) eroux     (1000)     3532 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono.egg-info/PKG-INFO
--rw-r--r--   0 eroux     (1000) eroux     (1000)      558 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono.egg-info/SOURCES.txt
--rw-r--r--   0 eroux     (1000) eroux     (1000)        1 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono.egg-info/dependency_links.txt
--rw-r--r--   0 eroux     (1000) eroux     (1000)        8 2023-01-14 15:47:21.000000 bophono-0.1.2/bophono.egg-info/top_level.txt
--rw-r--r--   0 eroux     (1000) eroux     (1000)       38 2023-01-14 15:47:21.000000 bophono-0.1.2/setup.cfg
--rw-r--r--   0 eroux     (1000) eroux     (1000)     1456 2023-01-14 15:45:22.000000 bophono-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:03:22.585115 bophono-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-18 07:03:13.000000 bophono-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-18 07:03:22.581115 bophono-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-18 07:03:13.000000 bophono-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:03:22.581115 bophono-0.2.0/bophono/
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/PhonStateCAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/PhonStateKVP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/PhonStateLKT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/PhonStateMST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/UnicodeToApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/apitochinese.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:03:22.581115 bophono-0.2.0/bophono/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:03:22.581115 bophono-0.2.0/bophono/data/chinese/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/chinese/chinese_trad.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/chinese/exception.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/chinese/zhuyin.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/ends.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/exceptions-kvp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/exceptions-lkt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/exceptions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/data/roots.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-18 07:03:13.000000 bophono-0.2.0/bophono/sdtrie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:03:22.581115 bophono-0.2.0/bophono.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-18 07:03:22.000000 bophono-0.2.0/bophono.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-18 07:03:22.000000 bophono-0.2.0/bophono.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:03:22.000000 bophono-0.2.0/bophono.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 07:03:22.000000 bophono-0.2.0/bophono.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:03:22.585115 bophono-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-18 07:03:13.000000 bophono-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bophono-0.1.2/README.md` & `bophono-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/PhonStateCAT.py` & `bophono-0.2.0/bophono/PhonStateCAT.py`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/PhonStateKVP.py` & `bophono-0.2.0/bophono/PhonStateKVP.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,25 @@
         self.end = None
         self.tone = None
         self.phon = ''
         self.options = options
         self.splitNG = options['splitNG'] if 'splitNG' in options else False
         self.splitKN = options['splitKN'] if 'splitKN' in options else False
         self.accentuateWL = options['accentuateWL'] if 'accentuateWL' in options else ["rime", "de", "ame", "chone", "dune", "dome", "tone", "chime", "done", "mine", "lame", "pale", "mare"]
+        self.accentuateall = options['accentuateWL'] if 'accentuateWL' in options else True
 
     def doCombineCurEnd(self, endofword, nrc='', nextvowel=''): # nrc = next root consonant
         """ combined the self.end into the self.phon """
         if not self.end:
             return
         # ' from ends.csv should be replaced with a space
         self.end = self.end.replace("'", ' ')
         # e at the end of a word becomes é
         if self.end.endswith("e") and endofword:
-            if self.phon+'e' in self.accentuateWL:
+            if self.accentuateall or self.phon+'e' in self.accentuateWL:
                 self.end = self.end[:-1]+"é"
         # suffix ga is "k" except in the middle of words
         if self.end.endswith("k") and not endofword:
             self.end = self.end[:-1]+"g"
         # nng or ngg -> ng
         if self.end.endswith("g") and nrc.startswith("g"):
             self.end = self.end[:-1]+"k"
@@ -73,15 +74,7 @@
                 # we suppose that roots are always null
                 self.combineWith(endsyl[:1], endsyl[1:])
         else:
             self.end = nextend
     
     def finish(self):
         self.doCombineCurEnd(True)
-
-if __name__ == '__main__':
-    """ Example use """
-    s = PhonStateKVP()
-    s.combineWith("dz-", "og")
-    s.combineWith("dz-", "og")
-    s.finish()
-    print(s.phon)
```

### Comparing `bophono-0.1.2/bophono/PhonStateMST.py` & `bophono-0.2.0/bophono/PhonStateMST.py`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/UnicodeToApi.py` & `bophono-0.2.0/bophono/UnicodeToApi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,44 @@
-import sys
-import csv
 import os
 from .sdtrie import *
 from .PhonStateMST import *
 from .PhonStateCAT import *
 from .PhonStateKVP import *
+from .PhonStateLKT import *
 
 class UnicodeToApi:
+    
     def __init__(self, schema="MST", options={}):
-        self.schema = schema
-        self.options = options
-        self.columnIndex = 1
-        if schema == "CAT":
+
+        if schema == 'MST':
+            self.columnIndex = 1
+            exceptions = "exceptions.csv"
+        
+        elif schema == "CAT":
             self.columnIndex = 2
-        if schema == "KVP":
+            exceptions = "exceptions.csv"
+        
+        elif schema == "KVP":
             self.columnIndex = 3
+            exceptions = "exceptions-kvp.csv"
+        
+        elif schema == 'LKT':
+            self.columnIndex = 4
+            exceptions = "exceptions-lkt.csv"
+            
+        else:
+            raise ValueError("schema must be MST, CAT, KVP, or LKT")
+
+        self.options = options
+        self.schema = schema
+        
         self.roots = get_trie_from_file(self.__get_trie_path("roots.csv"), "roots", self.columnIndex)
         self.ends = get_trie_from_file(self.__get_trie_path("ends.csv"), "ends", self.columnIndex)
-        if schema == "KVP":
-            self.exceptions = get_trie_from_file(self.__get_trie_path("exceptions-kvp.csv"), "exceptions", 1, self.ends)
-        else:
-            self.exceptions = get_trie_from_file(self.__get_trie_path("exceptions.csv"), "exceptions", 1, self.ends)
+        self.exceptions = get_trie_from_file(self.__get_trie_path(exceptions), "exceptions", 1, self.ends)
+
         self.ignored_chars = {'\u0FAD': True, '\u0F35': True, '\u0F37': True}
 
     def __get_trie_path(self, name):
         return os.path.join(os.path.split(__file__)[0], 'data', name)
 
     def __is_tib_letter(self, c):
         """is a tibetan letter"""
@@ -42,20 +56,14 @@
         """finds first letter index in tibstr after current index"""
         for i in range(current, eindex):
             letter = tibstr[i]
             if not self.__is_tib_letter(letter):
                 return i
         return -1
 
-    # def _combine(previous, rootinfo, endinfo=None):
-    #     rootinfod = rootinfo['d']
-    #     previousendinfod = previous and previous['endinfod'] or None
-    #     curphon = previous and previous['phon'] or ''
-    #     res = previous and previous['phon']+rootinfo['d'] or rootinfo['d']
-    #     return endinfo and res+endinfo['d'] or res
     def __combine_next_syll_phon(self, tibstr, bindex, state, eindex):
         # here we consider that we deal with a syllable starting at bindex, ending at eindex
         rootinfo = self.roots.get_longest_match_with_data(tibstr, bindex, eindex, self.ignored_chars)
         if not rootinfo:
             return -1
         endinfo = self.ends.get_longest_match_with_data(tibstr, rootinfo['i'], eindex, self.ignored_chars)
         if not endinfo:
@@ -68,22 +76,24 @@
 
     def get_api(self, tibstr, bindex=0, eindex=-1, pos=None, endOfSentence=False):
         if eindex == -1:
             eindex = len(tibstr)
         i = self.__get_next_letter_index(tibstr, bindex, eindex)
         if (i==-1):
             return ''
-        state = None
         # recreating one each time is suboptimal
-        if self.schema == 'CAT':
+        if self.schema == 'MST':
+            state = PhonStateMST(self.options, pos, endOfSentence)
+        elif self.schema == 'CAT':
             state = PhonStateCAT(self.options, pos, endOfSentence)
         elif self.schema == 'KVP':
             state = PhonStateKVP(self.options, pos, endOfSentence)
-        else:
-            state = PhonStateMST(self.options, pos, endOfSentence)
+        elif self.schema == 'LKT':
+            state = PhonStateLKT(self.options, pos, endOfSentence)
+
         while i < eindex and i >= 0: # > 0 covers the case where next_letter_index returns -1
             exceptioninfo = self.exceptions.get_longest_match_with_data(tibstr, i, eindex, self.ignored_chars)
             if (exceptioninfo and (state.position > 0 or not exceptioninfo['d'].startswith('2:'))) and (
                     exceptioninfo['i'] >= eindex or not self.__is_tib_letter(tibstr[exceptioninfo['i']])):
                 # if it starts with '2:' and we're in the first syllable, we ignore it:
                 if exceptioninfo['d'].startswith('2:'):
                     exceptioninfo['d'] = exceptioninfo['d'][2:]
```

### Comparing `bophono-0.1.2/bophono/apitochinese.py` & `bophono-0.2.0/bophono/apitochinese.py`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/README.md` & `bophono-0.2.0/bophono/data/README.md`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/chinese/chinese_trad.csv` & `bophono-0.2.0/bophono/data/chinese/chinese_trad.csv`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/chinese/exception.csv` & `bophono-0.2.0/bophono/data/chinese/exception.csv`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/chinese/zhuyin.csv` & `bophono-0.2.0/bophono/data/chinese/zhuyin.csv`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/ends.csv` & `bophono-0.2.0/bophono/data/ends.csv`

 * *Files 25% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-,a,a,a
-འ,a:,a,a
-ག,ak,əx,ak
-གས,ak,əx,ak
-ང,ang,əng,ang
-ངས,ang~,əng,ang
-ད,ä',ɛt,e
-ན,än,ɛn,en
-བ,ap,ab,ab
-བས,ap,ab,ab
-མ,am,am,am
-མས,am~,am,am
-ལ,äl,ɛl,al
-འི,äj,ɨ,e
-འིའོ,a|-i|-o,i|wo,e'o
-འོ,a|-o,a|o,a'o
-འང,a|-ang,a|wang,ang
-འམ,a|-am,a:m,am
-ར,ar,ər,ar
-ས,ä',e,e
-ི,i,i,i
-ིག,ik,ɨx,ik
-ིགས,ik,ɨx,ik
-ིང,ing,ang,ing
-ིངས,ing~,ang,ing
-ིད,i',it,i
-ིན,in,in,in
-ིབ,ip,ib,ib
-ིབས,ip,ib
-ིམ,im,im,im
-ིམས,im~,im,im
-ིལ,il,il,il
-ིའི,i:,i:,i
-ིའིའོ,i:|-o,,i'o
-ིའོ,i|-o,,i'o
-ིའང,i|-ang,,i'ang
-ིའམ,i|-am,,i'am
-ིར,ir,ir,ir
-ིས,i',i,i
-ུ,u,u,u
-ུག,uk,ɨx,uk
-ུགས,uk,ɨx,uk
-ུང,ung,ong,ung
-ུངས,ung~,ong,ung
-ུད,ü',ut,ü
-ུན,ün,un,ün
-ུབ,up,ub,ub
-ུབས,up,ub,ub
-ུམ,um,um,um
-ུམས,um~,um,um
-ུལ,ül,ul,ul
-ུའི,üj,ɨ,ü
-ུའིའོ,u|-i|-o,,ü'o
-ུའོ,u|-o,,ü'o
-ུའང,u|-ang,,u'ang
-ུའམ,u|-am,,u'am
-ུར,ur,ur,ur
-ུས,ü',i,ü
-ེ,e,e,e
-ེག,ek,əx,ek
-ེགས,ek,əx,ek
-ེང,eng,ang,eng
-ེངས,eng~,ang,eng
-ེད,e',et,e
-ེན,en,en,en
-ེབ,ep,eb,eb
-ེབས,ep,eb,eb
-ེམ,em,em,em
-ེམས,em~,em,em
-ེལ,el,el,el
-ེའི,ej,,e
-ེའིའོ,e|-i|-o,,e'o
-ེའོ,e|-o,,e'o
-ེའང,e|-ang,,e'ang
-ེའམ,e|-am,,e'am
-ེར,er,er,er
-ེས,e',i,e
-ོ,o,o,o
-ོག,ok,ox,ok
-ོགས,ok,ox,ok
-ོང,ong,ong,ong
-ོངས,ong~,ong,ong
-ོད,ö',ot,ö
-ོན,ön,wən,ön
-ོབ,op,ob,ob
-ོབས,op,ob,ob
-ོམ,om,om,om
-ོམས,om~,om,om
-ོལ,öl,ol,ol
-ོའི,öj,,ö
-ོའིའོ,o|-i|-o,,o
-ོའོ,o|-o,,o
-ོའང,o|-ang,,o'ang
-ོའམ,o|-am,,o'am
-ོར,or,or,or
-ོས,ö',i,ö
-འུ,a|-u,-u,a'u
-འུའི,a|-u|-i,,a'u
-འུའིའོ,a|-u|-i|-o,,a'u'o
-འུའོ,a|-u|-o,,a'u'o
-འུའང,a|-u|-ang,,a'u'ang
-འུའམ,a|-u|-am,,a'u'am
-འུར,a|-ur,ur,a'ur
-འུས,a|-ü',i,a'u
-ིའུ,i|-u,u,i'u
-ིའུའི,i|-u|-i,,i'ü
-ིའུའིའོ,i|-u|-i|-o,,i'ü'o
-ིའུའོ,i|-u|-o,,i'u'o
-ིའུའང,i|-u|-ang,,i'u'ang
-ིའུའམ,i|-u|-am,,i'u'am
-ིའུར,i|-ur,,i'ur
-ིའུས,i|-ü',,i'ü
-ུའུ,u|-u,u,u'u
-ུའུའི,u|-u|-i,u,u'ü
-ུའུའིའོ,u|-u|-i|-o,,u'ü'o
-ུའུའོ,u|-u|-o,,u'u'o
-ུའུའང,u|-u|-ang,,u'u'ang
-ུའུའམ,u|-u|-am,,u'u'am
-ུའུར,u|-ur,,e'ur
-ུའུས,u|-ü',,e'ü
-ེའུ,e|-u,u,e'u
-ེའུའི,e|-u|-i,,e'ü
-ེའུའིའོ,e|-u|-i|-o,,e'ü'o
-ེའུའོ,e|-u|-o,,e'u'o
-ེའུའང,e|-u|-ang,,e'u'ang
-ེའུའམ,e|-u|-am,,e'u'am
-ེའུར,e|-ur,,e'ur
-ེའུས,e|-ü',,e'ü
-ོའུ,o|-u,u,o'u
-ོའུའི,o|-u|-i,,o'ü
-ོའུའིའོ,o|-u|-i|-o,,o'ü'o
-ོའུའོ,o|-u|-o,,o'u'o
-ོའུའང,o|-u|-ang,,o'u'ang
-ོའུའམ,o|-u|-am,,o'u'am
-ོའུར,o|-ur,,o'ur
-ོའུས,o|-ü',,o'ü
+,a,a,a,a
+འ,a:,a,a,a
+ག,ak,əx,ak,ak
+གས,ak,əx,ak,ak
+ང,ang,əng,ang,ang
+ངས,ang~,əng,ang,ang
+ད,ä',ɛt,e,e
+ན,än,ɛn,en,en
+བ,ap,ab,ab,ab
+བས,ap,ab,ab,ab
+མ,am,am,am,am
+མས,am~,am,am,am
+ལ,äl,ɛl,al,al
+འི,äj,ɨ,e,e
+འིའོ,a|-i|-o,i|wo,e'o,e'o
+འོ,a|-o,a|o,a'o,a'o
+འང,a|-ang,a|wang,ang,ang
+འམ,a|-am,a:m,am,am
+ར,ar,ər,ar,ar
+ས,ä',e,e,e
+ི,i,i,i,i
+ིག,ik,ɨx,ik,ik
+ིགས,ik,ɨx,ik,ik
+ིང,ing,ang,ing,ing
+ིངས,ing~,ang,ing,ing
+ིད,i',it,i,i
+ིན,in,in,in,in
+ིབ,ip,ib,ib,ib
+ིབས,ip,ib,,
+ིམ,im,im,im,im
+ིམས,im~,im,im,im
+ིལ,il,il,il,il
+ིའི,i:,i:,i,i
+ིའིའོ,i:|-o,,i'o,i'o
+ིའོ,i|-o,,i'o,i'o
+ིའང,i|-ang,,i'ang,i'ang
+ིའམ,i|-am,,i'am,i'am
+ིར,ir,ir,ir,ir
+ིས,i',i,i,i
+ུ,u,u,u,u
+ུག,uk,ɨx,uk,uk
+ུགས,uk,ɨx,uk,uk
+ུང,ung,ong,ung,ung
+ུངས,ung~,ong,ung,ung
+ུད,ü',ut,ü,ü
+ུན,ün,un,ün,ün
+ུབ,up,ub,ub,ub
+ུབས,up,ub,ub,ub
+ུམ,um,um,um,um
+ུམས,um~,um,um,um
+ུལ,ül,ul,ul,ul
+ུའི,üj,ɨ,ü,ü
+ུའིའོ,u|-i|-o,,ü'o,ü'o
+ུའོ,u|-o,,ü'o,ü'o
+ུའང,u|-ang,,u'ang,u'ang
+ུའམ,u|-am,,u'am,u'am
+ུར,ur,ur,ur,ur
+ུས,ü',i,ü,ü
+ེ,e,e,e,e
+ེག,ek,əx,ek,ek
+ེགས,ek,əx,ek,ek
+ེང,eng,ang,eng,eng
+ེངས,eng~,ang,eng,eng
+ེད,e',et,e,e
+ེན,en,en,en,en
+ེབ,ep,eb,eb,eb
+ེབས,ep,eb,eb,eb
+ེམ,em,em,em,em
+ེམས,em~,em,em,em
+ེལ,el,el,el,el
+ེའི,ej,,e,e
+ེའིའོ,e|-i|-o,,e'o,e'o
+ེའོ,e|-o,,e'o,e'o
+ེའང,e|-ang,,e'ang,e'ang
+ེའམ,e|-am,,e'am,e'am
+ེར,er,er,er,er
+ེས,e',i,e,e
+ོ,o,o,o,o
+ོག,ok,ox,ok,ok
+ོགས,ok,ox,ok,ok
+ོང,ong,ong,ong,ong
+ོངས,ong~,ong,ong,ong
+ོད,ö',ot,ö,ö
+ོན,ön,wən,ön,ön
+ོབ,op,ob,ob,ob
+ོབས,op,ob,ob,ob
+ོམ,om,om,om,om
+ོམས,om~,om,om,om
+ོལ,öl,ol,ol,ol
+ོའི,öj,,ö,ö
+ོའིའོ,o|-i|-o,,o,o
+ོའོ,o|-o,,o,o
+ོའང,o|-ang,,o'ang,o'ang
+ོའམ,o|-am,,o'am,o'am
+ོར,or,or,or,or
+ོས,ö',i,ö,ö
+འུ,a|-u,-u,a'u,a'u
+འུའི,a|-u|-i,,a'u,a'u
+འུའིའོ,a|-u|-i|-o,,a'u'o,a'u'o
+འུའོ,a|-u|-o,,a'u'o,a'u'o
+འུའང,a|-u|-ang,,a'u'ang,a'u'ang
+འུའམ,a|-u|-am,,a'u'am,a'u'am
+འུར,a|-ur,ur,a'ur,a'ur
+འུས,a|-ü',i,a'u,a'u
+ིའུ,i|-u,u,i'u,i'u
+ིའུའི,i|-u|-i,,i'ü,i'ü
+ིའུའིའོ,i|-u|-i|-o,,i'ü'o,i'ü'o
+ིའུའོ,i|-u|-o,,i'u'o,i'u'o
+ིའུའང,i|-u|-ang,,i'u'ang,i'u'ang
+ིའུའམ,i|-u|-am,,i'u'am,i'u'am
+ིའུར,i|-ur,,i'ur,i'ur
+ིའུས,i|-ü',,i'ü,i'ü
+ུའུ,u|-u,u,u'u,u'u
+ུའུའི,u|-u|-i,u,u'ü,u'ü
+ུའུའིའོ,u|-u|-i|-o,,u'ü'o,u'ü'o
+ུའུའོ,u|-u|-o,,u'u'o,u'u'o
+ུའུའང,u|-u|-ang,,u'u'ang,u'u'ang
+ུའུའམ,u|-u|-am,,u'u'am,u'u'am
+ུའུར,u|-ur,,e'ur,e'ur
+ུའུས,u|-ü',,e'ü,e'ü
+ེའུ,e|-u,u,e'u,e'u
+ེའུའི,e|-u|-i,,e'ü,e'ü
+ེའུའིའོ,e|-u|-i|-o,,e'ü'o,e'ü'o
+ེའུའོ,e|-u|-o,,e'u'o,e'u'o
+ེའུའང,e|-u|-ang,,e'u'ang,e'u'ang
+ེའུའམ,e|-u|-am,,e'u'am,e'u'am
+ེའུར,e|-ur,,e'ur,e'ur
+ེའུས,e|-ü',,e'ü,e'ü
+ོའུ,o|-u,u,o'u,o'u
+ོའུའི,o|-u|-i,,o'ü,o'ü
+ོའུའིའོ,o|-u|-i|-o,,o'ü'o,o'ü'o
+ོའུའོ,o|-u|-o,,o'u'o,o'u'o
+ོའུའང,o|-u|-ang,,o'u'ang,o'u'ang
+ོའུའམ,o|-u|-am,,o'u'am,o'u'am
+ོའུར,o|-ur,,o'ur,o'ur
+ོའུས,o|-ü',,o'ü,o'ü
```

### Comparing `bophono-0.1.2/bophono/data/exceptions-kvp.csv` & `bophono-0.2.0/bophono/data/exceptions-kvp.csv`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/exceptions.csv` & `bophono-0.2.0/bophono/data/exceptions.csv`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono/data/roots.csv` & `bophono-0.2.0/bophono/data/roots.csv`

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-ཀ,k+,k,k
-ཀྱ,ky+,c,ky
-ཀྲ,tr+,tr,kr
-ཀླ,l+,l,l
-དཀ,k+,[r]k,k
-དཀྱ,ky+,[r]c,ky
-དཀྲ,tr+,[r]tr,tr
-བཀ,k+,[b]k,k
-བཀྱ,ky+,[b]c,ky
-བཀྲ,tr+,[b]tr,tr
-བཀླ,l+,[b]l,l,
-རྐ,k+,[r]k,k
-རྐྱ,ky+,[r]c,ky
-ལྐ,k+,[l]k,k
-སྐ,k+,[s]k,k
-སྐྱ,ky+,[s]c,ky
-སྐྲ,tr+,[s]tr,tr
-བརྐ,k+,[b]k,k
-བརྐྱ,ky+,[b]c,ky
-བསྐ,k+,[b]k,k
-བསྐྱ,ky+,[b]c,ky
-བསྐྲ,tr+,[b]tr,kr
-ཁ,kh+,k+,kh
-ཁྱ,khy+,c+,khy
-ཁྲ,thr+,tr+,tr
-མཁ,~kh+,[m]k+,kh
-མཁྱ,~khy+,[m]c+,khy
-མཁྲ,~thr+,[m]tr+,tr
-འཁ,~kh+,[']k+,kh
-འཁྱ,~khy+,[']c+,khy
-འཁྲ,~thr+,[']tr+,tr
-ག,kh-,k,g
-གྱ,khy-,c,gy
-གྲ,thr-,tr,tr
-གླ,l+,l,l
-དག*,k-,[r]g,g
-དགྱ,ky-,[r]j,gy
-དགྲ,tr-,[r]dr,dr
-བག*,k-,[b]g,g
-བགྱ,ky-,[b]j,gy
-བགྲ,tr-,[b]dr,dr
-མག*,~k-,[m]g,g
-མགྱ,~ky-,[m]j,gy
-མགྲ,~tr-,[m]dr,dr
-འག*,~k-,[']g,g
-འགྱ,~ky-,[']j,gy
-འགྲ,~tr-,[']dr,dr
-རྒ,k-,[r]g,g
-རྒྱ,ky-,[r]j,gy
-ལྒ,k-,[l]g,g
-སྒ,k-,[s]g,g
-སྒྱ,ky-,[s]j,gy
-སྒྲ,tr-,[s]dr,dr
-བརྒ,k-,g,g
-བརྒྱ,ky-,[b]j,gy
-བསྒ,k-,[b]g,g
-བསྒྱ,ky-,[b]j,gy
-བསྒྲ,tr-,[b]dr,dr
-ང,ng-,ng,ng
-དང*,ng+,[r]ng,ng
-མང*,~ng+,[m]ng,ng
-རྔ,ng+,[r]ng,ng
-ལྔ,ng+,[l]ng,ng
-སྔ,ng+,[s]ng,ng
-བརྔ,ng+,[b]ng,ng
-བསྔ,ng+,[b]ng,ng
-ཅ,c+,c,ch
-གཅ,c+,[r]c,ch
-བཅ,c+,[b]c,ch
-ལྕ,c+,[l]c,ch
-ཆ,ch+,c+,ch
-མཆ,~ch+,[m]c+,ch
-འཆ,~ch+,[b]c+,ch
-ཇ,ch-,c,j
-མཇ,~c-,[m]j,j
-འཇ,~c-,[']j,j
-རྗ,c-,[r]j,j
-ལྗ,~c-,[l]j,j
-བརྗ,c-,[b]j,j
-ཉ,ny-,ny,ny
-གཉ,ny+,[r]ny,ny
-མཉ,~ny+,[m]ny,ny
-རྙ,ny+,[r]ny,ny
-སྙ,ny+,[s]ny,ny
-བརྙ,ny+,[b]ny,ny
-བསྙ,ny+,[b]ny,ny
-ཏ,t+,t,t
-གཏ,t+,[r]t,t
-བཏ,t+,[b]t,t
-རྟ,t+,[r]t,t
-ལྟ,~t+,[l]t,t
-སྟ,t+,[s]t,t
-བརྟ,t+,[b]t,t
-བལྟ,t+,[b]t,t
-བསྟ,t+,[b]t,t
-ཐ,th+,t+,t
-མཐ,~th+,[m]t+,t
-འཐ,~th+,[']t+,t
-ད,th-,t,d
-དྲ,thr-,tr,d
-གད*,t-,[r]d,d
-བད*,t-,[b]d,d
-མད*,~t-,[m]d,d
-འད*,~t-,[']d,d
-འདྲ,~tr-,[']dr,dr
-རྡ,t-,[r]d,d
-ལྡ,~t-,[l]d,d
-སྡ,t-,[s]d,d
-བརྡ,t-,[b]d,d
-བལྡ,t-,[b]d,d
-བསྡ,t-,[b]d,d
-ན,n-,n,n
-གན*,n+,[r]n,n
-མན*,~n+,[m]n,n
-རྣ,n+,[r]n,n
-སྣ,n+,[s]n,n
-བརྣ,n+,[b]n,n
-བསྣ,n+,[b]n,n
-པ,p+,p,p
-པྱ,c+,sh,ch
-པྲ,tr+,tr,tr
-དཔ,p+,hw,p
-དཔྱ,c+,[r]sh,ch
-དཔྲ,tr+,tr,tr
-ལྤ,p+,[l]p,p
-སྤ,p+,[s]p,p
-སྤྱ,c+,[s]c,ch
-སྤྲ,tr+,[s]tr,tr
-ཕ,ph+,p+,p
-ཕྱ,ch+,sh,ch
-ཕྲ,thr+,tr+,tr
-འཕ,~ph+,[']ph,p
-འཕྱ,~ch+,[']sh,ch
-འཕྲ,~thr+,[']tr+,tr
-བ,ph-,w,b
-བྱ,ch-,sh,j
-བྲ,thr-,tr,dr
-བླ,l+,l,l
-དབ*,+,R,-
-དབྱ,y+,[r]y,y
-དབྲ,r+,,r
-འབ*,~p-,[']b,b
-འབྱ,~c-,[']j,j
-འབྲ,~tr-,,dr
-རྦ,p-,[r]b,b
-ལྦ,p-,[l]b,b
-སྦ,p-,[s]p,b
-སྦྱ,c-,[s]j,j
-སྦྲ,tr-,[s]dr,dr
-མ,m-,m,m
-མྱ,ny-,ny,ny
-དམ*,m+,[r]m,m
-དམྱ,ny+,[r]ny,ny
-རྨ,m+,[r]m,m
-རྨྱ,ny+,[r]ny,ny
-སྨ,m+,[s]m,m
-སྨྱ,ny+,[s]ny,ny
-ཙ,ts+,ts,ts
-གཙ,ts+,[r],ts
-བཙ,ts+,[b]ts,ts
-རྩ,ts+,[r]ts,ts
-སྩ,ts+,[s]ts,ts
-བརྩ,ts+,[b]ts,ts
-བསྩ,ts+,[b]ts,ts
-ཚ,tsh+,ts+,ts
-མཚ,~tsh+,[m]ts+,ts
-འཚ,~tsh+,[']ts+,ts
-ཛ,tsh-,ts,dz
-མཛ,~ts-,[m]ts,dz
-འཛ,~ts-,[']ts,dz
-རྫ,ts-,[r]dz,dz
-བརྫ,ts-,[b]dz,dz
-ཝ,w-,Rw,w
-ཞ,sh-,sh,zh
-གཞ,sh-,[r]sh,zh
-བཞ,sh-,[b]sh,zh
-ཟ,s-,s,z
-ཟླ,~t-,d,d
-གཟ,s-,[r]z,z
-བཟ,s-,[b]z,z
-བཟླ,t-,[b]d,d
-འ,-,_,-
-ཡ,y-,y,y
-གཡ,y+,[r]y,y
-ར,r-,r,r
-རླ,l+,[r]l,l
-བརླ,l+,[r]l,l
-ལ,l-,l,l
-ཤ,sh+,x,sh
-གཤ,sh+,[r]x,sh
-བཤ,sh+,[b]x,sh
-ས,s+,s+,s
-སྲ,s+,sr,s
-སླ,l+,l+,l
-གས*,s+,[r]s+,s
-བས*,s+,[b]s+,s
-བསྲ,s+,[b]sr,s
-བསླ,l+,[b]l+,l
-ཧ,h+,h,h
-ཧྲ,rh+,sr,hr
-ལྷ,lh+,l+,lh
-ཨ,+,_,-
-བགླ,l+,l,l
-མྲ,m+,m,m
-སྨྲ,m+,m,m
-ཏྲ,tr+,tr,tr
-བརྟ,t+,[b]t,t
-ཐྲ,thr+,tr+,tr
-སྣྲ,n+,[b]n,n
+ཀ,k+,k,k,k
+ཀྱ,ky+,c,ky,ky
+ཀྲ,tr+,tr,kr,kr
+ཀླ,l+,l,l,l
+དཀ,k+,[r]k,k,k
+དཀྱ,ky+,[r]c,ky,ky
+དཀྲ,tr+,[r]tr,tr,tr
+བཀ,k+,[b]k,k,k
+བཀྱ,ky+,[b]c,ky,ky
+བཀྲ,tr+,[b]tr,tr,tr
+བཀླ,l+,[b]l,l,l
+རྐ,k+,[r]k,k,k
+རྐྱ,ky+,[r]c,ky,ky
+ལྐ,k+,[l]k,k,k
+སྐ,k+,[s]k,k,k
+སྐྱ,ky+,[s]c,ky,ky
+སྐྲ,tr+,[s]tr,tr,tr
+བརྐ,k+,[b]k,k,k
+བརྐྱ,ky+,[b]c,ky,ky
+བསྐ,k+,[b]k,k,k
+བསྐྱ,ky+,[b]c,ky,ky
+བསྐྲ,tr+,[b]tr,kr,kr
+ཁ,kh+,k+,kh,kh
+ཁྱ,khy+,c+,khy,khy
+ཁྲ,thr+,tr+,tr,tr
+མཁ,~kh+,[m]k+,kh,kh
+མཁྱ,~khy+,[m]c+,khy,khy
+མཁྲ,~thr+,[m]tr+,tr,tr
+འཁ,~kh+,[']k+,kh,kh
+འཁྱ,~khy+,[']c+,khy,khy
+འཁྲ,~thr+,[']tr+,tr,tr
+ག,kh-,k,g,g
+གྱ,khy-,c,gy,gy
+གྲ,thr-,tr,tr,tr
+གླ,l+,l,l,l
+དག*,k-,[r]g,g,g
+དགྱ,ky-,[r]j,gy,gy
+དགྲ,tr-,[r]dr,dr,dr
+བག*,k-,[b]g,g,g
+བགྱ,ky-,[b]j,gy,gy
+བགྲ,tr-,[b]dr,dr,dr
+མག*,~k-,[m]g,g,g
+མགྱ,~ky-,[m]j,gy,gy
+མགྲ,~tr-,[m]dr,dr,dr
+འག*,~k-,[']g,g,g
+འགྱ,~ky-,[']j,gy,gy
+འགྲ,~tr-,[']dr,dr,dr
+རྒ,k-,[r]g,g,g
+རྒྱ,ky-,[r]j,gy,gy
+ལྒ,k-,[l]g,g,g
+སྒ,k-,[s]g,g,g
+སྒྱ,ky-,[s]j,gy,gy
+སྒྲ,tr-,[s]dr,dr,dr
+བརྒ,k-,g,g,g
+བརྒྱ,ky-,[b]j,gy,gy
+བསྒ,k-,[b]g,g,g
+བསྒྱ,ky-,[b]j,gy,gy
+བསྒྲ,tr-,[b]dr,dr,dr
+ང,ng-,ng,ng,ng
+དང*,ng+,[r]ng,ng,ng
+མང*,~ng+,[m]ng,ng,ng
+རྔ,ng+,[r]ng,ng,ng
+ལྔ,ng+,[l]ng,ng,ng
+སྔ,ng+,[s]ng,ng,ng
+བརྔ,ng+,[b]ng,ng,ng
+བསྔ,ng+,[b]ng,ng,ng
+ཅ,c+,c,ch,ch
+གཅ,c+,[r]c,ch,ch
+བཅ,c+,[b]c,ch,ch
+ལྕ,c+,[l]c,ch,ch
+ཆ,ch+,c+,ch,ch
+མཆ,~ch+,[m]c+,ch,ch
+འཆ,~ch+,[b]c+,ch,ch
+ཇ,ch-,c,j,j
+མཇ,~c-,[m]j,j,j
+འཇ,~c-,[']j,j,j
+རྗ,c-,[r]j,j,j
+ལྗ,~c-,[l]j,j,j
+བརྗ,c-,[b]j,j,j
+ཉ,ny-,ny,ny,ny
+གཉ,ny+,[r]ny,ny,ny
+མཉ,~ny+,[m]ny,ny,ny
+རྙ,ny+,[r]ny,ny,ny
+སྙ,ny+,[s]ny,ny,ny
+བརྙ,ny+,[b]ny,ny,ny
+བསྙ,ny+,[b]ny,ny,ny
+ཏ,t+,t,t,t
+གཏ,t+,[r]t,t,t
+བཏ,t+,[b]t,t,t
+རྟ,t+,[r]t,t,t
+ལྟ,~t+,[l]t,t,t
+སྟ,t+,[s]t,t,t
+བརྟ,t+,[b]t,t,t
+བལྟ,t+,[b]t,t,t
+བསྟ,t+,[b]t,t,t
+ཐ,th+,t+,t,t
+མཐ,~th+,[m]t+,t,t
+འཐ,~th+,[']t+,t,t
+ད,th-,t,d,d
+དྲ,thr-,tr,d,d
+གད*,t-,[r]d,d,d
+བད*,t-,[b]d,d,d
+མད*,~t-,[m]d,d,d
+འད*,~t-,[']d,d,d
+འདྲ,~tr-,[']dr,dr,dr
+རྡ,t-,[r]d,d,d
+ལྡ,~t-,[l]d,d,d
+སྡ,t-,[s]d,d,d
+བརྡ,t-,[b]d,d,d
+བལྡ,t-,[b]d,d,d
+བསྡ,t-,[b]d,d,d
+ན,n-,n,n,n
+གན*,n+,[r]n,n,n
+མན*,~n+,[m]n,n,n
+རྣ,n+,[r]n,n,n
+སྣ,n+,[s]n,n,n
+བརྣ,n+,[b]n,n,n
+བསྣ,n+,[b]n,n,n
+པ,p+,p,p,p
+པྱ,c+,sh,ch,ch
+པྲ,tr+,tr,tr,tr
+དཔ,p+,hw,p,p
+དཔྱ,c+,[r]sh,ch,ch
+དཔྲ,tr+,tr,tr,tr
+ལྤ,p+,[l]p,p,p
+སྤ,p+,[s]p,p,p
+སྤྱ,c+,[s]c,ch,ch
+སྤྲ,tr+,[s]tr,tr,tr
+ཕ,ph+,p+,p,p
+ཕྱ,ch+,sh,ch,ch
+ཕྲ,thr+,tr+,tr,tr
+འཕ,~ph+,[']ph,p,p
+འཕྱ,~ch+,[']sh,ch,ch
+འཕྲ,~thr+,[']tr+,tr,tr
+བ,ph-,w,b,b
+བྱ,ch-,sh,j,j
+བྲ,thr-,tr,dr,dr
+བླ,l+,l,l,l
+དབ*,+,R,-,-
+དབྱ,y+,[r]y,y,y
+དབྲ,r+,,r,r
+འབ*,~p-,[']b,b,b
+འབྱ,~c-,[']j,j,j
+འབྲ,~tr-,,dr,dr
+རྦ,p-,[r]b,b,b
+ལྦ,p-,[l]b,b,b
+སྦ,p-,[s]p,b,b
+སྦྱ,c-,[s]j,j,j
+སྦྲ,tr-,[s]dr,dr,dr
+མ,m-,m,m,m
+མྱ,ny-,ny,ny,ny
+དམ*,m+,[r]m,m,m
+དམྱ,ny+,[r]ny,ny,ny
+རྨ,m+,[r]m,m,m
+རྨྱ,ny+,[r]ny,ny,ny
+སྨ,m+,[s]m,m,m
+སྨྱ,ny+,[s]ny,ny,ny
+ཙ,ts+,ts,ts,ts
+གཙ,ts+,[r],ts,ts
+བཙ,ts+,[b]ts,ts,ts
+རྩ,ts+,[r]ts,ts,ts
+སྩ,ts+,[s]ts,ts,ts
+བརྩ,ts+,[b]ts,ts,ts
+བསྩ,ts+,[b]ts,ts,ts
+ཚ,tsh+,ts+,ts,ts
+མཚ,~tsh+,[m]ts+,ts,ts
+འཚ,~tsh+,[']ts+,ts,ts
+ཛ,tsh-,ts,dz,dz
+མཛ,~ts-,[m]ts,dz,dz
+འཛ,~ts-,[']ts,dz,dz
+རྫ,ts-,[r]dz,dz,dz
+བརྫ,ts-,[b]dz,dz,dz
+ཝ,w-,Rw,w,w
+ཞ,sh-,sh,zh,zh
+གཞ,sh-,[r]sh,zh,zh
+བཞ,sh-,[b]sh,zh,zh
+ཟ,s-,s,z,z
+ཟླ,~t-,d,d,d
+གཟ,s-,[r]z,z,z
+བཟ,s-,[b]z,z,z
+བཟླ,t-,[b]d,d,d
+འ,-,_,-,-
+ཡ,y-,y,y,y
+གཡ,y+,[r]y,y,y
+ར,r-,r,r,r
+རླ,l+,[r]l,l,l
+བརླ,l+,[r]l,l,l
+ལ,l-,l,l,l
+ཤ,sh+,x,sh,sh
+གཤ,sh+,[r]x,sh,sh
+བཤ,sh+,[b]x,sh,sh
+ས,s+,s+,s,s
+སྲ,s+,sr,s,s
+སླ,l+,l+,l,l
+གས*,s+,[r]s+,s,s
+བས*,s+,[b]s+,s,s
+བསྲ,s+,[b]sr,s,s
+བསླ,l+,[b]l+,l,l
+ཧ,h+,h,h,h
+ཧྲ,rh+,sr,hr,hr
+ལྷ,lh+,l+,lh,lh
+ཨ,+,_,-,-
+བགླ,l+,l,l,l
+མྲ,m+,m,m,m
+སྨྲ,m+,m,m,m
+ཏྲ,tr+,tr,tr,tr
+བརྟ,t+,[b]t,t,t
+ཐྲ,thr+,tr+,tr,tr
+སྣྲ,n+,[b]n,n,n
```

### Comparing `bophono-0.1.2/bophono/sdtrie.py` & `bophono-0.2.0/bophono/sdtrie.py`

 * *Files identical despite different names*

### Comparing `bophono-0.1.2/bophono.egg-info/SOURCES.txt` & `bophono-0.2.0/bophono.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+LICENSE
 README.md
 setup.py
 bophono/PhonStateCAT.py
 bophono/PhonStateKVP.py
+bophono/PhonStateLKT.py
 bophono/PhonStateMST.py
-bophono/PhonStateMSTP.py
 bophono/UnicodeToApi.py
 bophono/__init__.py
 bophono/apitochinese.py
 bophono/sdtrie.py
 bophono.egg-info/PKG-INFO
 bophono.egg-info/SOURCES.txt
 bophono.egg-info/dependency_links.txt
 bophono.egg-info/top_level.txt
 bophono/data/README.md
 bophono/data/ends.csv
 bophono/data/exceptions-kvp.csv
+bophono/data/exceptions-lkt.csv
 bophono/data/exceptions.csv
 bophono/data/roots.csv
 bophono/data/chinese/chinese_trad.csv
 bophono/data/chinese/exception.csv
 bophono/data/chinese/zhuyin.csv
```

### Comparing `bophono-0.1.2/setup.py` & `bophono-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 assert(parse_version(setuptools.__version__) >= parse_version("38.6.0"))
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="bophono",
-    version="0.1.2",  #edit version in __init__.py
+    version="0.2.0",  #edit version in __init__.py
     author="Esukhia development team",
     author_email="roux.elie@gmail.com",
     description="Python utils for Tibetan phonetics in different dialects",
     license="MIT",
     keywords="phonetics IPA tibetan",
     url="https://github.com/Esukhia/bophono",
     packages=find_packages(),
```

