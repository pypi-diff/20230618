# Comparing `tmp/euroleague_api-0.0.1.tar.gz` & `tmp/euroleague_api-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "euroleague_api-0.0.1.tar", last modified: Sat Jun 17 15:00:58 2023, max compression
+gzip compressed data, was "euroleague_api-0.0.2a0.tar", last modified: Sun Jun 18 19:26:30 2023, max compression
```

## Comparing `euroleague_api-0.0.1.tar` & `euroleague_api-0.0.2a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:00:58.248268 euroleague_api-0.0.1/
--rw-rw-rw-   0        0        0     1097 2023-06-13 23:32:02.000000 euroleague_api-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1500 2023-06-17 15:00:58.248268 euroleague_api-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2023-06-13 23:45:48.000000 euroleague_api-0.0.1/README.md
--rw-rw-rw-   0        0        0       88 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      717 2023-06-17 15:00:58.250714 euroleague_api-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-17 15:00:58.198673 euroleague_api-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-17 15:00:58.221925 euroleague_api-0.0.1/src/euroleague_api/
--rw-rw-rw-   0        0        0      277 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/__init__.py
--rw-rw-rw-   0        0        0     4413 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/game_stats.py
--rw-rw-rw-   0        0        0    10352 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/player_stats.py
--rw-rw-rw-   0        0        0     2466 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/shot_data.py
--rw-rw-rw-   0        0        0     1323 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/standings.py
--rw-rw-rw-   0        0        0     3804 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/team_stats.py
--rw-rw-rw-   0        0        0    17871 2023-06-13 23:33:55.000000 euroleague_api-0.0.1/src/euroleague_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:00:58.248268 euroleague_api-0.0.1/src/euroleague_api.egg-info/
--rw-rw-rw-   0        0        0     1500 2023-06-17 15:00:58.000000 euroleague_api-0.0.1/src/euroleague_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-06-17 15:00:58.000000 euroleague_api-0.0.1/src/euroleague_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:00:58.000000 euroleague_api-0.0.1/src/euroleague_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-17 15:00:58.000000 euroleague_api-0.0.1/src/euroleague_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-17 15:00:58.000000 euroleague_api-0.0.1/src/euroleague_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 19:26:30.204076 euroleague_api-0.0.2a0/
+-rw-rw-rw-   0        0        0     1097 2023-06-13 23:32:02.000000 euroleague_api-0.0.2a0/LICENSE
+-rw-rw-rw-   0        0        0     2038 2023-06-18 19:26:30.204076 euroleague_api-0.0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1577 2023-06-18 19:16:51.000000 euroleague_api-0.0.2a0/README.md
+-rw-rw-rw-   0        0        0       88 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0      723 2023-06-18 19:26:30.204076 euroleague_api-0.0.2a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 19:26:30.161143 euroleague_api-0.0.2a0/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 19:26:30.179083 euroleague_api-0.0.2a0/src/euroleague_api/
+-rw-rw-rw-   0        0        0      277 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/__init__.py
+-rw-rw-rw-   0        0        0     4413 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/game_stats.py
+-rw-rw-rw-   0        0        0    10352 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/player_stats.py
+-rw-rw-rw-   0        0        0     2466 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/shot_data.py
+-rw-rw-rw-   0        0        0     1323 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/standings.py
+-rw-rw-rw-   0        0        0     3804 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/team_stats.py
+-rw-rw-rw-   0        0        0    17871 2023-06-13 23:33:55.000000 euroleague_api-0.0.2a0/src/euroleague_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:26:30.204076 euroleague_api-0.0.2a0/src/euroleague_api.egg-info/
+-rw-rw-rw-   0        0        0     2038 2023-06-18 19:26:30.000000 euroleague_api-0.0.2a0/src/euroleague_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-06-18 19:26:30.000000 euroleague_api-0.0.2a0/src/euroleague_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 19:26:30.000000 euroleague_api-0.0.2a0/src/euroleague_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-18 19:26:30.000000 euroleague_api-0.0.2a0/src/euroleague_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 19:26:30.000000 euroleague_api-0.0.2a0/src/euroleague_api.egg-info/top_level.txt
```

### Comparing `euroleague_api-0.0.1/LICENSE` & `euroleague_api-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.1/setup.cfg` & `euroleague_api-0.0.2a0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7572 6f6c 6561 6775 655f 6170   = euroleague_ap
 00000020: 690d 0a76 6572 7369 6f6e 203d 2030 2e30  i..version = 0.0
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2047 656f  .1..author = Geo
-00000040: 7267 696f 7320 4769 6173 656d 6964 6973  rgios Giasemidis
-00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000060: 2067 2e67 6961 7365 6d69 6469 7340 676d   g.giasemidis@gm
-00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
-00000080: 7469 6f6e 203d 2041 2050 7974 686f 6e20  tion = A Python 
-00000090: 7772 6170 7065 7220 6f66 2074 6865 2045  wrapper of the E
-000000a0: 7572 6f6c 6561 6775 6520 4150 490d 0a64  uroleague API..d
-000000b0: 6573 6372 6970 7469 6f6e 2d66 696c 6520  escription-file 
-000000c0: 3d20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  = README.md..lon
-000000d0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-000000e0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-000000f0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000100: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000110: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000120: 6b65 7977 6f72 6473 203d 2065 7572 6f6c  keywords = eurol
-00000130: 6561 6775 652c 2061 7069 2c20 6261 736b  eague, api, bask
-00000140: 6574 6261 6c6c 0d0a 7572 6c20 3d20 6874  etball..url = ht
-00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000160: 2f67 6961 7365 6d69 6469 732f 6575 726f  /giasemidis/euro
-00000170: 6c65 6167 7565 5f61 7069 0d0a 646f 776e  league_api..down
-00000180: 6c6f 6164 5f75 726c 203d 2068 7474 7073  load_url = https
-00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 6769  ://github.com/gi
-000001a0: 6173 656d 6964 6973 2f65 7572 6f6c 6561  asemidis/eurolea
-000001b0: 6775 655f 6170 692f 6172 6368 6976 652f  gue_api/archive/
-000001c0: 7265 6673 2f74 6167 732f 7630 2e30 2e31  refs/tags/v0.0.1
-000001d0: 2d61 6c70 6861 2e74 6172 2e67 7a0d 0a0d  -alpha.tar.gz...
-000001e0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-000001f0: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000200: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000210: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000220: 7569 7265 7320 3d20 3e3d 332e 360d 0a69  uires = >=3.6..i
-00000230: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000240: 3d20 0d0a 0972 6571 7565 7374 730d 0a09  = ...requests...
-00000250: 7061 6e64 6173 0d0a 096e 756d 7079 0d0a  pandas...numpy..
-00000260: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000270: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000280: 203d 2073 7263 0d0a 6578 636c 7564 6520   = src..exclude 
-00000290: 3d20 0d0a 096e 6f74 6562 6f6f 6b73 2a0d  = ...notebooks*.
-000002a0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000002b0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000002c0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000030: 2e32 2d61 6c70 6861 0d0a 6175 7468 6f72  .2-alpha..author
+00000040: 203d 2047 656f 7267 696f 7320 4769 6173   = Georgios Gias
+00000050: 656d 6964 6973 0d0a 6175 7468 6f72 5f65  emidis..author_e
+00000060: 6d61 696c 203d 2067 2e67 6961 7365 6d69  mail = g.giasemi
+00000070: 6469 7340 676d 6169 6c2e 636f 6d0d 0a64  dis@gmail.com..d
+00000080: 6573 6372 6970 7469 6f6e 203d 2041 2050  escription = A P
+00000090: 7974 686f 6e20 7772 6170 7065 7220 6f66  ython wrapper of
+000000a0: 2074 6865 2045 7572 6f6c 6561 6775 6520   the Euroleague 
+000000b0: 4150 490d 0a64 6573 6372 6970 7469 6f6e  API..description
+000000c0: 2d66 696c 6520 3d20 5245 4144 4d45 2e6d  -file = README.m
+000000d0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000e0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000f0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000100: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000110: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000120: 646f 776e 0d0a 6b65 7977 6f72 6473 203d  down..keywords =
+00000130: 2065 7572 6f6c 6561 6775 652c 2061 7069   euroleague, api
+00000140: 2c20 6261 736b 6574 6261 6c6c 0d0a 7572  , basketball..ur
+00000150: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+00000160: 7562 2e63 6f6d 2f67 6961 7365 6d69 6469  ub.com/giasemidi
+00000170: 732f 6575 726f 6c65 6167 7565 5f61 7069  s/euroleague_api
+00000180: 0d0a 646f 776e 6c6f 6164 5f75 726c 203d  ..download_url =
+00000190: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000001a0: 636f 6d2f 6769 6173 656d 6964 6973 2f65  com/giasemidis/e
+000001b0: 7572 6f6c 6561 6775 655f 6170 692f 6172  uroleague_api/ar
+000001c0: 6368 6976 652f 7265 6673 2f74 6167 732f  chive/refs/tags/
+000001d0: 7630 2e30 2e32 2d61 6c70 6861 2e74 6172  v0.0.2-alpha.tar
+000001e0: 2e67 7a0d 0a0d 0a5b 6f70 7469 6f6e 735d  .gz....[options]
+000001f0: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000200: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+00000210: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+00000220: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000230: 332e 360d 0a69 6e73 7461 6c6c 5f72 6571  3.6..install_req
+00000240: 7569 7265 7320 3d20 0d0a 0972 6571 7565  uires = ...reque
+00000250: 7374 730d 0a09 7061 6e64 6173 0d0a 096e  sts...pandas...n
+00000260: 756d 7079 0d0a 0d0a 5b6f 7074 696f 6e73  umpy....[options
+00000270: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000280: 0a77 6865 7265 203d 2073 7263 0d0a 6578  .where = src..ex
+00000290: 636c 7564 6520 3d20 0d0a 096e 6f74 6562  clude = ...noteb
+000002a0: 6f6f 6b73 2a0d 0a0d 0a5b 6567 675f 696e  ooks*....[egg_in
+000002b0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000002c0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000002d0: 0a0d 0a                                  ...
```

### Comparing `euroleague_api-0.0.1/src/euroleague_api/game_stats.py` & `euroleague_api-0.0.2a0/src/euroleague_api/game_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.1/src/euroleague_api/player_stats.py` & `euroleague_api-0.0.2a0/src/euroleague_api/player_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.1/src/euroleague_api/shot_data.py` & `euroleague_api-0.0.2a0/src/euroleague_api/shot_data.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.1/src/euroleague_api/standings.py` & `euroleague_api-0.0.2a0/src/euroleague_api/standings.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.1/src/euroleague_api/team_stats.py` & `euroleague_api-0.0.2a0/src/euroleague_api/team_stats.py`

 * *Files identical despite different names*

### Comparing `euroleague_api-0.0.1/src/euroleague_api/utils.py` & `euroleague_api-0.0.2a0/src/euroleague_api/utils.py`

 * *Files identical despite different names*

