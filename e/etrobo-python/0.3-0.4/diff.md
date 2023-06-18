# Comparing `tmp/etrobo_python-0.3.tar.gz` & `tmp/etrobo_python-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/etrobo_python-0.3.tar", last modified: Tue May 17 10:26:37 2022, max compression
+gzip compressed data, was "dist/etrobo_python-0.4.tar", last modified: Sun Jun 18 13:12:02 2023, max compression
```

## Comparing `etrobo_python-0.3.tar` & `etrobo_python-0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.147826 etrobo_python-0.3/
--rw-r--r--   0 atushi     (501) staff       (20)     1071 2022-05-05 20:12:25.000000 etrobo_python-0.3/LICENSE
--rw-r--r--   0 atushi     (501) staff       (20)      980 2022-05-17 10:26:37.147472 etrobo_python-0.3/PKG-INFO
--rw-r--r--   0 atushi     (501) staff       (20)      578 2022-05-17 10:25:33.000000 etrobo_python-0.3/README.txt
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.139293 etrobo_python-0.3/etrobo_python/
--rw-r--r--   0 atushi     (501) staff       (20)      199 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/__init__.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.140983 etrobo_python-0.3/etrobo_python/backends/
--rw-r--r--   0 atushi     (501) staff       (20)        0 2022-05-05 20:12:25.000000 etrobo_python-0.3/etrobo_python/backends/__init__.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.142666 etrobo_python-0.3/etrobo_python/backends/pybricks/
--rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.3/etrobo_python/backends/pybricks/__init__.py
--rw-r--r--   0 atushi     (501) staff       (20)     3872 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/pybricks/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     1463 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/pybricks/dispatcher.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.145318 etrobo_python-0.3/etrobo_python/backends/raspike/
--rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/raspike/__init__.py
--rw-r--r--   0 atushi     (501) staff       (20)     9755 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/raspike/connector.py
--rw-r--r--   0 atushi     (501) staff       (20)     3146 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/raspike/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     1360 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/raspike/dispatcher.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.146929 etrobo_python-0.3/etrobo_python/backends/simulator/
--rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.3/etrobo_python/backends/simulator/__init__.py
--rw-r--r--   0 atushi     (501) staff       (20)     7238 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/simulator/connector.py
--rw-r--r--   0 atushi     (501) staff       (20)     3295 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/simulator/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     2278 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/backends/simulator/dispatcher.py
--rw-r--r--   0 atushi     (501) staff       (20)     4804 2022-05-07 15:07:21.000000 etrobo_python-0.3/etrobo_python/device.py
--rw-r--r--   0 atushi     (501) staff       (20)     5329 2022-05-17 10:25:33.000000 etrobo_python-0.3/etrobo_python/etrobo.py
-drwxr-xr-x   0 atushi     (501) staff       (20)        0 2022-05-17 10:26:37.140731 etrobo_python-0.3/etrobo_python.egg-info/
--rw-r--r--   0 atushi     (501) staff       (20)      980 2022-05-17 10:26:36.000000 etrobo_python-0.3/etrobo_python.egg-info/PKG-INFO
--rw-r--r--   0 atushi     (501) staff       (20)      770 2022-05-17 10:26:37.000000 etrobo_python-0.3/etrobo_python.egg-info/SOURCES.txt
--rw-r--r--   0 atushi     (501) staff       (20)        1 2022-05-17 10:26:36.000000 etrobo_python-0.3/etrobo_python.egg-info/dependency_links.txt
--rw-r--r--   0 atushi     (501) staff       (20)       14 2022-05-17 10:26:36.000000 etrobo_python-0.3/etrobo_python.egg-info/top_level.txt
--rw-r--r--   0 atushi     (501) staff       (20)       38 2022-05-17 10:26:37.147950 etrobo_python-0.3/setup.cfg
--rw-r--r--   0 atushi     (501) staff       (20)      643 2022-05-09 21:18:48.000000 etrobo_python-0.3/setup.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.232245 etrobo_python-0.4/
+-rw-r--r--   0 atushi     (501) staff       (20)     1071 2022-05-05 20:12:25.000000 etrobo_python-0.4/LICENSE
+-rw-r--r--   0 atushi     (501) staff       (20)      965 2023-06-18 13:12:02.231589 etrobo_python-0.4/PKG-INFO
+-rw-r--r--   0 atushi     (501) staff       (20)      578 2023-06-18 12:59:11.000000 etrobo_python-0.4/README.txt
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.222167 etrobo_python-0.4/etrobo_python/
+-rw-r--r--   0 atushi     (501) staff       (20)      199 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/__init__.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.225462 etrobo_python-0.4/etrobo_python/backends/
+-rw-r--r--   0 atushi     (501) staff       (20)        0 2022-05-05 20:12:25.000000 etrobo_python-0.4/etrobo_python/backends/__init__.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.226726 etrobo_python-0.4/etrobo_python/backends/pybricks/
+-rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.4/etrobo_python/backends/pybricks/__init__.py
+-rw-r--r--   0 atushi     (501) staff       (20)     4314 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/pybricks/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     1463 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/pybricks/dispatcher.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.228440 etrobo_python-0.4/etrobo_python/backends/raspike/
+-rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/raspike/__init__.py
+-rw-r--r--   0 atushi     (501) staff       (20)    10152 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/raspike/connector.py
+-rw-r--r--   0 atushi     (501) staff       (20)     3493 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/raspike/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     1360 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/raspike/dispatcher.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.230855 etrobo_python-0.4/etrobo_python/backends/simulator/
+-rw-r--r--   0 atushi     (501) staff       (20)       92 2022-05-05 20:12:25.000000 etrobo_python-0.4/etrobo_python/backends/simulator/__init__.py
+-rw-r--r--   0 atushi     (501) staff       (20)     7337 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/simulator/connector.py
+-rw-r--r--   0 atushi     (501) staff       (20)     3718 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/backends/simulator/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     2278 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/backends/simulator/dispatcher.py
+-rw-r--r--   0 atushi     (501) staff       (20)     6003 2023-06-18 12:59:11.000000 etrobo_python-0.4/etrobo_python/device.py
+-rw-r--r--   0 atushi     (501) staff       (20)     5329 2022-05-17 10:25:33.000000 etrobo_python-0.4/etrobo_python/etrobo.py
+drwxr-xr-x   0 atushi     (501) staff       (20)        0 2023-06-18 13:12:02.224846 etrobo_python-0.4/etrobo_python.egg-info/
+-rw-r--r--   0 atushi     (501) staff       (20)      965 2023-06-18 13:12:01.000000 etrobo_python-0.4/etrobo_python.egg-info/PKG-INFO
+-rw-r--r--   0 atushi     (501) staff       (20)      770 2023-06-18 13:12:02.000000 etrobo_python-0.4/etrobo_python.egg-info/SOURCES.txt
+-rw-r--r--   0 atushi     (501) staff       (20)        1 2023-06-18 13:12:01.000000 etrobo_python-0.4/etrobo_python.egg-info/dependency_links.txt
+-rw-r--r--   0 atushi     (501) staff       (20)       14 2023-06-18 13:12:01.000000 etrobo_python-0.4/etrobo_python.egg-info/top_level.txt
+-rw-r--r--   0 atushi     (501) staff       (20)       38 2023-06-18 13:12:02.232439 etrobo_python-0.4/setup.cfg
+-rw-r--r--   0 atushi     (501) staff       (20)      648 2023-06-18 12:59:11.000000 etrobo_python-0.4/setup.py
```

### Comparing `etrobo_python-0.3/LICENSE` & `etrobo_python-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.3/PKG-INFO` & `etrobo_python-0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: etrobo_python
-Version: 0.3
-Summary: Python middleware for ET-ROBOCON 2022.
+Version: 0.4
+Summary: Python middleware for ET-ROBOCON 2023.
 Home-page: https://github.com/takedarts/etrobo-python
 Author: Atsushi TAKEDA
-Author-email: takeda@cs.tohoku-gakuin.ac.jp
+Author-email: takedarts@mail.tohoku-gakuin.ac.jp
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python middleware for ET-ROBOCON 2022.
+Python middleware for ET-ROBOCON 2023.
 
 This is a python middleware to develop embedded programs to control robots at
-ET-ROBOCON 2022 which is a embedded software contest in Japan. Using this
+ET-ROBOCON 2023 which is a embedded software contest in Japan. Using this
 middleware, developers can write python programs that run both in robots
 (ev3dev/raspike) and simulators. See the following GitHub repository, if you
 would like to know more about this middleware (This repository supports only
 Japanese, and does not have a planto support English).
 
-ET-ROBOCON 2022:
+ET-ROBOCON 2023:
 https://www.etrobo.jp/
 
 Github repository:
 https://github.com/takedarts/etrobo-python
-
-
```

### Comparing `etrobo_python-0.3/README.txt` & `etrobo_python-0.4/README.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Python middleware for ET-ROBOCON 2022.
+Python middleware for ET-ROBOCON 2023.
 
 This is a python middleware to develop embedded programs to control robots at
-ET-ROBOCON 2022 which is a embedded software contest in Japan. Using this
+ET-ROBOCON 2023 which is a embedded software contest in Japan. Using this
 middleware, developers can write python programs that run both in robots
 (ev3dev/raspike) and simulators. See the following GitHub repository, if you
 would like to know more about this middleware (This repository supports only
 Japanese, and does not have a planto support English).
 
-ET-ROBOCON 2022:
+ET-ROBOCON 2023:
 https://www.etrobo.jp/
 
 Github repository:
 https://github.com/takedarts/etrobo-python
```

### Comparing `etrobo_python-0.3/etrobo_python/backends/pybricks/device.py` & `etrobo_python-0.4/etrobo_python/backends/raspike/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,140 +1,132 @@
 import time
+from typing import Any, Tuple
 
 import etrobo_python
 
-import pybricks.ev3devices as ev3dev
-import pybricks.hubs as hubs
-from pybricks.parameters import Port, Color
-
-try:
-    from typing import Any, Tuple
-except BaseException:
-    pass
+from . import connector
 
 
 def create_device(device_type: str, port: str) -> Any:
     if device_type == 'hub':
         return Hub()
-
-    ev3_port = get_ev3_port(port)
-
-    if device_type == 'motor':
-        return Motor(ev3_port)
+    elif device_type == 'motor':
+        return Motor(get_raspike_port(port))
     elif device_type == 'color_sensor':
-        return ColorSensor(ev3_port)
+        return ColorSensor()
     elif device_type == 'touch_sensor':
-        return TouchSensor(ev3_port)
+        return TouchSensor()
     elif device_type == 'sonar_sensor':
-        return SonarSensor(ev3_port)
+        return SonarSensor()
     elif device_type == 'gyro_sensor':
-        return GyroSensor(ev3_port)
+        return GyroSensor()
     else:
-        raise NotImplementedError(
-            'Unsupported device: {}'.format(device_type))
+        raise NotImplementedError(f'Unsupported device: {device_type}')
 
 
-def get_ev3_port(port: str) -> Port:
+def get_raspike_port(port: str) -> int:
     port_names = ('A', 'B', 'C', 'D', '1', '2', '3', '4')
-    port_values = (Port.A, Port.B, Port.C, Port.D,
-                   Port.S1, Port.S2, Port.S3, Port.S4)
+    port_values = (0, 1, 2, -1, -1, -1, -1, -1)
 
     if port in port_names:
         return port_values[port_names.index(port)]
     else:
-        raise Exception('Unknown port: {}'.format(port))
+        raise Exception(f'Unknown port: {port}')
 
 
 class Hub(object):
-    def __init__(self) -> None:
-        self.ev3brick = hubs.EV3Brick()
+    def __init__(self):
+        self.hub = connector.Hub()
 
     def set_led(self, color: str) -> None:
-        color_value = color.lower()[0]
-        if color_value == 'r':
-            self.ev3brick.light.on(Color.RED)
-        elif color_value == 'g':
-            self.ev3brick.light.on(Color.GREEN)
-        elif color_value == 'o':
-            self.ev3brick.light.on(Color.ORANGE)
-        else:
-            self.ev3brick.light.on(Color.BLACK)
+        pass
 
     def get_time(self) -> float:
         return time.time()
 
     def get_battery_voltage(self) -> int:
-        return self.ev3brick.battery.voltage()
+        return self.hub.get_battery_voltage()
 
     def get_battery_current(self) -> int:
-        return self.ev3brick.battery.current()
+        return self.hub.get_battery_current()
 
     def play_speaker_tone(self, frequency: int, duration: float) -> None:
-        self.ev3brick.speaker.beep(frequency, round(duration * 1000))
+        pass
 
     def set_speaker_volume(self, volume: int) -> None:
-        self.ev3brick.speaker.set_volume(volume)
+        pass
+
+    def is_left_button_pressed(self) -> bool:
+        return (self.hub.get_button_pressed() & 0x01) != 0
+
+    def is_right_button_pressed(self) -> bool:
+        return (self.hub.get_button_pressed() & 0x02) != 0
+
+    def is_up_button_pressed(self) -> bool:
+        return False
+
+    def is_down_button_pressed(self) -> bool:
+        return False
 
 
 class Motor(etrobo_python.Motor):
-    def __init__(self, port: Port) -> None:
-        self.motor = ev3dev.Motor(port)
+    def __init__(self, port: int) -> None:
+        self.motor = connector.Motor(port)
 
     def get_count(self) -> int:
-        return self.motor.angle()
+        return self.motor.get_count()
 
     def reset_count(self) -> None:
-        self.motor.reset_angle(0)
+        self.motor.reset_count()
 
     def set_power(self, power: int) -> None:
-        self.motor.run(power)
+        self.motor.set_pwm(power)
 
     def set_brake(self, brake: bool) -> None:
-        if brake:
-            self.motor.brake()
+        self.motor.set_brake(brake)
 
 
 class ColorSensor(etrobo_python.ColorSensor):
-    def __init__(self, port: Port) -> None:
-        self.color_sensor = ev3dev.ColorSensor(port)
+    def __init__(self) -> None:
+        self.color_sensor = connector.ColorSensor()
 
     def get_brightness(self) -> int:
-        return self.color_sensor.reflection()
+        return self.color_sensor.get_brightness()
 
     def get_ambient(self) -> int:
-        return self.color_sensor.ambient()
+        return self.color_sensor.get_ambient()
 
     def get_raw_color(self) -> Tuple[int, int, int]:
-        return self.color_sensor.rgb()
+        return self.color_sensor.get_raw_color()
 
 
 class TouchSensor(etrobo_python.TouchSensor):
-    def __init__(self, port: Port) -> None:
-        self.touch_sensor = ev3dev.TouchSensor(port)
+    def __init__(self) -> None:
+        self.touch_sensor = connector.TouchSensor()
 
     def is_pressed(self) -> bool:
-        return self.touch_sensor.pressed()
+        return self.touch_sensor.is_pressed()
 
 
 class SonarSensor(etrobo_python.SonarSensor):
-    def __init__(self, port: Port) -> None:
-        self.sonar_sensor = ev3dev.UltrasonicSensor(port)
+    def __init__(self) -> None:
+        self.sonar_sensor = connector.SonarSensor()
 
     def listen(self) -> bool:
-        return self.sonar_sensor.presence()
+        return self.sonar_sensor.listen()
 
     def get_distance(self) -> int:
-        return self.sonar_sensor.distance()
+        return self.sonar_sensor.get_distance()
 
 
 class GyroSensor(etrobo_python.GyroSensor):
-    def __init__(self, port: Port) -> None:
-        self.gyro_sensor = ev3dev.GyroSensor(port)
+    def __init__(self) -> None:
+        self.gyro_sensor = connector.GyroSensor()
 
     def reset(self) -> None:
-        self.gyro_sensor.reset_angle(0)
+        self.gyro_sensor.reset()
 
     def get_angle(self) -> int:
-        return self.gyro_sensor.angle()
+        return self.gyro_sensor.get_angle()
 
     def get_angler_velocity(self) -> int:
-        return self.gyro_sensor.speed()
+        return self.gyro_sensor.get_angler_velocity()
```

### Comparing `etrobo_python-0.3/etrobo_python/backends/pybricks/dispatcher.py` & `etrobo_python-0.4/etrobo_python/backends/pybricks/dispatcher.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.3/etrobo_python/backends/raspike/connector.py` & `etrobo_python-0.4/etrobo_python/backends/raspike/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import threading
 import time
 from typing import Callable, Optional, Tuple
 
 import serial
 
+# モーターの回転方向
+# モーターの設定値と取得値の方向を設定する
+# +1 か -1 を設定すること
+MOTOR_SIGN = -1
+
 _CONNECTOR: Optional['_Connector'] = None
 
 # 受信データ
 # バッファ内の位置: 命令番号 - 意味
 # 00:  1 - カラーセンサ（ambient)
 # 01:  2 - カラーセンサ（color）
 # 02:  3 - カラーセンサ（reflect）
@@ -20,16 +25,17 @@
 # 09: 23 - 超音波センサ（Listen）
 # 10: 28 - タッチセンサ（Pressed）
 # 11: 29 - バッテリ電流
 # 12: 30 - バッテリ電圧
 # 13: 64 - モータA（Count）
 # 14: 65 - モータB（Count）
 # 15: 66 - モータC（Count）
+# 16:  0 - 本体のボタン(左:+1, 右:+2, 中央:+16)
 _RECV_CMD_INDEX = [
-    -1, 0, 1, 2, 3, 4, 5, 6, 7, -1,
+    16, 0, 1, 2, 3, 4, 5, 6, 7, -1,
     -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
     -1, -1, 8, 9, -1, -1, -1, -1, 10, 11,
     12, -1, -1, -1, -1, -1, -1, -1, -1, -1,
     -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
     -1, -1, -1, -1, -1, -1, -1, -1, -1, -1,
     -1, -1, -1, -1, 13, 14, 15, -1, -1, -1,
 ]
@@ -109,15 +115,15 @@
         port: str,
         baudrate: int,
         timeout: float,
     ) -> None:
         self.handler = handler
         self.interval = interval
 
-        self.recv_data = [0] * 16
+        self.recv_data = [0] * (max(_RECV_CMD_INDEX) + 1)
         self.send_data = bytearray(3)
         self.running = False
 
         self.serial = serial.Serial(
             port=port, baudrate=baudrate, timeout=timeout)
         self.event = threading.Event()
 
@@ -181,15 +187,15 @@
                     self.event.set()
                     continue
 
                 # 命令と値を取り出す
                 command, value = _parse_received_command(buffer)
 
                 # 受信データを反映する
-                if 0 <= command < len(_RECV_CMD_INDEX):
+                if 0 <= command < len(_RECV_CMD_INDEX) and _RECV_CMD_INDEX[command] != -1:
                     self.recv_data[_RECV_CMD_INDEX[command]] = value
         finally:
             self.running = False
 
     def _run_handler(self) -> None:
         previous_time = 0
 
@@ -243,27 +249,31 @@
 class Hub(object):
     def get_battery_voltage(self) -> int:
         return _get_connector().recv_data[12]
 
     def get_battery_current(self) -> int:
         return _get_connector().recv_data[11]
 
+    def get_button_pressed(self) -> int:
+        return _get_connector().recv_data[16]
+
 
 class Motor(object):
     def __init__(self, port: int) -> None:
         self.port = port
 
     def get_count(self) -> int:
-        return _get_connector().recv_data[13 + self.port]
+        return MOTOR_SIGN * _get_connector().recv_data[13 + self.port]
 
     def reset_count(self) -> None:
         _get_connector().send_command(
             command=9 + self.port, value=0, wait_for_ack=True)
 
     def set_pwm(self, power: int) -> None:
+        power = MOTOR_SIGN * power
         _get_connector().send_command(
             command=1 + self.port, value=power, wait_for_ack=False)
 
     def set_brake(self, brake: bool) -> None:
         _get_connector().send_command(
             command=1 + self.port, value=int(brake), wait_for_ack=False)
```

### Comparing `etrobo_python-0.3/etrobo_python/backends/raspike/device.py` & `etrobo_python-0.4/etrobo_python/backends/simulator/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,80 @@
-import time
 from typing import Any, Tuple
 
 import etrobo_python
-
 from . import connector
 
 
 def create_device(device_type: str, port: str) -> Any:
     if device_type == 'hub':
         return Hub()
     elif device_type == 'motor':
-        return Motor(get_raspike_port(port))
+        return Motor(get_sim_port(port))
     elif device_type == 'color_sensor':
         return ColorSensor()
     elif device_type == 'touch_sensor':
         return TouchSensor()
     elif device_type == 'sonar_sensor':
         return SonarSensor()
     elif device_type == 'gyro_sensor':
         return GyroSensor()
     else:
         raise NotImplementedError(f'Unsupported device: {device_type}')
 
 
-def get_raspike_port(port: str) -> int:
+def get_sim_port(port: str) -> int:
     port_names = ('A', 'B', 'C', 'D', '1', '2', '3', '4')
-    port_values = (0, 1, 2, -1, -1, -1, -1, -1)
+    port_values = (0, 1, 2, 3, -1, -1, -1, -1)
 
     if port in port_names:
         return port_values[port_names.index(port)]
     else:
         raise Exception(f'Unknown port: {port}')
 
 
 class Hub(object):
     def __init__(self):
         self.hub = connector.Hub()
 
     def set_led(self, color: str) -> None:
-        pass
+        color_value = color.lower()[0]
+        color_names = ('b', 'r', 'g', 'o')
+
+        if color_value in color_names:
+            self.hub.set_led(color_names.index(color_value))
+        else:
+            self.hub.set_led(0)
 
     def get_time(self) -> float:
-        return time.time()
+        return self.hub.get_time()
 
     def get_battery_voltage(self) -> int:
-        return self.hub.get_battery_voltage()
+        return 8000
 
     def get_battery_current(self) -> int:
-        return self.hub.get_battery_current()
+        return 200
 
     def play_speaker_tone(self, frequency: int, duration: float) -> None:
         pass
 
     def set_speaker_volume(self, volume: int) -> None:
         pass
 
+    def is_left_button_pressed(self) -> bool:
+        return (self.hub.get_button_pressed() & 0x01) != 0
+
+    def is_right_button_pressed(self) -> bool:
+        return (self.hub.get_button_pressed() & 0x02) != 0
+
+    def is_up_button_pressed(self) -> bool:
+        return (self.hub.get_button_pressed() & 0x04) != 0
+
+    def is_down_button_pressed(self) -> bool:
+        return (self.hub.get_button_pressed() & 0x08) != 0
+
 
 class Motor(etrobo_python.Motor):
     def __init__(self, port: int) -> None:
         self.motor = connector.Motor(port)
 
     def get_count(self) -> int:
         return self.motor.get_count()
```

### Comparing `etrobo_python-0.3/etrobo_python/backends/raspike/dispatcher.py` & `etrobo_python-0.4/etrobo_python/backends/raspike/dispatcher.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.3/etrobo_python/backends/simulator/connector.py` & `etrobo_python-0.4/etrobo_python/backends/simulator/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,17 @@
 class Hub(object):
     def set_led(self, color: int) -> None:
         _get_connector().write_values('<I', 32, color)
 
     def get_time(self) -> float:
         return _get_connector().recv_time / 1_000_000
 
+    def get_button_pressed(self) -> int:
+        return _get_connector().read_values('<i', 32)[0]
+
 
 class Motor(object):
     def __init__(self, port: int) -> None:
         self.port = port
 
     def get_count(self) -> int:
         return _get_connector().read_values('<i', 288 + self.port * 4)[0]
```

### Comparing `etrobo_python-0.3/etrobo_python/backends/simulator/dispatcher.py` & `etrobo_python-0.4/etrobo_python/backends/simulator/dispatcher.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.3/etrobo_python/device.py` & `etrobo_python-0.4/etrobo_python/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,14 +56,50 @@
         シミュレータ環境の場合は何もしない。
 
         Args:
             volume: スピーカーの音量（単位は%）。
         '''
         raise NotImplementedError()
 
+    def is_left_button_pressed(self) -> bool:
+        '''左ボタンの状態を返す。
+        左ボタンが押されていればTrueを返し、押されていなければFalseを返す。
+
+        Returns:
+            左ボタンの状態。
+        '''
+        raise NotImplementedError()
+
+    def is_right_button_pressed(self) -> bool:
+        '''右ボタンの状態を返す。
+        右ボタンが押されていればTrueを返し、押されていなければFalseを返す。
+
+        Returns:
+            右ボタンの状態。
+        '''
+        raise NotImplementedError()
+
+    def is_up_button_pressed(self) -> bool:
+        '''上ボタンの状態を返す。
+        上ボタンが押されていればTrueを返し、押されていなければFalseを返す。
+
+        Returns:
+            上ボタンの状態。
+        '''
+        raise NotImplementedError()
+
+    def is_down_button_pressed(self) -> bool:
+        '''下ボタンの状態を返す。
+        下ボタンが押されていればTrueを返し、押されていなければFalseを返す。
+
+        Returns:
+            下ボタンの状態。
+        '''
+        raise NotImplementedError()
+
 
 class Device(object):
     pass
 
 
 class Motor(Device):
     def get_count(self) -> int:
```

### Comparing `etrobo_python-0.3/etrobo_python/etrobo.py` & `etrobo_python-0.4/etrobo_python/etrobo.py`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.3/etrobo_python.egg-info/PKG-INFO` & `etrobo_python-0.4/etrobo_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: etrobo-python
-Version: 0.3
-Summary: Python middleware for ET-ROBOCON 2022.
+Version: 0.4
+Summary: Python middleware for ET-ROBOCON 2023.
 Home-page: https://github.com/takedarts/etrobo-python
 Author: Atsushi TAKEDA
-Author-email: takeda@cs.tohoku-gakuin.ac.jp
+Author-email: takedarts@mail.tohoku-gakuin.ac.jp
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python middleware for ET-ROBOCON 2022.
+Python middleware for ET-ROBOCON 2023.
 
 This is a python middleware to develop embedded programs to control robots at
-ET-ROBOCON 2022 which is a embedded software contest in Japan. Using this
+ET-ROBOCON 2023 which is a embedded software contest in Japan. Using this
 middleware, developers can write python programs that run both in robots
 (ev3dev/raspike) and simulators. See the following GitHub repository, if you
 would like to know more about this middleware (This repository supports only
 Japanese, and does not have a planto support English).
 
-ET-ROBOCON 2022:
+ET-ROBOCON 2023:
 https://www.etrobo.jp/
 
 Github repository:
 https://github.com/takedarts/etrobo-python
-
-
```

### Comparing `etrobo_python-0.3/etrobo_python.egg-info/SOURCES.txt` & `etrobo_python-0.4/etrobo_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etrobo_python-0.3/setup.py` & `etrobo_python-0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 import etrobo_python
 
 setuptools.setup(
     name='etrobo_python',
     version=etrobo_python.__version__,
     author=etrobo_python.__author__,
-    author_email='takeda@cs.tohoku-gakuin.ac.jp',
+    author_email='takedarts@mail.tohoku-gakuin.ac.jp',
     license='MIT',
     description=pathlib.Path('README.txt').read_text().split('\n')[0],
     long_description=pathlib.Path('README.txt').read_text(),
     url='https://github.com/takedarts/etrobo-python',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

