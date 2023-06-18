# Comparing `tmp/git-debranch-0.1.6.tar.gz` & `tmp/git-debranch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-debranch-0.1.6.tar", last modified: Sat Jun  3 13:01:20 2023, max compression
+gzip compressed data, was "git-debranch-0.1.7.tar", last modified: Sun Jun 18 10:57:41 2023, max compression
```

## Comparing `git-debranch-0.1.6.tar` & `git-debranch-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-03 13:01:06.000000 git-debranch-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-03 13:01:20.817450 git-debranch-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-03 13:01:06.000000 git-debranch-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:01:20.817450 git-debranch-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-03 13:01:06.000000 git-debranch-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.813450 git-debranch-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.813450 git-debranch-0.1.6/src/git_debranch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/src/git_debranch/bpmn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/process_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/spawn.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/process_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/script_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/src/git_debranch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:41.753579 git-debranch-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-18 10:57:30.000000 git-debranch-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-18 10:57:41.753579 git-debranch-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-18 10:57:30.000000 git-debranch-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 10:57:41.753579 git-debranch-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-18 10:57:30.000000 git-debranch-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:41.749579 git-debranch-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:41.749579 git-debranch-0.1.7/src/git_debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:41.753579 git-debranch-0.1.7/src/git_debranch/bpmn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:41.753579 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/process_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/spawn.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/bpmn/process_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/script_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 10:57:30.000000 git-debranch-0.1.7/src/git_debranch/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:57:41.753579 git-debranch-0.1.7/src/git_debranch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-18 10:57:41.000000 git-debranch-0.1.7/src/git_debranch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-18 10:57:41.000000 git-debranch-0.1.7/src/git_debranch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:57:41.000000 git-debranch-0.1.7/src/git_debranch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-18 10:57:41.000000 git-debranch-0.1.7/src/git_debranch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 10:57:41.000000 git-debranch-0.1.7/src/git_debranch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 10:57:41.000000 git-debranch-0.1.7/src/git_debranch.egg-info/top_level.txt
```

### Comparing `git-debranch-0.1.6/LICENSE` & `git-debranch-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/PKG-INFO` & `git-debranch-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-debranch
-Version: 0.1.6
+Version: 0.1.7
 Summary: Remove git branches
 Author: Jon Herron
 Author-email: jon.herron@yahoo.com
 License: lGPLv2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `git-debranch-0.1.6/README.md` & `git-debranch-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/setup.py` & `git-debranch-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn` & `git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn` & `git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn` & `git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/spawn.bpmn` & `git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

 * *Files 2% similar despite different names*

#### Comparing `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/spawn.bpmn` & `git-debranch-0.1.7/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

```diff
@@ -21,14 +21,16 @@
     <bpmn:serviceTask id="Activity_1wobbp0" name="Spawn a process">
       <bpmn:extensionElements>
         <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
           <spiffworkflow:parameters>
             <spiffworkflow:parameter id="args" type="any" value="spawn_args"/>
           </spiffworkflow:parameters>
         </spiffworkflow:serviceTaskOperator>
+        <spiffworkflow:postScript/>
+        <spiffworkflow:preScript/>
       </bpmn:extensionElements>
       <bpmn:incoming>Flow_090xnqj</bpmn:incoming>
       <bpmn:outgoing>Flow_1cl2vgj</bpmn:outgoing>
     </bpmn:serviceTask>
     <bpmn:sequenceFlow id="Flow_0utbnx3" sourceRef="Activity_1ufh8x7" targetRef="Event_08pdzal"/>
     <bpmn:endEvent id="Event_08pdzal">
       <bpmn:incoming>Flow_0utbnx3</bpmn:incoming>
@@ -44,18 +46,14 @@
     <bpmn:textAnnotation id="TextAnnotation_1gt83ai">
       <bpmn:text>Not how i want to handle this but I might be in too deep with the subprocesses and what is supported.</bpmn:text>
     </bpmn:textAnnotation>
     <bpmn:association id="Association_1hdvgtw" sourceRef="Activity_1ufh8x7" targetRef="TextAnnotation_1gt83ai"/>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
     <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="spawn_process">
-      <bpmndi:BPMNShape id="TextAnnotation_1gt83ai_di" bpmnElement="TextAnnotation_1gt83ai">
-        <dc:Bounds x="500" y="370" width="100" height="142"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
         <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_0o5auw6_di" bpmnElement="Gateway_0o5auw6" isMarkerVisible="true">
         <dc:Bounds x="425" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Event_1vc03l8_di" bpmnElement="Event_1vc03l8">
@@ -68,18 +66,18 @@
       <bpmndi:BPMNShape id="Event_12c7q1f_di" bpmnElement="Event_08pdzal">
         <dc:Bounds x="622" y="272" width="36" height="36"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_1hcqe3e_di" bpmnElement="Activity_1ufh8x7">
         <dc:Bounds x="480" y="250" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNEdge id="Association_1hdvgtw_di" bpmnElement="Association_1hdvgtw">
-        <di:waypoint x="538" y="330"/>
-        <di:waypoint x="547" y="370"/>
-      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNShape id="TextAnnotation_1gt83ai_di" bpmnElement="TextAnnotation_1gt83ai">
+        <dc:Bounds x="500" y="370" width="100" height="142"/>
+        <bpmndi:BPMNLabel/>
+      </bpmndi:BPMNShape>
       <bpmndi:BPMNEdge id="Flow_090xnqj_di" bpmnElement="Flow_090xnqj">
         <di:waypoint x="215" y="177"/>
         <di:waypoint x="270" y="177"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_1cl2vgj_di" bpmnElement="Flow_1cl2vgj">
         <di:waypoint x="370" y="177"/>
         <di:waypoint x="425" y="177"/>
@@ -93,10 +91,14 @@
         <di:waypoint x="450" y="290"/>
         <di:waypoint x="480" y="290"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_0utbnx3_di" bpmnElement="Flow_0utbnx3">
         <di:waypoint x="580" y="290"/>
         <di:waypoint x="622" y="290"/>
       </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Association_1hdvgtw_di" bpmnElement="Association_1hdvgtw">
+        <di:waypoint x="538" y="330"/>
+        <di:waypoint x="547" y="370"/>
+      </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.6/src/git_debranch/loader.py` & `git-debranch-0.1.7/src/git_debranch/loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import json
 import os
 import pkgutil
 
 from SpiffWorkflow.bpmn.workflow import BpmnWorkflow
 from SpiffWorkflow.spiff.parser.process import SpiffBpmnParser
 
@@ -30,20 +31,21 @@
         "branch_parser.bpmn",
         "deletion_prompt.bpmn",
         "delete_branches.bpmn",
         "spawn.bpmn",
     ]
     return map(_bpmn_data_path, bpmn_filenames)
 
+def _get_data(data_path):
+    return pkgutil.get_data("git_debranch", data_path)
+
 def _get_data_str(data_path):
-    return pkgutil.get_data("git_debranch", data_path).decode("utf-8")
+    return _get_data(data_path).decode("utf-8")
 
-def _bpmn_strs():
-    return map(_get_data_str, _bpmn_data_paths())
+def _bpmn_data():
+    return map(_get_data, _bpmn_data_paths())
 
 def _parser():
     parser = SpiffBpmnParser()
-    for bpmn_str in _bpmn_strs():
-        # TODO: hack - replace with better solution - add_bpmn_str doesn't allow:
-        bpmn_str = bpmn_str.replace('<?xml version="1.0" encoding="UTF-8"?>', '')
-        parser.add_bpmn_str(bpmn_str)
+    for data in _bpmn_data():
+        parser.add_bpmn_io(io.BytesIO(data))
     return parser
```

### Comparing `git-debranch-0.1.6/src/git_debranch/runner.py` & `git-debranch-0.1.7/src/git_debranch/runner.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/script_engine.py` & `git-debranch-0.1.7/src/git_debranch/script_engine.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch/workflow.py` & `git-debranch-0.1.7/src/git_debranch/workflow.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.6/src/git_debranch.egg-info/PKG-INFO` & `git-debranch-0.1.7/src/git_debranch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-debranch
-Version: 0.1.6
+Version: 0.1.7
 Summary: Remove git branches
 Author: Jon Herron
 Author-email: jon.herron@yahoo.com
 License: lGPLv2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `git-debranch-0.1.6/src/git_debranch.egg-info/SOURCES.txt` & `git-debranch-0.1.7/src/git_debranch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

