# Comparing `tmp/pyceurmake-0.2.4.tar.gz` & `tmp/pyceurmake-0.2.5.tar.gz`

## Comparing `pyceurmake-0.2.4.tar` & `pyceurmake-0.2.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/.pydevproject
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/.github/workflows/cache.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/__init__.py
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/ceur_ws.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/ceur_ws_cmd.py
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/indexparser.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/namedqueries.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/papertocparser.py
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/querydisplay.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/template.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/textparser.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/version.py
--rw-r--r--   0        0        0    44784 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/volumebrowser.py
--rw-r--r--   0        0        0    17626 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/volumeparser.py
--rw-r--r--   0        0        0    51440 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/wikidatasync.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/workshop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/models/__init__.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/models/dblp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/resources/ceurws.db
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/resources/queries/ceurws.yaml
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/resources/queries/dblp.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/utils/__init__.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/utils/download.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/utils/json_cache.py
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/ceurws/utils/webscrape.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/css/ceur-ws-semantic.css
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/css/ceur-ws.css
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/css/md_style_indigo.css
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/css/pygments.css
--rw-r--r--   0        0        0    19162 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/resources/queries.yaml
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/doc
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/getceurws
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/install
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/installAndTest
--rwxr-xr-x   0        0        0     3066 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/k10plus
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/queries
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/test
--rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/scripts/wdquery
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/basetest.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_indexhtml_scrape.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_namedqueries.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_papertocparser.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_sessions.py
--rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_volume.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_volumeparser.py
--rw-r--r--   0        0        0    31472 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_wikidatasync.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/tests/test_workshop.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/LICENSE
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/README.md
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyceurmake-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/.pydevproject
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/.github/workflows/cache.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/__init__.py
+-rw-r--r--   0        0        0    23247 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/ceur_ws.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/ceur_ws_cmd.py
+-rw-r--r--   0        0        0     9667 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/indexparser.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/namedqueries.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/papertocparser.py
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/querydisplay.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/template.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/textparser.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/version.py
+-rw-r--r--   0        0        0    44757 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/volumebrowser.py
+-rw-r--r--   0        0        0    17626 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/volumeparser.py
+-rw-r--r--   0        0        0    51440 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/wikidatasync.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/workshop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/models/__init__.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/models/dblp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/resources/ceurws.db
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/resources/queries/ceurws.yaml
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/resources/queries/dblp.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/utils/__init__.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/utils/download.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/utils/json_cache.py
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/ceurws/utils/webscrape.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/css/ceur-ws-semantic.css
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/css/ceur-ws.css
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/css/md_style_indigo.css
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/css/pygments.css
+-rw-r--r--   0        0        0    19162 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/resources/queries.yaml
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/doc
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/getceurws
+-rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/install
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/installAndTest
+-rwxr-xr-x   0        0        0     3066 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/k10plus
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/queries
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/test
+-rwxr-xr-x   0        0        0      694 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/scripts/wdquery
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/basetest.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_indexhtml_scrape.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_papertocparser.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_sessions.py
+-rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_volume.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_volumeparser.py
+-rw-r--r--   0        0        0    31472 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_wikidatasync.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/tests/test_workshop.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/README.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 pyceurmake-0.2.5/PKG-INFO
```

### Comparing `pyceurmake-0.2.4/.project` & `pyceurmake-0.2.5/.project`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/.github/workflows/build.yml` & `pyceurmake-0.2.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/.github/workflows/cache.yml` & `pyceurmake-0.2.5/.github/workflows/cache.yml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/.github/workflows/upload-to-pypi.yml` & `pyceurmake-0.2.5/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/ceur_ws.py` & `pyceurmake-0.2.5/ceurws/ceur_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,14 +328,15 @@
         super(VolumeManager, self).__init__(listName="volumes",
                                             clazz=Volume,
                                             tableName=tableName,
                                             entityName=Volume.__class__.__name__,
                                             primaryKey="number",
                                             entityPluralName="volumes",
                                             config=CEURWS.CONFIG,
+                                            handleInvalidListTypes=True,
                                             name=self.__class__.__name__)
 
 
     def load(self):
         '''
         load the volumeManager
         '''
```

### Comparing `pyceurmake-0.2.4/ceurws/ceur_ws_cmd.py` & `pyceurmake-0.2.5/ceurws/ceur_ws_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     parser = ArgumentParser(description=description, formatter_class=RawDescriptionHelpFormatter)
     parser.add_argument("-a","--about",help="show about info [default: %(default)s]",action="store_true")
     parser.add_argument("-c","--client", action="store_true", help="start client [default: %(default)s]")
     parser.add_argument("-d", "--debug", dest="debug", action="store_true", help="show debug info [default: %(default)s]")
     parser.add_argument("--host",default=JustpyServer.getDefaultHost(),help="the host to serve / listen from [default: %(default)s]")
     parser.add_argument("-l", "--list", action="store_true", help="list all volumes [default: %(default)s]")
-    parser.add_argument("-rc","--recreate",action="store_true",help="recreated volume table")
+    parser.add_argument("-rc","--recreate",action="store_true",help="recreate caches e.g. volume table")
     parser.add_argument("-den","--dblp_endpoint_name",help="name of dblp endpoint to use %(default)s",default="qlever-dblp-plus")       
     parser.add_argument("-wen","--wikidata_endpoint_name",help="name of wikidata endpoint to use %(default)s",default="wikidata")       
     parser.add_argument("-wdu","--wikidata_update",action="store_true",help="update tables from wikidata")
     parser.add_argument("--port",type=int,default=9998,help="the port to serve from [default: %(default)s]")
     parser.add_argument("-s","--serve", action="store_true", help="start webserver [default: %(default)s]")
     parser.add_argument("-nq","--namedqueries", action="store_true", help="generate named queries [default: %(default)s]")
     parser.add_argument("-V", "--version", action='version', version=version_msg)
```

### Comparing `pyceurmake-0.2.4/ceurws/indexparser.py` & `pyceurmake-0.2.5/ceurws/indexparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,17 +132,37 @@
                         line=line.replace(tag,"")
                     line=line.replace("\r"," ")
                     title+=line+delim
                     delim=" "
                     tdIndex+=1
                 volume["tdtitle"]=html.unescape(title).strip()
 
+    def setSeeAlsoVolumes(self, volume:dict, firstLine: int, lastLine: int):
+        """
+        Extract and set the volume numbers form the see also list
+        Example result {"seealso": ["Vol-3067"]}
+
+        Args:
+            volume: the volumeRecord to modify
+            lineIndex: where to start setting the volumeTitle
+        """
+        volumes = []
+        see_also = ""
+        for line in range(firstLine, lastLine):
+            see_also += self.lines[line]
+        see_also_section = re.search(r'see also:(.*?)</font>', see_also, re.DOTALL | re.IGNORECASE)
+
+        if see_also_section:
+            # Extract the volumes using regex from the see also section
+            volumes = re.findall(r'<a href="#(Vol-\d+)">', see_also_section.group(1), re.IGNORECASE)
+        volume["seealso"] = volumes
+
     def getInfo(self,volume:dict,info:str,pattern,line:str):
         '''
-        get the info info for the given patterns trying to match the pattern on
+        get the info for the given patterns trying to match the pattern on
         the given line
         
         Args:
             volume(dict): the result dict
             info(str): the name of the dict key to fill
             pattern(regexp): the regular expression to check
             line(str): the line to check
@@ -183,14 +203,15 @@
         volume["toLine"]=toLine
         volume["valid"]=False
         volume["url"]=None
         volume["acronym"]=None
         volume["title"]=None
         volume["loctime"]=None
         self.setVolumeTitle(volume, fromLine)
+        self.setSeeAlsoVolumes(volume, fromLine, toLine)
         
         infoPattern={}
         infoMappings = [
             ("URN","urn"),
             ("ONLINE","url"),
             ("ARCHIVE","archive"),
             ("Edited by","editors"),
```

### Comparing `pyceurmake-0.2.4/ceurws/namedqueries.py` & `pyceurmake-0.2.5/ceurws/namedqueries.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/papertocparser.py` & `pyceurmake-0.2.5/ceurws/papertocparser.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/querydisplay.py` & `pyceurmake-0.2.5/ceurws/querydisplay.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/template.py` & `pyceurmake-0.2.5/ceurws/template.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/textparser.py` & `pyceurmake-0.2.5/ceurws/textparser.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/version.py` & `pyceurmake-0.2.5/ceurws/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class Version(object):
     """
     Version handling for VolumeBrowser
     """
     name = "CEUR-WS Volume Browser"
     version = ceurws.__version__
     date = '2022-08-14'
-    updated = '2023-03-28'
+    updated = '2023-06-18'
     description = 'CEUR-WS Volume browser',
     
     authors = 'Tim Holzheim, Wolfgang Fahl'
     
     doc_url="https://wiki.bitplan.com/index.php/pyCEURmake"
     chat_url="https://github.com/WolfgangFahl/pyCEURmake/discussions"
     cm_url="https://github.com/WolfgangFahl/pyCEURmake"
```

### Comparing `pyceurmake-0.2.4/ceurws/volumebrowser.py` & `pyceurmake-0.2.5/ceurws/volumebrowser.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 import asyncio
 import re
 import time
 from typing import List
 
 import justpy as jp
-from fastapi import APIRouter, HTTPException
+from fastapi import HTTPException
 from fastapi.responses import ORJSONResponse
 from jpwidgets.bt5widgets import About, Alert, App, IconButton, Switch, ProgressBar
 
 from ceurws.ceur_ws import Volume
 from ceurws.querydisplay import QueryDisplay
 from ceurws.wikidatasync import DblpEndpoint, WikidataSync
 from ceurws.template import TemplateEnv
@@ -841,15 +841,15 @@
         @jp.app.get("/volumes.json")
         async def volumes():
             """
             direct fastapi return of volumes
             """
             wdSync=self.assureWikidataSync()
             volumeList=wdSync.vm.getList()
-            return ORJSONResponse(volumeList)
+            return volumeList
         
         @jp.app.get("/proceedings.json")
         async def proceedings():
             """
             direct fastapi return of proceedings
             """
             wdSync=self.assureWikidataSync()
```

### Comparing `pyceurmake-0.2.4/ceurws/volumeparser.py` & `pyceurmake-0.2.5/ceurws/volumeparser.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/wikidatasync.py` & `pyceurmake-0.2.5/ceurws/wikidatasync.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/models/dblp.py` & `pyceurmake-0.2.5/ceurws/models/dblp.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/resources/queries/ceurws.yaml` & `pyceurmake-0.2.5/ceurws/resources/queries/ceurws.yaml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/resources/queries/dblp.yaml` & `pyceurmake-0.2.5/ceurws/resources/queries/dblp.yaml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/utils/download.py` & `pyceurmake-0.2.5/ceurws/utils/download.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/utils/json_cache.py` & `pyceurmake-0.2.5/ceurws/utils/json_cache.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/ceurws/utils/webscrape.py` & `pyceurmake-0.2.5/ceurws/utils/webscrape.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/css/ceur-ws-semantic.css` & `pyceurmake-0.2.5/css/ceur-ws-semantic.css`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/css/ceur-ws.css` & `pyceurmake-0.2.5/css/ceur-ws.css`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/css/md_style_indigo.css` & `pyceurmake-0.2.5/css/md_style_indigo.css`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/css/pygments.css` & `pyceurmake-0.2.5/css/pygments.css`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/resources/queries.yaml` & `pyceurmake-0.2.5/resources/queries.yaml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/scripts/doc` & `pyceurmake-0.2.5/scripts/doc`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/scripts/getceurws` & `pyceurmake-0.2.5/scripts/getceurws`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/scripts/k10plus` & `pyceurmake-0.2.5/scripts/k10plus`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/scripts/wdquery` & `pyceurmake-0.2.5/scripts/wdquery`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/basetest.py` & `pyceurmake-0.2.5/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/test_indexhtml_scrape.py` & `pyceurmake-0.2.5/tests/test_papertocparser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,102 +1,100 @@
 '''
-Created on 2022-08-11
+Created on 2023-03-22
 
 @author: wf
 '''
 from tests.basetest import Basetest
-from ceurws.ceur_ws import VolumeManager, CEURWS
-import datetime
-from ceurws.indexparser import IndexHtmlParser
-import logging
+
+from ceurws.ceur_ws import VolumeManager
+from ceurws.papertocparser import PaperTocParser
 from lodstorage.lod import LOD
+from ceurws.volumeparser import VolumeParser
+import json
+from tqdm import tqdm
+from collections import Counter
+import unittest
 
-class TestIndexHtml(Basetest):
+class TestPaperTocParser(Basetest):
     '''
-    Test reading the index HTML
+    Test parsing Volume pages
     '''
     
     def setUp(self, debug=False, profile=True):
+        """
+        setUp the tests
+        """
         Basetest.setUp(self, debug=debug, profile=profile)
         self.url= 'http://ceur-ws.org'
-        
-    def checkVolumes(self,volumes):
-        volumeCount=len(volumes)
-        print(f"{volumeCount} volumes found")
-        for index,volume in enumerate(volumes.values()):
-            volumeNumber=volume["number"]
-            expectedVolumeNumber=volumeCount-index
-            if volumeNumber!=expectedVolumeNumber:
-                print (f'{expectedVolumeNumber:4}:{volumeNumber:4} {expectedVolumeNumber-volumeNumber}')
-    
-    def volumesAsCsv(self,volumes,minVolumeNumber,maxVolumeNumber):
-        '''
-        show the given range of volumes in CSV format
-        '''
-        for volume in volumes:
-            if volume.number>=minVolumeNumber and volume.number<=maxVolumeNumber:
-                print(f"{volume.number}\t{volume.acronym}\t{volume.desc}\t{volume.h1}\t{volume.title}\tQ1860\t{volume.published}\t{volume.urn}\t{volume.url}")
+        self.vm=VolumeManager()
+        self.volumeParser=VolumeParser(self.url,showHtml=False)
+        self.vm.load()
+        self.volumeList=self.vm.getList()
+        self.volumesByNumber, _duplicates = LOD.getLookup(self.volumeList, 'number')
+        
+    def check_paper_toc_parser(self,vol_number:str,counter:Counter,debug:bool=False,show_failure:bool=True)->list:
+        """
+        check the PaperTocParser with the given parameters
+        
+        Args:
+            vol_number(str): the number of the volume to parser
+            counter(Counter): the counter to keep track of the results and failures
+            debug(bool): if True print debugging information
+            show_failure: if True show reason message for failures / exceptions
             
-    def testVolumeManagerFromHtml(self):
-        vm=VolumeManager()
-        vm.loadFromIndexHtml(force=True)
-        withStore=False
-        if withStore:
-            vm.store()
-        
-    def testDates(self):
-        dateFormat='%d-%b-%Y'
-        now=datetime.datetime.now()
-        nows=now.strftime(dateFormat)
-        print(f"testing {nows} with {dateFormat}")
-        _pdate=datetime.datetime.strptime(nows, dateFormat)
-        
-        
-    def testReadingHtml(self):
-        '''
-        test reading the HTML file
-        '''
+        Returns:
+            list: a list paper records
+        """
+        try:
+            record,soup = self.volumeParser.parse_volume(vol_number)
+            if debug:
+                print(json.dumps(record,indent=2))
+            if soup:
+                    ptp=PaperTocParser(number=vol_number,soup=soup,debug=debug)
+                    paper_records=ptp.parsePapers()
+                    if debug:
+                        print(json.dumps(paper_records,indent=2))
+                    for paper_record in paper_records:
+                        for key in paper_record:
+                            counter[key]+=1
+                    return paper_records
+        except Exception as ex:
+            counter["failure"]+=1
+            if show_failure:
+                print(f"{vol_number} paper toc parsing fails with {str(ex)})")
+            return []
+        
+    def test_volExamples(self):
+        """
+        tests parsing of volume examples
+        """
+        vol_examples = [(3343,7),(2376,35),(2379,8),(1,15),(83,12),(3264,10)]
+        counter=Counter()
         debug=self.debug
         #debug=True
+        for vol_number,expected_papers in vol_examples:
+            paper_records=self.check_paper_toc_parser(vol_number, counter, debug)
+            self.assertEqual(expected_papers,len(paper_records),vol_number)
         if debug:
-            logging.basicConfig(level=logging.DEBUG)
-        vm=VolumeManager()
-        htmlText=vm.getIndexHtml(force=False)
-        indexParser=IndexHtmlParser(htmlText,debug=debug) 
-        lineCount=len(indexParser.lines)
-        self.assertTrue(lineCount>89500)
-        if debug or self.inPublicCI():
-            print(f"{lineCount} lines found in CEUR-WS index.html")
-        #limit=10
-        # volumes=indexParser.parse(limit=10,verbose=True)
-        volumes=indexParser.parse()
-        self.checkVolumes(volumes)
-        
-    def testVolumesAsCsv(self):
-        '''
-        test getting volumes from CSV
-        '''
-        vm=VolumeManager()
-        vm.load()
-        volumes=vm.getList()
-        self.volumesAsCsv(volumes,3185,3186)       
-        
-    def testReadVolumePages(self):
-        '''
-        test reading the volume pages
-        '''
-        withStore=False
-        vm=VolumeManager()
-        vm.loadFromIndexHtml(force=withStore)
-        volumesByNumber, _duplicates = LOD.getLookup(vm.getList(), 'number')
-        debug=self.debug or withStore
-        if self.inPublicCI():
-            limit=10
-        else:
-            limit=len(volumesByNumber)+1
-        for number in range(1,limit):
-            volume=volumesByNumber[number]
-            volume.extractValuesFromVolumePage()
-            if debug and volume.valid:
-                print(f"{volume.url}:{volume.acronym}:{volume.desc}:{volume.h1}:{volume.title}")
-        if withStore:
-            vm.store()
+            print(counter.most_common())
+        self.assertTrue(counter["pages"]>=60)
+          
+    @unittest.skipIf(True, "Only for manual testing or if github cache is implemented")           
+    def test_parse_all_papertocs(self):
+        """
+        test parsing all paper table of contents
+        """
+        debug=self.debug
+        t=None
+        progress=True
+        counter=Counter()
+        if progress:
+            t=tqdm(total=len(self.volumeList))
+        for volume in self.volumeList:
+            self.check_paper_toc_parser(volume.number, counter, debug)
+            if t:
+                t.description=f"{volume.number}"
+                t.update()
+        print(counter.most_common())
+            
+       
+
```

### Comparing `pyceurmake-0.2.4/tests/test_namedqueries.py` & `pyceurmake-0.2.5/tests/test_namedqueries.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/test_sessions.py` & `pyceurmake-0.2.5/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/test_volume.py` & `pyceurmake-0.2.5/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/test_volumeparser.py` & `pyceurmake-0.2.5/tests/test_volumeparser.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/test_wikidatasync.py` & `pyceurmake-0.2.5/tests/test_wikidatasync.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/tests/test_workshop.py` & `pyceurmake-0.2.5/tests/test_workshop.py`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/.gitignore` & `pyceurmake-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/LICENSE` & `pyceurmake-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/README.md` & `pyceurmake-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/pyproject.toml` & `pyceurmake-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyceurmake-0.2.4/PKG-INFO` & `pyceurmake-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCEURmake
-Version: 0.2.4
+Version: 0.2.5
 Project-URL: Home, https://github.com/WolfgangFahl/py-sidif
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Py-sidif
 Project-URL: Source, https://github.com/WolfgangFahl/py-sidif
 Author-email: Tim Holzheim <tim.holzheim@rwth-aachen.de>, Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Tim Holzheim <tim.holzheim@rwth-aachen.de>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

