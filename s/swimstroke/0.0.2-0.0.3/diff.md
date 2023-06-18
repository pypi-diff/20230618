# Comparing `tmp/swimstroke-0.0.2-py3-none-any.whl.zip` & `tmp/swimstroke-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8249 bytes, number of entries: 14
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-11 10:09 swimstroke/__init__.py
--rw-r--r--  2.0 unx      657 b- defN 23-Jun-11 10:09 swimstroke/__main__.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Jun-11 10:09 swimstroke/ev3.py
--rw-r--r--  2.0 unx     4815 b- defN 23-Jun-11 10:09 swimstroke/helpers.py
--rw-r--r--  2.0 unx    13053 b- defN 23-Jun-11 10:09 swimstroke/hy3.py
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-11 10:09 swimstroke/scb.py
--rw-r--r--  2.0 unx       47 b- defN 23-Jun-11 10:09 swimstroke/sd3.py
--rw-r--r--  2.0 unx      586 b- defN 23-Jun-11 10:09 swimstroke/util.py
--rw-r--r--  2.0 unx       47 b- defN 23-Jun-11 10:09 swimstroke/yaml.py
--rw-rw-rw-  2.0 unx     1103 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-11 10:10 swimstroke-0.0.2.dist-info/RECORD
-14 files, 25462 bytes uncompressed, 6477 bytes compressed:  74.6%
+Zip file size: 8453 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-18 05:24 swimstroke/__init__.py
+-rw-r--r--  2.0 unx      657 b- defN 23-Jun-18 05:24 swimstroke/__main__.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Jun-18 05:24 swimstroke/ev3.py
+-rw-r--r--  2.0 unx     5945 b- defN 23-Jun-18 05:24 swimstroke/helpers.py
+-rw-r--r--  2.0 unx    13053 b- defN 23-Jun-18 05:24 swimstroke/hy3.py
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-18 05:24 swimstroke/scb.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-18 05:24 swimstroke/sd3.py
+-rw-r--r--  2.0 unx      586 b- defN 23-Jun-18 05:24 swimstroke/util.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-18 05:24 swimstroke/yaml.py
+-rw-rw-rw-  2.0 unx     1103 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/RECORD
+14 files, 26592 bytes uncompressed, 6681 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: swimstroke/util.py
 Comment: 
 
 Filename: swimstroke/yaml.py
 Comment: 
 
-Filename: swimstroke-0.0.2.dist-info/LICENSE
+Filename: swimstroke-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: swimstroke-0.0.2.dist-info/METADATA
+Filename: swimstroke-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: swimstroke-0.0.2.dist-info/WHEEL
+Filename: swimstroke-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: swimstroke-0.0.2.dist-info/top_level.txt
+Filename: swimstroke-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: swimstroke-0.0.2.dist-info/RECORD
+Filename: swimstroke-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swimstroke/helpers.py

```diff
@@ -66,60 +66,84 @@
     # pad some 0s on the event_str to make a lexicographic sort possible
     event_str = entry['event_str']
     while len(event_str)<6:
         event_str = "0"+event_str
     return event_prefix+"-"+event_str
 
 def get_events(meetinfo):
-    teams_by_short_name = {}
-    events_by_key = {}
-    for team in meetinfo['teams']:
-        swimmers_by_code = {}
-        teams_by_short_name[team['short_name']] = team
-        for swimmer in team['swimmers']:
-            assert swimmer['swimmer_code'] not in swimmers_by_code
-            swimmers_by_code[swimmer['swimmer_code']] = swimmer
-        for entry in team['entries']:
-            event_key = _event_key_from_entry(entry)
-            if event_key not in events_by_key:
-                events_by_key[event_key] = {
-                    "event":entry['event_str'],
-                    "event_number":int(entry['event']),
-                    "date":entry['event_date'],
-                    "gender":entry['event_gender'],
-                    "gendercode":entry['event_gendercode'],
-                    "course":entry['event_course'],
-                    "coursecode":entry['event_coursecode'],
-                    "stroke":entry['stroke'],
-                    "strokeshort":entry['strokeshort'],
-                    "distance":entry['distance'],
-                    "relay":entry['relay'],
-                    "type":entry['event_type'],
-                    "entries":[],
-                    "num_heats":None
-                }
-                event = events_by_key[event_key]
-                name = "%s %d %s"%(event['gender'],event['distance'],event['strokeshort'])
-                if entry['relay']:
-                    name += " Relay"
-                event['name'] = name
-
-            entry = entry.copy()
-            entry['swimmers'] = [swimmers_by_code[s] for s in entry['swimmer_codes']]
-
-            events_by_key[event_key]['entries'].append(entry)
-            if entry['heat'] is not None:
-                if events_by_key[event_key]['num_heats'] is None or \
-                        events_by_key[event_key]['num_heats']<entry['heat_number']:
-                    events_by_key[event_key]['num_heats'] = entry['heat_number']
+    if 'teams' in meetinfo:
+        teams_by_short_name = {}
+        events_by_key = {}
+        for team in meetinfo['teams']:
+            swimmers_by_code = {}
+            teams_by_short_name[team['short_name']] = team
+            for swimmer in team['swimmers']:
+                assert swimmer['swimmer_code'] not in swimmers_by_code
+                swimmers_by_code[swimmer['swimmer_code']] = swimmer
+            for entry in team['entries']:
+                event_key = _event_key_from_entry(entry)
+                if event_key not in events_by_key:
+                    events_by_key[event_key] = {
+                        "event":entry['event_str'],
+                        "event_number":int(entry['event']),
+                        "date":entry['event_date'],
+                        "gender":entry['event_gender'],
+                        "gendercode":entry['event_gendercode'],
+                        "course":entry['event_course'],
+                        "coursecode":entry['event_coursecode'],
+                        "stroke":entry['stroke'],
+                        "strokeshort":entry['strokeshort'],
+                        "distance":entry['distance'],
+                        "relay":entry['relay'],
+                        "type":entry['event_type'],
+                        "entries":[],
+                        "num_heats":None
+                    }
+                    event = events_by_key[event_key]
+                    name = "%s %d %s"%(event['gender'],event['distance'],event['strokeshort'])
+                    if entry['relay']:
+                        name += " Relay"
+                    event['name'] = name
+
+                entry = entry.copy()
+                entry['swimmers'] = [swimmers_by_code[s] for s in entry['swimmer_codes']]
+
+                events_by_key[event_key]['entries'].append(entry)
+                if entry['heat'] is not None:
+                    if events_by_key[event_key]['num_heats'] is None or \
+                            events_by_key[event_key]['num_heats']<entry['heat_number']:
+                        events_by_key[event_key]['num_heats'] = entry['heat_number']
 
-    events = [events_by_key[event_key] for event_key in sorted([event_key for event_key in events_by_key.keys()])]
-    return events
+        return [events_by_key[event_key] for event_key in sorted([event_key for event_key in events_by_key.keys()])]
+    elif 'events' in meetinfo:
+        return meetinfo['events']
+    else:
+        raise ValueError("meetinfo doesn't have entries or events keys")
+
+def populate_heats(event):
+    event['heats'] = []
+    heats_by_key = {}
+    for entry in event['entries']:
+        if entry['heat'] is not None:
+            if entry['heat_number'] not in heats_by_key:
+                heats_by_key[entry['heat_number']] = {
+                    "heat":entry['heat'],
+                    "heat_number":entry['heat_number'],
+                    "entries":[]
+                }
+            heats_by_key[entry['heat_number']]['entries'].append(entry)
+    for heat_num in sorted([hnum for hnum in heats_by_key.keys()]):
+        heats_by_key[heat_num]['entries'].sort(key=lambda e:e['lane'])
+        event['heats'].append(heats_by_key[heat_num])
+    return event
 
 def get_lanes(meetinfo):
-    lanes = []
-    for team in meetinfo['teams']:
-        for entry in team['entries']:
-            if entry['lane'] is not None and entry['lane'] not in lanes:
-                lanes.append(entry['lane'])
-    lanes.sort()
-    return lanes
+    if 'teams' in meetinfo:
+        lanes = []
+        for team in meetinfo['teams']:
+            for entry in team['entries']:
+                if entry['lane'] is not None and entry['lane'] not in lanes:
+                    lanes.append(entry['lane'])
+        lanes.sort()
+        return lanes
+    else:
+        raise ValueError("meetinfo doesn't have entries")
```

## Comparing `swimstroke-0.0.2.dist-info/LICENSE` & `swimstroke-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swimstroke-0.0.2.dist-info/RECORD` & `swimstroke-0.0.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swimstroke/__init__.py,sha256=HTxCVaw1TLgpHMH8guB3hHYQ80cX6_fSEoPT_hz2Y8w,23
 swimstroke/__main__.py,sha256=XtPUjZM3ZTd_fEMmgZBqFlkp65eqXXcVWTXmQR9PF_A,657
 swimstroke/ev3.py,sha256=P5IkzYCqAH3E5ZzhJMyFztxo0PE4_-wmwIyOsDkagws,3793
-swimstroke/helpers.py,sha256=fyvNQ-62_2TgvK-CAf0M7Qcdg_XeIQb1w7aikP2qY_o,4815
+swimstroke/helpers.py,sha256=HgdD5bPzPZXHRWQANyha_n0oloZFPpjZ4pccd_4ICDE,5945
 swimstroke/hy3.py,sha256=Exs_cjsISZqOGUBaowhOQrspL_lcGvcWbESQ6CI8ZZc,13053
 swimstroke/scb.py,sha256=cC-rhzRvKpq60ux7MHm0ylj16qc21ZqhUBLQqxdJMQI,86
 swimstroke/sd3.py,sha256=JMYeTOk66YJInRReB3KMFyB1JKnX69sCHdC2_Ey2ypg,47
 swimstroke/util.py,sha256=s7cBEfHsdbYuID3bH2bAnw72zYHC2A4LroSf8iTH74o,586
 swimstroke/yaml.py,sha256=JMYeTOk66YJInRReB3KMFyB1JKnX69sCHdC2_Ey2ypg,47
-swimstroke-0.0.2.dist-info/LICENSE,sha256=ua_EyrQ3shMEJAhfgGjSeK_mFf6AIT-QiFG2lQfsntY,1103
-swimstroke-0.0.2.dist-info/METADATA,sha256=wiGs2ob_q022sNICybsHcSnbKyQUDb9B_FyUY6nkva4,77
-swimstroke-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swimstroke-0.0.2.dist-info/top_level.txt,sha256=C15CTf7t6T4k83ycljKbwYVziBgz5vqOBEYdK8Y6FfY,11
-swimstroke-0.0.2.dist-info/RECORD,,
+swimstroke-0.0.3.dist-info/LICENSE,sha256=ua_EyrQ3shMEJAhfgGjSeK_mFf6AIT-QiFG2lQfsntY,1103
+swimstroke-0.0.3.dist-info/METADATA,sha256=WgM6E9-UJM8e95NVtSxzEAA6LjkIwmA6-lYvbBXkHBk,77
+swimstroke-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swimstroke-0.0.3.dist-info/top_level.txt,sha256=C15CTf7t6T4k83ycljKbwYVziBgz5vqOBEYdK8Y6FfY,11
+swimstroke-0.0.3.dist-info/RECORD,,
```

