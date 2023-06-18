# Comparing `tmp/minidevice-2.0.4.tar.gz` & `tmp/minidevice-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.4.tar", last modified: Sat Jun 17 15:29:10 2023, max compression
+gzip compressed data, was "minidevice-2.0.5.tar", last modified: Sun Jun 18 04:26:33 2023, max compression
```

## Comparing `minidevice-2.0.4.tar` & `minidevice-2.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:29:10.361579 minidevice-2.0.4/
--rw-rw-rw-   0        0        0     2392 2023-06-17 15:29:10.360183 minidevice-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2098 2023-06-17 15:02:43.000000 minidevice-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 15:29:10.342630 minidevice-2.0.4/minidevice/
--rw-rw-rw-   0        0        0     2745 2023-06-17 13:52:23.000000 minidevice-2.0.4/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.4/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      226 2023-06-17 14:47:51.000000 minidevice-2.0.4/minidevice/__init__.py
--rw-rw-rw-   0        0        0    20907 2023-06-17 11:44:42.000000 minidevice-2.0.4/minidevice/adb.py
--rw-rw-rw-   0        0        0    20739 2023-06-17 15:28:08.000000 minidevice-2.0.4/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.4/minidevice/logger.py
--rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.4/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.4/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.4/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.4/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:29:10.359184 minidevice-2.0.4/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2392 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 15:29:10.000000 minidevice-2.0.4/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 15:29:10.361579 minidevice-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-17 15:28:26.000000 minidevice-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:26:33.153939 minidevice-2.0.5/
+-rw-rw-rw-   0        0        0     2392 2023-06-18 04:26:33.151649 minidevice-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2098 2023-06-17 15:02:43.000000 minidevice-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 04:26:33.123551 minidevice-2.0.5/minidevice/
+-rw-rw-rw-   0        0        0     2758 2023-06-18 04:18:15.000000 minidevice-2.0.5/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.5/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      226 2023-06-17 14:47:51.000000 minidevice-2.0.5/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    21023 2023-06-18 04:23:42.000000 minidevice-2.0.5/minidevice/adb.py
+-rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.5/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.5/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12808 2023-06-18 04:22:01.000000 minidevice-2.0.5/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1714 2023-06-18 04:22:45.000000 minidevice-2.0.5/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      685 2023-06-18 04:24:38.000000 minidevice-2.0.5/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.5/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:26:33.150674 minidevice-2.0.5/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     2392 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-18 04:26:33.000000 minidevice-2.0.5/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 04:26:32.000000 minidevice-2.0.5/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 04:26:33.153939 minidevice-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-18 04:15:42.000000 minidevice-2.0.5/setup.py
```

### Comparing `minidevice-2.0.4/PKG-INFO` & `minidevice-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.4
+Version: 2.0.5
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.4/README.md` & `minidevice-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.4/minidevice/DroidCast.py` & `minidevice-2.0.5/minidevice/DroidCast.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 class DroidCast(ScreenCap):
     def __init__(self, device, DroidCastServerPort=53516) -> None:
         self.droidcast_adb = ADB(device)
         self.DroidCastServerPort = DroidCastServerPort
         self.class_path = APK_ANDROID_PATH 
         self.DroidCastSession = requests.Session()
-        self._install()
-        self._start()
+        self.__install()
+        self.__start()
 
-    def _install(self):
+    def __install(self):
         self.droidcast_adb.push_file(APK_PATH, self.class_path)
         self.droidcast_adb.install_apk(APK_PATH)
 
-    def _start_droidcast(self):
+    def __start_droidcast(self):
         out = str(
             self.droidcast_adb.adb_command(
                 ["shell", "pm", "path", "com.rayworks.droidcast"]
             )
         )
         prefix = "package:"
         postfix = ".apk"
@@ -52,32 +52,33 @@
                 self.class_path,
                 start_droidcast_cmd,
             ],
             stderr=subprocess.DEVNULL,
             stdout=subprocess.DEVNULL,
         )
 
-    def _forward_port(self):
+    def __forward_port(self):
         self.droidcast_port = self.droidcast_adb.forward_port(
             "tcp:{}".format(self.DroidCastServerPort)
         )
         self.droidcast_url = "http://localhost:{}/screenshot".format(
             self.droidcast_port
         )
         print(self.droidcast_adb.list_forward_port())
         print(self.droidcast_url)
 
-    def _start(self):
-        self._start_droidcast()
-        self._forward_port()
+    def __start(self):
+        self.__start_droidcast()
+        self.__forward_port()
         print("DroidCast启动完成")
 
-    def _stop(self):
+    def __stop(self):
         self.droidcast_adb.remove_forward(self.droidcast_port)  # 清理转发端口
         if self.droidcast_popen.poll() is None:
             self.droidcast_popen.kill()  # 关闭管道
 
     def screencap_raw(self) -> bytes:
         if self.droidcast_popen.poll() is not None:
-            self._stop()
-            self._start()
+            self.__stop()
+            self.__start()
         return self.DroidCastSession.get(self.droidcast_url, timeout=3).content
+
```

### Comparing `minidevice-2.0.4/minidevice/QueueUtils.py` & `minidevice-2.0.5/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.4/minidevice/adb.py` & `minidevice-2.0.5/minidevice/adb.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             else:
                 logger.error("ADB命令执行失败\n报错信息:{}".format(err))
         except FileNotFoundError:
             logger.error("ADB不存在或无法执行")
         except subprocess.TimeoutExpired:
             logger.error("ADB命令执行超时")
 
-    def _run_adb_command(self, command: list):
+    def __run_adb_command(self, command: list):
         adb_command = [ADB_PATH]
         if self.device:
             adb_command.extend(["-s", self.device])
         adb_command.extend(command)
         try:
             result = subprocess.run(adb_command, capture_output=True, text=True)
             if result.returncode != 0:
@@ -56,498 +56,498 @@
             # 命令执行超时，处理超时情况
             logger.error("命令执行超时")
 
     def forward_port(self, server, port=None) -> int:
         while True:
             localport = random.randint(11111, 20000) if port is None else port
             local = "tcp:{}".format(localport)
-            result = self._run_adb_command(["forward", local, server])
+            result = self.__run_adb_command(["forward", local, server])
             if result.split(":")[-1] != "":
                 return int(result.split(":")[-1])
             else:
                 if port is not None:
                     self.remove_forward(port)
 
     def remove_forward(self, port):
-        self._run_adb_command(["forward", "--remove", "tcp:{}".format(port)])
+        self.__run_adb_command(["forward", "--remove", "tcp:{}".format(port)])
 
     @staticmethod
     def list_forward_port():
         output = subprocess.run(
             [ADB_PATH, "forward", "--list"], capture_output=True, text=True
         )
         list_port = output.stdout.split("\n")[:-2]
         return list_port
 
     def get_version(self):
-        output = self._run_adb_command(["version"])
+        output = self.__run_adb_command(["version"])
         return output.strip()
 
     def start_server(self):
-        self._run_adb_command(["start-server"])
+        self.__run_adb_command(["start-server"])
 
     def stop_server(self):
-        self._run_adb_command(["kill-server"])
+        self.__run_adb_command(["kill-server"])
 
     def enable_root(self):
-        self._run_adb_command(["root"])
+        self.__run_adb_command(["root"])
 
     def set_port(self, port):
-        self._run_adb_command(["tcpip", str(port)])
+        self.__run_adb_command(["tcpip", str(port)])
 
     def clean_forward(self):
-        self._run_adb_command(["forward", "--remove-all"])
+        self.__run_adb_command(["forward", "--remove-all"])
 
     @staticmethod
     def list_devices():
-        output = ADB._run_adb_command(ADB(), ["devices"])
+        output = ADB.__run_adb_command(ADB(), ["devices"])
         devices = output.split("\n")[1:]
         devices = [device.split("\t")[0] for device in devices if device.strip()]
         return devices
 
     @staticmethod
     def list_devices_info():
-        output = ADB._run_adb_command(ADB(), ["devices", "-l"])
+        output = ADB.__run_adb_command(ADB(), ["devices", "-l"])
         devices = output.split("\n")[1:]
         devices = [device.split("\t")[0] for device in devices if device.strip()]
         status = [device.split("\t")[1] for device in devices if device.strip()]
         remark = [device.split("\t")[2] for device in devices if device.strip()]
         return list(zip(devices, status, remark))
 
     def install_apk(self, apk_path):
-        self._run_adb_command(["install", apk_path])
+        self.__run_adb_command(["install", apk_path])
 
     def uninstall_app(self, package_name, save_data=False):
         adb_command = (
             ["uninstall", "-k", package_name]
             if save_data
             else ["uninstall", package_name]
         )
-        self._run_adb_command(adb_command)
+        self.__run_adb_command(adb_command)
 
     def clear_app_data(self, package_name):
-        self._run_adb_command(["shell", "pm", "clear", package_name])
+        self.__run_adb_command(["shell", "pm", "clear", package_name])
 
     def list_apps(self, system=False, third_party=False, package_name_contains=None):
         command = ["shell", "pm", "list", "packages"]
         if system:
             command.append("-s")
         if third_party:
             command.append("-3")
-        output = self._run_adb_command(command).strip()
+        output = self.__run_adb_command(command).strip()
         packages = output.split("\n")
         if package_name_contains:
             packages = [
                 package for package in packages if package_name_contains in package
             ]
         packages = [package.split(":")[-1] for package in packages]
         return packages
 
     def get_foreground_activity(self):
-        output = self._run_adb_command(
+        output = self.__run_adb_command(
             [
                 "shell",
                 "dumpsys",
                 "activity",
                 "activities",
                 "|",
                 "grep",
                 "mResumedActivity",
             ]
         )
         return output.strip()
 
     def get_running_services(self):
-        output = self._run_adb_command(["shell", "dumpsys", "activity", "services"])
+        output = self.__run_adb_command(["shell", "dumpsys", "activity", "services"])
         return output.strip()
 
     def get_app_info(self, package_name):
-        output = self._run_adb_command(["shell", "dumpsys", "package", package_name])
+        output = self.__run_adb_command(["shell", "dumpsys", "package", package_name])
         return output.strip()
 
     def get_app_install_path(self, package_name):
-        output = self._run_adb_command(["shell", "pm", "path", package_name])
+        output = self.__run_adb_command(["shell", "pm", "path", package_name])
         return output.strip()
 
     def start_app(self, package_name, activity_name):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "am", "start", "-n", f"{package_name}/{activity_name}"]
         )
 
     def start_service(self, package_name, service_name):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "am", "startservice", f"{package_name}/{service_name}"]
         )
 
     def stop_service(self, package_name, service_name):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "am", "stopservice", f"{package_name}/{service_name}"]
         )
 
     def send_broadcast(self, action):
-        self._run_adb_command(["shell", "am", "broadcast", "-a", action])
+        self.__run_adb_command(["shell", "am", "broadcast", "-a", action])
 
     def force_stop_app(self, package_name):
-        self._run_adb_command(["shell", "am", "force-stop", package_name])
+        self.__run_adb_command(["shell", "am", "force-stop", package_name])
 
     def trim_memory(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "am", "send-trim-memory", "org.example.package", "HIDDEN"]
         )
 
     def pull_file(self, device_path, local_path):
-        self._run_adb_command(["pull", device_path, local_path])
+        self.__run_adb_command(["pull", device_path, local_path])
 
     def push_file(self, local_path, device_path):
-        self._run_adb_command(["push", local_path, device_path])
+        self.__run_adb_command(["push", local_path, device_path])
 
     def press_power_button(self):
-        self._run_adb_command(["shell", "input", "keyevent", "26"])
+        self.__run_adb_command(["shell", "input", "keyevent", "26"])
 
     def press_menu_button(self):
-        self._run_adb_command(["shell", "input", "keyevent", "82"])
+        self.__run_adb_command(["shell", "input", "keyevent", "82"])
 
     def press_home_button(self):
-        self._run_adb_command(["shell", "input", "keyevent", "3"])
+        self.__run_adb_command(["shell", "input", "keyevent", "3"])
 
     def press_back_button(self):
-        self._run_adb_command(["shell", "input", "keyevent", "4"])
+        self.__run_adb_command(["shell", "input", "keyevent", "4"])
 
     def control_volume(self, direction):
         if direction == "up":
-            self._run_adb_command(["shell", "input", "keyevent", "24"])
+            self.__run_adb_command(["shell", "input", "keyevent", "24"])
         elif direction == "down":
-            self._run_adb_command(["shell", "input", "keyevent", "25"])
+            self.__run_adb_command(["shell", "input", "keyevent", "25"])
 
     def control_media(self, action):
         if action == "play":
-            self._run_adb_command(["shell", "input", "keyevent", "85"])
+            self.__run_adb_command(["shell", "input", "keyevent", "85"])
         elif action == "pause":
-            self._run_adb_command(["shell", "input", "keyevent", "86"])
+            self.__run_adb_command(["shell", "input", "keyevent", "86"])
         elif action == "next":
-            self._run_adb_command(["shell", "input", "keyevent", "87"])
+            self.__run_adb_command(["shell", "input", "keyevent", "87"])
         elif action == "previous":
-            self._run_adb_command(["shell", "input", "keyevent", "88"])
+            self.__run_adb_command(["shell", "input", "keyevent", "88"])
 
     def turn_on_screen(self):
-        self._run_adb_command(["shell", "input", "keyevent", "224"])
+        self.__run_adb_command(["shell", "input", "keyevent", "224"])
 
     def turn_off_screen(self):
-        self._run_adb_command(["shell", "input", "keyevent", "223"])
+        self.__run_adb_command(["shell", "input", "keyevent", "223"])
 
     def swipe_unlock(self):
-        self._run_adb_command(["shell", "input", "swipe", "100", "500", "500", "500"])
+        self.__run_adb_command(["shell", "input", "swipe", "100", "500", "500", "500"])
 
     def input_text(self, text):
-        self._run_adb_command(["shell", "input", "text", text])
+        self.__run_adb_command(["shell", "input", "text", text])
 
     def view_logcat(self):
-        self._run_adb_command(["logcat"])
+        self.__run_adb_command(["logcat"])
 
     def filter_logcat_by_level(self, log_level):
-        self._run_adb_command(["logcat", "*:" + log_level])
+        self.__run_adb_command(["logcat", "*:" + log_level])
 
     def filter_logcat_by_tag_and_level(self, tag, log_level):
-        self._run_adb_command(["logcat", tag + ":" + log_level])
+        self.__run_adb_command(["logcat", tag + ":" + log_level])
 
     def set_log_format(self, log_format):
-        self._run_adb_command(["logcat", "-v", log_format])
+        self.__run_adb_command(["logcat", "-v", log_format])
 
     def clear_logcat(self):
-        self._run_adb_command(["logcat", "-c"])
+        self.__run_adb_command(["logcat", "-c"])
 
     def view_kernel_log(self):
-        self._run_adb_command(["shell", "dmesg"])
+        self.__run_adb_command(["shell", "dmesg"])
 
     def get_device_model(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.product.model"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.product.model"])
         return output.strip()
 
     def get_battery_status(self):
-        output = self._run_adb_command(["shell", "dumpsys", "battery"])
+        output = self.__run_adb_command(["shell", "dumpsys", "battery"])
         return str_to_dict(output.strip())
 
     def get_screen_resolution(self):
-        output = self._run_adb_command(["shell", "wm", "size"])
+        output = self.__run_adb_command(["shell", "wm", "size"])
         return str_to_dict(output.strip())["Physical size"]
 
     def get_screen_density(self):
-        output = self._run_adb_command(["shell", "wm", "density"])
+        output = self.__run_adb_command(["shell", "wm", "density"])
         return str_to_dict(output.strip())["Physical density"]
 
     def get_display_info(self):
-        output = self._run_adb_command(["shell", "dumpsys", "display"])
+        output = self.__run_adb_command(["shell", "dumpsys", "display"])
         return str_to_dict(output.strip())
 
     def get_android_id(self):
-        output = self._run_adb_command(
+        output = self.__run_adb_command(
             ["shell", "settings", "get", "secure", "android_id"]
         )
         return output.strip()
 
     def get_imei(self):
-        output = self._run_adb_command(
+        output = self.__run_adb_command(
             ["shell", "service", "call", "iphonesubinfo", "1"]
         )
         return output.strip()
 
     def get_android_version(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.build.version.release"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.build.version.release"])
         return output.strip()
 
     def get_ip_address(self):
-        output = self._run_adb_command(["shell", "ifconfig", "wlan0"])
+        output = self.__run_adb_command(["shell", "ifconfig", "wlan0"])
         return output.strip()
 
     def get_mac_address(self):
-        output = self._run_adb_command(["shell", "cat", "/sys/class/net/wlan0/address"])
+        output = self.__run_adb_command(["shell", "cat", "/sys/class/net/wlan0/address"])
         return output.strip()
 
     def get_cpu_info(self):
-        output = self._run_adb_command(["shell", "cat", "/proc/cpuinfo"])
+        output = self.__run_adb_command(["shell", "cat", "/proc/cpuinfo"])
         return str_to_dict(output.strip())
 
     def get_memory_info(self):
-        output = self._run_adb_command(["shell", "cat", "/proc/meminfo"])
+        output = self.__run_adb_command(["shell", "cat", "/proc/meminfo"])
         return str_to_dict(output.strip())
 
     def print_build_prop(self):
-        output = self._run_adb_command(["shell", "cat", "/system/build.prop"])
+        output = self.__run_adb_command(["shell", "cat", "/system/build.prop"])
         return output.strip()
 
     def get_sdk(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.build.version.sdk"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.build.version.sdk"])
         return int(output.strip())
 
     def get_security_patch(self):
-        output = self._run_adb_command(
+        output = self.__run_adb_command(
             ["shell", "getprop", "ro.build.version.security_patch"]
         )
         return output.strip()
 
     def get_product_brand(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.product.brand"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.product.brand"])
         return output.strip()
 
     def get_product_name(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.product.name"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.product.name"])
         return output.strip()
 
     def get_product_board(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.product.board"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.product.board"])
         return output.strip()
 
     def get_product_cpu_abilist(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.product.cpu.abilist"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.product.cpu.abilist"])
         return output.strip()
 
     def get_abi(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.product.cpu.abi"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.product.cpu.abi"])
         return output.strip()
 
     def get_isUsbOtgEnabled(self):
-        output = self._run_adb_command(
+        output = self.__run_adb_command(
             ["shell", "getprop", "persist.sys.isUsbOtgEnabled"]
         )
         return output.strip()
 
     def get_heapsize(self):
-        output = self._run_adb_command(["shell", "getprop", "dalvik.vm.heapsize"])
+        output = self.__run_adb_command(["shell", "getprop", "dalvik.vm.heapsize"])
         return output.strip()
 
     def get_lcd_density(self):
-        output = self._run_adb_command(["shell", "getprop", "ro.sf.lcd_density"])
+        output = self.__run_adb_command(["shell", "getprop", "ro.sf.lcd_density"])
         return output.strip()
 
     def set_resolution(self, width, height):
-        self._run_adb_command(["shell", "wm", "size", f"{width}x{height}"])
+        self.__run_adb_command(["shell", "wm", "size", f"{width}x{height}"])
 
     def set_density(self, density):
-        self._run_adb_command(["shell", "wm", "density", str(density)])
+        self.__run_adb_command(["shell", "wm", "density", str(density)])
 
     def set_display_area(self, left, top, right, bottom):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "wm", "overscan", f"{left},{top},{right},{bottom}"]
         )
 
     def disable_usb_debugging(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "settings", "put", "global", "adb_enabled", "0"]
         )
 
     def allow_non_sdk_api(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "settings", "put", "global", "hidden_api_policy", "1"]
         )
 
     def disable_non_sdk_api(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "settings", "put", "global", "hidden_api_policy", "0"]
         )
 
     def hide_status_bar(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             [
                 "shell",
                 "settings",
                 "put",
                 "global",
                 "policy_control",
                 "immersive.status=*",
             ]
         )
 
     def show_status_bar(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "settings", "put", "global", "policy_control", "null"]
         )
 
     def hide_navigation_bar(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             [
                 "shell",
                 "settings",
                 "put",
                 "global",
                 "policy_control",
                 "immersive.navigation=*",
             ]
         )
 
     def show_navigation_bar(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "settings", "put", "global", "policy_control", "null"]
         )
 
     def take_screenshot(self, file_path):
-        self._run_adb_command(["exec-out", "screencap", "-p", ">", file_path])
+        self.__run_adb_command(["exec-out", "screencap", "-p", ">", file_path])
 
     def start_screen_recording(self, file_path):
-        self._run_adb_command(["shell", "screenrecord", file_path])
+        self.__run_adb_command(["shell", "screenrecord", file_path])
 
     def remount_system_partition(self):
-        self._run_adb_command(["shell", "mount", "-o", "remount,rw", "/system"])
+        self.__run_adb_command(["shell", "mount", "-o", "remount,rw", "/system"])
 
     def get_wifi_password(self, ssid):
-        output = self._run_adb_command(
+        output = self.__run_adb_command(
             [
                 "shell",
                 "su",
                 "-c",
                 f'cat /data/misc/wifi/wpa_supplicant.conf | grep -A 4 "ssid=\\"{ssid}\\""',
             ]
         )
         return output.strip()
 
     def set_date_time(self, date_time):
-        self._run_adb_command(["shell", "su", "-c", f'date -s "{date_time}"'])
+        self.__run_adb_command(["shell", "su", "-c", f'date -s "{date_time}"'])
 
     def reboot_device(self):
-        self._run_adb_command(["shell", "su", "-c", "reboot"])
+        self.__run_adb_command(["shell", "su", "-c", "reboot"])
 
     def check_root_status(self):
-        output = self._run_adb_command(["shell", "su", "-c", "id"])
+        output = self.__run_adb_command(["shell", "su", "-c", "id"])
         if "root" in output.strip():
             return True
         else:
             return False
 
     def enable_monkey_stress_test(self):
-        self._run_adb_command(["shell", "settings", "put", "global", "monkey", "0"])
+        self.__run_adb_command(["shell", "settings", "put", "global", "monkey", "0"])
 
     def disable_monkey_stress_test(self):
-        self._run_adb_command(["shell", "settings", "put", "global", "monkey", "1"])
+        self.__run_adb_command(["shell", "settings", "put", "global", "monkey", "1"])
 
     def enable_wifi(self):
-        self._run_adb_command(["shell", "svc", "wifi", "enable"])
+        self.__run_adb_command(["shell", "svc", "wifi", "enable"])
 
     def disable_wifi(self):
-        self._run_adb_command(["shell", "svc", "wifi", "disable"])
+        self.__run_adb_command(["shell", "svc", "wifi", "disable"])
 
     def reboot_recovery(self):
-        self._run_adb_command(["reboot", "recovery"])
+        self.__run_adb_command(["reboot", "recovery"])
 
     def reboot_android(self):
-        self._run_adb_command(["reboot"])
+        self.__run_adb_command(["reboot"])
 
     def reboot_fastboot(self):
-        self._run_adb_command(["reboot", "bootloader"])
+        self.__run_adb_command(["reboot", "bootloader"])
 
     def sideload_update(self, update_zip_path):
-        self._run_adb_command(["sideload", update_zip_path])
+        self.__run_adb_command(["sideload", update_zip_path])
 
     def enable_selinux(self):
-        self._run_adb_command(["shell", "setenforce", "1"])
+        self.__run_adb_command(["shell", "setenforce", "1"])
 
     def disable_selinux(self):
-        self._run_adb_command(["shell", "setenforce", "0"])
+        self.__run_adb_command(["shell", "setenforce", "0"])
 
     def enable_dm_verity(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "su", "-c", "setprop", "verity.mode", "enforcing"]
         )
 
     def disable_dm_verity(self):
-        self._run_adb_command(
+        self.__run_adb_command(
             ["shell", "su", "-c", "setprop", "verity.mode", "disabled"]
         )
 
     def swipe(self, start_x, start_y, end_x, end_y, duration=250):
         adb_command = ["shell", "input", "touchscreen", "swipe"]
         adb_command.extend(
             [str(start_x), str(start_y), str(end_x), str(end_y), str(duration)]
         )
-        self._run_adb_command(adb_command)
+        self.__run_adb_command(adb_command)
 
     def click(self, x: int, y: int, duration=150):
         adb_command = ["shell", "input", "touchscreen", "swipe"]
         adb_command.extend([str(x), str(y), str(x), str(y), str(duration)])
-        self._run_adb_command(adb_command)
+        self.__run_adb_command(adb_command)
 
     def change_file_permission(self, permission, file_path):
-        self._run_adb_command(["shell", "chmod", permission, file_path])
+        self.__run_adb_command(["shell", "chmod", permission, file_path])
 
     def check_disk_space(self):
-        output = self._run_adb_command(["shell", "df"])
+        output = self.__run_adb_command(["shell", "df"])
         return output.strip()
 
     def kill_process(self, pid):
-        self._run_adb_command(["shell", "kill", str(pid)])
+        self.__run_adb_command(["shell", "kill", str(pid)])
 
     def list_directory_contents(self, directory):
-        output = self._run_adb_command(["shell", "ls", "-la", directory])
+        output = self.__run_adb_command(["shell", "ls", "-la", directory])
         return output.strip()
 
     def move_file(self, source_path, destination_path):
-        self._run_adb_command(["shell", "mv", source_path, destination_path])
+        self.__run_adb_command(["shell", "mv", source_path, destination_path])
 
     def view_running_processes(self):
-        output = self._run_adb_command(["shell", "ps"])
+        output = self.__run_adb_command(["shell", "ps"])
         return output.strip()
 
     def remove_file(self, file_path):
-        self._run_adb_command(["shell", "rm", "-rf", file_path])
+        self.__run_adb_command(["shell", "rm", "-rf", file_path])
 
     def view_top_processes(self):
-        output = self._run_adb_command(["shell", "top", "-n", "1"])
+        output = self.__run_adb_command(["shell", "top", "-n", "1"])
         return output.strip()
 
     def get_service_list(self):
-        output = self._run_adb_command(["shell", "service", "list"])
+        output = self.__run_adb_command(["shell", "service", "list"])
         return output.strip()
 
     def get_iomem(self):
-        output = self._run_adb_command(["shell", "cat", "/proc/iomem"])
+        output = self.__run_adb_command(["shell", "cat", "/proc/iomem"])
         return output.strip()
 
     def get_procrank(self):
-        output = self._run_adb_command(["shell", "procrank"])
+        output = self.__run_adb_command(["shell", "procrank"])
         return output.strip()
 
-    def screencap_raw(self):
+    def __screencap_raw(self):
         """获取截图源数据"""
         return self.adb_command(["exec-out", "screencap", "-p"])
 
 
 def str_to_dict(str):
     dict_info = {}
     lines = str.splitlines()
@@ -566,15 +566,15 @@
         """
         screencap_raw ADB截图
 
         Returns:
             图像字节流 (bytes): 
         """
         logger.debug(f"screen by ADB")
-        return ADB.screencap_raw(self)
+        return ADB.__screencap_raw(self)
 
 
 
 class ADBtouch(Touch, ADB):
     def __init__(self, device=None) -> None:
         ADB.__init__(self, device=device)
```

### Comparing `minidevice-2.0.4/minidevice/images.py` & `minidevice-2.0.5/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.4/minidevice/minicap.py` & `minidevice-2.0.5/minidevice/minicap.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,65 +202,65 @@
         rate=15,
         quality=100,
         use_stream=True,
         ip="127.0.0.1",
     ) -> None:
         self.minicap_adb = ADB(device)
         self.use_stream = use_stream
-        self._get_device_info()
+        self.__get_device_info()
         if minicap_name is None:
             minicap_name = "minicap_{}".format(time.time())
         minicap_params = {
             "minicap_name": minicap_name,
             "rate": rate,
             "quality": quality,
             "ip": ip,
         }
-        self._get_minicap_params(**minicap_params)
+        self.__get_minicap_params(**minicap_params)
         if self.use_stream:
-            self._start_minicap_by_stream()
+            self.__start_minicap_by_stream()
 
     def screencap_raw(self) -> bytes:
         if self.use_stream:
             if self.minicap_popen.poll() is not None:
                 logger.warning("尝试重启minicap中")
-                self._stop_minicap_by_stream()
-                self._start_minicap_by_stream()
+                self.__stop_minicap_by_stream()
+                self.__start_minicap_by_stream()
             logger.debug("screen by minicap stream")
             return self.screen_queue.get()
         else:
             logger.debug("screen by minicap frame")
-            return self._minicap_frame()
+            return self.__minicap_frame()
 
-    def _minicap_frame(self):
+    def __minicap_frame(self):
         adb_command = [
             "shell",
             "LD_LIBRARY_PATH=/data/local/tmp",
             "/data/local/tmp/minicap",
         ]
         adb_command.extend(["-P", f"{self.vm_size}@{self.vm_size}/0"])
         adb_command.extend(["-Q", str(self.quality)])
         adb_command.extend(["-s"])
         raw_data = self.minicap_adb.adb_command(adb_command)
         jpg_data = raw_data.split(b"for JPG encoder\n" + line_breaker(self.sdk))[-1]
         jpg_data = jpg_data.replace(line_breaker(self.sdk), b"\n")
         return jpg_data
 
-    def _get_device_info(self):
+    def __get_device_info(self):
         self.vm_size = self.minicap_adb.get_screen_resolution()
         self.abi = self.minicap_adb.get_abi()
         self.sdk = self.minicap_adb.get_sdk()
 
-    def _get_minicap_params(self, minicap_name, quality, rate, ip):
+    def __get_minicap_params(self, minicap_name, quality, rate, ip):
         self.minicap_name = minicap_name
         self.quality = quality
         self.rate = rate
         self.ip = ip
 
-    def _minicap_available(func):
+    def __minicap_available(func):
         def wrapper(self, *args, **kwargs):
             try:
                 adb_command = [
                     "shell",
                     "LD_LIBRARY_PATH=/data/local/tmp",
                     "/data/local/tmp/minicap",
                 ]
@@ -271,29 +271,29 @@
                     return func(self, *args, **kwargs)
                 return False
             except subprocess.CalledProcessError:
                 return False
 
         return wrapper
 
-    def _minicap_install(self):
+    def __minicap_install(self):
         if self.sdk == 32 and self.abi == "x86_64":
             self.abi = "x86"
 
         MNC_HOME = "/data/local/tmp/minicap"
         MNC_SO_HOME = "/data/local/tmp/minicap.so"
 
         self.minicap_adb.push_file(f"{MINICAP_PATH}/{self.abi}/minicap", MNC_HOME)
         self.minicap_adb.push_file(
             f"{MINICAPSO_PATH}/android-{self.sdk}/{self.abi}/minicap.so", MNC_SO_HOME
         )
         self.minicap_adb.change_file_permission("+x", MNC_HOME)
 
-    @_minicap_available
-    def _start_minicap(self):
+    @__minicap_available
+    def __start_minicap(self):
         """启动adb"""
         adb_command = [ADB_PATH]
         if self.minicap_adb.device is not None:
             adb_command.extend(["-s", self.minicap_adb.device])
         adb_command.extend(
             ["shell", "LD_LIBRARY_PATH=/data/local/tmp", "/data/local/tmp/minicap"]
         )
@@ -305,35 +305,35 @@
         self.minicap_popen = subprocess.Popen(
             adb_command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
         time.sleep(2)
         logger.info("启动minicap")
         return True
 
-    def _forward_minicap(self):
+    def __forward_minicap(self):
         """端口转发"""
         self.minicap_port = self.minicap_adb.forward_port(
             "localabstract:{}".format(self.minicap_name)
         )
 
-    def _read_minicap_stream(self):
+    def __read_minicap_stream(self):
         self.minicap_stream = MinicapStream.getBuilder(self.ip, self.minicap_port)
         self.minicap_stream.run()
         self.banner = self.minicap_stream.banner
         self.screen_queue = self.minicap_stream.queue
 
-    def _start_minicap_by_stream(self):
-        if not self._start_minicap():
-            self._minicap_install()
-            if not self._start_minicap():
+    def __start_minicap_by_stream(self):
+        if not self.__start_minicap():
+            self.__minicap_install()
+            if not self.__start_minicap():
                 raise Exception("minicap不可用")
-        self._forward_minicap()
-        self._read_minicap_stream()
+        self.__forward_minicap()
+        self.__read_minicap_stream()
 
-    def _stop_minicap_by_stream(self):
+    def __stop_minicap_by_stream(self):
         self.minicap_stream.stop()  # 停止stream
         self.minicap_adb.remove_forward(self.minicap_port)  # 清理端口
         if self.minicap_popen.poll() is None:  # 清理管道
             self.minicap_popen.kill()
 
 
 if __name__ == "__main__":
```

### Comparing `minidevice-2.0.4/minidevice/minitouch.py` & `minidevice-2.0.5/minidevice/minitouch.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 WORK_DIR = os.path.dirname(__file__)
 MINITOUCH_PATH = "{}/bin/minitouch/libs".format(WORK_DIR)
 
 
 class Minitouch(Touch, MNTDevice):
     def __init__(self, device):
         self.minitouch_adb = ADB(device)
-        self._get_device_info()
-        self._minitouch_install()
+        self.__get_device_info()
+        self.__minitouch_install()
         MNTDevice.__init__(self, device)
 
-    def _get_device_info(self):
+    def __get_device_info(self):
         self.abi = self.minitouch_adb.get_abi()
 
-    def _minitouch_install(self):
+    def __minitouch_install(self):
         MNT_HOME = "/data/local/tmp/minitouch"
         self.minitouch_adb.push_file(f"{MINITOUCH_PATH}/{self.abi}/minitouch", MNT_HOME)
         self.minitouch_adb.change_file_permission("+x", MNT_HOME)
 
     def click(self, x: int, y: int, duration: int):
         """
         click minitouch 点击
@@ -41,12 +41,15 @@
         swipe 滑动
 
         Args:
             points (list): [(x,y),(x,y),(x,y)] 坐标列表
             duration (int): 持续时间. Defaults to 300.
         """
         MNTDevice.swipe(self, points, duration=duration)
-        logger.debug(f"minitouch swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms")
+        logger.debug(
+            f"minitouch swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
+        )
 
-if __name__=="__main__":
-    a=Minitouch("127.0.0.1:16384")
-    a.stop()
+
+if __name__ == "__main__":
+    a = Minitouch("127.0.0.1:16384")
+    a.stop()
```

### Comparing `minidevice-2.0.4/minidevice/screencap.py` & `minidevice-2.0.5/minidevice/screencap.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     def save_screencap(self, filename="screencap.png"):
         """
         save_screencap 保存截图
 
         Args:
             filename (str, optional): 截图保存路径. Defaults to "screencap.png".
         """
-        cv2.imwrite(filename, self.screencap_opencv())
+        cv2.imencode(ext=".jpg", img=self.screencap_opencv())[1].tofile(filename)
```

### Comparing `minidevice-2.0.4/minidevice.egg-info/PKG-INFO` & `minidevice-2.0.5/minidevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.4
+Version: 2.0.5
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.4/setup.py` & `minidevice-2.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.4',
+      version='2.0.5',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

