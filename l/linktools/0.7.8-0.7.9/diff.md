# Comparing `tmp/linktools-0.7.8.tar.gz` & `tmp/linktools-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.7.8.tar", last modified: Fri Mar  3 10:48:34 2023, max compression
+gzip compressed data, was "linktools-0.7.9.tar", last modified: Sat Mar 25 16:10:33 2023, max compression
```

## Comparing `linktools-0.7.8.tar` & `linktools-0.7.9.tar`

### file list

```diff
@@ -1,104 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-03-03 10:48:31.000000 linktools-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-03 10:48:31.000000 linktools-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    31931 2023-03-03 10:48:34.136032 linktools-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31504 2023-03-03 10:48:31.000000 linktools-0.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 10:48:34.136032 linktools-0.7.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-03-03 10:48:31.000000 linktools-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.120032 linktools-0.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.128032 linktools-0.7.8/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.128032 linktools-0.7.8/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/android/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.132032 linktools-0.7.8/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    81735 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/chrome-driver.json
--rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/fake_useragent_0.1.11.json
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (123)    20950 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.120032 linktools-0.7.8/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.132032 linktools-0.7.8/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/assets/tools.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.132032 linktools-0.7.8/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.120032 linktools-0.7.8/src/linktools/cli/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/cli/commands/android/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2253 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2146 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15211 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2638 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6942 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6108 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16180 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4531 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/cli/commands/common/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7671 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/common/grep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/common/shell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3565 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/cli/commands/ios/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6028 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (123)    23374 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/frida/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ios/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ios/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/ios/sib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/references/fake_useragent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.136032 linktools-0.7.8/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_url.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8422 2023-03-03 10:48:31.000000 linktools-0.7.8/src/linktools/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-03 10:48:33.000000 linktools-0.7.8/src/linktools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 10:48:34.128032 linktools-0.7.8/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31931 2023-03-03 10:48:34.000000 linktools-0.7.8/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-03 10:48:34.000000 linktools-0.7.8/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 10:48:34.000000 linktools-0.7.8/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-03 10:48:34.000000 linktools-0.7.8/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-03 10:48:34.000000 linktools-0.7.8/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-03 10:48:34.000000 linktools-0.7.8/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-03-25 16:10:23.000000 linktools-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-25 16:10:23.000000 linktools-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31931 2023-03-25 16:10:33.075611 linktools-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31504 2023-03-25 16:10:23.000000 linktools-0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 16:10:33.075611 linktools-0.7.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-03-25 16:10:23.000000 linktools-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.067611 linktools-0.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/android/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20405 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    81735 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/chrome-driver.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42687 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/fake_useragent_0.1.11.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20950 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.067611 linktools-0.7.9/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/assets/tools.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.067611 linktools-0.7.9/src/linktools/cli/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools/cli/commands/android/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2144 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15209 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2636 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6942 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6106 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16178 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4529 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/cli/commands/common/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7669 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/common/grep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/common/shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/cli/commands/ios/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6028 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/ios/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/ios/sib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/references/fake_useragent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.075611 linktools-0.7.9/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_url.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8751 2023-03-25 16:10:23.000000 linktools-0.7.9/src/linktools/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-25 16:10:31.000000 linktools-0.7.9/src/linktools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 16:10:33.071611 linktools-0.7.9/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31931 2023-03-25 16:10:33.000000 linktools-0.7.9/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-25 16:10:33.000000 linktools-0.7.9/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 16:10:33.000000 linktools-0.7.9/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-25 16:10:33.000000 linktools-0.7.9/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-25 16:10:33.000000 linktools-0.7.9/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-25 16:10:33.000000 linktools-0.7.9/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.7.8/LICENSE` & `linktools-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/PKG-INFO` & `linktools-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.7.8
+Version: 0.7.9
 Summary: linktools toolkit
 Home-page: https://github.com/ice-black-tea/Zelda/tree/master
 Author: Hu Ji
 Author-email: 669898595@qq.com
 License: Apache 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.7.8/README.md` & `linktools-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/setup.py` & `linktools-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/__init__.py` & `linktools-0.7.9/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/__main__.py` & `linktools-0.7.9/src/linktools/cli/commands/android/adb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : __main__.py 
-@time    : 2022/12/13
+@file    : at_adb.py
+@time    : 2019/03/04
 @site    :  
 @software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
@@ -25,59 +25,49 @@
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser
 from typing import Optional
 
-from rich import get_console
-from rich.tree import Tree
+from linktools import cli
+from linktools.android import Adb
 
-from . import __description__, cli
 
+class Command(cli.AndroidCommand):
+    """
+    Adb that supports multiple devices
+    """
+
+    _GENERAL_COMMANDS = [
+        "devices",
+        "help",
+        "version",
+        "connect",
+        "disconnect",
+        "keygen",
+        "wait-for-",
+        "start-server",
+        "kill-server",
+        "reconnect",
+    ]
+
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        parser.add_argument("adb_args", nargs="...", help="adb args")
+
+    def run(self, args: [str]) -> Optional[int]:
+        args, extra = self.argument_parser.parse_known_args(args)
+
+        adb_args = [*extra, *args.adb_args]
+        if not extra:
+            if args.adb_args and args.adb_args[0] not in self._GENERAL_COMMANDS:
+                device = args.parse_device()
+                process = device.popen(*adb_args, capture_output=False)
+                return process.call()
 
-class Command(cli.Command):
-
-    @property
-    def _commands(self):
-        return cli.get_commands()
-
-    def _add_arguments(self, parser: ArgumentParser) -> None:
-        sub_parsers = parser.add_subparsers()
-        for category, commands in cli.get_commands().items():
-            parser = sub_parsers.add_parser(
-                category.name,
-                description=category.description
-            )
-            parser.set_defaults(help=parser.print_help)
-            catalog_parser = parser.add_subparsers()
-            for command in commands:
-                parser = catalog_parser.add_parser(
-                    command.name,
-                    help=command.description,
-                    add_help=False,
-                    prefix_chars=chr(0)
-                )
-                parser.add_argument("args", nargs="...")
-                parser.set_defaults(func=command.command)
-
-    def _run(self, args: [str]) -> Optional[int]:
-        args = self.argument_parser.parse_args(args)
-        if hasattr(args, "func") and hasattr(args, "args"):
-            return args.func(args.args)
-        elif hasattr(args, "help"):
-            return args.help()
-
-        tree = Tree("📎 All commands")
-        for category, commands in cli.get_commands().items():
-            node = tree.add(f"📖 {category}")
-            for command in commands:
-                node.add(f"👉 {command.category.prefix}[bold red]{command.name}[/bold red]: {command.description}")
-
-        console = get_console()
-        console.print(__description__, highlight=False)
-        console.print(tree, highlight=False)
+        process = Adb.popen(*adb_args, capture_output=False)
+        return process.call()
 
 
 command = Command()
-if __name__ == '__main__':
+if __name__ == "__main__":
     command.main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `linktools-0.7.8/src/linktools/_config.py` & `linktools-0.7.9/src/linktools/_config.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/_environ.py` & `linktools-0.7.9/src/linktools/_environ.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/_logging.py` & `linktools-0.7.9/src/linktools/_logging.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/_resource.py` & `linktools-0.7.9/src/linktools/_resource.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/_tools.py` & `linktools-0.7.9/src/linktools/_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
         :param ignore_errors: 忽略错误，报错不会抛异常
         :param log_output: 把输出打印到logger中
         :return: 返回stdout输出内容
         """
         process = self.popen(*args, capture_output=True)
 
         try:
-            out, err = process.run(timeout, log_stdout=log_output, log_stderr=log_output)
+            out, err = process.exec(timeout, log_stdout=log_output, log_stderr=log_output)
             if not ignore_errors and process.poll() not in (0, None):
                 if isinstance(err, bytes):
                     err = err.decode(errors="ignore")
                     err = err.strip()
                 elif isinstance(err, str):
                     err = err.strip()
                 if err:
```

### Comparing `linktools-0.7.8/src/linktools/android/__init__.py` & `linktools-0.7.9/src/linktools/android/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/android/adb.py` & `linktools-0.7.9/src/linktools/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/android/struct.py` & `linktools-0.7.9/src/linktools/android/struct.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/android-tools.apk` & `linktools-0.7.9/src/linktools/assets/android-tools.apk`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/chrome-driver.json` & `linktools-0.7.9/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/fake_useragent_0.1.11.json` & `linktools-0.7.9/src/linktools/assets/fake_useragent_0.1.11.json`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/frida.js` & `linktools-0.7.9/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/frida.min.js` & `linktools-0.7.9/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.7.9/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/assets/tools.yml` & `linktools-0.7.9/src/linktools/assets/tools.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   <<: *JAR
   version: 2.5.2
   download_url: https://bitbucket.org/JesusFreke/smali/downloads/smali-{version}.jar
   target_path: smali-{version}.jar
 
 GENERAL_TOOL_APKTOOL:
   <<: *JAR
-  version: 2.6.1
+  version: 2.7.0
   download_url: https://bitbucket.org/iBotPeaches/apktool/downloads/apktool_{version}.jar
   target_path: apktool-{version}.jar
 
 GENERAL_TOOL_APPCRAWLER:
   <<: *JAR
   cmdline: appcrawler
   version: 2.7.4
```

### Comparing `linktools-0.7.8/src/linktools/cli/__init__.py` & `linktools-0.7.9/src/linktools/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,9 +23,9 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from ._cli import get_commands
+from ._cli import walk_commands
 from ._command import Command, AndroidCommand, IOSCommand
```

### Comparing `linktools-0.7.8/src/linktools/cli/_command.py` & `linktools-0.7.9/src/linktools/cli/_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,103 +46,59 @@
 from .._logging import LogHandler, get_logger
 from ..decorator import cached_property
 from ..utils import ignore_error
 from ..version import __version__, __description__
 
 
 class Command(abc.ABC):
-    logger: logging.Logger = property(lambda self: self._logger)
-    description: str = cached_property(lambda self: textwrap.dedent((self.__doc__ or "").strip()))
-    argument_parser: ArgumentParser = cached_property(lambda self: self._create_argument_parser())
-    known_errors: Tuple[Type[BaseException]] = property(lambda self: self._known_errors)
-
-    def main(self, *args, **kwargs) -> None:
-        try:
-            self._main_init()
-            logging.basicConfig(
-                level=logging.INFO,
-                format="%(message)s",
-                datefmt="[%X]",
-                handlers=[LogHandler()]
-            )
-            exit(self(*args, **kwargs))
-        finally:
-            self._main_deinit()
-
-    def _main_init(self):
-        pass
-
-    def _main_deinit(self):
-        pass
 
     @property
-    def _logger(self) -> logging.Logger:
+    def logger(self) -> logging.Logger:
         return get_logger()
 
+    @cached_property
+    def description(self) -> str:
+        return textwrap.dedent((self.__doc__ or "").strip())
+
+    @cached_property
+    def argument_parser(self) -> ArgumentParser:
+        return self.create_argument_parser()
+
     @property
-    def _known_errors(self) -> Tuple[Type[BaseException]]:
+    def known_errors(self) -> Tuple[Type[BaseException]]:
         return tuple()
 
     @abc.abstractmethod
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         pass
 
-    @abc.abstractmethod
-    def _run(self, args: [str]) -> Optional[int]:
-        pass
-
-    def __call__(self, args: [str] = None) -> int:
-        try:
-            args = args if args is not None else sys.argv[1:]
-            exit_code = self._run(args) or 0
-
-        except SystemExit as e:
-            exit_code = e.code
-
-        except (KeyboardInterrupt, EOFError, *self.known_errors) as e:
-            exit_code = 1
-            error_type, error_message = e.__class__.__name__, str(e).strip()
-            self.logger.error(
-                f"{error_type}: {error_message}" if error_message else error_type,
-                exc_info=True if environ.debug else None,
-            )
-
-        except:
-            exit_code = 1
-            if environ.debug:
-                console = get_console()
-                console.print_exception(show_locals=True)
-            else:
-                self.logger.error(traceback.format_exc())
-
-        return exit_code
-
-    def _create_argument_parser(self):
+    def create_argument_parser(self):
 
         description = self.description.strip()
         if description:
             description += os.linesep + os.linesep
         description += __description__
 
         parser = ArgumentParser(
             formatter_class=RawDescriptionHelpFormatter,
             description=description,
             conflict_handler="resolve"
         )
-        self._add_base_arguments(parser)
-        self._add_arguments(parser)
+        self.add_log_arguments(parser)
+        self.add_base_arguments(parser)
+        self.add_arguments(parser)
 
         return parser
 
-    def _add_base_arguments(self, parser: ArgumentParser):
+    def add_log_arguments(self, parser: ArgumentParser):
 
         class VerboseAction(Action):
 
             def __call__(self, parser, namespace, values, option_string=None):
-                environ.logger.setLevel(logging.DEBUG)
+                logging.root.setLevel(logging.DEBUG)
 
         class DebugAction(Action):
 
             def __call__(self, parser, namespace, values, option_string=None):
                 environ.debug = True
                 environ.logger.setLevel(logging.DEBUG)
 
@@ -159,38 +115,88 @@
 
         class LogLevelAction(BooleanOptionalAction):
 
             def __call__(self, parser, namespace, values, option_string=None):
                 if option_string in self.option_strings:
                     environ.show_log_level = not option_string.startswith("--no-")
 
-        parser.add_argument("--version", action="version", version="%(prog)s " + __version__)
-
         group = parser.add_argument_group(title="log arguments")
         group.add_argument("--verbose", action=VerboseAction, nargs=0, const=True, dest=SUPPRESS,
                            help="increase log verbosity")
         group.add_argument("--debug", action=DebugAction, nargs=0, const=True, dest=SUPPRESS,
                            help="enable debug mode and increase log verbosity")
 
         if LogHandler.get_instance():
             group.add_argument("--time", "--no-time", action=LogTimeAction, nargs=0, dest=SUPPRESS,
                                help="show log time")
             group.add_argument("--level", "--no-level", action=LogLevelAction, nargs=0, dest=SUPPRESS,
                                help="show log level")
 
+    def add_base_arguments(self, parser: ArgumentParser):
+        parser.add_argument("--version", action="version", version="%(prog)s " + __version__)
+
+    def main(self, *args, **kwargs) -> None:
+        try:
+            self.on_main_init()
+            logging.basicConfig(
+                level=logging.INFO,
+                format="%(message)s",
+                datefmt="[%X]",
+                handlers=[LogHandler()]
+            )
+            exit(self(*args, **kwargs))
+        finally:
+            self.on_main_deinit()
+
+    def on_main_init(self):
+        pass
+
+    def on_main_deinit(self):
+        pass
+
+    @abc.abstractmethod
+    def run(self, args: [str]) -> Optional[int]:
+        pass
+
+    def __call__(self, args: [str] = None) -> int:
+        try:
+            args = args if args is not None else sys.argv[1:]
+            exit_code = self.run(args) or 0
+
+        except SystemExit as e:
+            exit_code = e.code
+
+        except (KeyboardInterrupt, EOFError, *self.known_errors) as e:
+            exit_code = 1
+            error_type, error_message = e.__class__.__name__, str(e).strip()
+            self.logger.error(
+                f"{error_type}: {error_message}" if error_message else error_type,
+                exc_info=True if environ.debug else None,
+            )
+
+        except:
+            exit_code = 1
+            if environ.debug:
+                console = get_console()
+                console.print_exception(show_locals=True)
+            else:
+                self.logger.error(traceback.format_exc())
+
+        return exit_code
+
 
 class AndroidCommand(Command, ABC):
 
     @property
-    def _known_errors(self) -> Tuple[Type[BaseException]]:
+    def known_errors(self) -> Tuple[Type[BaseException]]:
         from linktools.android import AdbError
         return AdbError,
 
-    def _add_base_arguments(self, parser: ArgumentParser):
-        super()._add_base_arguments(parser)
+    def add_base_arguments(self, parser: ArgumentParser):
+        super().add_base_arguments(parser)
 
         from linktools.android import Adb, Device, AdbError
         cache_path = environ.resource.get_temp_path("cache", "device", "android", create_parent=True)
 
         def parse_handler(fn):
             @functools.wraps(fn)
             def wrapper(*args, **kwargs):
@@ -302,20 +308,20 @@
         group.add_argument("-l", "--last", dest="parse_device", nargs=0, const=True, action=LastAction,
                            help="use last device")
 
 
 class IOSCommand(Command, ABC):
 
     @property
-    def _known_errors(self) -> Tuple[Type[BaseException]]:
+    def known_errors(self) -> Tuple[Type[BaseException]]:
         from linktools.ios import SibError
         return SibError,
 
-    def _add_base_arguments(self, parser: ArgumentParser):
-        super()._add_base_arguments(parser)
+    def add_base_arguments(self, parser: ArgumentParser):
+        super().add_base_arguments(parser)
 
         from linktools.ios import Sib, SibError, Device
         cache_path = environ.resource.get_temp_path("cache", "device", "ios", create_parent=True)
 
         def parse_handler(fn):
             @functools.wraps(fn)
             def wrapper(*args, **kwargs):
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/adb.py` & `linktools-0.7.9/src/linktools/cli/commands/android/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : at_adb.py
-@time    : 2019/03/04
+@file    : at_call_agent.py
+@time    : 2018/12/02
 @site    :  
 @software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
@@ -26,48 +26,37 @@
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser
 from typing import Optional
 
 from linktools import cli
-from linktools.android import Adb
 
 
 class Command(cli.AndroidCommand):
     """
-    Adb that supports multiple devices
+    Debug android-tools.apk
     """
 
-    _GENERAL_COMMANDS = [
-        "devices",
-        "help",
-        "version",
-        "connect",
-        "disconnect",
-        "keygen",
-        "wait-for-",
-        "start-server",
-        "kill-server",
-        "reconnect",
-    ]
-
-    def _add_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument("adb_args", nargs="...", help="adb args")
-
-    def _run(self, args: [str]) -> Optional[int]:
-        args, extra = self.argument_parser.parse_known_args(args)
-
-        adb_args = [*extra, *args.adb_args]
-        if not extra:
-            if args.adb_args and args.adb_args[0] not in self._GENERAL_COMMANDS:
-                device = args.parse_device()
-                process = device.popen(*adb_args, capture_output=False)
-                return process.call()
-
-        process = Adb.popen(*adb_args, capture_output=False)
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        parser.add_argument("-p", "--privilege", action="store_true", default=False,
+                            help="run with root privilege")
+        parser.add_argument("agent_args", nargs="...", help="agent args")
+
+    def run(self, args: [str]) -> Optional[int]:
+        args = self.argument_parser.parse_args(args)
+        device = args.parse_device()
+        adb_args = [
+            "CLASSPATH=%s" % device.init_agent(),
+            "app_process", "/", device.agent_info["main"],
+            *args.agent_args
+        ]
+        adb_args = ["shell", *adb_args] \
+            if not args.privilege or device.uid == 0 \
+            else ["shell", "su", "-c", *adb_args]
+        process = device.popen(*adb_args)
         return process.call()
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/agent.py` & `linktools-0.7.9/src/linktools/cli/commands/ios/ssh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : at_call_agent.py
-@time    : 2018/12/02
+@file    : ssh.py 
+@time    : 2022/11/27
 @site    :  
 @software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
@@ -23,40 +23,51 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser
-from typing import Optional
+from typing import Optional, Tuple, Type
 
-from linktools import cli
+import paramiko
+from paramiko.ssh_exception import SSHException
 
+from linktools import cli, utils
+from linktools.ios import Device
 
-class Command(cli.AndroidCommand):
+
+class Command(cli.IOSCommand):
     """
-    Debug android-tools.apk
+    OpenSSH remote login client (require iOS device jailbreak)
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument("-p", "--privilege", action="store_true", default=False,
-                            help="run with root privilege")
-        parser.add_argument("agent_args", nargs="...", help="agent args")
+    @property
+    def known_errors(self) -> Tuple[Type[BaseException]]:
+        return super().known_errors + tuple([SSHException])
+
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        parser.add_argument("-u", "--username", action="store", default="root",
+                            help="iOS ssh username (default: root)")
+        parser.add_argument("-p", "--port", action="store", type=int, default=22,
+                            help="iOS ssh port (default: 22)")
+        parser.add_argument("--password", action="store",
+                            help="iOS ssh password")
+        parser.add_argument('ssh_args', nargs='...', help="ssh args")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
-        device = args.parse_device()
-        adb_args = [
-            "CLASSPATH=%s" % device.init_agent(),
-            "app_process", "/", device.agent_info["main"],
-            *args.agent_args
-        ]
-        adb_args = ["shell", *adb_args] \
-            if not args.privilege or device.uid == 0 \
-            else ["shell", "su", "-c", *adb_args]
-        process = device.popen(*adb_args)
-        return process.call()
+        device: Device = args.parse_device()
+
+        local_port = utils.pick_unused_port()
+        with device.forward(local_port, args.port):
+            with utils.SSHClient() as client:
+                client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+                client.connect_with_pwd("localhost", port=local_port, username=args.username, password=args.password)
+                client.open_shell(*args.ssh_args)
+
+        return 0
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/app.py` & `linktools-0.7.9/src/linktools/cli/commands/android/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Fetch application info
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group()
         group.add_argument('-t', '--top', action='store_true', default=False,
                            help='fetch current running app only')
         group.add_argument('-a', '--all', action='store_true', default=False,
                            help='fetch all apps')
         group.add_argument('-p', '--packages', metavar="pkg", action='store', nargs='+', default=None,
                            help='fetch target apps only')
@@ -249,15 +249,15 @@
         parser.add_argument('--dangerous', action='store_true', default=False,
                             help='display dangerous permissions and components only')
         parser.add_argument('-o', '--order-by', metavar="field", action='store', nargs='+', default=['userId', 'name'],
                             choices=['name', 'appName', 'userId', 'sourceDir',
                                      'enabled', 'system', 'debuggable', 'allowBackup'],
                             help='order by target field')
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         if not utils.is_empty(args.packages):
             packages = device.get_packages(*args.packages, simple=args.simple)
         elif not utils.is_empty(args.uids):
             packages = device.get_packages_for_uid(*args.uids, simple=args.simple)
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/debug.py` & `linktools-0.7.9/src/linktools/cli/commands/android/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     Debug app by jdb
     """
 
     @property
     def _description(self) -> str:
         return "debugger"
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('package', action='store', default=None,
                             help='regular expression')
         parser.add_argument('activity', action='store', default=None,
                             help='regular expression')
         parser.add_argument('-p', '--port', action='store', type=int, default=8701,
                             help='fetch all apps')
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         device.shell("am", "force-stop", args.package, log_output=True)
         device.shell("am", "start", "-D", "-n", "{}/{}".format(args.package, args.activity), log_output=True)
 
         pid = utils.int(device.shell("top", "-n", "1", "|", "grep", args.package).split()[0])
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/frida.py` & `linktools-0.7.9/src/linktools/cli/commands/android/frida.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Easy to use frida (require Android device rooted)
     """
 
-    def _main_init(self):
+    def on_main_init(self):
         environ.show_log_time = True
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-p", "--package", action="store", default=None,
                             help="target package (default: frontmost application)")
         parser.add_argument("--spawn", action="store_true", default=False,
                             help="inject after spawn (default: false)")
 
         parser.add_argument("-P", "--parameters", metavar=("KEY", "VALUE"),
                             action="append", nargs=2, dest="user_parameters", default=[],
@@ -69,15 +69,15 @@
         parser.add_argument("--redirect-port", metavar="PORT", action="store", dest="redirect_port",
                             type=utils.range_type(1, 65536),
                             help="redirect traffic to target port (default: 8080)")
 
         parser.add_argument("-a", "--auto-start", action="store_true", default=False,
                             help="automatically start when all processes exits")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
         package = args.package
 
         user_parameters = {p[0]: p[1] for p in args.user_parameters}
         user_scripts = args.user_scripts
         for user_script in user_scripts:
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/info.py` & `linktools-0.7.9/src/linktools/cli/commands/android/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,18 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Fetch device information
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('agent_args', nargs='...', help="agent args")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         logger.info(f"Property", style="red")
         for prop in props:
             logger.info(
                 f"{prop}: {device.get_prop(prop)}",
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/intent.py` & `linktools-0.7.9/src/linktools/cli/commands/android/intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Common intent actions
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group(required=True)
         group.add_argument('--setting', dest='package', action='store_true',
                            help='start setting activity')
         group.add_argument('--setting-dev', dest='package', action='store_true',
                            help='start development setting activity')
         group.add_argument('--setting-dev2', dest='package', action='store_true',
                            help='start development setting activity')
@@ -53,15 +53,15 @@
         group.add_argument('--setting-cert', dest='path', action='store', default="",
                            help='install cert (need \'/data/local/tmp\' write permission)')
         group.add_argument('--install', dest='path', action='store', default="",
                            help='install apk file (need \'/data/local/tmp\' write permission)')
         group.add_argument('--browser', dest='url', action='store', default="",
                            help='start browser activity and jump to url (need scheme, such as https://antiy.cn)')
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         if "--setting" in sys.argv:
             device.shell("am", "start", "--user", "0",
                          "-a", "android.settings.SETTINGS",
                          log_output=True)
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/objection.py` & `linktools-0.7.9/src/linktools/cli/commands/android/objection.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Easy to use objection (require Android device rooted)
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-p", "--package", action="store", default=None,
                             help="target package (default: frontmost application)")
         parser.add_argument("-s", "--startup-command", action="append", default=[],
                             help="A command to run before the repl polls the device for information.")
         parser.add_argument("-c", "--file-commands", action="store",
                             help="A file containing objection commands, separated by a "
                                  "newline, that will run before the repl polls the device for information.")
@@ -54,15 +54,15 @@
         parser.add_argument("--redirect-address", metavar="ADDRESS", action="store", dest="redirect_address",
                             type=str,
                             help="redirect traffic to target address (default: localhost)")
         parser.add_argument("--redirect-port", metavar="PORT", action="store", dest="redirect_port",
                             type=utils.range_type(1, 65536),
                             help="redirect traffic to target port (default: 8080)")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         with AndroidFridaServer(device=device, local_port=utils.pick_unused_port()) as server:
 
             objection_args = ["objection"]
             if environ.debug:
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.7.9/src/linktools/cli/commands/android/pidcat.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Filter logcat by package name
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('package', nargs='*', help='application package name(s)')
         parser.add_argument('-w', '--tag-width', metavar='N', dest='tag_width', type=int, default=23,
                             help='width of log tag')
         parser.add_argument('-l', '--min-level', dest='min_level', type=str, choices=LOG_LEVELS + LOG_LEVELS.lower(),
                             default='V', help='minimum level to be displayed')
         parser.add_argument('--color-gc', dest='color_gc', action='store_true', help='color garbage collection')
         parser.add_argument('--always-display-tags', dest='always_tags', action='store_true',
@@ -77,15 +77,15 @@
         parser.add_argument('-i', '--ignore-tag', dest='ignored_tag', action='append',
                             help='filter output by ignoring specified tag(s)')
         parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__,
                             help='print the version number and exit')
         parser.add_argument('-a', '--all', dest='all', action='store_true', default=False,
                             help='print all log messages')
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
         package = args.package
         min_level = LOG_LEVELS_MAP[args.min_level.upper()]
 
         if args.current_app:
             package.append(device.get_current_package())
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/android/top.py` & `linktools-0.7.9/src/linktools/cli/commands/android/top.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,30 +36,30 @@
 
 
 class Command(cli.AndroidCommand):
     """
     Fetch current running app's basic information
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group()
         group.add_argument('-p', '--package', action='store_const', const=True, default=False,
                            help='show current package name')
         group.add_argument('-a', '--activity', action='store_const', const=True, default=False,
                            help='show current activity name')
         group.add_argument('--path', action='store_const', const=True, default=False,
                            help='show current apk path')
         group.add_argument('--kill', action='store_const', const=True, default=False,
                            help='kill current package')
         group.add_argument('--apk', metavar='DEST', action='store', type=str, nargs='?', default=".",
                            help='pull current apk file')
         group.add_argument('--screen', metavar='DEST', action='store', type=str, nargs='?', default=".",
                            help='capture screen and pull file')
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         if args.package:
             logger.info(device.get_current_package())
         elif args.activity:
             logger.info(device.get_current_activity())
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/common/grep.py` & `linktools-0.7.9/src/linktools/cli/commands/common/grep.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,23 +192,23 @@
 
 
 class Command(cli.Command):
     """
     Match files with regular expression
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('-i', '--ignore-case', action='store_true', default=False,
                             help='ignore case')
         parser.add_argument('pattern', action='store', default=None,
                             help='regular expression')
         parser.add_argument('files', metavar="file", action='store', nargs='*', default=None,
                             help='target files path')
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
 
         flags = 0
         if args.ignore_case:
             flags = flags | re.I
         pattern = re.compile(bytes(args.pattern, encoding="utf8"), flags=flags)
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/common/shell.py` & `linktools-0.7.9/src/linktools/cli/commands/common/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
             if "SHELL" in os.environ:
                 self._shell_path = os.environ["SHELL"]
         elif tools.system in ["windows"]:
             self._shell_path = shutil.which("powershell") or shutil.which("cmd")
             if "ComSpec" in os.environ:
                 self._shell_path = os.environ["ComSpec"]
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-c", "--command", action="store", default=None, help="shell command")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         if args.command:
             process = utils.Popen(args.command, shell=True)
             return process.call()
 
         if not self._shell_path or not os.path.exists(self._shell_path):
             raise NotImplementedError(f"unsupported system {tools.system}")
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/common/tools.py` & `linktools-0.7.9/src/linktools/cli/commands/common/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,30 @@
 class Command(cli.Command):
     """
     Tools downloaded from the web
     """
 
     _TOOL_NAMES = sorted([tool.name for tool in iter(tools)])
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group()
         parser.add_argument("--set", metavar=("KEY", "VALUE"),
                             action="append", nargs=2, dest="configs", default=[],
                             help="set the config of tool")
         group.add_argument("-c", "--config", action="store_true", default=False,
                            help="show the config of tool")
         group.add_argument("--download", action="store_true", default=False,
                            help="download tool files")
         group.add_argument("--clear", action="store_true", default=False,
                            help="clear tool files")
         group.add_argument("-d", "--daemon", action="store_true", default=False,
                            help="execute tools as a daemon")
         parser.add_argument("tool", nargs="...", choices=self._TOOL_NAMES)
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         if len(args.tool) == 0 or args.tool[0] not in self._TOOL_NAMES:
             self.argument_parser.print_help()
             return -1
 
         tool_name = args.tool[0]
         tool_args = args.tool[1:]
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/ios/frida.py` & `linktools-0.7.9/src/linktools/cli/commands/ios/frida.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
 
 class Command(cli.IOSCommand):
     """
     Easy to use frida (require iOS device jailbreak)
     """
 
-    def _main_init(self):
+    def on_main_init(self):
         environ.show_log_time = True
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-b", "--bundle-id", action="store", default=None,
                             help="target bundle id (default: frontmost application)")
         parser.add_argument("--spawn", action="store_true", default=False,
                             help="inject after spawn (default: false)")
 
         parser.add_argument("-P", "--parameters", metavar=("KEY", "VALUE"),
                             action="append", nargs=2, dest="user_parameters", default=[],
@@ -62,15 +62,15 @@
         parser.add_argument("-c", "--codeshare", metavar="URL", action="append", dest="user_scripts",
                             type=lambda o: FridaShareScript(o, cached=False),
                             help="load share script url")
 
         parser.add_argument("-a", "--auto-start", action="store_true", default=False,
                             help="automatically start when all processes exits")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
         bundle_id = args.bundle_id
 
         user_parameters = {p[0]: p[1] for p in args.user_parameters}
         user_scripts = args.user_scripts
         for user_script in user_scripts:
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/ios/objection.py` & `linktools-0.7.9/src/linktools/cli/commands/ios/objection.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 
 
 class Command(cli.IOSCommand):
     """
     Easy to use objection (require iOS device jailbreak)
     """
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-b", "--bundle-id", action="store", default=None,
                             help="target bundle id (default: frontmost application)")
         parser.add_argument("-s", "--startup-command", action="append", default=[],
                             help="A command to run before the repl polls the device for information.")
         parser.add_argument("-c", "--file-commands", action="store",
                             help="A file containing objection commands, separated by a "
                                  "newline, that will run before the repl polls the device for information.")
         parser.add_argument("-S", "--startup-script", action="store",
                             help="A script to import and run before the repl polls the device for information.")
         parser.add_argument("-P", "--plugin-folder", action="store", default=resource.get_asset_path("objection"),
                             help="The folder to load plugins from.")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device = args.parse_device()
 
         with IOSFridaServer(device=device, local_port=utils.pick_unused_port()) as server:
 
             objection_args = ["objection"]
             if environ.debug:
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/ios/scp.py` & `linktools-0.7.9/src/linktools/cli/commands/ios/scp.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,31 @@
 
 class Command(cli.IOSCommand):
     """
     OpenSSH secure file copy (require iOS device jailbreak)
     """
 
     @property
-    def _known_errors(self) -> Tuple[Type[BaseException]]:
-        return super()._known_errors + tuple([NotImplementedError, FileNotFoundError, SSHException])
+    def known_errors(self) -> Tuple[Type[BaseException]]:
+        return super().known_errors + tuple([NotImplementedError, FileNotFoundError, SSHException])
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("-u", "--username", action="store", default="root",
                             help="iOS ssh username (default: root)")
         parser.add_argument("-p", "--port", action="store", type=int, default=22,
                             help="iOS ssh port (default: 22)")
         parser.add_argument("--password", action="store",
                             help="iOS ssh password")
 
         parser.add_argument("source", action="store", type=SCPFile, default=None,
                             help=f"source file path, remote path needs to be prefixed with \"{_REMOTE_PATH_PREFIX}\"")
         parser.add_argument("target", action="store", type=SCPFile, default=None,
                             help=f"target file path, remote path needs to be prefixed with \"{_REMOTE_PATH_PREFIX}\"")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args = self.argument_parser.parse_args(args)
         device: Device = args.parse_device()
 
         local_port = utils.pick_unused_port()
         with device.forward(local_port, args.port):
             with utils.SSHClient() as client:
                 client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
```

### Comparing `linktools-0.7.8/src/linktools/cli/commands/ios/sib.py` & `linktools-0.7.9/src/linktools/cli/commands/ios/sib.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         "completion",
         "devices",
         "help",
         "version",
         "remote",
     ]
 
-    def _add_arguments(self, parser: ArgumentParser) -> None:
+    def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('sib_args', nargs='...', help="sib args")
 
-    def _run(self, args: [str]) -> Optional[int]:
+    def run(self, args: [str]) -> Optional[int]:
         args, extra = self.argument_parser.parse_known_args(args)
 
         sib_args = [*extra, *args.sib_args]
         if not extra:
             if args.sib_args and args.sib_args[0] not in self._GENERAL_COMMANDS:
                 device = args.parse_device()
                 process = device.popen(*sib_args, capture_output=False)
```

### Comparing `linktools-0.7.8/src/linktools/decorator.py` & `linktools-0.7.9/src/linktools/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,22 @@
 import typing
 
 _T = typing.TypeVar('_T')
 
 
 def singleton(cls: typing.Type[_T]) -> typing.Callable[..., _T]:
     instances = {}
+    lock = threading.RLock()
 
     @functools.wraps(cls)
     def wrapper(*args, **kwargs):
         if cls not in instances:
-            instances[cls] = cls(*args, **kwargs)
+            with lock:
+                if cls not in instances:
+                    instances[cls] = cls(*args, **kwargs)
         return instances[cls]
 
     return wrapper
 
 
 def try_except(errors: typing.Tuple[typing.Type[BaseException]] = (Exception,), default: typing.Any = None):
     def decorator(fn: typing.Callable[..., _T]) -> typing.Callable[..., _T]:
```

### Comparing `linktools-0.7.8/src/linktools/frida/__init__.py` & `linktools-0.7.9/src/linktools/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/frida/android.py` & `linktools-0.7.9/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/frida/app.py` & `linktools-0.7.9/src/linktools/frida/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import _frida
 import frida
 from frida.core import Session, Script
 
 from .script import FridaUserScript, FridaEvalCode, FridaScriptFile
 from .server import FridaServer
-from .utils import Counter
+from ._utils import Counter
 from .. import utils, resource, get_logger, environ
 
 _logger = get_logger("frida.app")
 
 
 class FridaSession(utils.get_derived_type(Session)):  # proxy for frida.core.Session
 
@@ -71,25 +71,33 @@
             else f"Session(pid={self.pid})"
 
     __str__ = __repr__
 
 
 class FridaScript(utils.get_derived_type(Script)):  # proxy for frida.core.Script
 
+    __super__: Script
+
     def __init__(self, session: FridaSession, script: Script):
         super().__init__(script)
         self._session: FridaSession = session
         self._message_handler = None
         self._destroyed_handler = None
         self._session.append(self)
 
     @property
     def session(self) -> FridaSession:
         return self._session
 
+    @property
+    def exports_sync(self):
+        if hasattr(self.__super__, "exports_sync"):
+            return self.__super__.exports_sync
+        return self.__super__.exports
+
     def add_message_handler(self, handler: "FridaScriptHandler"):
         self.remove_message_handler()
         self._message_handler = lambda msg, data: handler.on_script_message(self, msg, data)
         self.on("message", self._message_handler)
 
     def remove_message_handler(self):
         if self._message_handler is not None:
@@ -422,23 +430,23 @@
 
         # read the internal script as an entrance
         source = self._internal_debug_script.source \
             if environ.debug \
             else self._internal_script.source
 
         script_kwargs = {}
-        if utils.split_version(frida.__version__) < (14,):
+        if utils.parse_version(frida.__version__) < (14,):
             script_kwargs["runtime"] = "v8"
         script = FridaScript(session, session.create_script(source, **script_kwargs))
         script.add_message_handler(self)
         script.add_destroyed_handler(self)
 
         try:
             script.load()
-            script.exports.load_scripts(self._load_script_files(), self._user_parameters)
+            script.exports_sync.load_scripts(self._load_script_files(), self._user_parameters)
         finally:
             if resume:
                 utils.ignore_error(self.device.resume, pid)
 
         self._reactor.schedule(lambda: self.on_script_loaded(script))
 
     def _attach_session(self, pid: int):
```

### Comparing `linktools-0.7.8/src/linktools/frida/ios.py` & `linktools-0.7.9/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/frida/script.py` & `linktools-0.7.9/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/frida/server.py` & `linktools-0.7.9/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/frida/utils.py` & `linktools-0.7.9/src/linktools/frida/_utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/ida/__init__.py` & `linktools-0.7.9/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/ida/ida.py` & `linktools-0.7.9/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/ios/ipa.py` & `linktools-0.7.9/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/ios/sib.py` & `linktools-0.7.9/src/linktools/ios/sib.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
 
         for i in range(10):
             if process.poll() is not None:
                 break
-            out, err = process.run(timeout=1, log_stderr=True)
+            out, err = process.exec(timeout=1, log_stderr=True)
             if out:
                 if isinstance(out, bytes):
                     out = out.decode(errors="ignore")
                 if "Listen on:" in out:
                     time.sleep(.1)
                     _logger.debug(f"Capture sib proxy process output: {out.rstrip()}")
                     break
```

### Comparing `linktools-0.7.8/src/linktools/references/fake_useragent/fake.py` & `linktools-0.7.9/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/references/fake_useragent/settings.py` & `linktools-0.7.9/src/linktools/references/fake_useragent/settings.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/references/fake_useragent/utils.py` & `linktools-0.7.9/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/utils/__init__.py` & `linktools-0.7.9/src/linktools/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Timeout, InterruptableEvent, ignore_error,
     cast, int, bool,
     is_contain, is_empty,
     get_item, pop_item, get_list_item,
     get_md5, get_sha1, get_sha256, make_uuid, gzip_compress,
     read_file, write_file,
     get_lan_ip, get_wan_ip,
-    split_version,
+    parse_version,
     range_type,
 )
 
 from ._proxy import (
     get_derived_type, lazy_load, lazy_raise,
 )
```

### Comparing `linktools-0.7.8/src/linktools/utils/_asyncio.py` & `linktools-0.7.9/src/linktools/utils/_asyncio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import asyncio
+import atexit
 import threading
 from typing import Optional, Callable, Any, Coroutine
 
 from .._logging import get_logger
+from ..decorator import singleton
 
 _logger = get_logger("utils.asyncio")
 
-event_loop_thread: Optional["EventLoopThread"] = None
-event_loop_thread_lock = threading.RLock()
-
 
+@singleton
 class EventLoopThread(threading.Thread):
 
     def __init__(self):
-        super().__init__()
+
+        def run():
+            self._loop = asyncio.new_event_loop()
+            event.set()
+            self._loop.run_forever()
+
+        super().__init__(target=run)
+
+        event = threading.Event()
         self.daemon = True
         self._loop: Optional[asyncio.AbstractEventLoop] = None
-        self._event = threading.Event()
-
-    def run(self):
-        loop = self._loop = asyncio.new_event_loop()
-        self._event.set()
-        loop.run_forever()
+        self.start()
+        event.wait()
+        atexit.register(self.stop)
 
     def stop(self):
         loop = self.get_event_loop()
         loop.call_soon_threadsafe(lambda: loop.stop())
 
     def call_soon(self, callback: Callable[..., Any]):
         loop = self.get_event_loop()
         return loop.call_soon_threadsafe(callback)
 
     def call_task_soon(self, coro: Coroutine):
         loop = self.get_event_loop()
         return loop.call_soon_threadsafe(lambda: loop.create_task(coro))
 
     def get_event_loop(self) -> asyncio.AbstractEventLoop:
-        if self._loop is None:
-            self._event.wait()
-        assert self._loop is not None
         return self._loop
 
 
 def get_event_loop_thread():
-    global event_loop_thread
-    global event_loop_thread_lock
-    if event_loop_thread is None:
-        with event_loop_thread_lock:
-            if event_loop_thread is None:
-                event_loop_thread = EventLoopThread()
-                event_loop_thread.start()
-    return event_loop_thread
+    return EventLoopThread()
```

### Comparing `linktools-0.7.8/src/linktools/utils/_port.py` & `linktools-0.7.9/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/utils/_proxy.py` & `linktools-0.7.9/src/linktools/utils/_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Datetime  : 2022/11/4 下午1:18
 # Author    : HuJi <jihu.hj@alibaba-inc.com>
 
 import functools
 from typing import TypeVar, Type, Callable
 
 
-# Code stolen from celery.local.Proxy.
+# Code stolen from celery.local.Proxy: https://github.com/celery/celery/blob/main/celery/local.py
 
 def _default_cls_attr(name, type_, cls_value):
     # Proxy uses properties to forward the standard
     # class attributes __module__, __name__ and __doc__ to the real
     # object, but these needs to be a string when accessed from
     # the Proxy class directly.  This is a hack to make that work.
     # -- See Issue #1087.
@@ -39,15 +39,15 @@
     __slots__ = ('__fn', '__object', '__dict__')
     __missing__ = object()
 
     def __init__(self, fn=None, obj=None, name=None, __doc__=None):
         if fn is None and obj is None:
             raise ValueError('fn and obj arguments may not be "None" at the same time')
         elif fn is not None and obj is not None:
-            raise ValueError('fn and obj arguments may not be specified at the same tim')
+            raise ValueError('fn and obj arguments may not be specified at the same time')
         object.__setattr__(self, "_Proxy__fn", fn or self.__missing__)
         object.__setattr__(self, "_Proxy__object", obj or self.__missing__)
         if name is not None:
             object.__setattr__(self, "__custom_name__", name)
         if __doc__ is not None:
             object.__setattr__(self, "__doc__", __doc__)
 
@@ -270,23 +270,23 @@
 
 def get_derived_type(t: Type[_T]) -> Type[_T]:
     """
     生成委托类型，常用于自定义类继承委托类，替换某些方法, 如：
 
     import subprocess
 
-    class Wrapper(get_derived_type(subprocess.Popen)):
+    class Popen(get_derived_type(subprocess.Popen)):
         __super__: subprocess.Popen
 
         def communicate(self, *args, **kwargs):
             out, err = self.__super__.communicate(*args, **kwargs)
-            return out, 'fake error!!!'
+            return 'fake out!!!', 'fake error!!!'
 
-    popen = Wrapper(subprocess.Popen(["/usr/bin/git", "status"]))
-    print(popen.communicate())  # (None, 'fake error!!!')
+    process = Popen(subprocess.Popen(["/usr/bin/git", "status"]))
+    print(process.communicate())  # ('fake out!!!', 'fake error!!!')
 
     :param t: 需要委托的类型
     :return: 同参数t，需要委托的类型
     """
 
     class Derived(_Proxy):
```

### Comparing `linktools-0.7.8/src/linktools/utils/_reactor.py` & `linktools-0.7.9/src/linktools/utils/_reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/utils/_ssh.py` & `linktools-0.7.9/src/linktools/utils/_ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools/utils/_subprocess.py` & `linktools-0.7.9/src/linktools/utils/_subprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,22 @@
             self._stderr_thread = threading.Thread(
                 target=self._iter_lines,
                 args=(stderr, self.STDERR, self._stderr_finished,)
             )
             self._stderr_thread.daemon = True
             self._stderr_thread.start()
 
+    @property
+    def is_alive(self):
+        if self._stdout_finished and not self._stdout_finished.is_set():
+            return True
+        if self._stderr_finished and not self._stderr_finished.is_set():
+            return True
+        return False
+
     def _iter_lines(self, io: IO[AnyStr], flag: int, event: threading.Event):
         try:
             while True:
                 data = io.readline()
                 if not data:
                     break
                 self._queue.put((flag, data))
@@ -56,30 +64,30 @@
             if e.errno != errno.EBADF:
                 _logger.debug(f"Handle output error: {e}")
         finally:
             event.set()
             self._queue.put((None, None))
 
     def get_lines(self, timeout: Timeout):
-        while True:
+        while self.is_alive:
             try:
-                flag, data = self._queue.get(timeout=timeout.remain)
+                # 给个1秒超时时间防止有多个线程消费的时候死锁
+                flag, data = self._queue.get(timeout=min(timeout.remain or 1, 1))
                 if flag is not None:
                     yield flag, data
-                elif self._stdout_finished and not self._stdout_finished.is_set():
-                    pass
-                elif self._stderr_finished and not self._stderr_finished.is_set():
-                    pass
-                else:
-                    # 线程都结束了，需要把剩余的数据都消费完
-                    while not self._queue.empty():
-                        flag, data = self._queue.get_nowait()
-                        if flag is not None:
-                            yield flag, data
+            except queue.Empty:
+                if not timeout.check():
                     break
+
+        while True:
+            try:
+                # 需要把剩余可消费的数据消费完
+                flag, data = self._queue.get_nowait()
+                if flag is not None:
+                    yield flag, data
             except queue.Empty:
                 break
 
 
 class Popen(subprocess.Popen):
 
     def __init__(self, *args, **kwargs):
@@ -98,15 +106,15 @@
         if "append_env" in kwargs:
             env = os.environ.copy()
             env.update(kwargs.pop("env", {}))
             env.update(kwargs.pop("append_env"))
             kwargs["env"] = env
 
         args = [str(arg) for arg in args]
-        _logger.debug(f"Exec cmdline: {' '.join(args)}")
+        _logger.debug(f"Exec cmdline: {list2cmdline(args)}")
 
         super().__init__(args, **kwargs)
 
     def call(self, timeout: Union[float, Timeout] = None) -> int:
         with self:
             try:
                 return self.wait(
@@ -133,27 +141,24 @@
                 if retcode:
                     raise subprocess.CalledProcessError(retcode, self.args)
                 return retcode
             except:
                 self.kill()
                 raise
 
-    def run(self, timeout: Union[float, Timeout] = None, log_stdout: bool = False, log_stderr: bool = False) \
+    def exec(self, timeout: Union[float, Timeout] = None, log_stdout: bool = False, log_stderr: bool = False) \
             -> Tuple[Optional[AnyStr], Optional[AnyStr]]:
         """
         执行命令
         :param timeout: 超时时间
         :param log_stdout: 把输出打印到logger中
         :param log_stderr: 把输出打印到logger中
         :return: 返回stdout输出内容
         """
 
-        if self.poll() is not None:
-            return None, None
-
         out = err = None
 
         if not isinstance(timeout, Timeout):
             timeout = Timeout(timeout)
 
         if self.stdout or self.stderr:
```

### Comparing `linktools-0.7.8/src/linktools/utils/_url.py` & `linktools-0.7.9/src/linktools/utils/_url.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,40 +34,45 @@
 import shelve
 import shutil
 from typing import Dict, Union, List, Tuple
 from urllib import parse
 
 from filelock import FileLock
 
-from ._utils import Timeout, get_md5, ignore_error, split_version
+from ._utils import Timeout, get_md5, ignore_error, parse_version
 from .._environ import resource, config, tools
 from .._logging import get_logger, create_log_progress
-from ..decorator import cached_property
+from ..decorator import cached_property, singleton
+from ..references.fake_useragent import UserAgent, VERSION as FAKE_USERAGENT_VERSION
 
 _logger = get_logger("utils.url")
-_user_agent = None
 
 DataType = Union[str, int, float]
 QueryType = Union[DataType, List[DataType], Tuple[DataType]]
 
 
+@singleton
+class _UserAgent(UserAgent):
+
+    def __init__(self):
+        super().__init__(
+            path=resource.get_asset_path(f"fake_useragent_{FAKE_USERAGENT_VERSION}.json")
+        )
+
+
 def user_agent(style=None) -> str:
     try:
-        from ..references.fake_useragent import UserAgent, VERSION
 
-        global _user_agent
-        if (not _user_agent) and style:
-            _user_agent = UserAgent(
-                path=resource.get_asset_path(f"fake_useragent_{VERSION}.json")
-            )
+        user_agent = _UserAgent()
 
         if style:
-            return _user_agent[style]
+            print(user_agent[style])
+            return user_agent[style]
 
-        return _user_agent.random
+        return user_agent.random
 
     except Exception as e:
         _logger.debug(f"fetch user agent error: {e}")
 
     return config["SETTING_DOWNLOAD_USER_AGENT"]
 
 
@@ -148,15 +153,14 @@
             initial = size
 
         self.headers = {
             "User-Agent": self.user_agent,
             "Range": f"bytes={initial}-",
         }
 
-
         try:
             import requests
             fn = self._download_with_requests
         except ModuleNotFoundError:
             fn = self._download_with_urllib
 
         with create_log_progress() as progress:
@@ -343,22 +347,22 @@
     pass
 
 
 def get_chrome_driver(version: str):
     chrome_driver = tools["chromedriver80"]
     base_url = chrome_driver.config.get("base_url")
 
-    versions = split_version(version)
+    versions = parse_version(version)
     if versions[0] >= 70:
         file = UrlFile(f"{base_url}/LATEST_RELEASE_{versions[0]}")
         with open(file.save(), "rt") as fd:
             return chrome_driver.copy(version=fd.read())
 
     path = resource.get_asset_path("chrome-driver.json")
     with open(path, "rt") as fd:
         version_map = json.load(fd)
 
     for key, value in version_map.items():
-        if versions[0] == split_version(value)[0]:
+        if versions[0] == parse_version(value)[0]:
             return chrome_driver.copy(version=key)
 
     raise NotFoundError(version)
```

### Comparing `linktools-0.7.8/src/linktools/utils/_utils.py` & `linktools-0.7.9/src/linktools/utils/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import gzip
 import hashlib
 import random
+import re
 import socket
 import threading
 import time
 import uuid
 from collections.abc import Iterable, Sized
 from typing import Union, Callable, Optional, Type, Any, List, TypeVar
 from urllib.request import urlopen
@@ -64,14 +65,18 @@
 
     def check(self) -> "bool":
         if self._deadline is not None:
             if time.time() > self._deadline:
                 return False
         return True
 
+    def ensure(self) -> None:
+        if not self.check():
+            raise TimeoutError()
+
     def __repr__(self):
         return f"Timeout(timeout={self._timeout})"
 
 
 class InterruptableEvent(threading.Event):
     """
     解决 Windows 上 event.wait 不支持 ctrl+c 中断的问题
@@ -333,16 +338,25 @@
     try:
         with urlopen("http://ifconfig.me/ip") as response:
             return response.read().decode().strip()
     except:
         return None
 
 
-def split_version(version: str) -> [int, ...]:
-    return tuple(int(i, 0) for i in version.split("."))
+def parse_version(version: str) -> [int, ...]:
+    result = []
+    for x in version.split("."):
+        if x.isdigit():
+            result.append(int(x))
+        else:
+            match = re.match(r"^\d+", x)
+            if not match:
+                break
+            result.append(int(match.group(0)))
+    return tuple(result)
 
 
 def range_type(min: int, max: int):
     def wrapper(o):
         value = int(o)
         if min <= value <= max:
             return value
```

### Comparing `linktools-0.7.8/src/linktools/version.py` & `linktools-0.7.9/src/linktools/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,16 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-__version__ = "0.7.8"
-if not __version__.startswith("__"):
-    prefix = "v"
-    if __version__.startswith(prefix):
-        __version__ = __version__[len(prefix):]
-else:
+__version__ = "0.7.9"
+if not __version__[:1].isdigit():
     __version__ = "0.0.1-debug"
 
 __name__ = "linktools"
 __author__ = "Hu Ji"
 __email__ = "669898595@qq.com"
 __url__ = "https://github.com/ice-black-tea/Zelda/tree/master"
 __summary__ = f"{__name__} toolkit"
```

### Comparing `linktools-0.7.8/src/linktools.egg-info/PKG-INFO` & `linktools-0.7.9/src/linktools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.7.8
+Version: 0.7.9
 Summary: linktools toolkit
 Home-page: https://github.com/ice-black-tea/Zelda/tree/master
 Author: Hu Ji
 Author-email: 669898595@qq.com
 License: Apache 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `linktools-0.7.8/src/linktools.egg-info/SOURCES.txt` & `linktools-0.7.9/src/linktools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,25 +48,24 @@
 src/linktools/cli/commands/ios/frida.py
 src/linktools/cli/commands/ios/objection.py
 src/linktools/cli/commands/ios/scp.py
 src/linktools/cli/commands/ios/sib.py
 src/linktools/cli/commands/ios/ssh.py
 src/linktools/frida/__init__.py
 src/linktools/frida/__main__.py
+src/linktools/frida/_utils.py
 src/linktools/frida/android.py
 src/linktools/frida/app.py
 src/linktools/frida/ios.py
 src/linktools/frida/script.py
 src/linktools/frida/server.py
-src/linktools/frida/utils.py
 src/linktools/ida/__init__.py
 src/linktools/ida/ida.py
 src/linktools/ios/__init__.py
 src/linktools/ios/__main__.py
-src/linktools/ios/device.py
 src/linktools/ios/ipa.py
 src/linktools/ios/sib.py
 src/linktools/references/__init__.py
 src/linktools/references/fake_useragent/__init__.py
 src/linktools/references/fake_useragent/errors.py
 src/linktools/references/fake_useragent/fake.py
 src/linktools/references/fake_useragent/log.py
```

### Comparing `linktools-0.7.8/src/linktools.egg-info/entry_points.txt` & `linktools-0.7.9/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.7.8/src/linktools.egg-info/requires.txt` & `linktools-0.7.9/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

