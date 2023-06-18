# Comparing `tmp/mycotools-0.9b8.tar.gz` & `tmp/mycotools-0.9b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mycotools-0.9b8.tar", last modified: Tue Oct 26 19:17:59 2021, max compression
+gzip compressed data, was "dist/mycotools-0.9b9.tar", last modified: Tue Oct 26 19:41:37 2021, max compression
```

## Comparing `mycotools-0.9b8.tar` & `mycotools-0.9b9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:17:59.053000 mycotools-0.9b8/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     2507 2021-10-26 19:17:59.050985 mycotools-0.9b8/PKG-INFO
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1827 2021-08-18 17:08:15.000000 mycotools-0.9b8/README.md
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:17:58.802018 mycotools-0.9b8/mycotools/
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:17:58.953981 mycotools-0.9b8/mycotools/mycotools/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        0 2021-04-08 17:43:14.000000 mycotools-0.9b8/mycotools/mycotools/__init__.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     2800 2021-08-31 22:38:02.000000 mycotools-0.9b8/mycotools/mycotools/abstractHmm.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     5685 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/acc2fa.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     4844 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/acc2gff.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    10375 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/aggClus.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     4788 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/annotationStats.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     6852 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/assemblyStats.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23082 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/curAnnotation.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    14023 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/db2blast.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13319 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/db2hmmsearch.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3294 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/dbFiles.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     5755 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/extractDB.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     6905 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/fa2hmmer2fa.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     8631 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/fa2tree.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3938 2021-08-31 22:38:03.000000 mycotools-0.9b8/mycotools/mycotools/gff2protein.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    25930 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/jgiDwnld.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:17:59.007983 mycotools-0.9b8/mycotools/mycotools/lib/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        0 2021-04-08 17:43:08.000000 mycotools-0.9b8/mycotools/mycotools/lib/__init__.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    19838 2021-10-26 19:17:56.000000 mycotools-0.9b8/mycotools/mycotools/lib/dbtools.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    10534 2021-10-20 17:10:28.000000 mycotools-0.9b8/mycotools/mycotools/lib/fastatools.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    20501 2021-10-26 19:17:56.000000 mycotools-0.9b8/mycotools/mycotools/lib/kontools.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3866 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/mycodb
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    22418 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/ncbiDwnld.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     2920 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/ome2name.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17406 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/predb2db.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1752 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/proteomeStats.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:17:59.033975 mycotools-0.9b8/mycotools/mycotools/utils/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        0 2021-02-21 17:14:58.000000 mycotools-0.9b8/mycotools/mycotools/utils/__init__.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     5683 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/utils/curGFF3.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1726 2021-10-26 19:17:56.000000 mycotools-0.9b8/mycotools/mycotools/utils/curProteomes.py
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     5643 2021-10-26 19:17:55.000000 mycotools-0.9b8/mycotools/mycotools/utils/gff2gff3.py
--rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3026 2021-10-26 19:17:56.000000 mycotools-0.9b8/mycotools/mycotools/utils/queryDB.py
-drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:17:58.977981 mycotools-0.9b8/mycotools/mycotools.egg-info/
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     2507 2021-10-26 19:17:57.000000 mycotools-0.9b8/mycotools/mycotools.egg-info/PKG-INFO
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1267 2021-10-26 19:17:58.000000 mycotools-0.9b8/mycotools/mycotools.egg-info/SOURCES.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2021-10-26 19:17:57.000000 mycotools-0.9b8/mycotools/mycotools.egg-info/dependency_links.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       26 2021-10-26 19:17:57.000000 mycotools-0.9b8/mycotools/mycotools.egg-info/requires.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       10 2021-10-26 19:17:57.000000 mycotools-0.9b8/mycotools/mycotools.egg-info/top_level.txt
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2021-10-26 19:17:59.053996 mycotools-0.9b8/setup.cfg
--rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1602 2021-10-26 19:17:56.000000 mycotools-0.9b8/setup.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:41:37.848868 mycotools-0.9b9/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     2507 2021-10-26 19:41:37.846865 mycotools-0.9b9/PKG-INFO
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1827 2021-08-18 17:08:15.000000 mycotools-0.9b9/README.md
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:41:37.615861 mycotools-0.9b9/mycotools/
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:41:37.761866 mycotools-0.9b9/mycotools/mycotools/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        0 2021-04-08 17:43:14.000000 mycotools-0.9b9/mycotools/mycotools/__init__.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     2800 2021-08-31 22:38:02.000000 mycotools-0.9b9/mycotools/mycotools/abstractHmm.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     5685 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/acc2fa.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     4844 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/acc2gff.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    10375 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/aggClus.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     4805 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/annotationStats.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     6755 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/assemblyStats.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    23082 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/curAnnotation.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    14023 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/db2blast.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    13319 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/db2hmmsearch.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3294 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/dbFiles.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     5755 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/extractDB.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     6905 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/fa2hmmer2fa.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     8631 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/fa2tree.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3938 2021-08-31 22:38:03.000000 mycotools-0.9b9/mycotools/mycotools/gff2protein.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    25930 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/jgiDwnld.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:41:37.799867 mycotools-0.9b9/mycotools/mycotools/lib/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        0 2021-04-08 17:43:08.000000 mycotools-0.9b9/mycotools/mycotools/lib/__init__.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    19838 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/lib/dbtools.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    10534 2021-10-20 17:10:28.000000 mycotools-0.9b9/mycotools/mycotools/lib/fastatools.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)    20569 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/lib/kontools.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3866 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/mycodb
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    22418 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/ncbiDwnld.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     2920 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/ome2name.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)    17406 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/predb2db.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     1752 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/proteomeStats.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:41:37.831861 mycotools-0.9b9/mycotools/mycotools/utils/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        0 2021-02-21 17:14:58.000000 mycotools-0.9b9/mycotools/mycotools/utils/__init__.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     5683 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/utils/curGFF3.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1726 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/utils/curProteomes.py
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     5643 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/utils/gff2gff3.py
+-rwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)     3026 2021-10-26 19:41:36.000000 mycotools-0.9b9/mycotools/mycotools/utils/queryDB.py
+drwxr-xr-x   0 osu10393 (24680) PAS1046   (4372)        0 2021-10-26 19:41:37.782867 mycotools-0.9b9/mycotools/mycotools.egg-info/
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     2507 2021-10-26 19:41:37.000000 mycotools-0.9b9/mycotools/mycotools.egg-info/PKG-INFO
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1267 2021-10-26 19:41:37.000000 mycotools-0.9b9/mycotools/mycotools.egg-info/SOURCES.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)        1 2021-10-26 19:41:37.000000 mycotools-0.9b9/mycotools/mycotools.egg-info/dependency_links.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       26 2021-10-26 19:41:37.000000 mycotools-0.9b9/mycotools/mycotools.egg-info/requires.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       10 2021-10-26 19:41:37.000000 mycotools-0.9b9/mycotools/mycotools.egg-info/top_level.txt
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)       38 2021-10-26 19:41:37.849863 mycotools-0.9b9/setup.cfg
+-rw-r--r--   0 osu10393 (24680) PAS1046   (4372)     1602 2021-10-26 19:41:36.000000 mycotools-0.9b9/setup.py
```

### Comparing `mycotools-0.9b8/PKG-INFO` & `mycotools-0.9b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycotools
-Version: 0.9b8
+Version: 0.9b9
 Summary: A compilation of bioinformatic and computation biology inspired python tools
 Home-page: https://gitlab.com/xonq/mycotools/mycotools
 Author: xonq
 Author-email: konkelzach@protonmail.com
 License: UNKNOWN
 Description: ![mycotools](https://gitlab.com/xonq/mycotools/-/raw/master/mycotools.png)
```

### Comparing `mycotools-0.9b8/README.md` & `mycotools-0.9b9/README.md`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/abstractHmm.py` & `mycotools-0.9b9/mycotools/mycotools/abstractHmm.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/acc2fa.py` & `mycotools-0.9b9/mycotools/mycotools/acc2fa.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/acc2gff.py` & `mycotools-0.9b9/mycotools/mycotools/acc2gff.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/aggClus.py` & `mycotools-0.9b9/mycotools/mycotools/aggClus.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/annotationStats.py` & `mycotools-0.9b9/mycotools/mycotools/annotationStats.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,17 @@
             res = pool.starmap(compileExon, cmds)
         out = {x[0]: x[1] for x in res if x}
         if len(sys.argv) < 3:
             output_file = os.path.basename(formatPath(sys.argv[1])) + '.annStats.tsv'
         else:
             output_file = sys.argv[2]
         with open(output_file, 'w') as write:
-            write.write('#gene2gene_length\ttgenes\tmean_length\tmedian_length\n')
+            write.write('#ome\tgene2gene_length\tgenes\tmean_length\tmedian_length\n')
             for ome in out:
-                write.write('\t'.join([str(x) for x in out[ome].values()]) + '\n')
+                write.write(ome + '\t' + '\t'.join([str(x) for x in out[ome].values()]) + '\n')
     else:
         ome, geneStats = compileExon( formatPath(sys.argv[1]), output )
         if output:
             out_str = 'total_len\tgenes\tmean_len\tmedian_len\n' + str(geneStats['total_len']) + \
                 '\t' + str(geneStats['genes']) + '\t' \
                 + str(geneStats['mean_len']) + '\t' + str(geneStats['median_len'])
```

### Comparing `mycotools-0.9b8/mycotools/mycotools/assemblyStats.py` & `mycotools-0.9b9/mycotools/mycotools/assemblyStats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #! /usr/bin/env python3
 '''
 Takes a database as argument 1 and an output for the .tsv as argument 2.
 Calculates basic genome statistics.
 '''
 
-import sys, os, pandas as pd
+import sys, os, pandas as pd, multiprocessing as mp
 from mycotools.lib.dbtools import db2df, log_editor
 from mycotools.lib.biotools import fa2dict
+from mycotools.lib.kontools import formatPath, eprint
 
 
 def calcMask( contig_list ):
 
     seq = ''.join([x['sequence'] for x in contig_list])
     mask = seq.count('a')
     mask += seq.count('t')
@@ -95,14 +96,18 @@
         
     except KeyError:
         out = False
 
 
     return out
 
+def mngr(assembly_path, ome = None):
+    sortedContigs = sortContigs(assembly_path)
+    calcs = n50l50(sortedContigs)
+    return ome, calcs
 
 def main():
 
     usage = '\nUSAGE: assembly statistics\tAssembly `fasta` or mycotoolsDB, optional output file if using database\n'
     if len(sys.argv) < 2:
         print( usage , flush = True)
         sys.exit( 1 )
@@ -111,46 +116,39 @@
 
     if formatPath(sys.argv[1])[-4:] not in {'gff3', '.gtf', '.gff'}:
         if len( sys.argv ) < 3:
             log_path = formatPath(sys.argv[1]) + '.assStats.tsv'
         else:
             log_path = sys.argv[2]
         db = db2df( sys.argv[1] )
-        ome_set = set()
 
         if not os.path.isfile( log_path ):
             head = '#ome\tn50-1000bp\tl50-1000bp\tl50%-1000bp\tn50\tl50\tl50%\tlargest_contig\tshortest_contig\tcontigs' + \
                 '\tcontigs-1000bp\tassembly_len\tassembly_len-1000bp\tgc\tgc-1000bp\tmask%\tmask%-1000bp'
             with open( log_path, 'w' ) as log_open:
                 log_open.write( head )
-        else:
-            with open( log_path, 'r' ) as log_read:
-                for line in log_read:
-                    if line.startswith('#'):
-                        continue
-                    data = line.split( '\t' )
-                    ome_set.add( data[0] )
-                    
 
+        cmds = []
         for i, row in db.iterrows():
-            if row['internal_ome'] in ome_set:
-                continue
             print('\t' + row['internal_ome'], flush = True)
             if not pd.isnull(row['assembly']):
-                sortedContigs = sortContigs( os.environ['MYCOFNA'] + '/' + row['assembly'] )
-                calcs = n50l50( sortedContigs )
-                if calcs:
-                    log_editor( log_path, row['internal_ome'], row['internal_ome'] + '\t' + str(calcs['n50-1000bp']) + '\t' + \
-                        str(calcs['l50-1000bp']) + '\t' + str(calcs['l50%-1000bp']) + '\t' + str(calcs['n50']) + '\t' + \
-                        str(calcs['l50']) + '\t' + str(calcs['l50%']) + '\t' + str(calcs['largest_contig']) + '\t' + \
-                        str(calcs['shortest_contig']) + '\t' + str(calcs['contigs']) + '\t' + str(calcs['contigs-1000bp']) + \
-                        '\t' + str(calcs['assembly_len']) + '\t' + str(calcs['assembly_len-1000bp']) + '\t' + str(calcs['gc']) + \
-                        '\t' + str(calcs['gc-1000bp'])) + '\t' + str(calcs['mask%']) + '\t' + str(calcs['mask%-1000bp'])
-                else:
-                    eprint('\t\tERROR:\t' + row['internal_ome'], flush = True)
+                cmds.append((formatPath('$MYCOFNA/' + row['assembly']), row['internal_ome']))
+        with mp.Pool(processes=os.cpu_count()) as pool:
+            results = pool.starmap(mngr, cmds)
+        for res in results:
+            ome, calcs = res[0], res[1]
+            if calcs:
+                log_editor( log_path, ome, ome + '\t' + str(calcs['n50-1000bp']) + '\t' + \
+                    str(calcs['l50-1000bp']) + '\t' + str(calcs['l50%-1000bp']) + '\t' + str(calcs['n50']) + '\t' + \
+                    str(calcs['l50']) + '\t' + str(calcs['l50%']) + '\t' + str(calcs['largest_contig']) + '\t' + \
+                    str(calcs['shortest_contig']) + '\t' + str(calcs['contigs']) + '\t' + str(calcs['contigs-1000bp']) + \
+                    '\t' + str(calcs['assembly_len']) + '\t' + str(calcs['assembly_len-1000bp']) + '\t' + str(calcs['gc']) + \
+                    '\t' + str(calcs['gc-1000bp'])) + '\t' + str(calcs['mask%']) + '\t' + str(calcs['mask%-1000bp'])
+            else:
+                eprint('\t\tERROR:\t' + row['internal_ome'], flush = True)
 
     else:
 
         sortedContigs = sortContigs( sys.argv[1] )
         calculations = n50l50( sortedContigs )
         if calculations:
             stats[ os.path.basename( os.path.abspath( sys.argv[1] )) ] = n50l50( sortedContigs )
```

### Comparing `mycotools-0.9b8/mycotools/mycotools/curAnnotation.py` & `mycotools-0.9b9/mycotools/mycotools/curAnnotation.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/db2blast.py` & `mycotools-0.9b9/mycotools/mycotools/db2blast.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/db2hmmsearch.py` & `mycotools-0.9b9/mycotools/mycotools/db2hmmsearch.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/dbFiles.py` & `mycotools-0.9b9/mycotools/mycotools/dbFiles.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/extractDB.py` & `mycotools-0.9b9/mycotools/mycotools/extractDB.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/fa2hmmer2fa.py` & `mycotools-0.9b9/mycotools/mycotools/fa2hmmer2fa.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/fa2tree.py` & `mycotools-0.9b9/mycotools/mycotools/fa2tree.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/gff2protein.py` & `mycotools-0.9b9/mycotools/mycotools/gff2protein.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/jgiDwnld.py` & `mycotools-0.9b9/mycotools/mycotools/jgiDwnld.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/lib/dbtools.py` & `mycotools-0.9b9/mycotools/mycotools/lib/dbtools.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/lib/fastatools.py` & `mycotools-0.9b9/mycotools/mycotools/lib/fastatools.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/lib/kontools.py` & `mycotools-0.9b9/mycotools/mycotools/lib/kontools.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         os.remove(dir_)
 
 def checkdir(dir_, unzip = False, to = None, rm = False):
     if os.path.isdir(dir_):
         return True
     elif os.path.isfile(formatPath(dir_) + '.tar.gz'):
         if unzip:
+            if dir_.endswith('/'):
+                dir_ = dir_[:-1]
             untardir(dir_ + '.tar.gz', rm = rm, to = to)
             return True
     return False
 
 
 def eprint( *args, **kwargs ):
     '''Prints to stderr'''
```

### Comparing `mycotools-0.9b8/mycotools/mycotools/mycodb` & `mycotools-0.9b9/mycotools/mycotools/mycodb`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/ncbiDwnld.py` & `mycotools-0.9b9/mycotools/mycotools/ncbiDwnld.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/ome2name.py` & `mycotools-0.9b9/mycotools/mycotools/ome2name.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/predb2db.py` & `mycotools-0.9b9/mycotools/mycotools/predb2db.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/proteomeStats.py` & `mycotools-0.9b9/mycotools/mycotools/proteomeStats.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/utils/curGFF3.py` & `mycotools-0.9b9/mycotools/mycotools/utils/curGFF3.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/utils/curProteomes.py` & `mycotools-0.9b9/mycotools/mycotools/utils/curProteomes.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/utils/gff2gff3.py` & `mycotools-0.9b9/mycotools/mycotools/utils/gff2gff3.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools/utils/queryDB.py` & `mycotools-0.9b9/mycotools/mycotools/utils/queryDB.py`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/mycotools/mycotools.egg-info/PKG-INFO` & `mycotools-0.9b9/mycotools/mycotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycotools
-Version: 0.9b8
+Version: 0.9b9
 Summary: A compilation of bioinformatic and computation biology inspired python tools
 Home-page: https://gitlab.com/xonq/mycotools/mycotools
 Author: xonq
 Author-email: konkelzach@protonmail.com
 License: UNKNOWN
 Description: ![mycotools](https://gitlab.com/xonq/mycotools/-/raw/master/mycotools.png)
```

### Comparing `mycotools-0.9b8/mycotools/mycotools.egg-info/SOURCES.txt` & `mycotools-0.9b9/mycotools/mycotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mycotools-0.9b8/setup.py` & `mycotools-0.9b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open( "README.md", "r" ) as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "mycotools",
-    version = "0.9b8",
+    version = "0.9b9",
     author = "xonq",
     author_email = "konkelzach@protonmail.com",
     description = "A compilation of bioinformatic and computation biology inspired " + \
         "python tools",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://gitlab.com/xonq/mycotools/mycotools",
```

