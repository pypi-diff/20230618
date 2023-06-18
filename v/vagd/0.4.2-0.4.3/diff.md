# Comparing `tmp/vagd-0.4.2.tar.gz` & `tmp/vagd-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-0.4.2.tar", last modified: Sat Jun 17 16:00:05 2023, max compression
+gzip compressed data, was "vagd-0.4.3.tar", last modified: Sun Jun 18 10:25:01 2023, max compression
```

## Comparing `vagd-0.4.2.tar` & `vagd-0.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.883415 vagd-0.4.2/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.2/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2928 2023-06-17 16:00:05.880082 vagd-0.4.2/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2344 2023-06-17 15:28:22.000000 vagd-0.4.2/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-06-17 15:21:56.000000 vagd-0.4.2/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-06-17 16:00:05.883415 vagd-0.4.2/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.873415 vagd-0.4.2/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.876748 vagd-0.4.2/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.2/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.2/src/vagd/box.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.880082 vagd-0.4.2/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.2/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.2/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.2/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.2/src/vagd/helper.py
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      839 2023-06-17 11:43:56.000000 vagd-0.4.2/src/vagd/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1759 2023-06-17 14:59:31.000000 vagd-0.4.2/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.880082 vagd-0.4.2/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5683 2023-06-17 15:38:36.000000 vagd-0.4.2/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10666 2023-06-17 15:51:31.000000 vagd-0.4.2/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10849 2023-06-17 15:49:55.000000 vagd-0.4.2/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.2/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.2/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.876748 vagd-0.4.2/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2928 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-06-17 16:00:05.000000 vagd-0.4.2/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 16:00:05.880082 vagd-0.4.2/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1206 2023-06-17 15:43:05.000000 vagd-0.4.2/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.208426 vagd-0.4.3/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.3/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4389 2023-06-18 10:25:01.208426 vagd-0.4.3/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3805 2023-06-17 16:19:04.000000 vagd-0.4.3/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-06-18 10:24:08.000000 vagd-0.4.3/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-06-18 10:25:01.208426 vagd-0.4.3/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.198426 vagd-0.4.3/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.201759 vagd-0.4.3/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.3/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.3/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.3/src/vagd/box.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.205092 vagd-0.4.3/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.3/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.3/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.3/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.3/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.3/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.3/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.3/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.3/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.3/src/vagd/helper.py
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      839 2023-06-17 11:43:56.000000 vagd-0.4.3/src/vagd/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1325 2023-06-18 10:20:53.000000 vagd-0.4.3/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.205092 vagd-0.4.3/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.3/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5683 2023-06-17 15:38:36.000000 vagd-0.4.3/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10666 2023-06-17 15:51:31.000000 vagd-0.4.3/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10849 2023-06-17 15:49:55.000000 vagd-0.4.3/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.3/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.3/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.3/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.201759 vagd-0.4.3/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4389 2023-06-18 10:25:01.000000 vagd-0.4.3/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-06-18 10:25:01.000000 vagd-0.4.3/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-06-18 10:25:01.000000 vagd-0.4.3/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-06-18 10:25:01.000000 vagd-0.4.3/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-06-18 10:25:01.000000 vagd-0.4.3/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-18 10:25:01.205092 vagd-0.4.3/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1206 2023-06-17 15:43:05.000000 vagd-0.4.3/test/test.py
```

### Comparing `vagd-0.4.2/LICENSE` & `vagd-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/pyproject.toml` & `vagd-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vagd"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="0x6fe1be2", email="author@example.com" },
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['pwntools', 'python-vagrant', 'docker']
```

### Comparing `vagd-0.4.2/src/vagd/box.py` & `vagd-0.4.3/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/gdb/__init__.pyi` & `vagd-0.4.3/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/gdb/events.pyi` & `vagd-0.4.3/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/gdb/printing.pyi` & `vagd-0.4.3/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/gdb/types.pyi` & `vagd-0.4.3/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/gdb/xmethod.pyi` & `vagd-0.4.3/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/helper.py` & `vagd-0.4.3/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/template.txt` & `vagd-0.4.3/src/vagd/template.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/templates.py` & `vagd-0.4.3/src/vagd/templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,33 +43,16 @@
 DOCKER_ALPINE_TEMPLATE = '''FROM {image}
 
 # install packages
 RUN apk update
 # we need make and linux-headers to compile gdb
 RUN apk add python3
 RUN apk add --no-cache musl-dbg
-RUN apk add --no-cache make
-RUN apk add --no-cache linux-headers
-RUN apk add --no-cache texinfo
-RUN apk add --no-cache gcc
-RUN apk add --no-cache g++
-RUN apk add --no-cache gfortran
 # install gdb
-# RUN apk add --no-cache gdb
-RUN mkdir gdb-build ;\
-    cd gdb-build;\
-    wget http://ftp.gnu.org/gnu/gdb/gdb-7.11.tar.xz;\
-    tar -xvf gdb-7.11.tar.xz;\
-    cd gdb-7.11;\
-    ./configure --prefix=/usr;\
-    make;\
-    make -C gdb install;\
-    cd ..;\
-    rm -rf gdb-build/;
-
+RUN apk add --no-cache gdb
 # install ssh server support and keys
 RUN apk add --no-cache openssh
 
 EXPOSE 22
 RUN adduser -h /home/vagd -s /bin/ash -D vagd
 RUN echo "vagd:vagd" | chpasswd
```

#### html2text {}

```diff
@@ -5,18 +5,13 @@
 DOCKER_TEMPLATE = '''FROM {image} # install packages RUN apt-get update && \\
 apt-get install -y {packages} \\ systemctl # init user and ssh EXPOSE 22 RUN
 useradd --create-home --shell /bin/bash {user} USER {user} WORKDIR /home/{user}
 COPY {keyfile} .ssh/authorized_keys USER root RUN mkdir -p /run/sshd && \\
 chmod 755 /run/sshd CMD /usr/sbin/sshd; \\ while true; do sleep 1m; done '''
 DOCKER_ALPINE_TEMPLATE = '''FROM {image} # install packages RUN apk update # we
 need make and linux-headers to compile gdb RUN apk add python3 RUN apk add --
-no-cache musl-dbg RUN apk add --no-cache make RUN apk add --no-cache linux-
-headers RUN apk add --no-cache texinfo RUN apk add --no-cache gcc RUN apk add -
--no-cache g++ RUN apk add --no-cache gfortran # install gdb # RUN apk add --no-
-cache gdb RUN mkdir gdb-build ;\ cd gdb-build;\ wget http://ftp.gnu.org/gnu/
-gdb/gdb-7.11.tar.xz;\ tar -xvf gdb-7.11.tar.xz;\ cd gdb-7.11;\ ./configure --
-prefix=/usr;\ make;\ make -C gdb install;\ cd ..;\ rm -rf gdb-build/; # install
-ssh server support and keys RUN apk add --no-cache openssh EXPOSE 22 RUN
-adduser -h /home/vagd -s /bin/ash -D vagd RUN echo "vagd:vagd" | chpasswd USER
-vagd WORKDIR /home/vagd COPY keyfile.pub .ssh/authorized_keys USER root RUN
-ssh-keygen -A RUN mkdir -p /run/sshd && \ chmod 755 /run/sshd CMD /usr/sbin/
-sshd; \ while true; do sleep 1m; done '''
+no-cache musl-dbg # install gdb RUN apk add --no-cache gdb # install ssh server
+support and keys RUN apk add --no-cache openssh EXPOSE 22 RUN adduser -h /home/
+vagd -s /bin/ash -D vagd RUN echo "vagd:vagd" | chpasswd USER vagd WORKDIR /
+home/vagd COPY keyfile.pub .ssh/authorized_keys USER root RUN ssh-keygen -A RUN
+mkdir -p /run/sshd && \ chmod 755 /run/sshd CMD /usr/sbin/sshd; \ while true;
+do sleep 1m; done '''
```

### Comparing `vagd-0.4.2/src/vagd/virts/dogd.py` & `vagd-0.4.3/src/vagd/virts/dogd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/virts/pwngd.py` & `vagd-0.4.3/src/vagd/virts/pwngd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/virts/qegd.py` & `vagd-0.4.3/src/vagd/virts/qegd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/virts/shgd.py` & `vagd-0.4.3/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/virts/vagd.py` & `vagd-0.4.3/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd/wrapper.py` & `vagd-0.4.3/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/src/vagd.egg-info/SOURCES.txt` & `vagd-0.4.3/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.4.2/test/test.py` & `vagd-0.4.3/test/test.py`

 * *Files identical despite different names*

