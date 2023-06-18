# Comparing `tmp/dtstools-0.0.1.tar.gz` & `tmp/dtstools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtstools-0.0.1.tar", last modified: Sat Jun 17 14:53:20 2023, max compression
+gzip compressed data, was "dtstools-0.0.2.tar", last modified: Sun Jun 18 11:22:30 2023, max compression
```

## Comparing `dtstools-0.0.1.tar` & `dtstools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-17 14:53:20.904538 dtstools-0.0.1/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.1/LICENSE
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11117 2023-06-17 14:53:20.903413 dtstools-0.0.1/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     9126 2023-06-17 11:06:19.000000 dtstools-0.0.1/README.md
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      867 2023-06-17 11:25:08.000000 dtstools-0.0.1/pyproject.toml
--rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-06-17 14:53:20.906813 dtstools-0.0.1/setup.cfg
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-17 14:53:20.895756 dtstools-0.0.1/src/
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-17 14:53:20.898947 dtstools-0.0.1/src/dtstools/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.1/src/dtstools/__init__.py
--rw-r--r--   0 reginaldosilva   (501) staff       (20)     7939 2023-06-17 10:54:35.000000 dtstools-0.0.1/src/dtstools/dtsTable.py
-drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-17 14:53:20.902073 dtstools-0.0.1/src/dtstools.egg-info/
--rw-r--r--   0 reginaldosilva   (501) staff       (20)    11117 2023-06-17 14:53:20.000000 dtstools-0.0.1/src/dtstools.egg-info/PKG-INFO
--rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-06-17 14:53:20.000000 dtstools-0.0.1/src/dtstools.egg-info/SOURCES.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-06-17 14:53:20.000000 dtstools-0.0.1/src/dtstools.egg-info/dependency_links.txt
--rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-06-17 14:53:20.000000 dtstools-0.0.1/src/dtstools.egg-info/top_level.txt
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 11:22:30.432920 dtstools-0.0.2/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     1072 2023-06-17 11:23:10.000000 dtstools-0.0.2/LICENSE
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11098 2023-06-18 11:22:30.432519 dtstools-0.0.2/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     9109 2023-06-18 11:17:00.000000 dtstools-0.0.2/README.md
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      865 2023-06-18 11:06:34.000000 dtstools-0.0.2/pyproject.toml
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)       38 2023-06-18 11:22:30.433015 dtstools-0.0.2/setup.cfg
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 11:22:30.427564 dtstools-0.0.2/src/
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 11:22:30.429653 dtstools-0.0.2/src/dtstools/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        0 2023-06-09 17:32:34.000000 dtstools-0.0.2/src/dtstools/__init__.py
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)     8089 2023-06-18 11:22:15.000000 dtstools-0.0.2/src/dtstools/dtsTable.py
+drwxr-xr-x   0 reginaldosilva   (501) staff       (20)        0 2023-06-18 11:22:30.431855 dtstools-0.0.2/src/dtstools.egg-info/
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)    11098 2023-06-18 11:22:30.000000 dtstools-0.0.2/src/dtstools.egg-info/PKG-INFO
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)      226 2023-06-18 11:22:30.000000 dtstools-0.0.2/src/dtstools.egg-info/SOURCES.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        1 2023-06-18 11:22:30.000000 dtstools-0.0.2/src/dtstools.egg-info/dependency_links.txt
+-rw-r--r--   0 reginaldosilva   (501) staff       (20)        9 2023-06-18 11:22:30.000000 dtstools-0.0.2/src/dtstools.egg-info/top_level.txt
```

### Comparing `dtstools-0.0.1/LICENSE` & `dtstools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtstools-0.0.1/PKG-INFO` & `dtstools-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package aims to provide features for working with Delta Lake.
 Author-email: Reginaldo Silva <reginaldo.silva@dataside.com.br>
 License: MIT License
         
         Copyright (c) 2023 Reginaldo Silva
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,44 +22,44 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: DataInAction, https://www.datainaction.dev/blog
-Project-URL: Bug Tracker, https://github.com/reginaldosilva27/Databricks
+Project-URL: Bug Tracker, https://github.com/reginaldosilva27/dtstools
 Project-URL: README, https://www.datainaction.dev/blog
 Project-URL: Dataside, https://www.dataside.com.br
 Keywords: tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <a href="https://www.datainaction.dev/" title="Data In Action" target="_blank">
     <img alt="Homepage" src="https://img.shields.io/website?down_color=%23FF4136&down_message=Down&label=Homepage&logo=home-assistant&logoColor=white&up_color=%232ECC40&up_message=Up&url=https%3A%2F%2Fmegabyte.space&style=for-the-badge" />
   </a>
-  <a href="https://github.com/reginaldosilva27/Databricks" title="Contributing" target="_blank">
+  <a href="https://github.com/reginaldosilva27/dtstools/blob/main/CONTRIBUTING.md" title="Contributing" target="_blank">
     <img alt="Contributing" src="https://img.shields.io/badge/Contributing-Guide-0074D9?logo=github-sponsors&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://join.slack.com/t/databricksbr/shared_invite/zt-1xe5tjy82-4O0fYQM8WnplLqrqIxQKqg" title="Slack" target="_blank">
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
-  <a href="https://github.com/reginaldosilva27/Databricks" title="GitHub" target="_blank">
+  <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.1" href="https://github.com/reginaldosilva27/Databricks" target="_blank">
-    <img alt="Version: 0.0.1" src="https://img.shields.io/badge/version-0.0.1-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.2" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.2" src="https://img.shields.io/badge/version-0.0.2-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
-    <a title="License: MIT" href="https://github.com/reginaldosilva27/Databricks" target="_blank">
+    <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
 </div>
 
@@ -131,14 +131,15 @@
 ```
 dtsTable.Help()
 ```
 <a href="#tablesize" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="how-to-use-tableSize"></a>
 ### How to use tableSize
+> Find out the true size of your table
 Call the tableSize function passing the database and table name, use display() to see the results.
 
 **This function returns a Dataframe.**
 
 ```
 dtsTable.tableSize(databaseName,tableName).display()
 ```
@@ -156,15 +157,15 @@
 ```
 for tb in spark.sql(f"show tables from bronze_renner_rma").collect():
     try:
         print(">> Collecting data... Table:",tb.tableName)
         dtsTable.tableSize(tb.database,tb.tableName) \
         .write.format('delta') \
         .mode('append') \
-        .saveAsTable("db_demo.tableSize",path='abfss://reginaldo@stdts360.dfs.core.windows.net/bronze/tableSize2')
+        .saveAsTable("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/bronze/tableSize')
     except Exception as e:
         print (f"###### Error to load tableName {tb.tableName} - {e}######")
 ```
 
 <a href="#tableMaintenance" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="how-to-use-tableMaintenance"></a>
@@ -179,15 +180,15 @@
 | optimize | True: OPTIMIZE will be executed, False: Skip OPTIMIZE | bool |
 | zorderColumns | If informed and optimize is equal to True, Zorder is applied to the list of columns separated by a comma (,) | string |
 | vacuumRetention | Number of hours to hold after vacuum runs | whole |
 | Debug | Just print the result on screen | bool |
 
 **Apply in a single table.**
 ```
-dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
+dtsTable.tableMaintenance(schemaName="Database", tableName="tableName", zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
 
 **Apply maintenance to all tables for YOUR database**
 ```
 for tb in spark.sql(f"show tables from db_demo").collect():
   dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
@@ -209,14 +210,14 @@
 > - Cost of Azure Storage Transactions: Read Operations (per 10,000) - $0.0258 (two cents per 10,000 operations) (Estimated price as of 4/21/2023)
 
 <a href="#references" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="references"></a>
 ## References
 
-<https://github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/delta/commands/VacuumCommand.scala>
+https://github.com/reginaldosilva27/dtstools
 <br>
 
 > ``Author: Reginaldo Silva``
   - [Blog Data In Action](https://datainaction.dev/)
-  - [Github](https://github.com/reginaldosilva27)
+  - [Github](https://github.com/reginaldosilva27/dtstools)
   - [Dataside](https://www.dataside.com.br/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.1 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.2 Summary: This package aims
 to provide features for working with Delta Lake. Author-email: Reginaldo Silva
 silva@dataside.com.br> License: MIT License Copyright (c) 2023 Reginaldo Silva
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -12,22 +12,22 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: DataInAction, https://
 www.datainaction.dev/blog Project-URL: Bug Tracker, https://github.com/
-reginaldosilva27/Databricks Project-URL: README, https://www.datainaction.dev/
+reginaldosilva27/dtstools Project-URL: README, https://www.datainaction.dev/
 blog Project-URL: Dataside, https://www.dataside.com.br Keywords:
 tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.1] [License:_MIT] [GitLab]
+                   [Version:_0.0.2] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
@@ -50,41 +50,41 @@
 Dataframet [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use dtstools
 **First install the package via PyPi** ``` pip install --upgrade -i https://
 test.pypi.org/simple/ dtstools ``` **Import the dtsTable module into your
 context** ``` from dtstools import dtsTable ``` **Use the function
 dtsTable.Help() to see examples of function usage and a summary of each
 function.** ``` dtsTable.Help() ``` [https://static.wixstatic.com/media/
-a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize Call
-the tableSize function passing the database and table name, use display() to
-see the results. **This function returns a Dataframe.** ``` dtsTable.tableSize
-(databaseName,tableName).display() ``` **Save the result in a Delta Table for
-monitoring and baseline** ``` dtsTable.tableSize(databaseName,tableName) \
-.write.format('delta') \ .mode('append') \ .saveAsTable
-("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/
-bronze/tableSize') ``` **Get the size of all tables in your database** ``` for
-tb in spark.sql(f"show tables from bronze_renner_rma").collect(): try: print
-(">> Collecting data... Table:",tb.tableName) dtsTable.tableSize
-(tb.database,tb.tableName) \ .write.format('delta') \ .mode('append') \
-.saveAsTable("db_demo.tableSize",path='abfss://
-reginaldo@stdts360.dfs.core.windows.net/bronze/tableSize2') except Exception as
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize >
+Find out the true size of your table Call the tableSize function passing the
+database and table name, use display() to see the results. **This function
+returns a Dataframe.** ``` dtsTable.tableSize(databaseName,tableName).display()
+``` **Save the result in a Delta Table for monitoring and baseline** ```
+dtsTable.tableSize(databaseName,tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') ``` **Get the size of
+all tables in your database** ``` for tb in spark.sql(f"show tables from
+bronze_renner_rma").collect(): try: print(">> Collecting data... Table:
+",tb.tableName) dtsTable.tableSize(tb.database,tb.tableName) \ .write.format
+('delta') \ .mode('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') except Exception as
 e: print (f"###### Error to load tableName {tb.tableName} - {e}######") ```
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use
 tableMaintenance Apply maintenance to a table, Optimize and Vacuum. | Parameter
 | Description | Type | ------------- | ------------- | ------------- | |
 schemaName | Name of the database where the table is created | string | |
 tableName | Name of the table that will be applied in the maintenance | string
 | | vacuum | True: Vacuum will run, False: Ignore vacuum | bool | | optimize |
 True: OPTIMIZE will be executed, False: Skip OPTIMIZE | bool | | zorderColumns
 | If informed and optimize is equal to True, Zorder is applied to the list of
 columns separated by a comma (,) | string | | vacuumRetention | Number of hours
 to hold after vacuum runs | whole | | Debug | Just print the result on screen |
 bool | **Apply in a single table.** ``` dtsTable.tableMaintenance
-(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
+(schemaName="Database", tableName="tableName", zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` **Apply
 maintenance to all tables for YOUR database** ``` for tb in spark.sql(f"show
 tables from db_demo").collect(): dtsTable.tableMaintenance
 (schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
 Future implementations > 1. Use Unity Catalog
@@ -95,13 +95,11 @@
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Notes > - For partitioned
 tables with many partitions, the execution time can take longer, so monitor the
 first executions well, the use is at your responsibility, despite not having
 any risk mapped so far, it can only generate more transactions for your storage
 > - Cost of Azure Storage Transactions: Read Operations (per 10,000) - $0.0258
 (two cents per 10,000 operations) (Estimated price as of 4/21/2023) [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
-References
-github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/
-delta/commands/VacuumCommand.scala>
+References https://github.com/reginaldosilva27/dtstools
 > ``Author: Reginaldo Silva`` - [Blog Data In Action](https://datainaction.dev/
-) - [Github](https://github.com/reginaldosilva27) - [Dataside](https://
-www.dataside.com.br/)
+) - [Github](https://github.com/reginaldosilva27/dtstools) - [Dataside](https:/
+/www.dataside.com.br/)
```

### Comparing `dtstools-0.0.1/README.md` & `dtstools-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <div align="center">
   <a href="https://www.datainaction.dev/" title="Data In Action" target="_blank">
     <img alt="Homepage" src="https://img.shields.io/website?down_color=%23FF4136&down_message=Down&label=Homepage&logo=home-assistant&logoColor=white&up_color=%232ECC40&up_message=Up&url=https%3A%2F%2Fmegabyte.space&style=for-the-badge" />
   </a>
-  <a href="https://github.com/reginaldosilva27/Databricks" title="Contributing" target="_blank">
+  <a href="https://github.com/reginaldosilva27/dtstools/blob/main/CONTRIBUTING.md" title="Contributing" target="_blank">
     <img alt="Contributing" src="https://img.shields.io/badge/Contributing-Guide-0074D9?logo=github-sponsors&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://join.slack.com/t/databricksbr/shared_invite/zt-1xe5tjy82-4O0fYQM8WnplLqrqIxQKqg" title="Slack" target="_blank">
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
-  <a href="https://github.com/reginaldosilva27/Databricks" title="GitHub" target="_blank">
+  <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.1" href="https://github.com/reginaldosilva27/Databricks" target="_blank">
-    <img alt="Version: 0.0.1" src="https://img.shields.io/badge/version-0.0.1-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.2" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.2" src="https://img.shields.io/badge/version-0.0.2-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
-    <a title="License: MIT" href="https://github.com/reginaldosilva27/Databricks" target="_blank">
+    <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
 </div>
 
@@ -92,14 +92,15 @@
 ```
 dtsTable.Help()
 ```
 <a href="#tablesize" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="how-to-use-tableSize"></a>
 ### How to use tableSize
+> Find out the true size of your table
 Call the tableSize function passing the database and table name, use display() to see the results.
 
 **This function returns a Dataframe.**
 
 ```
 dtsTable.tableSize(databaseName,tableName).display()
 ```
@@ -117,15 +118,15 @@
 ```
 for tb in spark.sql(f"show tables from bronze_renner_rma").collect():
     try:
         print(">> Collecting data... Table:",tb.tableName)
         dtsTable.tableSize(tb.database,tb.tableName) \
         .write.format('delta') \
         .mode('append') \
-        .saveAsTable("db_demo.tableSize",path='abfss://reginaldo@stdts360.dfs.core.windows.net/bronze/tableSize2')
+        .saveAsTable("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/bronze/tableSize')
     except Exception as e:
         print (f"###### Error to load tableName {tb.tableName} - {e}######")
 ```
 
 <a href="#tableMaintenance" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="how-to-use-tableMaintenance"></a>
@@ -140,15 +141,15 @@
 | optimize | True: OPTIMIZE will be executed, False: Skip OPTIMIZE | bool |
 | zorderColumns | If informed and optimize is equal to True, Zorder is applied to the list of columns separated by a comma (,) | string |
 | vacuumRetention | Number of hours to hold after vacuum runs | whole |
 | Debug | Just print the result on screen | bool |
 
 **Apply in a single table.**
 ```
-dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
+dtsTable.tableMaintenance(schemaName="Database", tableName="tableName", zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
 
 **Apply maintenance to all tables for YOUR database**
 ```
 for tb in spark.sql(f"show tables from db_demo").collect():
   dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
@@ -170,14 +171,14 @@
 > - Cost of Azure Storage Transactions: Read Operations (per 10,000) - $0.0258 (two cents per 10,000 operations) (Estimated price as of 4/21/2023)
 
 <a href="#references" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="references"></a>
 ## References
 
-<https://github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/delta/commands/VacuumCommand.scala>
+https://github.com/reginaldosilva27/dtstools
 <br>
 
 > ``Author: Reginaldo Silva``
   - [Blog Data In Action](https://datainaction.dev/)
-  - [Github](https://github.com/reginaldosilva27)
+  - [Github](https://github.com/reginaldosilva27/dtstools)
   - [Dataside](https://www.dataside.com.br/)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.1] [License:_MIT] [GitLab]
+                   [Version:_0.0.2] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
@@ -26,41 +26,41 @@
 Dataframet [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use dtstools
 **First install the package via PyPi** ``` pip install --upgrade -i https://
 test.pypi.org/simple/ dtstools ``` **Import the dtsTable module into your
 context** ``` from dtstools import dtsTable ``` **Use the function
 dtsTable.Help() to see examples of function usage and a summary of each
 function.** ``` dtsTable.Help() ``` [https://static.wixstatic.com/media/
-a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize Call
-the tableSize function passing the database and table name, use display() to
-see the results. **This function returns a Dataframe.** ``` dtsTable.tableSize
-(databaseName,tableName).display() ``` **Save the result in a Delta Table for
-monitoring and baseline** ``` dtsTable.tableSize(databaseName,tableName) \
-.write.format('delta') \ .mode('append') \ .saveAsTable
-("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/
-bronze/tableSize') ``` **Get the size of all tables in your database** ``` for
-tb in spark.sql(f"show tables from bronze_renner_rma").collect(): try: print
-(">> Collecting data... Table:",tb.tableName) dtsTable.tableSize
-(tb.database,tb.tableName) \ .write.format('delta') \ .mode('append') \
-.saveAsTable("db_demo.tableSize",path='abfss://
-reginaldo@stdts360.dfs.core.windows.net/bronze/tableSize2') except Exception as
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize >
+Find out the true size of your table Call the tableSize function passing the
+database and table name, use display() to see the results. **This function
+returns a Dataframe.** ``` dtsTable.tableSize(databaseName,tableName).display()
+``` **Save the result in a Delta Table for monitoring and baseline** ```
+dtsTable.tableSize(databaseName,tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') ``` **Get the size of
+all tables in your database** ``` for tb in spark.sql(f"show tables from
+bronze_renner_rma").collect(): try: print(">> Collecting data... Table:
+",tb.tableName) dtsTable.tableSize(tb.database,tb.tableName) \ .write.format
+('delta') \ .mode('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') except Exception as
 e: print (f"###### Error to load tableName {tb.tableName} - {e}######") ```
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use
 tableMaintenance Apply maintenance to a table, Optimize and Vacuum. | Parameter
 | Description | Type | ------------- | ------------- | ------------- | |
 schemaName | Name of the database where the table is created | string | |
 tableName | Name of the table that will be applied in the maintenance | string
 | | vacuum | True: Vacuum will run, False: Ignore vacuum | bool | | optimize |
 True: OPTIMIZE will be executed, False: Skip OPTIMIZE | bool | | zorderColumns
 | If informed and optimize is equal to True, Zorder is applied to the list of
 columns separated by a comma (,) | string | | vacuumRetention | Number of hours
 to hold after vacuum runs | whole | | Debug | Just print the result on screen |
 bool | **Apply in a single table.** ``` dtsTable.tableMaintenance
-(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
+(schemaName="Database", tableName="tableName", zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` **Apply
 maintenance to all tables for YOUR database** ``` for tb in spark.sql(f"show
 tables from db_demo").collect(): dtsTable.tableMaintenance
 (schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
 Future implementations > 1. Use Unity Catalog
@@ -71,13 +71,11 @@
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Notes > - For partitioned
 tables with many partitions, the execution time can take longer, so monitor the
 first executions well, the use is at your responsibility, despite not having
 any risk mapped so far, it can only generate more transactions for your storage
 > - Cost of Azure Storage Transactions: Read Operations (per 10,000) - $0.0258
 (two cents per 10,000 operations) (Estimated price as of 4/21/2023) [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
-References
-github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/
-delta/commands/VacuumCommand.scala>
+References https://github.com/reginaldosilva27/dtstools
 > ``Author: Reginaldo Silva`` - [Blog Data In Action](https://datainaction.dev/
-) - [Github](https://github.com/reginaldosilva27) - [Dataside](https://
-www.dataside.com.br/)
+) - [Github](https://github.com/reginaldosilva27/dtstools) - [Dataside](https:/
+/www.dataside.com.br/)
```

### Comparing `dtstools-0.0.1/src/dtstools/dtsTable.py` & `dtstools-0.0.2/src/dtstools/dtsTable.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,44 +126,49 @@
             spark.sql("set spark.databricks.delta.retentionDurationCheck.enabled = true")
             print(f">>> Successful cleaning {schemaName}.{tableName} <<< >>> {str(datetime.now())}")
         else:
             print(f"### VACUUM not run! ###")
 
 # Function to get help about
 def Help():
+    print("v0.0.2")
     print("""____  ______ __ ______  ___    ___  __    __  """)
     print('|| \\\\ | || |(( \| || | // \\\\  // \\\\ ||   (( \ ')
     print("""||  ))  ||   \\\\   ||  ((   ))((   ))||    \\\\  """)
     print("""||_//   ||  \_))  ||   \\\\_//  \\\\_// ||__|\_)) """)
     print("")
     print("------------------------------------------------------")
     print("Function tableSize(database, tableName)")
     print("------------------------------------------------------")
     print("This function return a Dataframe with result")
+    print("Find out the true size of your table")
     print("")
     print(">> Sample call:")
     print("dtsTable.tableSize('dbname','tbName').display()")
     print("")
     print(">> Save the result in a Delta Table for monitoring and baseline")
     print("dtsTable.tableSize(databaseName,tableName) \ ")
     print(" .write.format('delta') \ ")
     print(" .mode('append') \ ")
     print(" .saveAsTable('db_demo.tableSize',path='abfss://container@storage.dfs.core.windows.net/bronze/tableSize')")
     print("")
     print(">> Get the size of all tables in your database")
-    print("for tb in spark.sql(f'show tables from YourDatabase').collect():")
-    print("  print('>> Collecting data... Table:',tb.tableName)")
-    print("  dtsTable.tableSize(tb.database,tb.tableName) \ ")
-    print("  .write.format('delta') \ ")
-    print("  .mode('append') \ ")
-    print("  .saveAsTable('db_demo.tableSize',path='abfss://container@storage.dfs.core.windows.net/bronze/tableSize')")
+    print("for tb in spark.sql(f'show tables from db_demo').collect():")
+    print("try:")
+    print("    print('>> Collecting data... Table:',tb.tableName)")
+    print("    dtsTable.tableSize(tb.database,tb.tableName) \ ")
+    print("    .write.format('delta') \ ")
+    print("    .mode('append') \ ")
+    print("    .saveAsTable('db_demo.tableSize',path='abfss://container@storage.dfs.core.windows.net/bronze/tableSize') ")
+    print("except Exception as e:")
+    print("    print (f'###### Error to load tableName {tb.tableName} - {e}######') ') ")
     print("")
     print("------------------------------------------------------")
     print("Function tableMaintenance()")
     print("------------------------------------------------------")
     print("This function apply Optimize and Vacuum")
     print("")
     print(">> Sample call:")
     print("dtsTable.tableMaintenance(schemaName='silver', tableName='tableName', zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)")
     print("")
-    print("Reference: https://www.datainaction.dev/post/otimize-seu-delta-lake-e-reduza-custos-storage-databricks-e-computa%C3%A7%C3%A3o")
+    print("Reference: https://github.com/reginaldosilva27/dtstools")
```

### Comparing `dtstools-0.0.1/src/dtstools.egg-info/PKG-INFO` & `dtstools-0.0.2/src/dtstools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtstools
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package aims to provide features for working with Delta Lake.
 Author-email: Reginaldo Silva <reginaldo.silva@dataside.com.br>
 License: MIT License
         
         Copyright (c) 2023 Reginaldo Silva
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,44 +22,44 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: DataInAction, https://www.datainaction.dev/blog
-Project-URL: Bug Tracker, https://github.com/reginaldosilva27/Databricks
+Project-URL: Bug Tracker, https://github.com/reginaldosilva27/dtstools
 Project-URL: README, https://www.datainaction.dev/blog
 Project-URL: Dataside, https://www.dataside.com.br
 Keywords: tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <a href="https://www.datainaction.dev/" title="Data In Action" target="_blank">
     <img alt="Homepage" src="https://img.shields.io/website?down_color=%23FF4136&down_message=Down&label=Homepage&logo=home-assistant&logoColor=white&up_color=%232ECC40&up_message=Up&url=https%3A%2F%2Fmegabyte.space&style=for-the-badge" />
   </a>
-  <a href="https://github.com/reginaldosilva27/Databricks" title="Contributing" target="_blank">
+  <a href="https://github.com/reginaldosilva27/dtstools/blob/main/CONTRIBUTING.md" title="Contributing" target="_blank">
     <img alt="Contributing" src="https://img.shields.io/badge/Contributing-Guide-0074D9?logo=github-sponsors&logoColor=white&style=for-the-badge" />
   </a>
   <a href="https://join.slack.com/t/databricksbr/shared_invite/zt-1xe5tjy82-4O0fYQM8WnplLqrqIxQKqg" title="Slack" target="_blank">
     <img alt="Slack" src="https://img.shields.io/badge/Slack-Chat-e01e5a?logo=slack&logoColor=white&style=for-the-badge" />
   </a>
-  <a href="https://github.com/reginaldosilva27/Databricks" title="GitHub" target="_blank">
+  <a href="https://github.com/reginaldosilva27/dtstools" title="GitHub" target="_blank">
     <img alt="GitHub" src="https://img.shields.io/badge/Mirror-GitHub-333333?logo=github&style=for-the-badge" />
   </a>
 </div>
 <div align="center">
-  <a title="Version: 0.0.1" href="https://github.com/reginaldosilva27/Databricks" target="_blank">
-    <img alt="Version: 0.0.1" src="https://img.shields.io/badge/version-0.0.1-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
+  <a title="Version: 0.0.2" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
+    <img alt="Version: 0.0.2" src="https://img.shields.io/badge/version-0.0.2-blue.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAACNJREFUCNdjIACY//+BEp9hhM3hAzYQwoBIAqEDYQrCZLwAAGlFKxU1nF9cAAAAAElFTkSuQmCC&cacheSeconds=2592000&style=flat-square" />
   </a>
-    <a title="License: MIT" href="https://github.com/reginaldosilva27/Databricks" target="_blank">
+    <a title="License: MIT" href="https://github.com/reginaldosilva27/dtstools" target="_blank">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgAQMAAABJtOi3AAAABlBMVEUAAAD///+l2Z/dAAAAAXRSTlMAQObYZgAAAHpJREFUCNdjYOD/wMDAUP+PgYHxhzwDA/MB5gMM7AwMDxj4GBgKGGQYGCyAEEgbMDDwAAWAwmk8958xpIOI5zKH2RmOyhxmZjguAiKmgIgtQOIYmFgCIp4AlaQ9OczGkJYCJEAGgI0CGwo2HmwR2Eqw5SBnNIAdBHYaAJb6KLM15W/CAAAAAElFTkSuQmCC&style=flat-square" />
   </a>
     <a href="Spark" title="Platform" target="_blank">
     <img alt="GitLab" src="https://img.shields.io/badge/platform-spark-red" />
   </a>
 </div>
 
@@ -131,14 +131,15 @@
 ```
 dtsTable.Help()
 ```
 <a href="#tablesize" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="how-to-use-tableSize"></a>
 ### How to use tableSize
+> Find out the true size of your table
 Call the tableSize function passing the database and table name, use display() to see the results.
 
 **This function returns a Dataframe.**
 
 ```
 dtsTable.tableSize(databaseName,tableName).display()
 ```
@@ -156,15 +157,15 @@
 ```
 for tb in spark.sql(f"show tables from bronze_renner_rma").collect():
     try:
         print(">> Collecting data... Table:",tb.tableName)
         dtsTable.tableSize(tb.database,tb.tableName) \
         .write.format('delta') \
         .mode('append') \
-        .saveAsTable("db_demo.tableSize",path='abfss://reginaldo@stdts360.dfs.core.windows.net/bronze/tableSize2')
+        .saveAsTable("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/bronze/tableSize')
     except Exception as e:
         print (f"###### Error to load tableName {tb.tableName} - {e}######")
 ```
 
 <a href="#tableMaintenance" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="how-to-use-tableMaintenance"></a>
@@ -179,15 +180,15 @@
 | optimize | True: OPTIMIZE will be executed, False: Skip OPTIMIZE | bool |
 | zorderColumns | If informed and optimize is equal to True, Zorder is applied to the list of columns separated by a comma (,) | string |
 | vacuumRetention | Number of hours to hold after vacuum runs | whole |
 | Debug | Just print the result on screen | bool |
 
 **Apply in a single table.**
 ```
-dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
+dtsTable.tableMaintenance(schemaName="Database", tableName="tableName", zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
 
 **Apply maintenance to all tables for YOUR database**
 ```
 for tb in spark.sql(f"show tables from db_demo").collect():
   dtsTable.tableMaintenance(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none', vacuumRetention=168, vacuum=True, optimize=True, debug=False)
 ```
@@ -209,14 +210,14 @@
 > - Cost of Azure Storage Transactions: Read Operations (per 10,000) - $0.0258 (two cents per 10,000 operations) (Estimated price as of 4/21/2023)
 
 <a href="#references" style="width:100%"><img style="width:100%" src="https://static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png" /></a>
 
 <a id="references"></a>
 ## References
 
-<https://github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/delta/commands/VacuumCommand.scala>
+https://github.com/reginaldosilva27/dtstools
 <br>
 
 > ``Author: Reginaldo Silva``
   - [Blog Data In Action](https://datainaction.dev/)
-  - [Github](https://github.com/reginaldosilva27)
+  - [Github](https://github.com/reginaldosilva27/dtstools)
   - [Dataside](https://www.dataside.com.br/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dtstools Version: 0.0.1 Summary: This package aims
+Metadata-Version: 2.1 Name: dtstools Version: 0.0.2 Summary: This package aims
 to provide features for working with Delta Lake. Author-email: Reginaldo Silva
 silva@dataside.com.br> License: MIT License Copyright (c) 2023 Reginaldo Silva
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -12,22 +12,22 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: DataInAction, https://
 www.datainaction.dev/blog Project-URL: Bug Tracker, https://github.com/
-reginaldosilva27/Databricks Project-URL: README, https://www.datainaction.dev/
+reginaldosilva27/dtstools Project-URL: README, https://www.datainaction.dev/
 blog Project-URL: Dataside, https://www.dataside.com.br Keywords:
 tableSize,tableMaintenance,help,deltaLake,Spark,Databricks,Fabric Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                   [Homepage] [Contributing] [Slack] [GitHub]
-                   [Version:_0.0.1] [License:_MIT] [GitLab]
+                   [Version:_0.0.2] [License:_MIT] [GitLab]
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]
                      DTSTOOLS: Help with your Delta Lake
                    *** Library created by Data_In_Action ***
 ``` ##### ###### ##### ###### ### ### #### ##### ## ## ## ## ## ## ## ## ## ##
 ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##### ## ## ## ## ## ##
 ##### ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ## ##
@@ -50,41 +50,41 @@
 Dataframet [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use dtstools
 **First install the package via PyPi** ``` pip install --upgrade -i https://
 test.pypi.org/simple/ dtstools ``` **Import the dtsTable module into your
 context** ``` from dtstools import dtsTable ``` **Use the function
 dtsTable.Help() to see examples of function usage and a summary of each
 function.** ``` dtsTable.Help() ``` [https://static.wixstatic.com/media/
-a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize Call
-the tableSize function passing the database and table name, use display() to
-see the results. **This function returns a Dataframe.** ``` dtsTable.tableSize
-(databaseName,tableName).display() ``` **Save the result in a Delta Table for
-monitoring and baseline** ``` dtsTable.tableSize(databaseName,tableName) \
-.write.format('delta') \ .mode('append') \ .saveAsTable
-("db_demo.tableSize",path='abfss://container@storage.dfs.core.windows.net/
-bronze/tableSize') ``` **Get the size of all tables in your database** ``` for
-tb in spark.sql(f"show tables from bronze_renner_rma").collect(): try: print
-(">> Collecting data... Table:",tb.tableName) dtsTable.tableSize
-(tb.database,tb.tableName) \ .write.format('delta') \ .mode('append') \
-.saveAsTable("db_demo.tableSize",path='abfss://
-reginaldo@stdts360.dfs.core.windows.net/bronze/tableSize2') except Exception as
+a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use tableSize >
+Find out the true size of your table Call the tableSize function passing the
+database and table name, use display() to see the results. **This function
+returns a Dataframe.** ``` dtsTable.tableSize(databaseName,tableName).display()
+``` **Save the result in a Delta Table for monitoring and baseline** ```
+dtsTable.tableSize(databaseName,tableName) \ .write.format('delta') \ .mode
+('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') ``` **Get the size of
+all tables in your database** ``` for tb in spark.sql(f"show tables from
+bronze_renner_rma").collect(): try: print(">> Collecting data... Table:
+",tb.tableName) dtsTable.tableSize(tb.database,tb.tableName) \ .write.format
+('delta') \ .mode('append') \ .saveAsTable("db_demo.tableSize",path='abfss://
+container@storage.dfs.core.windows.net/bronze/tableSize') except Exception as
 e: print (f"###### Error to load tableName {tb.tableName} - {e}######") ```
 [https://static.wixstatic.com/media/
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ### How to use
 tableMaintenance Apply maintenance to a table, Optimize and Vacuum. | Parameter
 | Description | Type | ------------- | ------------- | ------------- | |
 schemaName | Name of the database where the table is created | string | |
 tableName | Name of the table that will be applied in the maintenance | string
 | | vacuum | True: Vacuum will run, False: Ignore vacuum | bool | | optimize |
 True: OPTIMIZE will be executed, False: Skip OPTIMIZE | bool | | zorderColumns
 | If informed and optimize is equal to True, Zorder is applied to the list of
 columns separated by a comma (,) | string | | vacuumRetention | Number of hours
 to hold after vacuum runs | whole | | Debug | Just print the result on screen |
 bool | **Apply in a single table.** ``` dtsTable.tableMaintenance
-(schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
+(schemaName="Database", tableName="tableName", zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` **Apply
 maintenance to all tables for YOUR database** ``` for tb in spark.sql(f"show
 tables from db_demo").collect(): dtsTable.tableMaintenance
 (schemaName=tb.database, tableName=tb.tableName, zorderColumns='none',
 vacuumRetention=168, vacuum=True, optimize=True, debug=False) ``` [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
 Future implementations > 1. Use Unity Catalog
@@ -95,13 +95,11 @@
 a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ## Notes > - For partitioned
 tables with many partitions, the execution time can take longer, so monitor the
 first executions well, the use is at your responsibility, despite not having
 any risk mapped so far, it can only generate more transactions for your storage
 > - Cost of Azure Storage Transactions: Read Operations (per 10,000) - $0.0258
 (two cents per 10,000 operations) (Estimated price as of 4/21/2023) [https://
 static.wixstatic.com/media/a794bc_b10266580b524f6586d3b2d835cfb036~mv2.png]  ##
-References
-github.com/delta-io/delta/blob/master/core/src/main/scala/org/apache/spark/sql/
-delta/commands/VacuumCommand.scala>
+References https://github.com/reginaldosilva27/dtstools
 > ``Author: Reginaldo Silva`` - [Blog Data In Action](https://datainaction.dev/
-) - [Github](https://github.com/reginaldosilva27) - [Dataside](https://
-www.dataside.com.br/)
+) - [Github](https://github.com/reginaldosilva27/dtstools) - [Dataside](https:/
+/www.dataside.com.br/)
```

