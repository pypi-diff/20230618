# Comparing `tmp/eva-shell-0.0.93.tar.gz` & `tmp/eva-shell-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva-shell-0.0.93.tar", last modified: Wed May 31 23:34:47 2023, max compression
+gzip compressed data, was "eva-shell-0.1.0.tar", last modified: Sun Jun 18 19:46:06 2023, max compression
```

## Comparing `eva-shell-0.0.93.tar` & `eva-shell-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.545655 eva-shell-0.0.93/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:07.000000 eva-shell-0.0.93/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-31 23:34:47.545655 eva-shell-0.0.93/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.0.93/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.541655 eva-shell-0.0.93/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.0.93/bin/eva
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.541655 eva-shell-0.0.93/eva4_shell/
--rw-r--r--   0 divisor   (1000) root         (0)       75 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    47371 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/ap.py
--rw-r--r--   0 divisor   (1000) root         (0)     7078 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/charts.py
--rw-r--r--   0 divisor   (1000) root         (0)    51601 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/cli.py
--rw-r--r--   0 divisor   (1000) root         (0)     2634 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/client.py
--rw-r--r--   0 divisor   (1000) root         (0)     4332 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/compl.py
--rw-r--r--   0 divisor   (1000) root         (0)      653 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/sharedobj.py
--rw-r--r--   0 divisor   (1000) root         (0)     1701 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/shell.py
--rw-r--r--   0 divisor   (1000) root         (0)    13863 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/tools.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.541655 eva-shell-0.0.93/eva_shell.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      382 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)      166 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       11 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-31 23:34:47.545655 eva-shell-0.0.93/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1188 2023-05-31 23:34:44.000000 eva-shell-0.0.93/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 19:46:06.960732 eva-shell-0.1.0/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:07.000000 eva-shell-0.1.0/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      458 2023-06-18 19:46:06.960732 eva-shell-0.1.0/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.1.0/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 19:46:06.956732 eva-shell-0.1.0/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.1.0/bin/eva
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 19:46:06.956732 eva-shell-0.1.0/eva4_shell/
+-rw-r--r--   0 divisor   (1000) root         (0)       74 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    47303 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/ap.py
+-rw-r--r--   0 divisor   (1000) root         (0)     7078 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/charts.py
+-rw-r--r--   0 divisor   (1000) root         (0)    51522 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/cli.py
+-rw-r--r--   0 divisor   (1000) root         (0)     2634 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/client.py
+-rw-r--r--   0 divisor   (1000) root         (0)     4332 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/compl.py
+-rw-r--r--   0 divisor   (1000) root         (0)      653 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/sharedobj.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1701 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/shell.py
+-rw-r--r--   0 divisor   (1000) root         (0)    13863 2023-06-18 19:45:56.000000 eva-shell-0.1.0/eva4_shell/tools.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-06-18 19:46:06.960732 eva-shell-0.1.0/eva_shell.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      458 2023-06-18 19:46:06.000000 eva-shell-0.1.0/eva_shell.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      382 2023-06-18 19:46:06.000000 eva-shell-0.1.0/eva_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-06-18 19:46:06.000000 eva-shell-0.1.0/eva_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)      166 2023-06-18 19:46:06.000000 eva-shell-0.1.0/eva_shell.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       11 2023-06-18 19:46:06.000000 eva-shell-0.1.0/eva_shell.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-06-18 19:46:06.960732 eva-shell-0.1.0/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1187 2023-06-18 19:45:56.000000 eva-shell-0.1.0/setup.py
```

### Comparing `eva-shell-0.0.93/LICENSE` & `eva-shell-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/eva4_shell/ap.py` & `eva-shell-0.1.0/eva4_shell/ap.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,15 @@
 def append_action_cli(root_sp):
     ap = root_sp.add_parser('action', help='action commands')
     sp = ap.add_subparsers(dest='_subc', help='sub command')
 
     p = sp.add_parser('exec', help='exec unit action')
     p.add_argument('i', metavar='OID',
                    help='unit OID').completer = ComplOIDtp('unit')
-    p.add_argument('status', metavar='STATUS', type=int)
-    p.add_argument('-v', '--value', metavar='VALUE')
+    p.add_argument('value', metavar='VALUE')
     p.add_argument('-p', '--priority', metavar='PRIORITY', type=int)
     p.add_argument('-w',
                    '--wait',
                    metavar='SEC',
                    type=float,
                    help='wait max seconds until the action is completed')
 
@@ -565,16 +564,16 @@
     p.add_argument('i', metavar='MASK').completer = ComplOID()
 
     p = sp.add_parser('edit', help='edit item config')
     p.add_argument('i', metavar='OID').completer = ComplOID()
 
     p = sp.add_parser('set', help='forcibly set item state')
     p.add_argument('i', metavar='OID').completer = ComplOID()
-    p.add_argument('status', metavar='STATUS', type=int)
-    p.add_argument('-v', '--value', metavar='VALUE')
+    p.add_argument('value', metavar='VALUE')
+    p.add_argument('-s', '--status', metavar='STATUS', type=int)
 
     sp.add_parser('summary', help='item summary per source')
 
     p = sp.add_parser('export', help='export item(s) to a deployment file')
     p.add_argument('i', metavar='MASK').completer = ComplOID()
     p.add_argument('-o', '--output', metavar='FILE',
                    help='output file').completer = ComplYamlFile()
@@ -612,15 +611,15 @@
 
 def append_lvar_cli(root_sp):
     ap = root_sp.add_parser('lvar', help='lvar commands')
     sp = ap.add_subparsers(dest='_subc', help='sub command')
 
     p = sp.add_parser('set', help='set lvar state')
     p.add_argument('i', metavar='OID').completer = ComplOIDtp('lvar')
-    p.add_argument('status', metavar='STATUS', nargs='?', type=int)
+    p.add_argument('-s', '--status', metavar='STATUS', type=int)
     p.add_argument('-v', '--value', metavar='VALUE')
 
     p = sp.add_parser('reset', help='reset lvar state')
     p.add_argument('i', metavar='OID').completer = ComplOIDtp('lvar')
 
     p = sp.add_parser('clear', help='clear lvar state')
     p.add_argument('i', metavar='OID').completer = ComplOIDtp('lvar')
```

### Comparing `eva-shell-0.0.93/eva4_shell/charts.py` & `eva-shell-0.1.0/eva4_shell/charts.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/eva4_shell/cli.py` & `eva-shell-0.1.0/eva4_shell/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,21 +640,19 @@
             print_result(
                 [d for d in data['clients'] if d['name'] != common.bus_name],
                 cols=[
                     'name', 'kind|n=type', 'source', 'port', 'r_frames',
                     'r_bytes', 'w_frames', 'w_bytes', 'queue', 'instances|n=ins'
                 ])
 
-    def action_exec(self, i, status, value, priority, wait):
+    def action_exec(self, i, value, priority, wait):
         params = dict(i=i, wait=wait)
         if priority is not None:
             params['priority'] = int(priority)
-        action_params = {'status': int(status)}
-        if value is not None:
-            action_params['value'] = format_value(value, advanced=True)
+        action_params = {'value': format_value(value, advanced=True)}
         params['params'] = action_params
         result = call_rpc('action', params)
         if current_command.json:
             import uuid
             result['uuid'] = str(uuid.UUID(bytes=result['uuid']))
             print_result(result)
         else:
@@ -913,37 +911,37 @@
                 print(dump)
             else:
                 write_file(output, dump)
                 print(f'{c} item(s) exported')
                 print()
 
     def item_set(self, i, status, value):
-        payload = dict(status=status, force=True)
-        if value is not None:
-            val = format_value(value)
-            payload['value'] = val
+        val = format_value(value)
+        payload = dict(status=1 if status is None else status,
+                       value=val,
+                       force=True)
         connect()
         common.bus.send(
             'RAW/' + i.replace(':', '/', 1),
             busrt.client.Frame(pack(payload), tp=busrt.client.OP_PUBLISH,
                                qos=1)).wait_completed()
         time.sleep(0.1)
         try:
             state = call_rpc('item.state', dict(i=i))[0]
         except IndexError:
             err('no such item')
             return
         try:
-            if state['status'] != status or (value is not None and
-                                             state['value'] != val):
+            if state['value'] != val or (status is not None and
+                                         state['status'] != status):
                 err('FAILED')
             else:
                 ok()
         except KeyError:
-            err(f'{i} has no status')
+            err(f'{i} has no state')
 
     def item_deploy(self, file=None):
         import yaml
         items = yaml.safe_load(read_file(file).decode()).pop('items')
         call_rpc('item.deploy', dict(items=items))
         print(f'{len(items)} item(s) deployed')
         print()
```

### Comparing `eva-shell-0.0.93/eva4_shell/client.py` & `eva-shell-0.1.0/eva4_shell/client.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/eva4_shell/compl.py` & `eva-shell-0.1.0/eva4_shell/compl.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/eva4_shell/sharedobj.py` & `eva-shell-0.1.0/eva4_shell/sharedobj.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/eva4_shell/shell.py` & `eva-shell-0.1.0/eva4_shell/shell.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/eva4_shell/tools.py` & `eva-shell-0.1.0/eva4_shell/tools.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.93/setup.py` & `eva-shell-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.93'
+__version__ = '0.1.0'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva-shell',
```

