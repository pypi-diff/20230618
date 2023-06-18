# Comparing `tmp/HAP-python-4.6.0.tar.gz` & `tmp/HAP-python-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HAP-python-4.6.0.tar", last modified: Sat Dec 10 09:22:27 2022, max compression
+gzip compressed data, was "HAP-python-4.7.0.tar", last modified: Sun Jun 18 12:00:48 2023, max compression
```

## Comparing `HAP-python-4.6.0.tar` & `HAP-python-4.7.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ivankalchev   (501) staff       (20)        0 2022-12-10 09:22:27.000000 HAP-python-4.6.0/
-drwxr-xr-x   0 ivankalchev   (501) staff       (20)        0 2022-12-10 09:22:22.000000 HAP-python-4.6.0/HAP_python.egg-info/
--rw-r--r--   0 ivankalchev   (501) staff       (20)    15777 2022-12-10 09:22:10.000000 HAP-python-4.6.0/HAP_python.egg-info/PKG-INFO
--rw-r--r--   0 ivankalchev   (501) staff       (20)      676 2022-12-10 09:22:11.000000 HAP-python-4.6.0/HAP_python.egg-info/SOURCES.txt
--rw-r--r--   0 ivankalchev   (501) staff       (20)        1 2022-12-10 09:22:10.000000 HAP-python-4.6.0/HAP_python.egg-info/dependency_links.txt
--rw-r--r--   0 ivankalchev   (501) staff       (20)      101 2022-12-10 09:22:10.000000 HAP-python-4.6.0/HAP_python.egg-info/requires.txt
--rw-r--r--   0 ivankalchev   (501) staff       (20)        6 2022-12-10 09:22:10.000000 HAP-python-4.6.0/HAP_python.egg-info/top_level.txt
--rw-r--r--   0 ivankalchev   (501) staff       (20)    12247 2021-08-22 20:16:19.000000 HAP-python-4.6.0/LICENSE
--rw-r--r--   0 ivankalchev   (501) staff       (20)       61 2021-08-22 20:16:19.000000 HAP-python-4.6.0/MANIFEST.in
--rw-r--r--   0 ivankalchev   (501) staff       (20)    15777 2022-12-10 09:22:27.000000 HAP-python-4.6.0/PKG-INFO
--rw-r--r--   0 ivankalchev   (501) staff       (20)    12338 2021-08-22 20:16:19.000000 HAP-python-4.6.0/README.md
-drwxr-xr-x   0 ivankalchev   (501) staff       (20)        0 2022-12-10 09:22:26.000000 HAP-python-4.6.0/pyhap/
--rw-r--r--   0 ivankalchev   (501) staff       (20)      497 2021-08-22 20:23:44.000000 HAP-python-4.6.0/pyhap/__init__.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)    13393 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/accessory.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)    35108 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/accessory_driver.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)    34138 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/camera.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)    13435 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/characteristic.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     2709 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/const.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     4523 2021-08-22 20:23:44.000000 HAP-python-4.6.0/pyhap/encoder.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     4207 2022-06-28 11:57:47.000000 HAP-python-4.6.0/pyhap/hap_crypto.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)      551 2021-08-22 20:23:44.000000 HAP-python-4.6.0/pyhap/hap_event.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)    28527 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/hap_handler.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)    10729 2022-06-28 11:57:47.000000 HAP-python-4.6.0/pyhap/hap_protocol.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     3104 2021-08-22 20:16:19.000000 HAP-python-4.6.0/pyhap/hap_server.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     3344 2021-08-22 20:16:19.000000 HAP-python-4.6.0/pyhap/hsrp.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     1936 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/iid_manager.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     2329 2021-10-07 21:06:41.000000 HAP-python-4.6.0/pyhap/loader.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     1254 2021-08-22 20:16:19.000000 HAP-python-4.6.0/pyhap/params.py
-drwxr-xr-x   0 ivankalchev   (501) staff       (20)        0 2022-12-10 09:22:26.000000 HAP-python-4.6.0/pyhap/resources/
--rw-r--r--   0 ivankalchev   (501) staff       (20)    35625 2022-12-10 09:19:03.000000 HAP-python-4.6.0/pyhap/resources/characteristics.json
--rw-r--r--   0 ivankalchev   (501) staff       (20)    14516 2022-12-10 09:19:04.000000 HAP-python-4.6.0/pyhap/resources/services.json
--rw-r--r--   0 ivankalchev   (501) staff       (20)   203005 2021-08-22 20:16:19.000000 HAP-python-4.6.0/pyhap/resources/snapshot.jpg
--rw-r--r--   0 ivankalchev   (501) staff       (20)     4653 2022-12-10 09:19:04.000000 HAP-python-4.6.0/pyhap/service.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     3118 2021-08-22 20:23:44.000000 HAP-python-4.6.0/pyhap/state.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     2212 2021-10-07 21:06:41.000000 HAP-python-4.6.0/pyhap/tlv.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)     4144 2022-12-10 09:19:04.000000 HAP-python-4.6.0/pyhap/util.py
--rw-r--r--   0 ivankalchev   (501) staff       (20)      107 2022-12-10 09:22:27.000000 HAP-python-4.6.0/setup.cfg
--rw-r--r--   0 ivankalchev   (501) staff       (20)     1887 2022-06-28 11:57:47.000000 HAP-python-4.6.0/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.479140 HAP-python-4.7.0/
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.473441 HAP-python-4.7.0/HAP_python.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)    13612 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      691 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      101 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        6 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/top_level.txt
+-rw-r--r--   0 ivan       (501) staff       (20)    12247 2023-06-18 11:42:25.000000 HAP-python-4.7.0/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)       61 2023-06-18 11:42:25.000000 HAP-python-4.7.0/MANIFEST.in
+-rw-r--r--   0 ivan       (501) staff       (20)    13612 2023-06-18 12:00:48.479205 HAP-python-4.7.0/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)    12362 2023-06-18 11:59:57.000000 HAP-python-4.7.0/README.md
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.478281 HAP-python-4.7.0/pyhap/
+-rw-r--r--   0 ivan       (501) staff       (20)      497 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)    13393 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/accessory.py
+-rw-r--r--   0 ivan       (501) staff       (20)    35373 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/accessory_driver.py
+-rw-r--r--   0 ivan       (501) staff       (20)    34138 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/camera.py
+-rw-r--r--   0 ivan       (501) staff       (20)    13435 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/characteristic.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2709 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/const.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4928 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/encoder.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4207 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_crypto.py
+-rw-r--r--   0 ivan       (501) staff       (20)      551 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_event.py
+-rw-r--r--   0 ivan       (501) staff       (20)    30302 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/hap_handler.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10729 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_protocol.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3104 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_server.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3344 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hsrp.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1936 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/iid_manager.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2371 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/loader.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1254 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/params.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.478778 HAP-python-4.7.0/pyhap/resources/
+-rw-r--r--   0 ivan       (501) staff       (20)    35625 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/resources/characteristics.json
+-rw-r--r--   0 ivan       (501) staff       (20)    14516 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/resources/services.json
+-rw-r--r--   0 ivan       (501) staff       (20)   203005 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/resources/snapshot.jpg
+-rw-r--r--   0 ivan       (501) staff       (20)     4653 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/service.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4010 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/state.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2212 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/tlv.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4156 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/util.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2648 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)      107 2023-06-18 12:00:48.479519 HAP-python-4.7.0/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1887 2023-06-18 11:42:25.000000 HAP-python-4.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `HAP-python-4.6.0/HAP_python.egg-info/PKG-INFO` & `HAP-python-4.7.0/HAP_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,292 +1,16 @@
 Metadata-Version: 2.1
 Name: HAP-python
-Version: 4.6.0
+Version: 4.7.0
 Summary: HomeKit Accessory Protocol implementation in python
 Home-page: https://github.com/ikalchev/HAP-python
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/ikalchev/HAP-python/issues
 Project-URL: Documentation, http://hap-python.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ikalchev/HAP-python/tree/master
-Description: [![PyPI version](https://badge.fury.io/py/HAP-python.svg)](https://badge.fury.io/py/HAP-python) [![Build Status](https://github.com/ikalchev/HAP-python/workflows/CI/badge.svg)](https://github.com/ikalchev/HAP-python) [![codecov](https://codecov.io/gh/ikalchev/HAP-python/branch/master/graph/badge.svg)](https://codecov.io/gh/ikalchev/HAP-python) [![Python Versions](https://img.shields.io/pypi/pyversions/HAP-python.svg)](https://pypi.python.org/pypi/HAP-python/) [![Documentation Status](https://readthedocs.org/projects/hap-python/badge/?version=latest)](http://hap-python.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/hap-python)](https://pepy.tech/project/hap-python)
-        # HAP-python
-        
-        HomeKit Accessory Protocol implementation in python 3.
-        With this project, you can integrate your own smart devices and add them to your
-        iOS Home app. Since Siri is integrated with the Home app, you can start voice-control your
-        accessories right away.
-        
-        Main features:
-        
-        * Camera - HAP-python supports the camera accessory from version 2.3.0!
-        * asyncio support - You can run various tasks or accessories in the event loop.
-        * Out of the box support for Apple-defined services - see them in [the resources folder](pyhap/resources).
-        * Secure pairing by just scanning the QR code.
-        * Integrated with the home automation framework [Home Assistant](https://github.com/home-assistant/home-assistant).
-        
-        The project was developed for a Raspberry Pi, but it should work on other platforms. To kick-start things,
-        you can open `main.py` or `busy_home.py`, where you will find some fake accessories.
-        Just run one of them, for example `python3 busy_home.py`, and you can add it in
-        the Home app (be sure to be in the same network).
-        Stop it by hitting Ctrl+C.
-        
-        There are example accessories as well as integrations with real products
-        in [the accessories folder](accessories). See how to configure your camera in
-        [camera_main.py](camera_main.py).
-        
-        ## Table of Contents
-        1. [API](#API)
-        2. [Installation](#Installation)
-        3. [Setting up a camera](#Camera)
-        4. [Run at boot (and a Switch to shutdown your device)](#AtBoot)
-        5. [Notice](#Notice)
-        
-        ## Installation <a name="Installation"></a>
-        
-        As of version 3.5.1, HAP-python no longer supports python older than 3.6, because we
-        are moving to asyncio. If your platform does not have a compatible python out of the
-        box, you can install it manually or just use an older version of HAP-python.
-        
-        As a prerequisite, you will need Avahi/Bonjour installed (due to zeroconf package).
-        On a Raspberry Pi, you can get it with:
-        ```
-        $ sudo apt-get install libavahi-compat-libdnssd-dev
-        ```
-        `avahi-utils` may also fit the bill. Then, you can install with `pip3` (you will need `sudo` or `--user` for the install):
-        ```sh
-        $ pip3 install HAP-python[QRCode]
-        ```
-        
-        This will install HAP-python in your python packages, so that you can import it as `pyhap`. To uninstall, just do:
-        ```
-        $ pip3 uninstall HAP-python
-        ```
-        
-        ## API <a name="API"></a>
-        
-        A typical flow for using HAP-python starts with implementing an Accessory. This is done by
-        subclassing [Accessory](pyhap/accessory.py) and putting in place a few details
-        (see below). After that, you give your accessory to an AccessoryDriver to manage. This
-        will take care of advertising it on the local network, setting a HAP server and
-        running the Accessory. Take a look at [main.py](main.py) for a quick start on that.
-        
-        ```python
-        from pyhap.accessory import Accessory, Category
-        import pyhap.loader as loader
-        
-        class TemperatureSensor(Accessory):
-            """Implementation of a mock temperature sensor accessory."""
-        
-            category = Category.SENSOR  # This is for the icon in the iOS Home app.
-        
-            def __init__(self, *args, **kwargs):
-                """Here, we just store a reference to the current temperature characteristic and
-                add a method that will be executed every time its value changes.
-                """
-                # If overriding this method, be sure to call the super's implementation first.
-                super().__init__(*args, **kwargs)
-        
-                # Add the services that this Accessory will support with add_preload_service here
-                temp_service = self.add_preload_service('TemperatureSensor')
-                self.temp_char = temp_service.get_characteristic('CurrentTemperature')
-        
-                # Having a callback is optional, but you can use it to add functionality.
-                self.temp_char.setter_callback = self.temperature_changed
-        
-            def temperature_changed(self, value):
-                """This will be called every time the value of the CurrentTemperature
-                is changed. Use setter_callbacks to react to user actions, e.g. setting the
-                lights On could fire some GPIO code to turn on a LED (see pyhap/accessories/LightBulb.py).
-                """
-                print('Temperature changed to: ', value)
-        
-            @Acessory.run_at_interval(3)  # Run this method every 3 seconds
-            # The `run` method can be `async` as well
-            def run(self):
-                """We override this method to implement what the accessory will do when it is
-                started.
-        
-                We set the current temperature to a random number. The decorator runs this method
-                every 3 seconds.
-                """
-                self.temp_char.set_value(random.randint(18, 26))
-        
-            # The `stop` method can be `async` as well
-            def stop(self):
-                """We override this method to clean up any resources or perform final actions, as
-                this is called by the AccessoryDriver when the Accessory is being stopped.
-                """
-                print('Stopping accessory.')
-        ```
-        
-        ## Service Callbacks
-        
-        When you are working with tightly coupled characteristics such as "On" and "Brightness,"
-        you may need to use a service callback to receive all changes in a single request.
-        
-        With characteristic callbacks, you do now know that a "Brightness" characteristic is
-        about to be processed right after an "On" and may end up setting a LightBulb to 100%
-        and then dim it back down to the expected level.
-        
-        ```python
-        from pyhap.accessory import Accessory
-        from pyhap.const import Category
-        import pyhap.loader as loader
-        
-        class Light(Accessory):
-            """Implementation of a mock light accessory."""
-        
-            category = Category.CATEGORY_LIGHTBULB  # This is for the icon in the iOS Home app.
-        
-            def __init__(self, *args, **kwargs):
-                """Here, we just store a reference to the on and brightness characteristics and
-                add a method that will be executed every time their value changes.
-                """
-                # If overriding this method, be sure to call the super's implementation first.
-                super().__init__(*args, **kwargs)
-        
-                # Add the services that this Accessory will support with add_preload_service here
-                serv_light = self.add_preload_service('Lightbulb')
-                self.char_on = serv_light.configure_char('On', value=self._state)
-                self.char_brightness = serv_light.configure_char('Brightness', value=100)
-        
-                serv_light.setter_callback = self._set_chars
-        
-            def _set_chars(self, char_values):
-                """This will be called every time the value of the on of the
-                characteristics on the service changes.
-                """
-                if "On" in char_values:
-                    print('On changed to: ', char_values["On"])
-                if "Brightness" in char_values:
-                    print('Brightness changed to: ', char_values["Brightness"])
-        
-            @Acessory.run_at_interval(3)  # Run this method every 3 seconds
-            # The `run` method can be `async` as well
-            def run(self):
-                """We override this method to implement what the accessory will do when it is
-                started.
-        
-                We set the current temperature to a random number. The decorator runs this method
-                every 3 seconds.
-                """
-                self.char_on.set_value(random.randint(0, 1))
-                self.char_brightness.set_value(random.randint(1, 100))
-        
-            # The `stop` method can be `async` as well
-            def stop(self):
-                """We override this method to clean up any resources or perform final actions, as
-                this is called by the AccessoryDriver when the Accessory is being stopped.
-                """
-                print('Stopping accessory.')
-        ```
-        
-        ## Setting up a camera <a name="Camera"></a>
-        
-        The [Camera accessory](pyhap/camera.py) implements the HomeKit Protocol for negotiating stream settings,
-        such as the picture width and height, number of audio channels and others.
-        Starting a video and/or audio stream is very platform specific. Because of this,
-        you need to figure out what video and audio settings your camera supports and set them
-        in the `options` parameter that is passed to the `Camera` Accessory. Refer to the
-        documentation for the `Camera` contructor for the settings you need to specify.
-        
-        By default, HAP-python will execute the `ffmpeg` command with the negotiated parameters
-        when the stream should be started and will `terminate` the started process when the
-        stream should be stopped (see the default: `Camera.FFMPEG_CMD`).
-        If the default command is not supported or correctly formatted for your platform,
-        the streaming can fail.
-        
-        For these cases, HAP-python has hooks so that you can insert your own command or implement
-        the logic for starting or stopping the stream. There are two options:
-        
-        1. Pass your own command that will be executed when the stream should be started.
-        
-            You pass the command as a value to the key `start_stream_cmd` in the `options` parameter to
-            the constuctor of the `Camera` Accessory. The command is formatted using the
-            negotiated stream configuration parameters. For example, if the negotiated width
-            is 640 and you pass `foo start -width {width}`, the command will be formatted as
-            `foo start -width 640`.
-        
-            The full list of negotiated stream configuration parameters can be found in the
-            documentation for the `Camera.start` method.
-        
-        2. Implement your own logic to start, stop and reconfigure the stream.
-        
-            If you need more flexibility in managing streams, you can directly implement the
-            `Camera` methods `start`, `stop` and `reconfigure`. Each will be called when the
-            stream should be respectively started, stopped or reconfigured. The start and
-            reconfigure methods are given the negotiated stream configuration parameters.
-        
-            Have a look at the documentation of these methods for more information.
-        
-        Finally, if you can take snapshots from the camera, you may want to implement the
-        `Camera.snapshot` method. By default, this serves a stock photo.
-        
-        ## Run at boot <a name="AtBoot"></a>
-        This is a quick way to get `HAP-python` to run at boot on a Raspberry Pi. It is recommended
-        to turn on "Wait for network" in `raspi-config`. If this turns to be unreliable, see
-        [this](https://www.raspberrypi.org/forums/viewtopic.php?f=66&t=187225).
-        
-        Copy the below in `/etc/systemd/system/HAP-python.service` (needs sudo).
-        ```
-        [Unit]
-        Description = HAP-python daemon
-        Wants = pigpiod.service  # Remove this if you don't depend on pigpiod
-        After = local-fs.target network-online.target pigpiod.service
-        
-        [Service]
-        User = lesserdaemon  # It's a good idea to use some unprivileged system user
-        # Script starting HAP-python, e.g. main.py
-        # Be careful to set any paths you use, e.g. for persisting the state.
-        ExecStart = /usr/bin/python3 /home/lesserdaemon/.hap-python/hap-python.py
-        
-        [Install]
-        WantedBy = multi-user.target
-        ```
-        
-        Test that everything is fine by doing:
-        
-        ```sh
-        > sudo systemctl start HAP-python
-        > systemctl status HAP-python
-        > sudo journalctl -u HAP-python  # to see the output of the start up script.
-        > sudo systemctl stop HAP-python
-        ```
-        
-        To enable or disable at boot, do:
-        
-        ```sh
-        > sudo systemctl enable HAP-python
-        > sudo systemctl disable HAP-python
-        ```
-        
-        ### Shutdown switch
-        
-        If you are running `HAP-python` on a Raspberry Pi, you may want to add a
-        [Shutdown Switch](pyhap/accessories/ShutdownSwitch.py) to your Home. This is a
-        Switch Accessory, which, when triggered, executes `sudo shutdown -h now`, i.e.
-        it shutdowns and halts the Pi. This allows you to safely unplug it.
-        
-        For the above to work, you need to enable passwordless `/sbin/shutdown` to whichever
-        user is running `HAP-python`. For example, do:
-        ```sh
-        $ sudo visudo # and add the line: "<hap-user> ALL=NOPASSWD: /sbin/shutdown".
-        ```
-        
-        ## Notice <a name="Notice"></a>
-        
-        Some HAP know-how was taken from [HAP-NodeJS by KhaosT](https://github.com/KhaosT/HAP-NodeJS).
-        
-        I am not aware of any bugs, but I am more than confident that such exist. If you find any,
-        please report and I will try to fix them.
-        
-        Suggestions are always welcome.
-        
-        Have fun!
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -297,7 +21,286 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: QRCode
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/HAP-python.svg)](https://badge.fury.io/py/HAP-python) [![Build Status](https://github.com/ikalchev/HAP-python/workflows/CI/badge.svg)](https://github.com/ikalchev/HAP-python) [![codecov](https://codecov.io/gh/ikalchev/HAP-python/branch/master/graph/badge.svg)](https://codecov.io/gh/ikalchev/HAP-python) [![Python Versions](https://img.shields.io/pypi/pyversions/HAP-python.svg)](https://pypi.python.org/pypi/HAP-python/) [![Documentation Status](https://readthedocs.org/projects/hap-python/badge/?version=latest)](http://hap-python.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/hap-python)](https://pepy.tech/project/hap-python)
+# HAP-python
+
+HomeKit Accessory Protocol implementation in python 3.
+With this project, you can integrate your own smart devices and add them to your
+iOS Home app. Since Siri is integrated with the Home app, you can start voice-control your
+accessories right away.
+
+Main features:
+
+* Camera - HAP-python supports the camera accessory from version 2.3.0!
+* asyncio support - You can run various tasks or accessories in the event loop.
+* Out of the box support for Apple-defined services - see them in [the resources folder](pyhap/resources).
+* Secure pairing by just scanning the QR code.
+* Integrated with the home automation framework [Home Assistant](https://github.com/home-assistant/home-assistant).
+
+The project was developed for a Raspberry Pi, but it should work on other platforms. To kick-start things,
+you can open `main.py` or `busy_home.py`, where you will find some fake accessories.
+Just run one of them, for example `python3 busy_home.py`, and you can add it in
+the Home app (be sure to be in the same network).
+Stop it by hitting <kbd>Ctrl</kbd>+<kbd>C</kbd>.
+
+There are example accessories as well as integrations with real products
+in [the accessories folder](accessories). See how to configure your camera in
+[camera_main.py](camera_main.py).
+
+## Table of Contents
+1. [API](#API)
+2. [Installation](#Installation)
+3. [Setting up a camera](#Camera)
+4. [Run at boot (and a Switch to shutdown your device)](#AtBoot)
+5. [Notice](#Notice)
+
+## Installation <a name="Installation"></a>
+
+As of version 3.5.1, HAP-python no longer supports python older than 3.6, because we
+are moving to asyncio. If your platform does not have a compatible python out of the
+box, you can install it manually or just use an older version of HAP-python.
+
+As a prerequisite, you will need Avahi/Bonjour installed (due to zeroconf package).
+On a Raspberry Pi, you can get it with:
+```
+$ sudo apt-get install libavahi-compat-libdnssd-dev
+```
+`avahi-utils` may also fit the bill. Then, you can install with `pip3` (you will need `sudo` or `--user` for the install):
+```sh
+$ pip3 install HAP-python[QRCode]
+```
+
+This will install HAP-python in your python packages, so that you can import it as `pyhap`. To uninstall, just do:
+```
+$ pip3 uninstall HAP-python
+```
+
+## API <a name="API"></a>
+
+A typical flow for using HAP-python starts with implementing an Accessory. This is done by
+subclassing [Accessory](pyhap/accessory.py) and putting in place a few details
+(see below). After that, you give your accessory to an AccessoryDriver to manage. This
+will take care of advertising it on the local network, setting a HAP server and
+running the Accessory. Take a look at [main.py](main.py) for a quick start on that.
+
+```python
+from pyhap.accessory import Accessory, Category
+import pyhap.loader as loader
+
+class TemperatureSensor(Accessory):
+    """Implementation of a mock temperature sensor accessory."""
+
+    category = Category.SENSOR  # This is for the icon in the iOS Home app.
+
+    def __init__(self, *args, **kwargs):
+        """Here, we just store a reference to the current temperature characteristic and
+        add a method that will be executed every time its value changes.
+        """
+        # If overriding this method, be sure to call the super's implementation first.
+        super().__init__(*args, **kwargs)
+
+        # Add the services that this Accessory will support with add_preload_service here
+        temp_service = self.add_preload_service('TemperatureSensor')
+        self.temp_char = temp_service.get_characteristic('CurrentTemperature')
+
+        # Having a callback is optional, but you can use it to add functionality.
+        self.temp_char.setter_callback = self.temperature_changed
+
+    def temperature_changed(self, value):
+        """This will be called every time the value of the CurrentTemperature
+        is changed. Use setter_callbacks to react to user actions, e.g. setting the
+        lights On could fire some GPIO code to turn on a LED (see pyhap/accessories/LightBulb.py).
+        """
+        print('Temperature changed to: ', value)
+
+    @Accessory.run_at_interval(3)  # Run this method every 3 seconds
+    # The `run` method can be `async` as well
+    def run(self):
+        """We override this method to implement what the accessory will do when it is
+        started.
+
+        We set the current temperature to a random number. The decorator runs this method
+        every 3 seconds.
+        """
+        self.temp_char.set_value(random.randint(18, 26))
+
+    # The `stop` method can be `async` as well
+    def stop(self):
+        """We override this method to clean up any resources or perform final actions, as
+        this is called by the AccessoryDriver when the Accessory is being stopped.
+        """
+        print('Stopping accessory.')
+```
+
+## Service Callbacks
+
+When you are working with tightly coupled characteristics such as "On" and "Brightness,"
+you may need to use a service callback to receive all changes in a single request.
+
+With characteristic callbacks, you do now know that a "Brightness" characteristic is
+about to be processed right after an "On" and may end up setting a LightBulb to 100%
+and then dim it back down to the expected level.
+
+```python
+from pyhap.accessory import Accessory
+from pyhap.const import Category
+import pyhap.loader as loader
+
+class Light(Accessory):
+    """Implementation of a mock light accessory."""
+
+    category = Category.CATEGORY_LIGHTBULB  # This is for the icon in the iOS Home app.
+
+    def __init__(self, *args, **kwargs):
+        """Here, we just store a reference to the on and brightness characteristics and
+        add a method that will be executed every time their value changes.
+        """
+        # If overriding this method, be sure to call the super's implementation first.
+        super().__init__(*args, **kwargs)
+
+        # Add the services that this Accessory will support with add_preload_service here
+        serv_light = self.add_preload_service('Lightbulb')
+        self.char_on = serv_light.configure_char('On', value=self._state)
+        self.char_brightness = serv_light.configure_char('Brightness', value=100)
+
+        serv_light.setter_callback = self._set_chars
+
+    def _set_chars(self, char_values):
+        """This will be called every time the value of the on of the
+        characteristics on the service changes.
+        """
+        if "On" in char_values:
+            print('On changed to: ', char_values["On"])
+        if "Brightness" in char_values:
+            print('Brightness changed to: ', char_values["Brightness"])
+
+    @Accessory.run_at_interval(3)  # Run this method every 3 seconds
+    # The `run` method can be `async` as well
+    def run(self):
+        """We override this method to implement what the accessory will do when it is
+        started.
+
+        We set the current temperature to a random number. The decorator runs this method
+        every 3 seconds.
+        """
+        self.char_on.set_value(random.randint(0, 1))
+        self.char_brightness.set_value(random.randint(1, 100))
+
+    # The `stop` method can be `async` as well
+    def stop(self):
+        """We override this method to clean up any resources or perform final actions, as
+        this is called by the AccessoryDriver when the Accessory is being stopped.
+        """
+        print('Stopping accessory.')
+```
+
+## Setting up a camera <a name="Camera"></a>
+
+The [Camera accessory](pyhap/camera.py) implements the HomeKit Protocol for negotiating stream settings,
+such as the picture width and height, number of audio channels and others.
+Starting a video and/or audio stream is very platform specific. Because of this,
+you need to figure out what video and audio settings your camera supports and set them
+in the `options` parameter that is passed to the `Camera` Accessory. Refer to the
+documentation for the `Camera` contructor for the settings you need to specify.
+
+By default, HAP-python will execute the `ffmpeg` command with the negotiated parameters
+when the stream should be started and will `terminate` the started process when the
+stream should be stopped (see the default: `Camera.FFMPEG_CMD`).
+If the default command is not supported or correctly formatted for your platform,
+the streaming can fail.
+
+For these cases, HAP-python has hooks so that you can insert your own command or implement
+the logic for starting or stopping the stream. There are two options:
+
+1. Pass your own command that will be executed when the stream should be started.
+
+    You pass the command as a value to the key `start_stream_cmd` in the `options` parameter to
+    the constuctor of the `Camera` Accessory. The command is formatted using the
+    negotiated stream configuration parameters. For example, if the negotiated width
+    is 640 and you pass `foo start -width {width}`, the command will be formatted as
+    `foo start -width 640`.
+
+    The full list of negotiated stream configuration parameters can be found in the
+    documentation for the `Camera.start` method.
+
+2. Implement your own logic to start, stop and reconfigure the stream.
+
+    If you need more flexibility in managing streams, you can directly implement the
+    `Camera` methods `start`, `stop` and `reconfigure`. Each will be called when the
+    stream should be respectively started, stopped or reconfigured. The start and
+    reconfigure methods are given the negotiated stream configuration parameters.
+
+    Have a look at the documentation of these methods for more information.
+
+Finally, if you can take snapshots from the camera, you may want to implement the
+`Camera.snapshot` method. By default, this serves a stock photo.
+
+## Run at boot <a name="AtBoot"></a>
+This is a quick way to get `HAP-python` to run at boot on a Raspberry Pi. It is recommended
+to turn on "Wait for network" in `raspi-config`. If this turns to be unreliable, see
+[this](https://www.raspberrypi.org/forums/viewtopic.php?f=66&t=187225).
+
+Copy the below in `/etc/systemd/system/HAP-python.service` (needs sudo).
+```
+[Unit]
+Description = HAP-python daemon
+Wants = pigpiod.service  # Remove this if you don't depend on pigpiod
+After = local-fs.target network-online.target pigpiod.service
+
+[Service]
+User = lesserdaemon  # It's a good idea to use some unprivileged system user
+# Script starting HAP-python, e.g. main.py
+# Be careful to set any paths you use, e.g. for persisting the state.
+ExecStart = /usr/bin/python3 /home/lesserdaemon/.hap-python/hap-python.py
+
+[Install]
+WantedBy = multi-user.target
+```
+
+Test that everything is fine by doing:
+
+```sh
+> sudo systemctl start HAP-python
+> systemctl status HAP-python
+> sudo journalctl -u HAP-python  # to see the output of the start up script.
+> sudo systemctl stop HAP-python
+```
+
+To enable or disable at boot, do:
+
+```sh
+> sudo systemctl enable HAP-python
+> sudo systemctl disable HAP-python
+```
+
+### Shutdown switch
+
+If you are running `HAP-python` on a Raspberry Pi, you may want to add a
+[Shutdown Switch](pyhap/accessories/ShutdownSwitch.py) to your Home. This is a
+Switch Accessory, which, when triggered, executes `sudo shutdown -h now`, i.e.
+it shutdowns and halts the Pi. This allows you to safely unplug it.
+
+For the above to work, you need to enable passwordless `/sbin/shutdown` to whichever
+user is running `HAP-python`. For example, do:
+```sh
+$ sudo visudo # and add the line: "<hap-user> ALL=NOPASSWD: /sbin/shutdown".
+```
+
+## Notice <a name="Notice"></a>
+
+Some HAP know-how was taken from [HAP-NodeJS by KhaosT](https://github.com/KhaosT/HAP-NodeJS).
+
+I am not aware of any bugs, but I am more than confident that such exist. If you find any,
+please report and I will try to fix them.
+
+Suggestions are always welcome.
+
+Have fun!
+
+
```

### Comparing `HAP-python-4.6.0/HAP_python.egg-info/SOURCES.txt` & `HAP-python-4.7.0/HAP_python.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 HAP_python.egg-info/PKG-INFO
 HAP_python.egg-info/SOURCES.txt
 HAP_python.egg-info/dependency_links.txt
 HAP_python.egg-info/requires.txt
 HAP_python.egg-info/top_level.txt
```

### Comparing `HAP-python-4.6.0/LICENSE` & `HAP-python-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/PKG-INFO` & `HAP-python-4.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,292 +1,16 @@
 Metadata-Version: 2.1
 Name: HAP-python
-Version: 4.6.0
+Version: 4.7.0
 Summary: HomeKit Accessory Protocol implementation in python
 Home-page: https://github.com/ikalchev/HAP-python
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/ikalchev/HAP-python/issues
 Project-URL: Documentation, http://hap-python.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ikalchev/HAP-python/tree/master
-Description: [![PyPI version](https://badge.fury.io/py/HAP-python.svg)](https://badge.fury.io/py/HAP-python) [![Build Status](https://github.com/ikalchev/HAP-python/workflows/CI/badge.svg)](https://github.com/ikalchev/HAP-python) [![codecov](https://codecov.io/gh/ikalchev/HAP-python/branch/master/graph/badge.svg)](https://codecov.io/gh/ikalchev/HAP-python) [![Python Versions](https://img.shields.io/pypi/pyversions/HAP-python.svg)](https://pypi.python.org/pypi/HAP-python/) [![Documentation Status](https://readthedocs.org/projects/hap-python/badge/?version=latest)](http://hap-python.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/hap-python)](https://pepy.tech/project/hap-python)
-        # HAP-python
-        
-        HomeKit Accessory Protocol implementation in python 3.
-        With this project, you can integrate your own smart devices and add them to your
-        iOS Home app. Since Siri is integrated with the Home app, you can start voice-control your
-        accessories right away.
-        
-        Main features:
-        
-        * Camera - HAP-python supports the camera accessory from version 2.3.0!
-        * asyncio support - You can run various tasks or accessories in the event loop.
-        * Out of the box support for Apple-defined services - see them in [the resources folder](pyhap/resources).
-        * Secure pairing by just scanning the QR code.
-        * Integrated with the home automation framework [Home Assistant](https://github.com/home-assistant/home-assistant).
-        
-        The project was developed for a Raspberry Pi, but it should work on other platforms. To kick-start things,
-        you can open `main.py` or `busy_home.py`, where you will find some fake accessories.
-        Just run one of them, for example `python3 busy_home.py`, and you can add it in
-        the Home app (be sure to be in the same network).
-        Stop it by hitting Ctrl+C.
-        
-        There are example accessories as well as integrations with real products
-        in [the accessories folder](accessories). See how to configure your camera in
-        [camera_main.py](camera_main.py).
-        
-        ## Table of Contents
-        1. [API](#API)
-        2. [Installation](#Installation)
-        3. [Setting up a camera](#Camera)
-        4. [Run at boot (and a Switch to shutdown your device)](#AtBoot)
-        5. [Notice](#Notice)
-        
-        ## Installation <a name="Installation"></a>
-        
-        As of version 3.5.1, HAP-python no longer supports python older than 3.6, because we
-        are moving to asyncio. If your platform does not have a compatible python out of the
-        box, you can install it manually or just use an older version of HAP-python.
-        
-        As a prerequisite, you will need Avahi/Bonjour installed (due to zeroconf package).
-        On a Raspberry Pi, you can get it with:
-        ```
-        $ sudo apt-get install libavahi-compat-libdnssd-dev
-        ```
-        `avahi-utils` may also fit the bill. Then, you can install with `pip3` (you will need `sudo` or `--user` for the install):
-        ```sh
-        $ pip3 install HAP-python[QRCode]
-        ```
-        
-        This will install HAP-python in your python packages, so that you can import it as `pyhap`. To uninstall, just do:
-        ```
-        $ pip3 uninstall HAP-python
-        ```
-        
-        ## API <a name="API"></a>
-        
-        A typical flow for using HAP-python starts with implementing an Accessory. This is done by
-        subclassing [Accessory](pyhap/accessory.py) and putting in place a few details
-        (see below). After that, you give your accessory to an AccessoryDriver to manage. This
-        will take care of advertising it on the local network, setting a HAP server and
-        running the Accessory. Take a look at [main.py](main.py) for a quick start on that.
-        
-        ```python
-        from pyhap.accessory import Accessory, Category
-        import pyhap.loader as loader
-        
-        class TemperatureSensor(Accessory):
-            """Implementation of a mock temperature sensor accessory."""
-        
-            category = Category.SENSOR  # This is for the icon in the iOS Home app.
-        
-            def __init__(self, *args, **kwargs):
-                """Here, we just store a reference to the current temperature characteristic and
-                add a method that will be executed every time its value changes.
-                """
-                # If overriding this method, be sure to call the super's implementation first.
-                super().__init__(*args, **kwargs)
-        
-                # Add the services that this Accessory will support with add_preload_service here
-                temp_service = self.add_preload_service('TemperatureSensor')
-                self.temp_char = temp_service.get_characteristic('CurrentTemperature')
-        
-                # Having a callback is optional, but you can use it to add functionality.
-                self.temp_char.setter_callback = self.temperature_changed
-        
-            def temperature_changed(self, value):
-                """This will be called every time the value of the CurrentTemperature
-                is changed. Use setter_callbacks to react to user actions, e.g. setting the
-                lights On could fire some GPIO code to turn on a LED (see pyhap/accessories/LightBulb.py).
-                """
-                print('Temperature changed to: ', value)
-        
-            @Acessory.run_at_interval(3)  # Run this method every 3 seconds
-            # The `run` method can be `async` as well
-            def run(self):
-                """We override this method to implement what the accessory will do when it is
-                started.
-        
-                We set the current temperature to a random number. The decorator runs this method
-                every 3 seconds.
-                """
-                self.temp_char.set_value(random.randint(18, 26))
-        
-            # The `stop` method can be `async` as well
-            def stop(self):
-                """We override this method to clean up any resources or perform final actions, as
-                this is called by the AccessoryDriver when the Accessory is being stopped.
-                """
-                print('Stopping accessory.')
-        ```
-        
-        ## Service Callbacks
-        
-        When you are working with tightly coupled characteristics such as "On" and "Brightness,"
-        you may need to use a service callback to receive all changes in a single request.
-        
-        With characteristic callbacks, you do now know that a "Brightness" characteristic is
-        about to be processed right after an "On" and may end up setting a LightBulb to 100%
-        and then dim it back down to the expected level.
-        
-        ```python
-        from pyhap.accessory import Accessory
-        from pyhap.const import Category
-        import pyhap.loader as loader
-        
-        class Light(Accessory):
-            """Implementation of a mock light accessory."""
-        
-            category = Category.CATEGORY_LIGHTBULB  # This is for the icon in the iOS Home app.
-        
-            def __init__(self, *args, **kwargs):
-                """Here, we just store a reference to the on and brightness characteristics and
-                add a method that will be executed every time their value changes.
-                """
-                # If overriding this method, be sure to call the super's implementation first.
-                super().__init__(*args, **kwargs)
-        
-                # Add the services that this Accessory will support with add_preload_service here
-                serv_light = self.add_preload_service('Lightbulb')
-                self.char_on = serv_light.configure_char('On', value=self._state)
-                self.char_brightness = serv_light.configure_char('Brightness', value=100)
-        
-                serv_light.setter_callback = self._set_chars
-        
-            def _set_chars(self, char_values):
-                """This will be called every time the value of the on of the
-                characteristics on the service changes.
-                """
-                if "On" in char_values:
-                    print('On changed to: ', char_values["On"])
-                if "Brightness" in char_values:
-                    print('Brightness changed to: ', char_values["Brightness"])
-        
-            @Acessory.run_at_interval(3)  # Run this method every 3 seconds
-            # The `run` method can be `async` as well
-            def run(self):
-                """We override this method to implement what the accessory will do when it is
-                started.
-        
-                We set the current temperature to a random number. The decorator runs this method
-                every 3 seconds.
-                """
-                self.char_on.set_value(random.randint(0, 1))
-                self.char_brightness.set_value(random.randint(1, 100))
-        
-            # The `stop` method can be `async` as well
-            def stop(self):
-                """We override this method to clean up any resources or perform final actions, as
-                this is called by the AccessoryDriver when the Accessory is being stopped.
-                """
-                print('Stopping accessory.')
-        ```
-        
-        ## Setting up a camera <a name="Camera"></a>
-        
-        The [Camera accessory](pyhap/camera.py) implements the HomeKit Protocol for negotiating stream settings,
-        such as the picture width and height, number of audio channels and others.
-        Starting a video and/or audio stream is very platform specific. Because of this,
-        you need to figure out what video and audio settings your camera supports and set them
-        in the `options` parameter that is passed to the `Camera` Accessory. Refer to the
-        documentation for the `Camera` contructor for the settings you need to specify.
-        
-        By default, HAP-python will execute the `ffmpeg` command with the negotiated parameters
-        when the stream should be started and will `terminate` the started process when the
-        stream should be stopped (see the default: `Camera.FFMPEG_CMD`).
-        If the default command is not supported or correctly formatted for your platform,
-        the streaming can fail.
-        
-        For these cases, HAP-python has hooks so that you can insert your own command or implement
-        the logic for starting or stopping the stream. There are two options:
-        
-        1. Pass your own command that will be executed when the stream should be started.
-        
-            You pass the command as a value to the key `start_stream_cmd` in the `options` parameter to
-            the constuctor of the `Camera` Accessory. The command is formatted using the
-            negotiated stream configuration parameters. For example, if the negotiated width
-            is 640 and you pass `foo start -width {width}`, the command will be formatted as
-            `foo start -width 640`.
-        
-            The full list of negotiated stream configuration parameters can be found in the
-            documentation for the `Camera.start` method.
-        
-        2. Implement your own logic to start, stop and reconfigure the stream.
-        
-            If you need more flexibility in managing streams, you can directly implement the
-            `Camera` methods `start`, `stop` and `reconfigure`. Each will be called when the
-            stream should be respectively started, stopped or reconfigured. The start and
-            reconfigure methods are given the negotiated stream configuration parameters.
-        
-            Have a look at the documentation of these methods for more information.
-        
-        Finally, if you can take snapshots from the camera, you may want to implement the
-        `Camera.snapshot` method. By default, this serves a stock photo.
-        
-        ## Run at boot <a name="AtBoot"></a>
-        This is a quick way to get `HAP-python` to run at boot on a Raspberry Pi. It is recommended
-        to turn on "Wait for network" in `raspi-config`. If this turns to be unreliable, see
-        [this](https://www.raspberrypi.org/forums/viewtopic.php?f=66&t=187225).
-        
-        Copy the below in `/etc/systemd/system/HAP-python.service` (needs sudo).
-        ```
-        [Unit]
-        Description = HAP-python daemon
-        Wants = pigpiod.service  # Remove this if you don't depend on pigpiod
-        After = local-fs.target network-online.target pigpiod.service
-        
-        [Service]
-        User = lesserdaemon  # It's a good idea to use some unprivileged system user
-        # Script starting HAP-python, e.g. main.py
-        # Be careful to set any paths you use, e.g. for persisting the state.
-        ExecStart = /usr/bin/python3 /home/lesserdaemon/.hap-python/hap-python.py
-        
-        [Install]
-        WantedBy = multi-user.target
-        ```
-        
-        Test that everything is fine by doing:
-        
-        ```sh
-        > sudo systemctl start HAP-python
-        > systemctl status HAP-python
-        > sudo journalctl -u HAP-python  # to see the output of the start up script.
-        > sudo systemctl stop HAP-python
-        ```
-        
-        To enable or disable at boot, do:
-        
-        ```sh
-        > sudo systemctl enable HAP-python
-        > sudo systemctl disable HAP-python
-        ```
-        
-        ### Shutdown switch
-        
-        If you are running `HAP-python` on a Raspberry Pi, you may want to add a
-        [Shutdown Switch](pyhap/accessories/ShutdownSwitch.py) to your Home. This is a
-        Switch Accessory, which, when triggered, executes `sudo shutdown -h now`, i.e.
-        it shutdowns and halts the Pi. This allows you to safely unplug it.
-        
-        For the above to work, you need to enable passwordless `/sbin/shutdown` to whichever
-        user is running `HAP-python`. For example, do:
-        ```sh
-        $ sudo visudo # and add the line: "<hap-user> ALL=NOPASSWD: /sbin/shutdown".
-        ```
-        
-        ## Notice <a name="Notice"></a>
-        
-        Some HAP know-how was taken from [HAP-NodeJS by KhaosT](https://github.com/KhaosT/HAP-NodeJS).
-        
-        I am not aware of any bugs, but I am more than confident that such exist. If you find any,
-        please report and I will try to fix them.
-        
-        Suggestions are always welcome.
-        
-        Have fun!
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -297,7 +21,286 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: QRCode
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/HAP-python.svg)](https://badge.fury.io/py/HAP-python) [![Build Status](https://github.com/ikalchev/HAP-python/workflows/CI/badge.svg)](https://github.com/ikalchev/HAP-python) [![codecov](https://codecov.io/gh/ikalchev/HAP-python/branch/master/graph/badge.svg)](https://codecov.io/gh/ikalchev/HAP-python) [![Python Versions](https://img.shields.io/pypi/pyversions/HAP-python.svg)](https://pypi.python.org/pypi/HAP-python/) [![Documentation Status](https://readthedocs.org/projects/hap-python/badge/?version=latest)](http://hap-python.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://pepy.tech/badge/hap-python)](https://pepy.tech/project/hap-python)
+# HAP-python
+
+HomeKit Accessory Protocol implementation in python 3.
+With this project, you can integrate your own smart devices and add them to your
+iOS Home app. Since Siri is integrated with the Home app, you can start voice-control your
+accessories right away.
+
+Main features:
+
+* Camera - HAP-python supports the camera accessory from version 2.3.0!
+* asyncio support - You can run various tasks or accessories in the event loop.
+* Out of the box support for Apple-defined services - see them in [the resources folder](pyhap/resources).
+* Secure pairing by just scanning the QR code.
+* Integrated with the home automation framework [Home Assistant](https://github.com/home-assistant/home-assistant).
+
+The project was developed for a Raspberry Pi, but it should work on other platforms. To kick-start things,
+you can open `main.py` or `busy_home.py`, where you will find some fake accessories.
+Just run one of them, for example `python3 busy_home.py`, and you can add it in
+the Home app (be sure to be in the same network).
+Stop it by hitting <kbd>Ctrl</kbd>+<kbd>C</kbd>.
+
+There are example accessories as well as integrations with real products
+in [the accessories folder](accessories). See how to configure your camera in
+[camera_main.py](camera_main.py).
+
+## Table of Contents
+1. [API](#API)
+2. [Installation](#Installation)
+3. [Setting up a camera](#Camera)
+4. [Run at boot (and a Switch to shutdown your device)](#AtBoot)
+5. [Notice](#Notice)
+
+## Installation <a name="Installation"></a>
+
+As of version 3.5.1, HAP-python no longer supports python older than 3.6, because we
+are moving to asyncio. If your platform does not have a compatible python out of the
+box, you can install it manually or just use an older version of HAP-python.
+
+As a prerequisite, you will need Avahi/Bonjour installed (due to zeroconf package).
+On a Raspberry Pi, you can get it with:
+```
+$ sudo apt-get install libavahi-compat-libdnssd-dev
+```
+`avahi-utils` may also fit the bill. Then, you can install with `pip3` (you will need `sudo` or `--user` for the install):
+```sh
+$ pip3 install HAP-python[QRCode]
+```
+
+This will install HAP-python in your python packages, so that you can import it as `pyhap`. To uninstall, just do:
+```
+$ pip3 uninstall HAP-python
+```
+
+## API <a name="API"></a>
+
+A typical flow for using HAP-python starts with implementing an Accessory. This is done by
+subclassing [Accessory](pyhap/accessory.py) and putting in place a few details
+(see below). After that, you give your accessory to an AccessoryDriver to manage. This
+will take care of advertising it on the local network, setting a HAP server and
+running the Accessory. Take a look at [main.py](main.py) for a quick start on that.
+
+```python
+from pyhap.accessory import Accessory, Category
+import pyhap.loader as loader
+
+class TemperatureSensor(Accessory):
+    """Implementation of a mock temperature sensor accessory."""
+
+    category = Category.SENSOR  # This is for the icon in the iOS Home app.
+
+    def __init__(self, *args, **kwargs):
+        """Here, we just store a reference to the current temperature characteristic and
+        add a method that will be executed every time its value changes.
+        """
+        # If overriding this method, be sure to call the super's implementation first.
+        super().__init__(*args, **kwargs)
+
+        # Add the services that this Accessory will support with add_preload_service here
+        temp_service = self.add_preload_service('TemperatureSensor')
+        self.temp_char = temp_service.get_characteristic('CurrentTemperature')
+
+        # Having a callback is optional, but you can use it to add functionality.
+        self.temp_char.setter_callback = self.temperature_changed
+
+    def temperature_changed(self, value):
+        """This will be called every time the value of the CurrentTemperature
+        is changed. Use setter_callbacks to react to user actions, e.g. setting the
+        lights On could fire some GPIO code to turn on a LED (see pyhap/accessories/LightBulb.py).
+        """
+        print('Temperature changed to: ', value)
+
+    @Accessory.run_at_interval(3)  # Run this method every 3 seconds
+    # The `run` method can be `async` as well
+    def run(self):
+        """We override this method to implement what the accessory will do when it is
+        started.
+
+        We set the current temperature to a random number. The decorator runs this method
+        every 3 seconds.
+        """
+        self.temp_char.set_value(random.randint(18, 26))
+
+    # The `stop` method can be `async` as well
+    def stop(self):
+        """We override this method to clean up any resources or perform final actions, as
+        this is called by the AccessoryDriver when the Accessory is being stopped.
+        """
+        print('Stopping accessory.')
+```
+
+## Service Callbacks
+
+When you are working with tightly coupled characteristics such as "On" and "Brightness,"
+you may need to use a service callback to receive all changes in a single request.
+
+With characteristic callbacks, you do now know that a "Brightness" characteristic is
+about to be processed right after an "On" and may end up setting a LightBulb to 100%
+and then dim it back down to the expected level.
+
+```python
+from pyhap.accessory import Accessory
+from pyhap.const import Category
+import pyhap.loader as loader
+
+class Light(Accessory):
+    """Implementation of a mock light accessory."""
+
+    category = Category.CATEGORY_LIGHTBULB  # This is for the icon in the iOS Home app.
+
+    def __init__(self, *args, **kwargs):
+        """Here, we just store a reference to the on and brightness characteristics and
+        add a method that will be executed every time their value changes.
+        """
+        # If overriding this method, be sure to call the super's implementation first.
+        super().__init__(*args, **kwargs)
+
+        # Add the services that this Accessory will support with add_preload_service here
+        serv_light = self.add_preload_service('Lightbulb')
+        self.char_on = serv_light.configure_char('On', value=self._state)
+        self.char_brightness = serv_light.configure_char('Brightness', value=100)
+
+        serv_light.setter_callback = self._set_chars
+
+    def _set_chars(self, char_values):
+        """This will be called every time the value of the on of the
+        characteristics on the service changes.
+        """
+        if "On" in char_values:
+            print('On changed to: ', char_values["On"])
+        if "Brightness" in char_values:
+            print('Brightness changed to: ', char_values["Brightness"])
+
+    @Accessory.run_at_interval(3)  # Run this method every 3 seconds
+    # The `run` method can be `async` as well
+    def run(self):
+        """We override this method to implement what the accessory will do when it is
+        started.
+
+        We set the current temperature to a random number. The decorator runs this method
+        every 3 seconds.
+        """
+        self.char_on.set_value(random.randint(0, 1))
+        self.char_brightness.set_value(random.randint(1, 100))
+
+    # The `stop` method can be `async` as well
+    def stop(self):
+        """We override this method to clean up any resources or perform final actions, as
+        this is called by the AccessoryDriver when the Accessory is being stopped.
+        """
+        print('Stopping accessory.')
+```
+
+## Setting up a camera <a name="Camera"></a>
+
+The [Camera accessory](pyhap/camera.py) implements the HomeKit Protocol for negotiating stream settings,
+such as the picture width and height, number of audio channels and others.
+Starting a video and/or audio stream is very platform specific. Because of this,
+you need to figure out what video and audio settings your camera supports and set them
+in the `options` parameter that is passed to the `Camera` Accessory. Refer to the
+documentation for the `Camera` contructor for the settings you need to specify.
+
+By default, HAP-python will execute the `ffmpeg` command with the negotiated parameters
+when the stream should be started and will `terminate` the started process when the
+stream should be stopped (see the default: `Camera.FFMPEG_CMD`).
+If the default command is not supported or correctly formatted for your platform,
+the streaming can fail.
+
+For these cases, HAP-python has hooks so that you can insert your own command or implement
+the logic for starting or stopping the stream. There are two options:
+
+1. Pass your own command that will be executed when the stream should be started.
+
+    You pass the command as a value to the key `start_stream_cmd` in the `options` parameter to
+    the constuctor of the `Camera` Accessory. The command is formatted using the
+    negotiated stream configuration parameters. For example, if the negotiated width
+    is 640 and you pass `foo start -width {width}`, the command will be formatted as
+    `foo start -width 640`.
+
+    The full list of negotiated stream configuration parameters can be found in the
+    documentation for the `Camera.start` method.
+
+2. Implement your own logic to start, stop and reconfigure the stream.
+
+    If you need more flexibility in managing streams, you can directly implement the
+    `Camera` methods `start`, `stop` and `reconfigure`. Each will be called when the
+    stream should be respectively started, stopped or reconfigured. The start and
+    reconfigure methods are given the negotiated stream configuration parameters.
+
+    Have a look at the documentation of these methods for more information.
+
+Finally, if you can take snapshots from the camera, you may want to implement the
+`Camera.snapshot` method. By default, this serves a stock photo.
+
+## Run at boot <a name="AtBoot"></a>
+This is a quick way to get `HAP-python` to run at boot on a Raspberry Pi. It is recommended
+to turn on "Wait for network" in `raspi-config`. If this turns to be unreliable, see
+[this](https://www.raspberrypi.org/forums/viewtopic.php?f=66&t=187225).
+
+Copy the below in `/etc/systemd/system/HAP-python.service` (needs sudo).
+```
+[Unit]
+Description = HAP-python daemon
+Wants = pigpiod.service  # Remove this if you don't depend on pigpiod
+After = local-fs.target network-online.target pigpiod.service
+
+[Service]
+User = lesserdaemon  # It's a good idea to use some unprivileged system user
+# Script starting HAP-python, e.g. main.py
+# Be careful to set any paths you use, e.g. for persisting the state.
+ExecStart = /usr/bin/python3 /home/lesserdaemon/.hap-python/hap-python.py
+
+[Install]
+WantedBy = multi-user.target
+```
+
+Test that everything is fine by doing:
+
+```sh
+> sudo systemctl start HAP-python
+> systemctl status HAP-python
+> sudo journalctl -u HAP-python  # to see the output of the start up script.
+> sudo systemctl stop HAP-python
+```
+
+To enable or disable at boot, do:
+
+```sh
+> sudo systemctl enable HAP-python
+> sudo systemctl disable HAP-python
+```
+
+### Shutdown switch
+
+If you are running `HAP-python` on a Raspberry Pi, you may want to add a
+[Shutdown Switch](pyhap/accessories/ShutdownSwitch.py) to your Home. This is a
+Switch Accessory, which, when triggered, executes `sudo shutdown -h now`, i.e.
+it shutdowns and halts the Pi. This allows you to safely unplug it.
+
+For the above to work, you need to enable passwordless `/sbin/shutdown` to whichever
+user is running `HAP-python`. For example, do:
+```sh
+$ sudo visudo # and add the line: "<hap-user> ALL=NOPASSWD: /sbin/shutdown".
+```
+
+## Notice <a name="Notice"></a>
+
+Some HAP know-how was taken from [HAP-NodeJS by KhaosT](https://github.com/KhaosT/HAP-NodeJS).
+
+I am not aware of any bugs, but I am more than confident that such exist. If you find any,
+please report and I will try to fix them.
+
+Suggestions are always welcome.
+
+Have fun!
+
+
```

### Comparing `HAP-python-4.6.0/README.md` & `HAP-python-4.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 * Secure pairing by just scanning the QR code.
 * Integrated with the home automation framework [Home Assistant](https://github.com/home-assistant/home-assistant).
 
 The project was developed for a Raspberry Pi, but it should work on other platforms. To kick-start things,
 you can open `main.py` or `busy_home.py`, where you will find some fake accessories.
 Just run one of them, for example `python3 busy_home.py`, and you can add it in
 the Home app (be sure to be in the same network).
-Stop it by hitting Ctrl+C.
+Stop it by hitting <kbd>Ctrl</kbd>+<kbd>C</kbd>.
 
 There are example accessories as well as integrations with real products
 in [the accessories folder](accessories). See how to configure your camera in
 [camera_main.py](camera_main.py).
 
 ## Table of Contents
 1. [API](#API)
@@ -86,15 +86,15 @@
     def temperature_changed(self, value):
         """This will be called every time the value of the CurrentTemperature
         is changed. Use setter_callbacks to react to user actions, e.g. setting the
         lights On could fire some GPIO code to turn on a LED (see pyhap/accessories/LightBulb.py).
         """
         print('Temperature changed to: ', value)
 
-    @Acessory.run_at_interval(3)  # Run this method every 3 seconds
+    @Accessory.run_at_interval(3)  # Run this method every 3 seconds
     # The `run` method can be `async` as well
     def run(self):
         """We override this method to implement what the accessory will do when it is
         started.
 
         We set the current temperature to a random number. The decorator runs this method
         every 3 seconds.
@@ -147,15 +147,15 @@
         characteristics on the service changes.
         """
         if "On" in char_values:
             print('On changed to: ', char_values["On"])
         if "Brightness" in char_values:
             print('Brightness changed to: ', char_values["Brightness"])
 
-    @Acessory.run_at_interval(3)  # Run this method every 3 seconds
+    @Accessory.run_at_interval(3)  # Run this method every 3 seconds
     # The `run` method can be `async` as well
     def run(self):
         """We override this method to implement what the accessory will do when it is
         started.
 
         We set the current temperature to a random number. The decorator runs this method
         every 3 seconds.
```

### Comparing `HAP-python-4.6.0/pyhap/accessory.py` & `HAP-python-4.7.0/pyhap/accessory.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/accessory_driver.py` & `HAP-python-4.7.0/pyhap/accessory_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 import asyncio
 import base64
 from concurrent.futures import ThreadPoolExecutor
 import hashlib
 import logging
 import os
 import re
-import socket
 import sys
 import tempfile
-import time
 import threading
+import time
+from typing import Optional
 
 from zeroconf import ServiceInfo
 from zeroconf.asyncio import AsyncZeroconf
 
 from pyhap import util
-from pyhap.accessory import get_topic
+from pyhap.accessory import Accessory, get_topic
 from pyhap.characteristic import CharacteristicError
 from pyhap.const import (
     HAP_PERMISSION_NOTIFY,
     HAP_PROTOCOL_SHORT_VERSION,
     HAP_REPR_ACCS,
     HAP_REPR_AID,
     HAP_REPR_CHARS,
     HAP_REPR_IID,
-    HAP_REPR_TTL,
     HAP_REPR_PID,
     HAP_REPR_STATUS,
+    HAP_REPR_TTL,
     HAP_REPR_VALUE,
     STANDALONE_AID,
 )
 from pyhap.encoder import AccessoryEncoder
 from pyhap.hap_server import HAPServer
 from pyhap.hsrp import Server as SrpServer
 from pyhap.loader import Loader
@@ -118,15 +118,15 @@
 
 
 class AccessoryMDNSServiceInfo(ServiceInfo):
     """A mDNS service info representation of an accessory."""
 
     def __init__(self, accessory, state, zeroconf_server=None):
         self.accessory = accessory
-        self.state = state
+        self.state: State = state
 
         adv_data = self._get_advert_data()
         valid_name = self._valid_name()
         short_mac = self.state.mac[-8:].replace(":", "")
         # Append part of MAC address to prevent name conflicts
         name = f"{valid_name} {short_mac}.{HAP_SERVICE_TYPE}"
         valid_host_name = self._valid_host_name()
@@ -135,15 +135,15 @@
             HAP_SERVICE_TYPE,
             name=name,
             server=server,
             port=self.state.port,
             weight=0,
             priority=0,
             properties=adv_data,
-            addresses=[socket.inet_aton(self.state.address)],
+            parsed_addresses=self.state.addresses,
         )
 
     def _valid_name(self):
         return re.sub(
             LEADING_TRAILING_SPACE_DASH,
             "",
             re.sub(VALID_MDNS_REGEX, " ", self.accessory.display_name),
@@ -240,18 +240,18 @@
             If not given, the driver will try to select a MAC address.
         :type mac: str
 
         :param listen_address: The local address on the HAPServer will listen.
             If not given, the value of the address parameter will be used.
         :type listen_address: str
 
-        :param advertised_address: The address of the HAPServer announced via mDNS.
+        :param advertised_address: The addresses of the HAPServer announced via mDNS.
             This can be used to announce an external address from behind a NAT.
             If not given, the value of the address parameter will be used.
-        :type advertised_address: str
+        :type advertised_address: str | list[str]
 
         :param interface_choice: The zeroconf interfaces to listen on.
         :type InterfacesType: [InterfaceChoice.Default, InterfaceChoice.All]
 
         :param async_zeroconf_instance: An AsyncZeroconf instance. When running multiple accessories or
             bridges a single zeroconf instance can be shared to avoid the overhead
             of processing the same data multiple times.
@@ -275,15 +275,15 @@
             self.tid = threading.current_thread()
         else:
             self.tid = threading.main_thread()
             self.executor = None
 
         self.loop = loop
 
-        self.accessory = None
+        self.accessory: Optional[Accessory] = None
         self.advertiser = async_zeroconf_instance
         self.zeroconf_server = zeroconf_server
         self.interface_choice = interface_choice
 
         self.persist_file = os.path.expanduser(persist_file)
         self.encoder = encoder or AccessoryEncoder()
         self.topics = {}  # topic: set of (address, port) of subscribed clients
@@ -362,17 +362,17 @@
         All of the above are started in separate threads. Accessory thread is set as
         daemon.
         """
         self._validate_start()
         self.aio_stop_event = asyncio.Event()
 
         logger.info(
-            "Starting accessory %s on address %s, port %s.",
+            "Starting accessory %s on addresses %s, port %s.",
             self.accessory.display_name,
-            self.state.address,
+            self.state.addresses,
             self.state.port,
         )
 
         # Start listening for requests
         logger.debug("Starting server.")
         await self.http_server.async_start(self.loop)
 
@@ -424,15 +424,15 @@
         self.aio_stop_event.set()
 
         self.http_server.async_stop()
 
         logger.info(
             "Stopping accessory %s on address %s, port %s.",
             self.accessory.display_name,
-            self.state.address,
+            self.state.addresses,
             self.state.port,
         )
 
         await self.async_add_job(self.accessory.stop)
 
         logger.debug(
             "AccessoryDriver for %s stopped successfully", self.accessory.display_name
@@ -639,15 +639,17 @@
         try:
             temp_dir = os.path.dirname(self.persist_file)
             with tempfile.NamedTemporaryFile(
                 mode="w", dir=temp_dir, delete=False
             ) as file_handle:
                 tmp_filename = file_handle.name
                 self.encoder.persist(file_handle, self.state)
-            if os.name == 'nt':  # Or `[WinError 5] Access Denied` will be raised on Windows
+            if (
+                os.name == "nt"
+            ):  # Or `[WinError 5] Access Denied` will be raised on Windows
                 os.chmod(tmp_filename, 0o644)
                 os.chmod(self.persist_file, 0o644)
             os.replace(tmp_filename, self.persist_file)
         except Exception:  # pylint: disable=broad-except
             logger.exception("Failed to persist accessory state")
             raise
         finally:
@@ -659,35 +661,44 @@
 
         Must run in executor.
         """
         with open(self.persist_file, "r", encoding="utf8") as file_handle:
             self.encoder.load_into(file_handle, self.state)
 
     @callback
-    def pair(self, client_uuid, client_public, client_permissions):
+    def pair(
+        self,
+        client_username_bytes: bytes,
+        client_public: bytes,
+        client_permissions: bytes,
+    ) -> bool:
         """Called when a client has paired with the accessory.
 
         Persist the new accessory state.
 
-        :param client_uuid: The client uuid.
-        :type client_uuid: uuid.UUID
+        :param client_username_bytes: The client username bytes.
+        :type client_username_bytes: bytes
 
         :param client_public: The client's public key.
         :type client_public: bytes
 
         :param client_permissions: The client's permissions.
         :type client_permissions: bytes (int)
 
         :return: Whether the pairing is successful.
         :rtype: bool
         """
         logger.info(
-            "Paired with %s with permissions %s.", client_uuid, client_permissions
+            "Paired with %s with permissions %s.",
+            client_username_bytes,
+            client_permissions,
+        )
+        self.state.add_paired_client(
+            client_username_bytes, client_public, client_permissions
         )
-        self.state.add_paired_client(client_uuid, client_public, client_permissions)
         self.async_persist()
         return True
 
     @callback
     def unpair(self, client_uuid):
         """Removes the paired client from the accessory.
```

### Comparing `HAP-python-4.6.0/pyhap/camera.py` & `HAP-python-4.7.0/pyhap/camera.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/characteristic.py` & `HAP-python-4.7.0/pyhap/characteristic.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/const.py` & `HAP-python-4.7.0/pyhap/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module contains constants used by other modules."""
 MAJOR_VERSION = 4
-MINOR_VERSION = 6
+MINOR_VERSION = 7
 PATCH_VERSION = 0
 __short_version__ = f"{MAJOR_VERSION}.{MINOR_VERSION}"
 __version__ = f"{__short_version__}.{PATCH_VERSION}"
 REQUIRED_PYTHON_VER = (3, 7)
 
 BASE_UUID = "-0000-1000-8000-0026BB765291"
```

### Comparing `HAP-python-4.6.0/pyhap/encoder.py` & `HAP-python-4.7.0/pyhap/encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 import uuid
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519
 
 from .const import CLIENT_PROP_PERMS
+from .state import State
 
 
 class AccessoryEncoder:
     """This class defines the Accessory encoder interface.
 
     The AccessoryEncoder is used by the AccessoryDriver to persist and restore the
     state of an Accessory between restarts. This is needed in order to allow iOS
@@ -41,15 +42,15 @@
     Note also that AIDs and IIDs must also survive a restore. However, this is managed
     by the Accessory and Bridge classes.
 
     @see: AccessoryDriver.persist AccessoryDriver.load AccessoryDriver.__init__
     """
 
     @staticmethod
-    def persist(fp, state):
+    def persist(fp, state: State):
         """Persist the state of the given Accessory to the given file object.
 
         Persists:
             - MAC address.
             - Public and private key.
             - UUID and public key of paired clients.
             - Config version.
@@ -57,20 +58,24 @@
         """
         paired_clients = {
             str(client): bytes.hex(key) for client, key in state.paired_clients.items()
         }
         client_properties = {
             str(client): props for client, props in state.client_properties.items()
         }
+        client_uuid_to_bytes = {
+            str(client): bytes.hex(key) for client, key in state.uuid_to_bytes.items()
+        }
         config_state = {
             "mac": state.mac,
             "config_version": state.config_version,
             "paired_clients": paired_clients,
             "client_properties": client_properties,
             "accessories_hash": state.accessories_hash,
+            "client_uuid_to_bytes": client_uuid_to_bytes,
             "private_key": bytes.hex(
                 state.private_key.private_bytes(
                     encoding=serialization.Encoding.Raw,
                     format=serialization.PrivateFormat.Raw,
                     encryption_algorithm=serialization.NoEncryption(),
                 )
             ),
@@ -80,15 +85,15 @@
                     format=serialization.PublicFormat.Raw,
                 )
             ),
         }
         json.dump(config_state, fp)
 
     @staticmethod
-    def load_into(fp, state):
+    def load_into(fp, state: State) -> None:
         """Load the accessory state from the given file object into the given Accessory.
 
         @see: AccessoryEncoder.persist
         """
         loaded = json.load(fp)
         state.mac = loaded["mac"]
         state.accessories_hash = loaded.get("accessories_hash")
@@ -111,7 +116,11 @@
         }
         state.private_key = ed25519.Ed25519PrivateKey.from_private_bytes(
             bytes.fromhex(loaded["private_key"])
         )
         state.public_key = ed25519.Ed25519PublicKey.from_public_bytes(
             bytes.fromhex(loaded["public_key"])
         )
+        state.uuid_to_bytes = {
+            uuid.UUID(client): bytes.fromhex(key)
+            for client, key in loaded.get("client_uuid_to_bytes", {}).items()
+        }
```

### Comparing `HAP-python-4.6.0/pyhap/hap_crypto.py` & `HAP-python-4.7.0/pyhap/hap_crypto.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/hap_event.py` & `HAP-python-4.7.0/pyhap/hap_event.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/hap_handler.py` & `HAP-python-4.7.0/pyhap/hap_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """This module implements the communication of HAP.
 
 The HAPServerHandler manages the state of the connection and handles incoming requests.
 """
 import asyncio
 from http import HTTPStatus
 import logging
-from urllib.parse import parse_qs, urlparse
+from typing import TYPE_CHECKING, Dict, Optional
+from urllib.parse import ParseResult, parse_qs, urlparse
 import uuid
 
+from chacha20poly1305_reuseable import ChaCha20Poly1305Reusable as ChaCha20Poly1305
 from cryptography.exceptions import InvalidSignature, InvalidTag
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519, x25519
-from chacha20poly1305_reuseable import ChaCha20Poly1305Reusable as ChaCha20Poly1305
+import h11
 
 from pyhap import tlv
-
 from pyhap.const import (
     CATEGORY_BRIDGE,
     HAP_PERMISSIONS,
     HAP_REPR_CHARS,
     HAP_REPR_STATUS,
     HAP_SERVER_STATUS,
 )
 from pyhap.util import long_to_bytes
 
 from .hap_crypto import hap_hkdf, pad_tls_nonce
-from .util import to_hap_json, from_hap_json
+from .state import State
+from .util import from_hap_json, to_hap_json
+
+if TYPE_CHECKING:
+    from .accessory_driver import AccessoryDriver
 
 # iOS will terminate the connection if it does not respond within
 # 10 seconds, so we only allow 9 seconds to avoid this.
 RESPONSE_TIMEOUT = 9
 
 
 logger = logging.getLogger(__name__)
@@ -130,32 +135,37 @@
     PVERIFY_2_NONCE = pad_tls_nonce(b"PV-Msg03")
 
     def __init__(self, accessory_handler, client_address):
         """
         @param accessory_handler: An object that controls an accessory's state.
         @type accessory_handler: AccessoryDriver
         """
-        self.accessory_handler = accessory_handler
-        self.state = self.accessory_handler.state
+        self.accessory_handler: AccessoryDriver = accessory_handler
+        self.state: State = self.accessory_handler.state
         self.enc_context = None
         self.client_address = client_address
         self.is_encrypted = False
-        self.client_uuid = None
+        self.client_uuid: Optional[uuid.UUID] = None
 
-        self.path = None
-        self.command = None
-        self.headers = None
-        self.request_body = None
-        self.parsed_url = None
+        self.path: Optional[str] = None
+        self.command: Optional[str] = None
+        self.headers: Optional[Dict[str, str]] = None
+        self.request_body: Optional[bytes] = None
+        self.parsed_url: Optional[ParseResult] = None
 
-        self.response = None
+        self.response: Optional[HAPResponse] = None
 
     def _set_encryption_ctx(
-        self, client_public, private_key, public_key, shared_key, pre_session_key
-    ):
+        self,
+        client_public: bytes,
+        private_key: x25519.X25519PrivateKey,
+        public_key: x25519.X25519PublicKey,
+        shared_key: bytes,
+        pre_session_key: bytes,
+    ) -> None:
         """Sets the encryption context.
 
         The encryption context is generated in pair verify step one and is used to
         create encrypted transported in pair verify step two.
 
         @param client_public: The client's session public key.
         @type client_public: bytes
@@ -174,31 +184,36 @@
             "client_public": client_public,
             "private_key": private_key,
             "public_key": public_key,
             "shared_key": shared_key,
             "pre_session_key": pre_session_key,
         }
 
-    def send_response(self, http_status):
+    def send_response(self, http_status: HTTPStatus) -> None:
         """Add the response header to the headers buffer and log the
         response code.
         Does not add Server or Date
         """
+        assert self.response is not None  # nosec
         self.response.status_code = http_status.value
         self.response.reason = http_status.phrase
 
-    def send_header(self, header, value):
+    def send_header(self, header: str, value: str) -> None:
         """Add the response header to the headers buffer."""
+        assert self.response is not None  # nosec
         self.response.headers.append((header, value))
 
-    def end_response(self, bytesdata):
+    def end_response(self, bytesdata: bytes) -> None:
         """Combines adding a length header and actually sending the data."""
+        assert self.response is not None  # nosec
         self.response.body = bytesdata
 
-    def dispatch(self, request, body=None):
+    def dispatch(
+        self, request: h11.Request, body: Optional[bytes] = None
+    ) -> HAPResponse:
         """Dispatch the request to the appropriate handler method."""
         self.path = request.target.decode()
         self.command = request.method.decode()
         self.headers = {k.decode(): v.decode() for k, v in request.headers}
         self.request_body = body
         self.parsed_url = urlparse(self.path)
         response = HAPResponse()
@@ -227,32 +242,34 @@
                 HTTPStatus.INTERNAL_SERVER_ERROR,
                 HAP_SERVER_STATUS.SERVICE_COMMUNICATION_FAILURE,
             )
 
         self.response = None
         return response
 
-    def generic_failure_response(self):
+    def generic_failure_response(self) -> HAPResponse:
         """Generate a generic failure response."""
         self.response = HAPResponse()
         self.send_response_with_status(
             HTTPStatus.INTERNAL_SERVER_ERROR,
             HAP_SERVER_STATUS.SERVICE_COMMUNICATION_FAILURE,
         )
         response = self.response
         self.response = None
         return response
 
-    def send_response_with_status(self, http_code, hap_server_status):
+    def send_response_with_status(
+        self, http_code: HTTPStatus, hap_server_status: int
+    ) -> None:
         """Send a generic HAP status response."""
         self.send_response(http_code)
         self.send_header("Content-Type", self.JSON_RESPONSE_TYPE)
         self.end_response(to_hap_json({"status": hap_server_status}))
 
-    def handle_pairing(self):
+    def handle_pairing(self) -> None:
         """Handles arbitrary step of the pairing process."""
         if self.state.paired:
             self._send_tlv_pairing_response(
                 tlv.encode(
                     HAP_TLV_TAGS.SEQUENCE_NUM,
                     HAP_TLV_STATES.M2,
                     HAP_TLV_TAGS.ERROR_CODE,
@@ -267,15 +284,15 @@
         if sequence == HAP_TLV_STATES.M1:
             self._pairing_one()
         elif sequence == HAP_TLV_STATES.M3:
             self._pairing_two(tlv_objects)
         elif sequence == HAP_TLV_STATES.M5:
             self._pairing_three(tlv_objects)
 
-    def _pairing_one(self):
+    def _pairing_one(self) -> None:
         """Send the SRP salt and public key to the client.
 
         The SRP verifier is created at this step.
         """
         logger.debug("%s: Pairing [1/5]", self.client_address)
         self.accessory_handler.setup_srp_verifier()
         salt, B = self.accessory_handler.srp_verifier.get_challenge()
@@ -286,15 +303,15 @@
             HAP_TLV_TAGS.SALT,
             salt,
             HAP_TLV_TAGS.PUBLIC_KEY,
             long_to_bytes(B),
         )
         self._send_tlv_pairing_response(data)
 
-    def _pairing_two(self, tlv_objects):
+    def _pairing_two(self, tlv_objects: Dict[bytes, bytes]) -> None:
         """Obtain the challenge from the client (A) and client's proof that it
         knows the password (M). Verify M and generate the server's proof based on
         A (H_AMK). Send the H_AMK to the client.
 
         @param tlv_objects: The TLV data received from the client.
         @type tlv_object: dict
         """
@@ -314,15 +331,15 @@
             HAP_TLV_TAGS.SEQUENCE_NUM,
             HAP_TLV_STATES.M4,
             HAP_TLV_TAGS.PASSWORD_PROOF,
             hamk,
         )
         self._send_tlv_pairing_response(data)
 
-    def _pairing_three(self, tlv_objects):
+    def _pairing_three(self, tlv_objects: Dict[bytes, bytes]) -> None:
         """Expand the SRP session key to obtain a new key. Use it to verify and decrypt
             the recieved data. Continue to step four.
 
         @param tlv_objects: The TLV data received from the client.
         @type tlv_object: dict
         """
         logger.debug("%s: Pairing [3/5]", self.client_address)
@@ -339,21 +356,29 @@
                 self.PAIRING_3_NONCE, bytes(encrypted_data), b""
             )
         except InvalidTag:
             self._send_authentication_error_tlv_response(HAP_TLV_STATES.M6)
             return
 
         dec_tlv_objects = tlv.decode(bytes(decrypted_data))
-        client_username = dec_tlv_objects[HAP_TLV_TAGS.USERNAME]
+        client_username_bytes = dec_tlv_objects[HAP_TLV_TAGS.USERNAME]
         client_ltpk = dec_tlv_objects[HAP_TLV_TAGS.PUBLIC_KEY]
         client_proof = dec_tlv_objects[HAP_TLV_TAGS.PROOF]
 
-        self._pairing_four(client_username, client_ltpk, client_proof, hkdf_enc_key)
+        self._pairing_four(
+            client_username_bytes, client_ltpk, client_proof, hkdf_enc_key
+        )
 
-    def _pairing_four(self, client_username, client_ltpk, client_proof, encryption_key):
+    def _pairing_four(
+        self,
+        client_username_bytes: bytes,
+        client_ltpk: bytes,
+        client_proof: bytes,
+        encryption_key: bytes,
+    ) -> None:
         """Expand the SRP session key to obtain a new key.
             Use it to verify that the client's proof of the private key. Continue to
             step five.
 
         @param client_username: The client's username.
         @type client_username: bytes.
 
@@ -368,26 +393,28 @@
         """
         logger.debug("%s: Pairing [4/5]", self.client_address)
         session_key = self.accessory_handler.srp_verifier.get_session_key()
         output_key = hap_hkdf(
             long_to_bytes(session_key), self.PAIRING_4_SALT, self.PAIRING_4_INFO
         )
 
-        data = output_key + client_username + client_ltpk
+        data = output_key + client_username_bytes + client_ltpk
         verifying_key = ed25519.Ed25519PublicKey.from_public_bytes(client_ltpk)
 
         try:
             verifying_key.verify(client_proof, data)
         except InvalidSignature:
             logger.error("Bad signature, abort.")
             raise
 
-        self._pairing_five(client_username, client_ltpk, encryption_key)
+        self._pairing_five(client_username_bytes, client_ltpk, encryption_key)
 
-    def _pairing_five(self, client_username, client_ltpk, encryption_key):
+    def _pairing_five(
+        self, client_username_bytes: bytes, client_ltpk: bytes, encryption_key: bytes
+    ) -> None:
         """At that point we know the client has the accessory password and has a valid key
         pair. Add it as a pair and send a sever proof.
 
         Parameters are as for _pairing_four.
         """
         logger.debug("%s: Pairing [5/5]", self.client_address)
         session_key = self.accessory_handler.srp_verifier.get_session_key()
@@ -413,21 +440,21 @@
             HAP_TLV_TAGS.PROOF,
             server_proof,
         )
 
         cipher = ChaCha20Poly1305(encryption_key)
         aead_message = bytes(cipher.encrypt(self.PAIRING_5_NONCE, bytes(message), b""))
 
-        client_username_str = str(client_username, "utf-8")
+        client_username_str = client_username_bytes.decode("utf-8")
         client_uuid = uuid.UUID(client_username_str)
         logger.debug(
             "Finishing pairing with admin %s uuid=%s", client_username_str, client_uuid
         )
         should_confirm = self.accessory_handler.pair(
-            client_uuid, client_ltpk, HAP_PERMISSIONS.ADMIN
+            client_username_bytes, client_ltpk, HAP_PERMISSIONS.ADMIN
         )
 
         if not should_confirm:
             self.send_response_with_status(
                 HTTPStatus.INTERNAL_SERVER_ERROR,
                 HAP_SERVER_STATUS.INVALID_VALUE_IN_REQUEST,
             )
@@ -435,18 +462,19 @@
 
         tlv_data = tlv.encode(
             HAP_TLV_TAGS.SEQUENCE_NUM,
             HAP_TLV_STATES.M6,
             HAP_TLV_TAGS.ENCRYPTED_DATA,
             aead_message,
         )
+        assert self.response is not None  # nosec
         self.response.pairing_changed = True
         self._send_tlv_pairing_response(tlv_data)
 
-    def handle_pair_verify(self):
+    def handle_pair_verify(self) -> None:
         """Handles arbitrary step of the pair verify process.
 
         Pair verify is session negotiation.
         """
         if not self.state.paired:
             self._send_authentication_error_tlv_response(HAP_TLV_STATES.M2)
             return
@@ -458,22 +486,22 @@
         elif sequence == HAP_TLV_STATES.M3:
             self._pair_verify_two(tlv_objects)
         else:
             raise ValueError(
                 f"Unknown pairing sequence of {sequence} during pair verify"
             )
 
-    def _pair_verify_one(self, tlv_objects):
+    def _pair_verify_one(self, tlv_objects: Dict[bytes, bytes]) -> None:
         """Generate new session key pair and send a proof to the client.
 
         @param tlv_objects: The TLV data received from the client.
         @type tlv_object: dict
         """
         logger.debug("%s: Pair verify [1/2].", self.client_address)
-        client_public = tlv_objects[HAP_TLV_TAGS.PUBLIC_KEY]
+        client_public: bytes = tlv_objects[HAP_TLV_TAGS.PUBLIC_KEY]
 
         private_key = x25519.X25519PrivateKey.generate()
         public_key = private_key.public_key()
         shared_key = private_key.exchange(
             x25519.X25519PublicKey.from_public_bytes(client_public)
         )
 
@@ -509,15 +537,15 @@
             public_key.public_bytes(
                 encoding=serialization.Encoding.Raw,
                 format=serialization.PublicFormat.Raw,
             ),
         )
         self._send_tlv_pairing_response(data)
 
-    def _pair_verify_two(self, tlv_objects):
+    def _pair_verify_two(self, tlv_objects: Dict[bytes, bytes]) -> None:
         """Verify the client proof and upgrade to encrypted transport.
 
         @param tlv_objects: The TLV data received from the client.
         @type tlv_object: dict
         """
         logger.debug("%s: Pair verify [2/2]", self.client_address)
         encrypted_data = tlv_objects[HAP_TLV_TAGS.ENCRYPTED_DATA]
@@ -541,17 +569,18 @@
             )
         )
 
         client_uuid = uuid.UUID(str(client_username, "utf-8"))
         perm_client_public = self.state.paired_clients.get(client_uuid)
         if perm_client_public is None:
             logger.error(
-                "%s: Client %s attempted pair verify without being paired to %s first.",
+                "%s: Client %s with uuid %s attempted pair verify without being paired first (paired clients=%s).",
                 self.client_address,
                 client_uuid,
+                self.state.paired_clients,
                 self.accessory_handler.accessory.display_name,
             )
             self._send_authentication_error_tlv_response(HAP_TLV_STATES.M4)
             return
 
         verifying_key = ed25519.Ed25519PublicKey.from_public_bytes(perm_client_public)
         try:
@@ -565,35 +594,37 @@
             "%s: Pair verify with client completed. Switching to "
             "encrypted transport.",
             self.client_address,
         )
 
         data = tlv.encode(HAP_TLV_TAGS.SEQUENCE_NUM, HAP_TLV_STATES.M4)
         self._send_tlv_pairing_response(data)
+        assert self.response is not None  # nosec
         self.response.shared_key = self.enc_context["shared_key"]
         self.is_encrypted = True
         self.client_uuid = client_uuid
         del self.enc_context
 
-    def handle_accessories(self):
+    def handle_accessories(self) -> None:
         """Handles a client request to get the accessories."""
         if not self.is_encrypted:
             raise UnprivilegedRequestException
 
         hap_rep = self.accessory_handler.get_accessories()
         self.send_response(HTTPStatus.OK)
         self.send_header("Content-Type", self.JSON_RESPONSE_TYPE)
         self.end_response(to_hap_json(hap_rep))
 
-    def handle_get_characteristics(self):
+    def handle_get_characteristics(self) -> None:
         """Handles a client request to get certain characteristics."""
         if not self.is_encrypted:
             raise UnprivilegedRequestException
 
         # Check that char exists and ...
+        assert self.parsed_url is not None  # nosec
         params = parse_qs(self.parsed_url.query)
         response = self.accessory_handler.get_characteristics(
             params["id"][0].split(",")
         )
         chars = response[HAP_REPR_CHARS]
 
         had_failure = any(
@@ -605,23 +636,24 @@
             self.send_response(HTTPStatus.OK)
             for result in chars:
                 del result[HAP_REPR_STATUS]
 
         self.send_header("Content-Type", self.JSON_RESPONSE_TYPE)
         self.end_response(to_hap_json(response))
 
-    def handle_set_characteristics(self):
+    def handle_set_characteristics(self) -> None:
         """Handles a client request to update certain characteristics."""
         if not self.is_encrypted:
             logger.warning(
                 "%s: Attempt to access unauthorised content", self.client_address
             )
             self.send_response(HTTPStatus.UNAUTHORIZED)
             return
 
+        assert self.request_body is not None  # nosec
         requested_chars = from_hap_json(self.request_body.decode("utf-8"))
         logger.debug(
             "%s: Set characteristics content: %s", self.client_address, requested_chars
         )
 
         response = self.accessory_handler.set_characteristics(
             requested_chars, self.client_address
@@ -647,17 +679,18 @@
         logger.debug("%s: prepare content: %s", self.client_address, request)
 
         response = self.accessory_handler.prepare(request, self.client_address)
         self.send_response(HTTPStatus.OK)
         self.send_header("Content-Type", self.JSON_RESPONSE_TYPE)
         self.end_response(to_hap_json(response))
 
-    def handle_pairings(self):
+    def handle_pairings(self) -> None:
         """Handles a client request to update or remove a pairing."""
         # Must be an admin to handle pairings
+        assert self.client_uuid is not None  # nosec
         if not self.is_encrypted or not self.state.is_admin(self.client_uuid):
             self._send_authentication_error_tlv_response(HAP_TLV_STATES.M2)
             return
 
         tlv_objects = tlv.decode(self.request_body)
         request_type = tlv_objects[HAP_TLV_TAGS.REQUEST_TYPE][0]
         if request_type == 3:
@@ -669,40 +702,37 @@
         else:
             raise ValueError(
                 f"Unknown pairing request type of {request_type} during pair verify"
             )
 
     def _handle_add_pairing(self, tlv_objects):
         """Update client information."""
-        client_username = tlv_objects[HAP_TLV_TAGS.USERNAME]
-        client_username_str = str(client_username, "utf-8")
+        client_username_bytes = tlv_objects[HAP_TLV_TAGS.USERNAME]
         client_public = tlv_objects[HAP_TLV_TAGS.PUBLIC_KEY]
         permissions = tlv_objects[HAP_TLV_TAGS.PERMISSIONS]
-        client_uuid = uuid.UUID(client_username_str)
         logger.debug(
-            "%s: Adding client pairing for %s uuid=%s with permissions %s.",
+            "%s: Adding client pairing for %s with permissions %s.",
             self.client_address,
-            client_username_str,
-            client_uuid,
+            client_username_bytes,
             permissions,
         )
         should_confirm = self.accessory_handler.pair(
-            client_uuid, client_public, permissions
+            client_username_bytes, client_public, permissions
         )
         if not should_confirm:
             self._send_authentication_error_tlv_response(HAP_TLV_STATES.M2)
             return
 
         data = tlv.encode(HAP_TLV_TAGS.SEQUENCE_NUM, HAP_TLV_STATES.M2)
         self._send_tlv_pairing_response(data)
 
-    def _handle_remove_pairing(self, tlv_objects):
+    def _handle_remove_pairing(self, tlv_objects: Dict[bytes, bytes]) -> None:
         """Remove pairing with the client."""
-        client_username = tlv_objects[HAP_TLV_TAGS.USERNAME]
-        client_username_str = str(client_username, "utf-8")
+        client_username_bytes: bytes = tlv_objects[HAP_TLV_TAGS.USERNAME]
+        client_username_str = client_username_bytes.decode("utf-8")
         client_uuid = uuid.UUID(client_username_str)
         was_paired = self.state.paired
         logger.debug(
             "%s: Removing client pairing (%s) uuid=%s (was previously paired=%s).",
             self.client_address,
             client_username_str,
             client_uuid,
@@ -717,58 +747,63 @@
         self._send_tlv_pairing_response(data)
 
         if not self.state.paired_clients and was_paired:
             # Only update the announcement when the last
             # client is removed, otherwise the controller
             # may not remove them all
             logger.debug("%s: updating mdns to unpaired", self.client_address)
+            assert self.response is not None  # nosec
             self.response.pairing_changed = True
 
-    def _handle_list_pairings(self):
+    def _handle_list_pairings(self) -> None:
         """List current pairings."""
         logger.debug("%s: list pairings", self.client_address)
         response = [HAP_TLV_TAGS.SEQUENCE_NUM, HAP_TLV_STATES.M2]
-        for client_uuid, client_public in self.state.paired_clients.items():
+        state = self.state
+        for client_uuid, client_public in state.paired_clients.items():
             admin = self.state.is_admin(client_uuid)
             response.extend(
                 [
                     HAP_TLV_TAGS.USERNAME,
                     # iOS 16+ requires the username to be uppercase
                     # or it will unpair the accessory because it thinks
-                    # the username is invalid
-                    str(client_uuid).encode("utf-8").upper(),
+                    # the username is invalid. We try to send back the
+                    # exact bytes that was used to pair if we have it
+                    state.uuid_to_bytes.get(client_uuid)
+                    or str(client_uuid).encode("utf-8").upper(),
                     HAP_TLV_TAGS.PUBLIC_KEY,
                     client_public,
                     HAP_TLV_TAGS.PERMISSIONS,
                     HAP_PERMISSIONS.ADMIN if admin else HAP_PERMISSIONS.USER,
                 ]
             )
 
         data = tlv.encode(*response)
         self._send_tlv_pairing_response(data)
 
-    def _send_authentication_error_tlv_response(self, sequence):
+    def _send_authentication_error_tlv_response(self, sequence: bytes) -> None:
         """Send an authentication error tlv response."""
         self._send_tlv_pairing_response(
             tlv.encode(
                 HAP_TLV_TAGS.SEQUENCE_NUM,
                 sequence,
                 HAP_TLV_TAGS.ERROR_CODE,
                 HAP_TLV_ERRORS.AUTHENTICATION,
             )
         )
 
-    def _send_tlv_pairing_response(self, data):
+    def _send_tlv_pairing_response(self, data: bytes) -> None:
         """Send a TLV encoded pairing response."""
         self.send_response(HTTPStatus.OK)
         self.send_header("Content-Type", self.PAIRING_RESPONSE_TYPE)
         self.end_response(data)
 
-    def handle_resource(self):
+    def handle_resource(self) -> None:
         """Get a snapshot from the camera."""
+        assert self.request_body is not None  # nosec
         data = from_hap_json(self.request_body.decode("utf-8"))
 
         if self.accessory_handler.accessory.category == CATEGORY_BRIDGE:
             accessory = self.accessory_handler.accessory.accessories.get(data["aid"])
             if not accessory:
                 raise ValueError(f"Accessory with aid == {data['aid']} not found")
         else:
@@ -784,8 +819,9 @@
                 "Got a request for snapshot, but the Accessory "
                 'does not define a "get_snapshot" or "async_get_snapshot" method'
             )
 
         task = asyncio.ensure_future(asyncio.wait_for(coro, RESPONSE_TIMEOUT))
         self.send_response(HTTPStatus.OK)
         self.send_header("Content-Type", "image/jpeg")
+        assert self.response is not None  # nosec
         self.response.task = task
```

### Comparing `HAP-python-4.6.0/pyhap/hap_protocol.py` & `HAP-python-4.7.0/pyhap/hap_protocol.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/hap_server.py` & `HAP-python-4.7.0/pyhap/hap_server.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/hsrp.py` & `HAP-python-4.7.0/pyhap/hsrp.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/iid_manager.py` & `HAP-python-4.7.0/pyhap/iid_manager.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/loader.py` & `HAP-python-4.7.0/pyhap/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 HAP services and characteristics from a json
 representation.
 
 The idea is, give a name of a service and you get an
 instance of it (as long as it is described in some
 json file).
 """
-import json
 import logging
 
+import orjson
+
 from pyhap import CHARACTERISTICS_FILE, SERVICES_FILE
 from pyhap.characteristic import Characteristic
 from pyhap.service import Service
 
 _loader = None
 logger = logging.getLogger(__name__)
 
@@ -30,15 +31,15 @@
         self.char_types = self._read_file(path_char)
         self.serv_types = self._read_file(path_service)
 
     @staticmethod
     def _read_file(path):
         """Read file and return a dict."""
         with open(path, "r", encoding="utf8") as file:
-            return json.load(file)
+            return orjson.loads(file.read())  # pylint: disable=no-member
 
     def get_char(self, name):
         """Return new Characteristic object."""
         char_dict = self.char_types[name].copy()
         if (
             "Format" not in char_dict
             or "Permissions" not in char_dict
```

### Comparing `HAP-python-4.6.0/pyhap/params.py` & `HAP-python-4.7.0/pyhap/params.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/resources/characteristics.json` & `HAP-python-4.7.0/pyhap/resources/characteristics.json`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/resources/services.json` & `HAP-python-4.7.0/pyhap/resources/services.json`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/resources/snapshot.jpg` & `HAP-python-4.7.0/pyhap/resources/snapshot.jpg`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/service.py` & `HAP-python-4.7.0/pyhap/service.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/tlv.py` & `HAP-python-4.7.0/pyhap/tlv.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.6.0/pyhap/util.py` & `HAP-python-4.7.0/pyhap/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,29 @@
     check the wrapped function for the same.
     """
     if isinstance(func, functools.partial):
         func = func.func
     return asyncio.iscoroutinefunction(func)
 
 
-def get_local_address():
+def get_local_address() -> str:
     """
     Grabs the local IP address using a socket.
 
     :return: Local IP Address in IPv4 format.
     :rtype: str
     """
     # TODO: try not to talk 8888 for this
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         s.connect(("8.8.8.8", 80))
         addr = s.getsockname()[0]
     finally:
         s.close()
-    return addr
+    return str(addr)
 
 
 def long_to_bytes(n):
     """
     Convert a ``long int`` to ``bytes``
 
     :param n: Long Integer
```

### Comparing `HAP-python-4.6.0/setup.py` & `HAP-python-4.7.0/setup.py`

 * *Files identical despite different names*

