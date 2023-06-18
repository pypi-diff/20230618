# Comparing `tmp/piwaterflow-0.5.8.tar.gz` & `tmp/piwaterflow-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.8.tar", last modified: Tue May 30 11:50:51 2023, max compression
+gzip compressed data, was "piwaterflow-0.5.9.tar", last modified: Thu Jun  1 12:02:41 2023, max compression
```

## Comparing `piwaterflow-0.5.8.tar` & `piwaterflow-0.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.531875 piwaterflow-0.5.8/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_003_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_004_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.671330 piwaterflow-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23595 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:02:41.671330 piwaterflow-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_003_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_004_events.py
```

### Comparing `piwaterflow-0.5.8/PKG-INFO` & `piwaterflow-0.5.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.8
+Version: 0.5.9
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.8/README.md` & `piwaterflow-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.8/piwaterflow/config_waterflow.py` & `piwaterflow-0.5.9/piwaterflow/config_waterflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 class WaterflowConfig(Config):
     """Config override for piwaterflow
     """
     def _after_reading(self):
         """ Adapt the data after reading the config yaml
         """
         # Customize values
-        for program in self.config['programs'].values():
+        for program in self.config['programs']:
             progtime = datetime.strptime(program['start_time'], '%H:%M')
             progtime = _set_timezone_utc(progtime)
             program['start_time'] = progtime
 
         # Sort the programs by time
         # self.config['programs'].sort(key=lambda prog: prog['start_time'])
 
     def _before_writting(self):
         """ Transforms the data before being written to the config file
         Returns:
             dict: Transformed config dictionary
         """
         configcopy = self.get_dict_copy()
         # Convert the date back from datetime to string
-        for program in configcopy['programs'].values():
+        for program in configcopy['programs']:
             program['start_time'] = program['start_time'].strftime('%H:%M')
 
         return configcopy
```

### Comparing `piwaterflow-0.5.8/piwaterflow/tests/test_000.py` & `piwaterflow-0.5.9/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.8/piwaterflow/waterflow.py` & `piwaterflow-0.5.9/piwaterflow/waterflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self, template_config_path: str = None, fake_now: datetime = None, dry_run: bool = False):
         """__init__ of the function
         Args:
             template_config_path (str, optional): Template config to use. Defaults to None.
             dry_run (bool, optional): If true, it will just simulate, and wont make any change. Defaults to False.
         """
         self.homevar = os.path.join(str(Path.home()), 'var', self.class_name())
-        
+
         self.dry_run = dry_run
         self.curr_time = fake_now
 
         if dry_run:
             self.homevar = os.path.join(self.homevar, 'dryrun')
             if os.path.exists(self.homevar): # Only one instance of waterflow can run at a time, so this is safe
                 shutil.rmtree(self.homevar)
@@ -69,22 +69,24 @@
             shutil.rmtree(self.homevar)
 
     @classmethod
     def class_name(cls):
         """ class name """
         return "waterflow"
 
-    def get_homevar_path(self, rel_path):
+    def _get_homevar_path(self, rel_path):
         return os.path.join(self.homevar, rel_path)
 
     def update_config(self, programs: dict):
         """Updates the config file with modified programs
         Args:
             programs (dict): New programs to be modified
         """
+        # TODO: Verify parameters in bounds
+
         # Update config in mem
         self.config.update({'programs': programs})
 
         # Write back config to disk
         self.config.write()
 
     def _get_program_data(self, program):
@@ -131,20 +133,15 @@
         """
         next_program_time = None
         program_name = None
 
         # Only used to get "today"... hour and minute will be overwritten for comparations with last_program_time
         current_time = self.curr_time.astimezone().replace(microsecond=0)
 
-        # Transform into a list to sort them
-        prog_list = []
-        for key, value in self.config['programs'].items():
-            temp = value
-            temp['name'] = key
-            prog_list.append(temp)
+        prog_list = self.config['programs']
         prog_list.sort(key=lambda prog: prog['start_time'])
 
         # Find if next program is today, considering the last program time executed
         for program in prog_list:
             if program['enabled'] is True:
                 candidate_time = current_time.replace(hour=program['start_time'].hour,
                                                       minute=program['start_time'].minute,
@@ -165,15 +162,15 @@
                                                                   second=0).astimezone()
                     program_name = program['name']
                     break
 
         return next_program_time, program_name
 
     def _last_program_path(self):
-        return self.get_homevar_path('lastprogram.yml')
+        return self._get_homevar_path('lastprogram.yml')
 
     def _read_last_program_time(self, default: datetime = None):
         last_program_path = self._last_program_path()
 
         if os.path.exists(last_program_path):
             with open(last_program_path, 'r', encoding="utf-8") as file:
                 data = file.readlines()
@@ -194,15 +191,15 @@
             file.write(self.time_to_str(time_last))
 
     def get_lock(self):
         """
         This is to ensure that only one execution will run from cron at the same time
         Use file as a lock... not using DB locks because we want to maximize resiliency
         """
-        lock_path = self.get_homevar_path('lock')
+        lock_path = self._get_homevar_path('lock')
 
         if not os.path.exists(lock_path):
             with open(lock_path, 'w', encoding="utf-8"):
                 return True
         else:
             modified_time = datetime.fromtimestamp(os.path.getmtime(lock_path)).astimezone()
             if (datetime.now().astimezone() - modified_time) > timedelta(minutes=self.config['max_loop_time']):
@@ -210,15 +207,15 @@
                 Path(lock_path).touch()  # Previous token expired (previous loop crashed?)... we will retouch to retry
                 return True
         return False
 
     def release_lock(self):
         """Lock the loop... so the 2 loops cannot happen at the same time
         """
-        lock_path = self.get_homevar_path('lock')
+        lock_path = self._get_homevar_path('lock')
 
         if os.path.exists(lock_path):
             os.remove(lock_path)
         else:
             self._add_event('CannotUnlock', None)
 
     def is_looping_correctly(self):
@@ -230,15 +227,15 @@
         return (time_now - self.last_loop_time()) < timedelta(minutes=self.config['max_loop_time'])
 
     def last_loop_time(self):
         """ Returns the last time in that a loop was succesfully executed
         Returns:
            datetime: Time in which last loop was executed
         """
-        token_path = self.get_homevar_path('token')
+        token_path = self._get_homevar_path('token')
         if os.path.exists(token_path):
             mod_time_since_epoc = os.path.getmtime(token_path)
             modification_time = datetime.fromtimestamp(mod_time_since_epoc).astimezone()
         else:
             modification_time = datetime.fromtimestamp(0) # Loop never run ok. Return oldest possible date
 
         return modification_time
@@ -253,104 +250,103 @@
 
         Returns:
             bool: If forced correctly
         """
         config = self.config.get_dict()
         if (type_force == 'program' and 0 <= value < len(config['programs'])) or \
            (type_force == 'valve' and 0 <= value < len(config['valves'])):
-            with open(self.get_homevar_path('force'), 'w', encoding="utf-8") as force_file:
+            with open(self._get_homevar_path('force'), 'w', encoding="utf-8") as force_file:
                 force_file.write(f'{{"type":"{type_force}","value":{value}}}')
                 return True
         else:
             return False
 
     def stop(self):
         """ Set the Stop-flag, so that the loop will stop the forced valve or program execution
         Returns:
             _type_: _description_
         """
-        stop_req_path = self.get_homevar_path('stop')
+        stop_req_path = self._get_homevar_path('stop')
         Path(stop_req_path).touch()
         return True
 
     def stop_remove(self):
         """ Returns if a stop has already been requested
         Returns:
            bool: Return true if a stop has been requested
         """
-        stop_req_path = self.get_homevar_path('stop')
+        stop_req_path = self._get_homevar_path('stop')
         return os.remove(stop_req_path)
 
     def stop_requested(self):
         """ Returns if a stop has already been requested
         Returns:
            bool: Return true if a stop has been requested
         """
-        stop_req_path = self.get_homevar_path('stop')
+        stop_req_path = self._get_homevar_path('stop')
         return os.path.exists(stop_req_path)
 
     def get_forced_info(self):
         """ Returns the forced info of the waterflow
         Returns:
             dict: Forced info
         """
-        force_file_path = self.get_homevar_path('force')
+        force_file_path = self._get_homevar_path('force')
         if os.path.exists(force_file_path):
             with open(force_file_path, 'r', encoding="utf-8") as force_file:
                 data = json.load(force_file)
                 return data
         else:
             return None
 
     def _add_event(self, event: str, value):
         self.events.append((self.time_to_str(datetime.now()), event, value))
 
-        events_file_path = self.get_homevar_path('events')
+        events_file_path = self._get_homevar_path('events')
         with open(events_file_path, 'w', encoding="utf-8") as events_file:
             json.dump(self.events, events_file)
 
     def _read_events(self):
         events = []
-        events_file_path = self.get_homevar_path('events')
+        events_file_path = self._get_homevar_path('events')
         if os.path.exists(events_file_path):
             with open(events_file_path, 'r', encoding="utf-8") as events_file:
                 events = json.load(events_file)
         return events
 
     def _get_event_string(self, event: tuple):
         if event[1] == 'ExecValve':
             result = f'Executing program {event[2]}.'
-        if event[1] == 'InverterON':
+        elif event[1] == 'InverterON':
             result = 'Inverter relay ON.'
-        if event[1] == 'InverterOFF':
+        elif event[1] == 'InverterOFF':
             result = 'Inverter relay OFF.'
-        if event[1] == 'ValveON':
+        elif event[1] == 'ValveON':
             result = f'Valve {event[2]} ON.'
-        if event[1] == 'ValveOFF':
+        elif event[1] == 'ValveOFF':
             result = f'Valve {event[2]} OFF.'
-        if event[1] == 'LastProg':
+        elif event[1] == 'LastProg':
             if event[2]:
                 result = f'Next program: {event[2]}.'
             else:
                 result = 'NO active program!'
-        if event[1] == 'LockExpired':
+        elif event[1] == 'LockExpired':
             result = 'Lock expired: Last loop ended abnormally?.'
-        if event[1] == 'CannotUnlock':
+        elif event[1] == 'CannotUnlock':
             result = "Could not release lock."
-        if event[1] == 'ForcedProg':
+        elif event[1] == 'ForcedProg':
             result = f'Forced program {event[2]} executing now.'
-        if event[1] == 'ForcedValve':
+        elif event[1] == 'ForcedValve':
             result = f'Forced valve {event[2]} executing now.'
-        if event[1] == 'Stop':
+        elif event[1] == 'Stop':
             result = 'Activity stopped.'
-        if event[1] == 'Exception':
+        elif event[1] == 'Exception':
             result = f'Error looping: {event[2]}'
 
-
-        return result
+        return f'{event[0]}:{result}'
 
     def get_log(self):
         """ Get the user log (not the debug log). This is the one the is shown in the wwwaterflow
         Returns:
             str: The whole user logs
         """
         log = ''
@@ -360,14 +356,20 @@
 
     def _sleep(self, time_sleep):
         """ Sleep "time_sleep" time, but checks every 5 seconds if a stop has been requested
         Args:
             time_sleep (int): Number of seconds to sleep
         """
         time_count = 0
+
+        # Clamp sleep time... as safety. Never let a valve stay ON more than this
+        if time_sleep > self.config['max_valve_time']:
+            time_sleep = self.config['max_valve_time']
+            self.debuglogger.info(f'Valve time clamped to {self.config["max_valve_time"]}')
+
         while not self.stop_requested() and time_count < time_sleep:
             time_count = time_count + 5
             time.sleep(5)  # Every X seconds
 
     def _emit_action_metric(self, action, forced):
         if self.config['metrics'] and self.conn:
             action_body = [
@@ -419,29 +421,34 @@
         Works for regular programs, or forced ones (if program number is sent)
         """
         self._add_event('ExecProg', program_name)
         # inverter_enable =  not GPIO.input(self.config['external_ac_signal_pin'])
         # if inverter_enable: # If we don't have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
         self._add_event('InverterON', None)
-        program_data = self.config['programs'][program_name]
-        for key, valve_time in program_data['valves_times'].items():
-            if valve_time > 0 and not self.stop_requested():
-                valve_pin = self.config['valves'][key]['pin']
+        program = None
+        for program_it in self.config['programs']:
+            if program_it['name'] == program_name:
+                program = program_it
+                break
+
+        for valve in program['valves']:
+            if valve['time'] > 0 and not self.stop_requested():
+                valve_pin = self.config['valves'][valve['name']]['pin']
                 GPIO.output(valve_pin, GPIO.HIGH)
-                self._add_event('ValveON', key)
+                self._add_event('ValveON', valve['name'])
 
                 # If dry run, then we fast forward the sleep
                 if not self.dry_run:
-                    self._sleep(valve_time * 60)
+                    self._sleep(valve['time'] * 60)
 
                 GPIO.output(valve_pin, GPIO.LOW)
-                self._add_event('ValveOFF', key)
+                self._add_event('ValveOFF', valve['name'])
             else:
-                self._add_event('ValveSkip', key)
+                self._add_event('ValveSkip', valve['name'])
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
         self._add_event('InverterOFF', None)
 
     def _log_next_program_time(self):
         new_next_program_time, _ = self._recalc_next_program(self.curr_time)
```

### Comparing `piwaterflow-0.5.8/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.9/piwaterflow.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.8
+Version: 0.5.9
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.8/piwaterflow.egg-info/SOURCES.txt` & `piwaterflow-0.5.9/piwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.8/setup.py` & `piwaterflow-0.5.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.8",
+    version="0.5.9",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
@@ -21,14 +21,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
     ],
     install_requires=[
         'log_mgr>=0.0.2',
-        'config_yml>=0.3.0',
+        'config_yml>=0.3.1',
         'RPi.GPIO>=0.7.0',
         'fake-rpigpio>=0.1.1',
         'influxdb_wrapper>=0.0.4'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `piwaterflow-0.5.8/tests/test_000_loop.py` & `piwaterflow-0.5.9/tests/test_000_loop.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.8/tests/test_001_forward.py` & `piwaterflow-0.5.9/tests/test_001_forward.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.8/tests/test_002_reverse.py` & `piwaterflow-0.5.9/tests/test_002_reverse.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.8/tests/test_003_lock.py` & `piwaterflow-0.5.9/tests/test_003_lock.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         first_lock = self.waterflow.get_lock()
         self.assertTrue(first_lock)
 
         second_lock = self.waterflow.get_lock()
         self.assertFalse(second_lock)
 
         # Simulate lock expiring
-        lock_path = self.waterflow.get_homevar_path('lock')
+        lock_path = self.waterflow._get_homevar_path('lock') # pylint: disable=protected-access
         past_epoch = time.time() - 1260
         os.utime(lock_path, (past_epoch, past_epoch) ) # 21 minutes before to simulate expiring
         third_lock = self.waterflow.get_lock()
         self.assertTrue(third_lock)
 
 
 if __name__ == '__main__':
```

### Comparing `piwaterflow-0.5.8/tests/test_004_events.py` & `piwaterflow-0.5.9/tests/test_004_events.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Unittesting """
 import unittest
 from pathlib import Path
 import gc
-import json
 
 from piwaterflow import Waterflow
 
 
 class Testing(unittest.TestCase):
     """ Unittesting class
     """
```

