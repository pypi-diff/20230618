# Comparing `tmp/certipy-ad-4.4.0.tar.gz` & `tmp/certipy-ad-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certipy-ad-4.4.0.tar", last modified: Thu Mar 23 00:12:13 2023, max compression
+gzip compressed data, was "certipy-ad-4.5.0.tar", last modified: Sun Jun 18 12:52:52 2023, max compression
```

## Comparing `certipy-ad-4.4.0.tar` & `certipy-ad-4.5.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.922864 certipy-ad-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-03-23 00:12:13.922864 certipy-ad-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40570 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.918864 certipy-ad-4.4.0/certipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.918864 certipy-ad-4.4.0/certipy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8712 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22216 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34330 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/cert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41865 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7021 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/forge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.918864 certipy-ad-4.4.0/certipy/commands/parsers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/cert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2590 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/find.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/forge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/ptt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2777 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3255 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/req.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/shadow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/target.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/parsers/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/ptt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15672 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24976 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/req.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/shadow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8468 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/commands/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.922864 certipy-ad-4.4.0/certipy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25989 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/certificate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17570 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/errors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/kerberos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14309 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/ldap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10623 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/pkinit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5138 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.922864 certipy-ad-4.4.0/certipy/lib/sspi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/sspi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32016 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/sspi/encryption.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/sspi/kerberos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    52996 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/sspi/netsecapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37531 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/structs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10790 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/lib/target.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      396 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/certipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 00:12:13.922864 certipy-ad-4.4.0/certipy_ad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-03-23 00:12:13.000000 certipy-ad-4.4.0/certipy_ad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-23 00:12:13.000000 certipy-ad-4.4.0/certipy_ad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 00:12:13.000000 certipy-ad-4.4.0/certipy_ad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-23 00:12:13.000000 certipy-ad-4.4.0/certipy_ad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-23 00:12:13.000000 certipy-ad-4.4.0/certipy_ad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 00:12:13.000000 certipy-ad-4.4.0/certipy_ad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 00:12:13.922864 certipy-ad-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-23 00:12:04.000000 certipy-ad-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40570 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.929927 certipy-ad-4.5.0/certipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.929927 certipy-ad-4.5.0/certipy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8712 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22273 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34330 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2408 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/cert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41865 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7949 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/forge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.933927 certipy-ad-4.5.0/certipy/commands/parsers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      224 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/cert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2590 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/find.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/forge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      907 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/ptt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3336 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/req.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/shadow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2903 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/target.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/parsers/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/ptt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15754 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25062 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/req.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14281 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/shadow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8468 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/commands/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1659 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.933927 certipy-ad-4.5.0/certipy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27227 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/certificate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17569 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2382 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/kerberos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14144 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/ldap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10623 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/pkinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5138 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2015 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.933927 certipy-ad-4.5.0/certipy/lib/sspi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32016 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/encryption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/kerberos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52996 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/sspi/netsecapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37531 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/structs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10790 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/lib/target.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      396 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/certipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/certipy_ad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40825 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:52:52.000000 certipy-ad-4.5.0/certipy_ad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:52:52.937928 certipy-ad-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-18 12:52:38.000000 certipy-ad-4.5.0/setup.py
```

### Comparing `certipy-ad-4.4.0/LICENSE` & `certipy-ad-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/PKG-INFO` & `certipy-ad-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certipy-ad
-Version: 4.4.0
+Version: 4.5.0
 Summary: Active Directory Certificate Services enumeration and abuse
 Home-page: https://github.com/ly4k/Certipy
 Author: ly4k
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `certipy-ad-4.4.0/README.md` & `certipy-ad-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/account.py` & `certipy-ad-4.5.0/certipy/commands/account.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/auth.py` & `certipy-ad-4.5.0/certipy/commands/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
             ldap_conn = ldap3.Connection(
                 ldap_server,
                 authentication=ldap3.SASL,
                 sasl_mechanism=ldap3.EXTERNAL,
                 sasl_credentials=sasl_credentials,
                 auto_bind=ldap3.AUTO_BIND_TLS_BEFORE_BIND,
                 raise_exceptions=True,
+                receive_timeout=self.target.timeout * 10
             )
         except ldap3.core.exceptions.LDAPUnavailableResult as e:
             logging.error("LDAP not configured for SSL/TLS connections")
             if self.verbose:
                 raise e
             return False
```

### Comparing `certipy-ad-4.4.0/certipy/commands/ca.py` & `certipy-ad-4.5.0/certipy/commands/ca.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/cert.py` & `certipy-ad-4.5.0/certipy/commands/cert.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/find.py` & `certipy-ad-4.5.0/certipy/commands/find.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/forge.py` & `certipy-ad-4.5.0/certipy/commands/forge.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import argparse
 import datetime
 from typing import Callable, Tuple
 
 from certipy.lib.certificate import (
     PRINCIPAL_NAME,
-    NameOID,
     UTF8String,
     cert_id_to_parts,
     create_pfx,
     encoder,
     generate_rsa_key,
     get_subject_from_str,
     load_pfx,
     x509,
+    asn1x509,
+    NTDS_CA_SECURITY_EXT,
+    szOID_NTDS_OBJECTSID
 )
 from certipy.lib.logger import logging
 
 
 class Forge:
     def __init__(
         self,
         ca_pfx: str = None,
         upn: str = None,
         dns: str = None,
+        sid: str = None,
         template: str = None,
         subject: str = None,
         issuer: str = None,
         crl: str = None,
         serial: str = None,
         key_size: int = 2048,
         out: str = None,
         **kwargs
     ):
         self.ca_pfx = ca_pfx
         self.alt_upn = upn
         self.alt_dns = dns
+        self.alt_sid = sid
         self.template = template
         self.subject = subject
         self.issuer = issuer
         self.crl = crl
         self.serial = serial
         self.key_size = key_size
         self.out = out
@@ -196,14 +200,38 @@
             sans.append(x509.OtherName(PRINCIPAL_NAME, alt_upn))
 
         cert = cert.add_extension(
             x509.SubjectAlternativeName(sans),
             False,
         )
 
+        alt_sid = self.alt_sid
+        if alt_sid:
+            if type(alt_sid) == str:
+                alt_sid = alt_sid.encode()
+
+            sid_extension = asn1x509.GeneralNames([asn1x509.GeneralName(
+                    {
+                        "other_name": asn1x509.AnotherName(
+                            {
+                                "type_id": szOID_NTDS_OBJECTSID,
+                                "value": asn1x509.OctetString(alt_sid).retag(
+                                    {"explicit": 0}
+                                ),
+                            }
+                        )
+                    }
+                )]
+            )
+
+            cert = cert.add_extension(
+                x509.UnrecognizedExtension(NTDS_CA_SECURITY_EXT, sid_extension.dump()),
+                False,
+            )
+
         cert = cert.sign(ca_key, signature_hash_algorithm())
 
         pfx = create_pfx(key, cert)
 
         out = self.out
         if not out:
             out, _ = cert_id_to_parts([(id_type, id_value)])
```

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/account.py` & `certipy-ad-4.5.0/certipy/commands/parsers/account.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/auth.py` & `certipy-ad-4.5.0/certipy/commands/parsers/auth.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/ca.py` & `certipy-ad-4.5.0/certipy/commands/parsers/ca.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/cert.py` & `certipy-ad-4.5.0/certipy/commands/parsers/cert.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/find.py` & `certipy-ad-4.5.0/certipy/commands/parsers/find.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/forge.py` & `certipy-ad-4.5.0/certipy/commands/parsers/forge.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         action="store",
         metavar="pfx/p12 file name",
         help="Path to CA certificate",
         required=True,
     )
     subparser.add_argument("-upn", action="store", metavar="alternative UPN")
     subparser.add_argument("-dns", action="store", metavar="alternative DNS")
+    subparser.add_argument("-sid", action="store", metavar="alternative Object SID")
     subparser.add_argument(
         "-template",
         action="store",
         metavar="pfx/p12 file name",
         help="Path to template certificate",
     )
     subparser.add_argument(
```

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/ptt.py` & `certipy-ad-4.5.0/certipy/commands/parsers/ptt.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/relay.py` & `certipy-ad-4.5.0/certipy/commands/parsers/relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         action="store",
         metavar="template name",
         help="If omitted, the template 'Machine' or 'User' is chosen by default depending on whether the relayed account name ends with '$'. Relaying a DC should require specifying the 'DomainController' template",
     )
 
     group.add_argument("-upn", action="store", metavar="alternative UPN")
     group.add_argument("-dns", action="store", metavar="alternative DNS")
+    group.add_argument("-sid", action="store", metavar="alternative Object SID")
     group.add_argument(
         "-retrieve",
         action="store",
         metavar="request ID",
         help="Retrieve an issued certificate specified by a request ID instead of requesting a new certificate",
         default=0,
         type=int,
```

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/req.py` & `certipy-ad-4.5.0/certipy/commands/parsers/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     group = subparser.add_argument_group("certificate request options")
     group.add_argument(
         "-template", action="store", metavar="template name", default="User"
     )
     group.add_argument("-upn", action="store", metavar="alternative UPN")
     group.add_argument("-dns", action="store", metavar="alternative DNS")
+    group.add_argument("-sid", action="store", metavar="alternative Object SID")
     group.add_argument(
         "-subject",
         action="store",
         metavar="subject",
         help="Subject to include certificate, e.g. CN=Administrator,CN=Users,DC=CORP,DC=LOCAL",
     )
     group.add_argument(
```

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/shadow.py` & `certipy-ad-4.5.0/certipy/commands/parsers/shadow.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/target.py` & `certipy-ad-4.5.0/certipy/commands/parsers/target.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/parsers/template.py` & `certipy-ad-4.5.0/certipy/commands/parsers/template.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/ptt.py` & `certipy-ad-4.5.0/certipy/commands/ptt.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/relay.py` & `certipy-ad-4.5.0/certipy/commands/relay.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         if template is None:
             template = "Machine" if self.username.endswith("$") else "User"
 
         csr, key = create_csr(
             self.username,
             alt_dns=self.adcs_relay.dns,
             alt_upn=self.adcs_relay.upn,
+            alt_sid=self.adcs_relay.sid,
             key_size=self.adcs_relay.key_size,
         )
 
         csr = csr_to_pem(csr).decode()
 
         attributes = ["CertificateTemplate:%s" % template]
 
@@ -370,14 +371,15 @@
 class Relay:
     def __init__(
         self,
         ca,
         template=None,
         upn=None,
         dns=None,
+        sid=None,
         retrieve=None,
         key_size: int = 2048,
         out=None,
         interface="0.0.0.0",
         port=445,
         forever=False,
         no_skip=False,
@@ -385,14 +387,15 @@
         debug=False,
         **kwargs
     ):
         self.ca = ca
         self.template = template
         self.upn = upn
         self.dns = dns
+        self.sid = sid
         self.request_id = int(retrieve)
         self.key_size = key_size
         self.out = out
         self.forever = forever
         self.no_skip = no_skip
         self.timeout = timeout
         self.verbose = debug
```

### Comparing `certipy-ad-4.4.0/certipy/commands/req.py` & `certipy-ad-4.5.0/certipy/commands/req.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,14 +520,15 @@
     def __init__(
         self,
         target: Target = None,
         ca: str = None,
         template: str = None,
         upn: str = None,
         dns: str = None,
+        sid: str = None,
         subject: str = None,
         retrieve: int = 0,
         on_behalf_of: str = None,
         pfx: str = None,
         key_size: int = None,
         archive_key: bool = False,
         renew: bool = False,
@@ -541,14 +542,15 @@
         **kwargs
     ):
         self.target = target
         self.ca = ca
         self.template = template
         self.alt_upn = upn
         self.alt_dns = dns
+        self.alt_sid = sid
         self.subject = subject
         self.request_id = int(retrieve)
         self.on_behalf_of = on_behalf_of
         self.pfx = pfx
         self.key_size = key_size
         self.archive_key = archive_key
         self.renew = renew
@@ -665,14 +667,15 @@
             with open(self.pfx, "rb") as f:
                 renewal_key, renewal_cert = load_pfx(f.read())
 
         csr, key = create_csr(
             username,
             alt_dns=self.alt_dns,
             alt_upn=self.alt_upn,
+            alt_sid=self.alt_sid,
             key=self.key,
             key_size=self.key_size,
             subject=self.subject,
             renewal_cert=renewal_cert,
         )
         self.key = key
```

### Comparing `certipy-ad-4.4.0/certipy/commands/shadow.py` & `certipy-ad-4.5.0/certipy/commands/shadow.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/commands/template.py` & `certipy-ad-4.5.0/certipy/commands/template.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/entry.py` & `certipy-ad-4.5.0/certipy/entry.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/certificate.py` & `certipy-ad-4.5.0/certipy/lib/certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import base64
 import math
 import os
 import struct
 import sys
-from typing import Callable, List, Tuple
+from typing import List, Tuple
 
 from asn1crypto import cms as asn1cms
 from asn1crypto import core as asn1core
 from asn1crypto import csr as asn1csr
 from asn1crypto import x509 as asn1x509
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes, serialization
@@ -46,25 +46,37 @@
     "G": NameOID.GIVEN_NAME,
     "GN": NameOID.GIVEN_NAME,
     "E": NameOID.EMAIL_ADDRESS,
     "UID": NameOID.USER_ID,
     "DC": NameOID.DOMAIN_COMPONENT,
 }
 
-PRINCIPAL_NAME = x509.ObjectIdentifier("1.3.6.1.4.1.311.20.2.3")
+asn1x509.ExtensionId._map.update(
+    {
+        "1.3.6.1.4.1.311.25.2": "security_ext",
+    }
+)
 
-NTDS_CA_SECURITY_EXT = x509.ObjectIdentifier("1.3.6.1.4.1.311.25.2")
+asn1x509.Extension._oid_specs.update(
+    {
+        "security_ext": asn1x509.GeneralNames,
+    }
+)
 
+PRINCIPAL_NAME = x509.ObjectIdentifier("1.3.6.1.4.1.311.20.2.3")
+NTDS_CA_SECURITY_EXT = x509.ObjectIdentifier("1.3.6.1.4.1.311.25.2")
+NTDS_OBJECTSID = x509.ObjectIdentifier("1.3.6.1.4.1.311.25.2.1")
 
 szOID_RENEWAL_CERTIFICATE = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.13.1")
 szOID_ENCRYPTED_KEY_HASH = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.21.21")
 szOID_PRINCIPAL_NAME = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.20.2.3")
 szOID_ENCRYPTED_KEY_HASH = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.21.21")
 szOID_CMC_ADD_ATTRIBUTES = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.10.10.1")
-
+szOID_NTDS_CA_SECURITY_EXT = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.25.2")
+szOID_NTDS_OBJECTSID = asn1cms.ObjectIdentifier("1.3.6.1.4.1.311.25.2.1")
 
 class TaggedCertificationRequest(asn1core.Sequence):
     _fields = [
         ("bodyPartID", asn1core.Integer),
         ("certificationRequest", asn1csr.CertificationRequest),
     ]
 
@@ -313,14 +325,15 @@
     return rsa.generate_private_key(public_exponent=0x10001, key_size=key_size)
 
 
 def create_csr(
     username: str,
     alt_dns: bytes = None,
     alt_upn: bytes = None,
+    alt_sid: bytes = None,
     key: rsa.RSAPrivateKey = None,
     key_size: int = 2048,
     subject: str = None,
     renewal_cert: x509.Certificate = None,
 ) -> Tuple[x509.CertificateSigningRequest, rsa.RSAPrivateKey]:
     if key is None:
         logging.debug("Generating RSA key")
@@ -356,16 +369,14 @@
         general_names = []
 
         if alt_dns:
             if type(alt_dns) == bytes:
                 alt_dns = alt_dns.decode()
             general_names.append(asn1x509.GeneralName({"dns_name": alt_dns}))
 
-        #         sans.append(x509.DNSName(alt_dns))
-
         if alt_upn:
             if type(alt_upn) == bytes:
                 alt_upn = alt_upn.decode()
 
             general_names.append(
                 asn1x509.GeneralName(
                     {
@@ -386,14 +397,42 @@
         )
 
         set_of_extensions = asn1csr.SetOfExtensions([[san_extension]])
 
         cri_attribute = asn1csr.CRIAttribute(
             {"type": "extension_request", "values": set_of_extensions}
         )
+
+        cri_attributes.append(cri_attribute)
+
+    if alt_sid:
+        if type(alt_sid) == str:
+            alt_sid = alt_sid.encode()
+
+
+        san_extension = asn1x509.Extension(
+            {"extn_id": "security_ext", "extn_value": [asn1x509.GeneralName(
+                {
+                    "other_name": asn1x509.AnotherName(
+                        {
+                            "type_id": szOID_NTDS_OBJECTSID,
+                            "value": asn1x509.OctetString(alt_sid).retag(
+                                {"explicit": 0}
+                            ),
+                        }
+                    )
+                }
+            )]}
+        )
+
+        set_of_extensions = asn1csr.SetOfExtensions([[san_extension]])
+
+        cri_attribute = asn1csr.CRIAttribute(
+            {"type": "extension_request", "values": set_of_extensions}
+        )
 
         cri_attributes.append(cri_attribute)
 
     if renewal_cert:
         cri_attributes.append(
             asn1csr.CRIAttribute(
                 {
```

### Comparing `certipy-ad-4.4.0/certipy/lib/constants.py` & `certipy-ad-4.5.0/certipy/lib/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     "1.3.6.1.4.1.311.20.1": "CTL Usage",
     "1.3.6.1.5.5.7.3.9": "OCSP Signing",
     "1.3.6.1.5.5.7.3.3": "Code Signing",
     "1.3.6.1.4.1.311.10.3.1": "Microsoft Trust List Signing",
     "1.3.6.1.4.1.311.10.3.2": "Microsoft Time Stamping",
     "1.3.6.1.4.1.311.76.8.1": "Microsoft Publishe",
     "1.3.6.1.5.5.7.3.2": "Client Authentication",
-    "1.3.6.1.5.2.3.4": "PKIINIT Client Authentication",
+    "1.3.6.1.5.2.3.4": "PKINIT Client Authentication",
     "1.3.6.1.4.1.311.10.3.13": "Lifetime Signing",
     "2.5.29.37.0": "Any Purpose",
     "1.3.6.1.4.1.311.64.1.1": "Server Trust",
     "1.3.6.1.4.1.311.10.3.7": "OEM Windows System Component Verification",
 }
```

### Comparing `certipy-ad-4.4.0/certipy/lib/errors.py` & `certipy-ad-4.5.0/certipy/lib/errors.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/formatting.py` & `certipy-ad-4.5.0/certipy/lib/formatting.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/kerberos.py` & `certipy-ad-4.5.0/certipy/lib/kerberos.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/ldap.py` & `certipy-ad-4.5.0/certipy/lib/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,21 +350,19 @@
         sids |= set(["S-1-1-0", "S-1-5-11", "S-1-5-32-545"])
 
         # Domain Users, Domain Computers, etc.
         primary_group_id = user.get("primaryGroupID")
         if primary_group_id is not None:
             sids.add("%s-%d" % (self.domain_sid, primary_group_id))
 
-        # Add Domain Computers group if Machine Account Quota > 0
-        if self.machine_account_quota > 0:
-            logging.debug(
-                "Adding Domain Computers to list of current user's SIDs (Machine Account Quota: %d > 0)"
-                % self.machine_account_quota
-            )
-            sids.add("%s-515" % self.domain_sid)
+        # Add Domain Computers group
+        logging.debug(
+            "Adding Domain Computers to list of current user's SIDs"
+        )
+        sids.add("%s-515" % self.domain_sid)
 
         dns = [user.get("distinguishedName")]
         for sid in sids:
             object = self.lookup_sid(sid)
             if "dn" in object:
                 dns.append(object["dn"])
```

### Comparing `certipy-ad-4.4.0/certipy/lib/logger.py` & `certipy-ad-4.5.0/certipy/lib/logger.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/pkinit.py` & `certipy-ad-4.5.0/certipy/lib/pkinit.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/rpc.py` & `certipy-ad-4.5.0/certipy/lib/rpc.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/security.py` & `certipy-ad-4.5.0/certipy/lib/security.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/sspi/encryption.py` & `certipy-ad-4.5.0/certipy/lib/sspi/encryption.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/sspi/kerberos.py` & `certipy-ad-4.5.0/certipy/lib/sspi/kerberos.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/sspi/netsecapi.py` & `certipy-ad-4.5.0/certipy/lib/sspi/netsecapi.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/structs.py` & `certipy-ad-4.5.0/certipy/lib/structs.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy/lib/target.py` & `certipy-ad-4.5.0/certipy/lib/target.py`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/certipy_ad.egg-info/PKG-INFO` & `certipy-ad-4.5.0/certipy_ad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certipy-ad
-Version: 4.4.0
+Version: 4.5.0
 Summary: Active Directory Certificate Services enumeration and abuse
 Home-page: https://github.com/ly4k/Certipy
 Author: ly4k
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `certipy-ad-4.4.0/certipy_ad.egg-info/SOURCES.txt` & `certipy-ad-4.5.0/certipy_ad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certipy-ad-4.4.0/setup.py` & `certipy-ad-4.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="certipy-ad",
-    version="4.4.0",
+    version="4.5.0",
     license="MIT",
     author="ly4k",
     url="https://github.com/ly4k/Certipy",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=[
         "asn1crypto",
@@ -20,14 +20,16 @@
         "dnspython",
         "dsinternals",
         "pyopenssl>=22.0.0",
         "requests",
         "requests_ntlm",
         'winacl; platform_system=="Windows"',
         'wmi; platform_system=="Windows"',
+        "pycryptodome",
+        "unicrypto"
     ],
     packages=[
         "certipy",
         "certipy.commands",
         "certipy.commands.parsers",
         "certipy.lib",
         "certipy.lib.sspi",
```

