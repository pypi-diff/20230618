# Comparing `tmp/adbtool-0.0.8.tar.gz` & `tmp/adbtool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbtool-0.0.8.tar", last modified: Tue Aug 24 03:38:25 2021, max compression
+gzip compressed data, was "adbtool-0.0.9.tar", last modified: Sun Dec 19 12:09:00 2021, max compression
```

## Comparing `adbtool-0.0.8.tar` & `adbtool-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 03:38:25.115054 adbtool-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-08-24 03:38:16.000000 adbtool-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-24 03:38:16.000000 adbtool-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5279 2021-08-24 03:38:25.115054 adbtool-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2021-08-24 03:38:16.000000 adbtool-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 03:38:25.115054 adbtool-0.0.8/adbtool/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/adbtool.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/config.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 03:38:25.115054 adbtool-0.0.8/adbtool/subcommands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3941 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/adbdevice.py
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/adbpush.py
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/apkinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/apkinstall.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/apksigner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/apkuninstall.py
--rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/subcommands/assetbundleinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-08-24 03:38:16.000000 adbtool-0.0.8/adbtool/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 03:38:25.115054 adbtool-0.0.8/adbtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5279 2021-08-24 03:38:24.000000 adbtool-0.0.8/adbtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-08-24 03:38:25.000000 adbtool-0.0.8/adbtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-24 03:38:24.000000 adbtool-0.0.8/adbtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-08-24 03:38:24.000000 adbtool-0.0.8/adbtool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-08-24 03:38:24.000000 adbtool-0.0.8/adbtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-24 03:38:24.000000 adbtool-0.0.8/adbtool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-08-24 03:38:16.000000 adbtool-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-08-24 03:38:25.119054 adbtool-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-08-24 03:38:16.000000 adbtool-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 12:09:00.246102 adbtool-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-12-19 12:08:50.000000 adbtool-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-12-19 12:08:50.000000 adbtool-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2021-12-19 12:09:00.246102 adbtool-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4078 2021-12-19 12:08:50.000000 adbtool-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 12:09:00.242102 adbtool-0.0.9/adbtool/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/adbtool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3863 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 12:09:00.246102 adbtool-0.0.9/adbtool/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3941 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/adbdevice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6393 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/adbpush.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2174 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/apkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/apkinstall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/apksigner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2223 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/apkuninstall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3125 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/assetbundleinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/subcommands/il2cpp.py
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-19 12:08:50.000000 adbtool-0.0.9/adbtool/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-19 12:09:00.242102 adbtool-0.0.9/adbtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2021-12-19 12:09:00.000000 adbtool-0.0.9/adbtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-12-19 12:09:00.000000 adbtool-0.0.9/adbtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-19 12:09:00.000000 adbtool-0.0.9/adbtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-19 12:09:00.000000 adbtool-0.0.9/adbtool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-19 12:09:00.000000 adbtool-0.0.9/adbtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-12-19 12:09:00.000000 adbtool-0.0.9/adbtool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-19 12:08:50.000000 adbtool-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-19 12:09:00.246102 adbtool-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2021-12-19 12:08:50.000000 adbtool-0.0.9/setup.py
```

### Comparing `adbtool-0.0.8/LICENSE` & `adbtool-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/PKG-INFO` & `adbtool-0.0.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,110 @@
-Metadata-Version: 2.1
-Name: adbtool
-Version: 0.0.8
-Summary: A friendly android adb command-line tool
-Home-page: https://github.com/litefeel/adbtool
-Author: litefeel
-Author-email: litefeel@gmail.com
-License: MIT
-Description: # Adbtool
-        A friendly android adb command-line tool
-        
-        [![Test 😎](https://github.com/litefeel/adbtool/workflows/Test%20%F0%9F%98%8E/badge.svg)](https://github.com/litefeel/adbtool/actions)
-        [![PyPI](https://img.shields.io/pypi/v/adbtool.svg)](https://pypi.org/project/adbtool/)
-        [![PyPI](https://img.shields.io/pypi/l/adbtool.svg)](https://pypi.org/project/adbtool/)
-        
-        
-        ### Python Requirements
-        * python 3.9+
-        * Android SDK
-        
-        
-        ### Commands
-        
-        
-        ~~~
-        adbt -h
-        usage: adbt [options]
-        
-        show android device list
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -c CONFIG, --config CONFIG
-                                global config
-          --version             show program's version number and exit
-        
-        sub commands:
-          {devices,push,install,apk}
-            devices             show android device list
-            push                push files to android device
-            install             install apk file
-            apk                 show apk packageName/activityName
-        ~~~
-        
-        ---
-        
-        ~~~
-        adbt devices -h
-        usage: adbt [options] devices [-h] [-d DEVICES [DEVICES ...]] [-l]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -d DEVICES [DEVICES ...], --devices DEVICES [DEVICES ...]
-                                filter of devices, [n | serial | a] n:index of list(start with 1), serial:at least 2 char,
-                                a:all
-          -l, --list            show devices list
-        ~~~
-        ---
-        ~~~
-        adbt push -h
-        usage: adbt [options] push [-h] [-r] [-n] [-j [HASHJSON]] [--hash [{sha1,mtime}]] [--localdir LOCALDIR]
-                                   [--remotedir REMOTEDIR] [--dontpush] [-d [DEVICES [DEVICES ...]]]
-                                   [path [path ...]]
-        
-        positional arguments:
-          path                  file or directory
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -r                    recursion all file
-          -n                    only push new file by last modify files, see -j
-          -j [HASHJSON]         hash json file, default: ./$deviceMode_$deviceSerial.json
-          --hash [{sha1,mtime}]
-                                hash function: mtime or sha1, default:mtime
-          --localdir LOCALDIR   local prefix and remote prefix, will replace local prefix to remote prefix
-          --remotedir REMOTEDIR
-                                local prefix and remote prefix, will replace local prefix to remote prefix
-          --dontpush            only outout json file, not really push file to remote
-          -d [DEVICES [DEVICES ...]], --devices [DEVICES [DEVICES ...]]
-                                filter of devices, [a | n | serial] a: all devices n: index of devices list(start with 1)
-                                serial: devices serial (at least 2 char) not argument is show device list
-        ~~~
-        ---
-        ~~~
-        adbt install -h
-        usage: adbt [options] install [-h] [-f [FILTER [FILTER ...]]] [-r] [-d [DEVICES [DEVICES ...]]] [apkpath]
-        
-        positional arguments:
-          apkpath
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f [FILTER [FILTER ...]], --filter [FILTER [FILTER ...]]
-                                filtered by file name
-          -r, --run             run app after install
-          -d [DEVICES [DEVICES ...]], --devices [DEVICES [DEVICES ...]]
-                                filter of devices, [a | n | serial] a: all devices n: index of devices list(start with 1)
-                                serial: devices serial (at least 2 char) not argument is show device list
-        ~~~
-        ---
-        ~~~
-        adbt apk -h
-        usage: adbt [options] apk [-h] [-r] [-d [DEVICES [DEVICES ...]]] [apkpath]
-        
-        positional arguments:
-          apkpath
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -r, --run             run app
-          -d [DEVICES [DEVICES ...]], --devices [DEVICES [DEVICES ...]]
-                                filter of devices, [a | n | serial] a: all devices n: index of devices list(start with 1)
-                                serial: devices serial (at least 2 char) not argument is show device list
-        ~~~
-        
-Keywords: Android,adb
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+# Adbtool
+A friendly android adb command-line tool
+
+[![Test 😎](https://github.com/litefeel/adbtool/workflows/Test%20%F0%9F%98%8E/badge.svg)](https://github.com/litefeel/adbtool/actions)
+[![PyPI](https://img.shields.io/pypi/v/adbtool.svg)](https://pypi.org/project/adbtool/)
+[![PyPI](https://img.shields.io/pypi/l/adbtool.svg)](https://pypi.org/project/adbtool/)
+
+
+### Python Requirements
+* python 3.9+
+* Android SDK
+
+
+### Commands
+
+
+~~~
+adbt -h
+usage: adbt [options]
+
+show android device list
+
+options:
+  -h, --help            show this help message and exit
+  -c CONFIG, --config CONFIG
+                        global config
+  --version             show program's version number and exit
+
+sub commands:
+  {devices,push,install,uninstall,apk,sign,ab,il2cpp}
+    devices             show android device list
+    push                push files to android device
+    install             install apk file
+    uninstall           uninstall apk file
+    apk                 show apk packageName/activityName
+    sign                sign apk with android debug(only windows)
+    ab                  extract unity asset bundle information
+    il2cpp              extract unity il2cpp information
+~~~
+
+---
+
+~~~
+adbt devices -h
+usage: adbt [options] devices [-h] [-d DEVICES [DEVICES ...]] [-l]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -d DEVICES [DEVICES ...], --devices DEVICES [DEVICES ...]
+                        filter of devices, [n | serial | a] n:index of list(start with 1), serial:at least 2 char,
+                        a:all
+  -l, --list            show devices list
+~~~
+---
+~~~
+adbt push -h
+usage: adbt [options] push [-h] [-r] [-n] [-j [HASHJSON]] [--hash [{sha1,mtime}]] [--localdir LOCALDIR]
+                           [--remotedir REMOTEDIR] [--dontpush] [-d [DEVICES [DEVICES ...]]]
+                           [path [path ...]]
+
+positional arguments:
+  path                  file or directory
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -r                    recursion all file
+  -n                    only push new file by last modify files, see -j
+  -j [HASHJSON]         hash json file, default: ./$deviceMode_$deviceSerial.json
+  --hash [{sha1,mtime}]
+                        hash function: mtime or sha1, default:mtime
+  --localdir LOCALDIR   local prefix and remote prefix, will replace local prefix to remote prefix
+  --remotedir REMOTEDIR
+                        local prefix and remote prefix, will replace local prefix to remote prefix
+  --dontpush            only outout json file, not really push file to remote
+  -d [DEVICES [DEVICES ...]], --devices [DEVICES [DEVICES ...]]
+                        filter of devices, [a | n | serial] a: all devices n: index of devices list(start with 1)
+                        serial: devices serial (at least 2 char) not argument is show device list
+~~~
+---
+~~~
+adbt install -h
+usage: adbt [options] install [-h] [-f [FILTER [FILTER ...]]] [-r] [-d [DEVICES [DEVICES ...]]] [apkpath]
+
+positional arguments:
+  apkpath
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f [FILTER [FILTER ...]], --filter [FILTER [FILTER ...]]
+                        filtered by file name
+  -r, --run             run app after install
+  -d [DEVICES [DEVICES ...]], --devices [DEVICES [DEVICES ...]]
+                        filter of devices, [a | n | serial] a: all devices n: index of devices list(start with 1)
+                        serial: devices serial (at least 2 char) not argument is show device list
+~~~
+---
+~~~
+adbt apk -h
+usage: adbt [options] apk [-h] [-r] [-d [DEVICES [DEVICES ...]]] [apkpath]
+
+positional arguments:
+  apkpath
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -r, --run             run app
+  -d [DEVICES [DEVICES ...]], --devices [DEVICES [DEVICES ...]]
+                        filter of devices, [a | n | serial] a: all devices n: index of devices list(start with 1)
+                        serial: devices serial (at least 2 char) not argument is show device list
+~~~
```

### Comparing `adbtool-0.0.8/adbtool/adbtool.py` & `adbtool-0.0.9/adbtool/adbtool.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     adbdevice,
     adbpush,
     apkinfo,
     apkinstall,
     apkuninstall,
     apksigner,
     assetbundleinfo,
+    il2cpp,
 )
 
 _VERSION_FILE_NAME = "version.txt"
 
 
 def get_version() -> str:
     dir_of_this_script = os.path.split(__file__)[0]
@@ -57,14 +58,15 @@
         Command("devices", adbdevice, "show android device list"),
         Command("push", adbpush, "push files to android device"),
         Command("install", apkinstall, "install apk file"),
         Command("uninstall", apkuninstall, "uninstall apk file"),
         Command("apk", apkinfo, "show apk packageName/activityName"),
         Command("sign", apksigner, "sign apk with android debug(only windows)"),
         Command("ab", assetbundleinfo, "extract unity asset bundle information"),
+        Command("il2cpp", il2cpp, "extract unity il2cpp information"),
     ]
 
     subparser = parser.add_subparsers(title="sub commands", dest="subcommand")
     addsubcommands(subparser, commands)
 
     args = parser.parse_args(_args)
     if args.subcommand is None:
```

### Comparing `adbtool-0.0.8/adbtool/cmd.py` & `adbtool-0.0.9/adbtool/cmd.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/config.py` & `adbtool-0.0.9/adbtool/config.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/adbdevice.py` & `adbtool-0.0.9/adbtool/subcommands/adbdevice.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/adbpush.py` & `adbtool-0.0.9/adbtool/subcommands/adbpush.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/apkinfo.py` & `adbtool-0.0.9/adbtool/subcommands/apkinfo.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/apkinstall.py` & `adbtool-0.0.9/adbtool/subcommands/apkinstall.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/apksigner.py` & `adbtool-0.0.9/adbtool/subcommands/apksigner.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/apkuninstall.py` & `adbtool-0.0.9/adbtool/subcommands/apkuninstall.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool/subcommands/assetbundleinfo.py` & `adbtool-0.0.9/adbtool/subcommands/assetbundleinfo.py`

 * *Files identical despite different names*

### Comparing `adbtool-0.0.8/adbtool.egg-info/SOURCES.txt` & `adbtool-0.0.9/adbtool.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 adbtool/subcommands/__init__.py
 adbtool/subcommands/adbdevice.py
 adbtool/subcommands/adbpush.py
 adbtool/subcommands/apkinfo.py
 adbtool/subcommands/apkinstall.py
 adbtool/subcommands/apksigner.py
 adbtool/subcommands/apkuninstall.py
-adbtool/subcommands/assetbundleinfo.py
+adbtool/subcommands/assetbundleinfo.py
+adbtool/subcommands/il2cpp.py
```

### Comparing `adbtool-0.0.8/setup.py` & `adbtool-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     license="MIT",
     url="https://github.com/litefeel/adbtool",
     author="litefeel",
     author_email="litefeel@gmail.com",
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     platforms="any",
-    install_requires=["litefeel-pycommon", "PyYAML", "semantic_version"],
+    install_requires=["litefeel-pycommon", "PyYAML", "semantic_version", "var_dump"],
     scripts=[],
     entry_points={"console_scripts": ["adbt = adbtool.adbtool:main"]},
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
```

