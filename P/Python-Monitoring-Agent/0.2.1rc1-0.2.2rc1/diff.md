# Comparing `tmp/Python Monitoring Agent-0.2.1rc1.tar.gz` & `tmp/Python Monitoring Agent-0.2.2rc1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python Monitoring Agent-0.2.1rc1.tar", last modified: Sat Jun 17 22:23:14 2023, max compression
+gzip compressed data, was "Python Monitoring Agent-0.2.2rc1.linux-x86_64.tar", last modified: Sat Jun 17 22:25:42 2023, max compression
```

## Comparing `Python Monitoring Agent-0.2.1rc1.tar` & `Python Monitoring Agent-0.2.2rc1.linux-x86_64.tar`

### file list

```diff
@@ -1,25 +1,42 @@
-drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:23:14.659502 Python Monitoring Agent-0.2.1rc1/
--rw-r--r--   0 szymon    (1337) szymon    (1337)    18092 2023-05-09 16:33:54.000000 Python Monitoring Agent-0.2.1rc1/LICENSE
--rw-r--r--   0 szymon    (1337) szymon    (1337)     7188 2023-06-17 22:23:14.659502 Python Monitoring Agent-0.2.1rc1/PKG-INFO
-drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:23:14.658502 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/
--rw-r--r--   0 szymon    (1337) szymon    (1337)     7188 2023-06-17 22:23:14.000000 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/PKG-INFO
--rw-r--r--   0 szymon    (1337) szymon    (1337)      475 2023-06-17 22:23:14.000000 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/SOURCES.txt
--rw-r--r--   0 szymon    (1337) szymon    (1337)        1 2023-06-17 22:23:14.000000 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/dependency_links.txt
--rw-r--r--   0 szymon    (1337) szymon    (1337)       40 2023-06-17 22:23:14.000000 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/entry_points.txt
--rw-r--r--   0 szymon    (1337) szymon    (1337)       71 2023-06-17 22:23:14.000000 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/requires.txt
--rw-r--r--   0 szymon    (1337) szymon    (1337)        4 2023-06-17 22:23:14.000000 Python Monitoring Agent-0.2.1rc1/Python_Monitoring_Agent.egg-info/top_level.txt
--rw-r--r--   0 szymon    (1337) szymon    (1337)     6842 2023-05-30 11:17:22.000000 Python Monitoring Agent-0.2.1rc1/README.md
-drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:23:14.659502 Python Monitoring Agent-0.2.1rc1/app/
--rw-r--r--   0 szymon    (1337) szymon    (1337)       84 2023-05-09 16:33:54.000000 Python Monitoring Agent-0.2.1rc1/app/__init__.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     5826 2023-06-16 17:26:11.000000 Python Monitoring Agent-0.2.1rc1/app/config.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     3230 2023-05-09 16:33:54.000000 Python Monitoring Agent-0.2.1rc1/app/cpu.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     2178 2023-05-30 11:17:22.000000 Python Monitoring Agent-0.2.1rc1/app/disks.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     7347 2023-06-17 10:28:43.000000 Python Monitoring Agent-0.2.1rc1/app/docker.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     7235 2023-06-17 15:58:09.000000 Python Monitoring Agent-0.2.1rc1/app/influx_writer.py
--rwxr-xr-x   0 szymon    (1337) szymon    (1337)      494 2023-06-17 15:56:03.000000 Python Monitoring Agent-0.2.1rc1/app/main.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     2402 2023-05-09 16:33:54.000000 Python Monitoring Agent-0.2.1rc1/app/memory.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)      615 2023-06-16 17:26:11.000000 Python Monitoring Agent-0.2.1rc1/app/metrics.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)     2704 2023-05-09 16:33:54.000000 Python Monitoring Agent-0.2.1rc1/app/net_interfaces.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)      136 2023-05-09 16:33:54.000000 Python Monitoring Agent-0.2.1rc1/app/start.py
--rw-r--r--   0 szymon    (1337) szymon    (1337)       38 2023-06-17 22:23:14.659502 Python Monitoring Agent-0.2.1rc1/setup.cfg
--rw-r--r--   0 szymon    (1337) szymon    (1337)      805 2023-06-17 22:23:12.000000 Python Monitoring Agent-0.2.1rc1/setup.py
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./home/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./home/szymon/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./home/szymon/PycharmProjects/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./home/szymon/PycharmProjects/python-monitoring-agent/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.768245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.768245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/bin/
+-rwxr-xr-x   0 szymon    (1337) szymon    (1337)     1060 2023-06-17 22:25:42.768245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/bin/pma
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.739245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.753245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.754245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     7188 2023-06-17 22:25:42.751245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 szymon    (1337) szymon    (1337)      475 2023-06-17 22:25:42.753245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 szymon    (1337) szymon    (1337)        1 2023-06-17 22:25:42.751245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 szymon    (1337) szymon    (1337)       40 2023-06-17 22:25:42.751245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/entry_points.txt
+-rw-r--r--   0 szymon    (1337) szymon    (1337)       71 2023-06-17 22:25:42.751245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/requires.txt
+-rw-r--r--   0 szymon    (1337) szymon    (1337)        4 2023-06-17 22:25:42.751245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/top_level.txt
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.740245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/
+-rw-r--r--   0 szymon    (1337) szymon    (1337)       84 2023-05-09 16:33:54.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__init__.py
+drwxr-xr-x   0 szymon    (1337) szymon    (1337)        0 2023-06-17 22:25:42.744245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/
+-rw-r--r--   0 szymon    (1337) szymon    (1337)      480 2023-06-17 22:25:42.740245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     8495 2023-06-17 22:25:42.742245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     6628 2023-06-17 22:25:42.740245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     3786 2023-06-17 22:25:42.742245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/disks.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)    12100 2023-06-17 22:25:42.743245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/docker.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     8211 2023-06-17 22:25:42.744245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/influx_writer.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     1167 2023-06-17 22:25:42.741245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     4607 2023-06-17 22:25:42.741245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/memory.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     1113 2023-06-17 22:25:42.744245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     4034 2023-06-17 22:25:42.741245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/net_interfaces.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)      569 2023-06-17 22:25:42.741245 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/__pycache__/start.cpython-311.pyc
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     5826 2023-06-16 17:26:11.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/config.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     3230 2023-05-09 16:33:54.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/cpu.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     2178 2023-05-30 11:17:22.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/disks.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     7347 2023-06-17 10:28:43.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/docker.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     7235 2023-06-17 15:58:09.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/influx_writer.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)      494 2023-06-17 15:56:03.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/main.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     2402 2023-05-09 16:33:54.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/memory.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)      615 2023-06-16 17:26:11.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/metrics.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)     2704 2023-05-09 16:33:54.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/net_interfaces.py
+-rw-r--r--   0 szymon    (1337) szymon    (1337)      136 2023-05-09 16:33:54.000000 ./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/start.py
```

### Comparing `Python Monitoring Agent-0.2.1rc1/PKG-INFO` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/Python_Monitoring_Agent-0.2.2rc1-py3.11.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Python Monitoring Agent
-Version: 0.2.1rc1
+Name: Python-Monitoring-Agent
+Version: 0.2.2rc1
 Summary: Simple, os independent monitoring agent
 Home-page: https://github.com/SzymonRysztof/python-monitoring-agent/
 Author: Szymon Rysztof
 Platform: Linux
 Platform: Windows
 Platform: Unix
 Requires-Python: >=3.6
```

### Comparing `Python Monitoring Agent-0.2.1rc1/app/config.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/config.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/cpu.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/cpu.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/disks.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/disks.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/docker.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/docker.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/influx_writer.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/influx_writer.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/memory.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/memory.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/metrics.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/metrics.py`

 * *Files identical despite different names*

### Comparing `Python Monitoring Agent-0.2.1rc1/app/net_interfaces.py` & `./home/szymon/PycharmProjects/python-monitoring-agent/venv/lib/python3.11/site-packages/app/net_interfaces.py`

 * *Files identical despite different names*

