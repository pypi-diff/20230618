# Comparing `tmp/wavebin-2.1.tar.gz` & `tmp/wavebin-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wavebin-2.1.tar", last modified: Sat Feb 27 02:28:13 2021, max compression
+gzip compressed data, was "wavebin-2.2.tar", last modified: Sun Jun 18 09:20:53 2023, max compression
```

## Comparing `wavebin-2.1.tar` & `wavebin-2.2.tar`

### file list

```diff
@@ -1,17 +1,59 @@
-drwxrwxrwx   0        0        0        0 2021-02-27 02:28:13.732767 wavebin-2.1/
--rw-rw-rw-   0        0        0     8165 2021-02-27 02:28:13.726768 wavebin-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6239 2021-02-27 00:45:36.000000 wavebin-2.1/README.md
--rw-rw-rw-   0        0        0       42 2021-02-27 02:28:13.732767 wavebin-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1300 2021-02-27 00:40:13.000000 wavebin-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-27 02:28:13.717767 wavebin-2.1/wavebin/
--rw-rw-rw-   0        0        0     2877 2021-02-27 01:13:19.000000 wavebin-2.1/wavebin/__main__.py
--rw-rw-rw-   0        0        0     4742 2021-02-27 00:46:58.000000 wavebin-2.1/wavebin/export.py
--rw-rw-rw-   0        0        0    16866 2021-02-27 02:22:39.000000 wavebin-2.1/wavebin/interface.py
--rw-rw-rw-   0        0        0     7712 2021-02-27 02:20:33.000000 wavebin-2.1/wavebin/plot.py
--rw-rw-rw-   0        0        0     5338 2021-02-27 00:46:40.000000 wavebin-2.1/wavebin/wave.py
-drwxrwxrwx   0        0        0        0 2021-02-27 02:28:13.725767 wavebin-2.1/wavebin.egg-info/
--rw-rw-rw-   0        0        0     8165 2021-02-27 02:28:13.000000 wavebin-2.1/wavebin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2021-02-27 02:28:13.000000 wavebin-2.1/wavebin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-27 02:28:13.000000 wavebin-2.1/wavebin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2021-02-27 02:28:13.000000 wavebin-2.1/wavebin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-02-27 02:28:13.000000 wavebin-2.1/wavebin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:53.060455 wavebin-2.2/
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:52.934517 wavebin-2.2/.github/
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:52.946037 wavebin-2.2/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      611 2023-06-18 09:10:35.000000 wavebin-2.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-rw-rw-   0        0        0     1307 2023-06-18 09:10:35.000000 wavebin-2.2/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:52.947038 wavebin-2.2/.vscode/
+-rw-rw-rw-   0        0        0      798 2023-06-18 09:10:35.000000 wavebin-2.2/.vscode/launch.json
+-rw-rw-rw-   0        0        0     2685 2023-06-18 09:10:35.000000 wavebin-2.2/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     2806 2023-06-18 09:18:19.000000 wavebin-2.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1081 2023-06-18 09:10:35.000000 wavebin-2.2/LICENSE
+-rw-rw-rw-   0        0        0     7250 2023-06-18 09:20:53.059449 wavebin-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6239 2023-06-18 09:20:16.000000 wavebin-2.2/README.md
+-rw-rw-rw-   0        0        0     1094 2023-06-18 09:10:35.000000 wavebin-2.2/icon.ico
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:52.948036 wavebin-2.2/samples/
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:53.007171 wavebin-2.2/samples/DSOX1102G/
+-rw-rw-rw-   0        0        0     8164 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/data.bin
+-rw-rw-rw-   0        0        0    35540 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/data.png
+-rw-rw-rw-   0        0        0      502 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/data.sr
+-rw-rw-rw-   0        0        0      400 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/data.txt
+-rw-rw-rw-   0        0        0   100316 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/digital.bin
+-rw-rw-rw-   0        0        0    22983 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/digital.png
+-rw-rw-rw-   0        0        0      605 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/digital.txt
+-rw-rw-rw-   0        0        0    32316 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/dual.bin
+-rw-rw-rw-   0        0        0    18133 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/dual.png
+-rw-rw-rw-   0        0        0      608 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/dual.txt
+-rw-rw-rw-   0        0        0     7976 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/single.bin
+-rw-rw-rw-   0        0        0    20555 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/single.png
+-rw-rw-rw-   0        0        0      487 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/single.txt
+-rw-rw-rw-   0        0        0  4000160 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/uart.bin
+-rw-rw-rw-   0        0        0    31886 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/uart.png
+-rw-rw-rw-   0        0        0      266 2023-06-18 09:10:35.000000 wavebin-2.2/samples/DSOX1102G/uart.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:53.030180 wavebin-2.2/samples/MSO5000/
+-rw-rw-rw-   0        0        0 16000620 2023-06-18 09:10:35.000000 wavebin-2.2/samples/MSO5000/Rigol_MSO5000_4CH_10MSPS_1Mpts.bin
+-rw-rw-rw-   0        0        0   118234 2023-06-18 09:10:35.000000 wavebin-2.2/samples/MSO5000/Rigol_MSO5000_4CH_10MSPS_1Mpts.png
+-rw-rw-rw-   0        0        0    16620 2023-06-18 09:10:35.000000 wavebin-2.2/samples/MSO5000/Rigol_MSO5000_4CH_200KSPS_1Kpts.bin
+-rw-rw-rw-   0        0        0    86931 2023-06-18 09:10:35.000000 wavebin-2.2/samples/MSO5000/Rigol_MSO5000_4CH_200KSPS_1Kpts.png
+-rw-rw-rw-   0        0        0 32000620 2023-06-18 09:10:35.000000 wavebin-2.2/samples/MSOX4154A.bin
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:53.037299 wavebin-2.2/screenshots/
+-rw-rw-rw-   0        0        0    43614 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/clipping.png
+-rw-rw-rw-   0        0        0    55807 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/console.png
+-rw-rw-rw-   0        0        0    34962 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/filtering.png
+-rw-rw-rw-   0        0        0    85506 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/pulseview.png
+-rw-rw-rw-   0        0        0    38675 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/subsampling.png
+-rw-rw-rw-   0        0        0    47437 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/wav.png
+-rw-rw-rw-   0        0        0    21403 2023-06-18 09:10:35.000000 wavebin-2.2/screenshots/wavebin.png
+-rw-rw-rw-   0        0        0       42 2023-06-18 09:20:53.060455 wavebin-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-06-18 09:15:34.000000 wavebin-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:53.044298 wavebin-2.2/wavebin/
+-rw-rw-rw-   0        0        0     2883 2023-06-18 09:15:44.000000 wavebin-2.2/wavebin/__main__.py
+-rw-rw-rw-   0        0        0     5263 2023-06-18 09:10:35.000000 wavebin-2.2/wavebin/export.py
+-rw-rw-rw-   0        0        0    16310 2023-06-18 09:10:35.000000 wavebin-2.2/wavebin/interface.py
+-rw-rw-rw-   0        0        0     7660 2023-06-18 09:10:35.000000 wavebin-2.2/wavebin/plot.py
+-rw-rw-rw-   0        0        0     5306 2023-06-18 09:10:35.000000 wavebin-2.2/wavebin/wave.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:20:53.058451 wavebin-2.2/wavebin.egg-info/
+-rw-rw-rw-   0        0        0     7250 2023-06-18 09:20:52.000000 wavebin-2.2/wavebin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2023-06-18 09:20:52.000000 wavebin-2.2/wavebin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 09:20:52.000000 wavebin-2.2/wavebin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-18 09:20:52.000000 wavebin-2.2/wavebin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 09:20:52.000000 wavebin-2.2/wavebin.egg-info/top_level.txt
```

### Comparing `wavebin-2.1/PKG-INFO` & `wavebin-2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,137 +1,111 @@
-Metadata-Version: 2.1
-Name: wavebin
-Version: 2.1
-Summary: Waveform capture viewer for Agilent, Keysight and Rigol oscilloscopes
-Home-page: https://github.com/sam210723/wavebin
-Author: sam210723
-Author-email: pypi@vksdr.com
-License: UNKNOWN
-Description: # <img src="https://raw.githubusercontent.com/sam210723/wavebin/master/icon.ico" width=24 /> Oscilloscope Waveform Capture Viewer
-        
-        [![GitHub release](https://img.shields.io/github/release/sam210723/wavebin.svg)](https://pypi.org/project/wavebin/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wavebin)](https://pypi.org/project/wavebin/)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dw/wavebin)](https://pypi.org/project/wavebin/)
-        [![GitHub license](https://img.shields.io/github/license/sam210723/wavebin.svg)](https://github.com/sam210723/wavebin/master/LICENSE)
-        
-        **wavebin** reads binary capture files generated by Agilent, Keysight and Rigol oscilloscopes and renders the waveforms in an interactive plot. Waveforms can be inspected, [filtered](#filtering), [clipped](#clipping), [subsampled](#subsampling) and exported to [sigrok PulseView](#export-to-pulseview) or [WAV files](#export-to-wav).
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/wavebin.png)
-        
-        **wavebin** has been tested with capture files from a [**Keysight DSO-X 1102G**](https://www.keysight.com/en/pdx-2766207-pn-DSOX1102G/oscilloscope-70-100-mhz-2-analog-channels), [**Keysight MSO-X 4154A**](https://www.keysight.com/en/pdx-x201943-pn-MSOX4154A/mixed-signal-oscilloscope-15-ghz-4-analog-plus-16-digital-channels) and [**Rigol MSO5074**](https://www.rigolna.com/products/digital-oscilloscopes/MSO5000/). If you have access to waveform files from other Agilent, Keysight or Rigol oscilloscopes, please submit them for testing through the [Sample Waveforms issue](https://github.com/sam210723/wavebin/issues/1).
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/console.png)
-        
-        
-        ## Getting Started
-        **wavebin** is available via the [Python Package Index (PyPI)](https://pypi.org/project/wavebin/) and is installed using [pip](https://pip.pypa.io/en/stable/).
-        
-        ```
-        > pip3 install wavebin
-        ```
-        
-        Keysight oscilloscopes save capture files to external USB Mass Storage devices for easy transfer to a PC. These files use the `.bin` extension.
-        To open a capture file in **wavebin**, start the application by running:
-        
-        ```
-        > python3 -m wavebin
-        ```
-        
-        Next, click *File* &#8594; *Open* and navigate to the `.bin` file.
-        
-        
-        Alternatively a capture file path can be specified when running **wavebin** using the `-i` argument.
-        
-        ```
-        > python3 -m wavebin -i [PATH TO BIN FILE]
-        ```
-        
-        For more information about the **wavebin** command-line arguments run:
-        
-        ```
-        > python3 -m wavebin -h
-                                      __    _
-           _      ______ __   _____  / /_  (_)___
-          | | /| / / __ `/ | / / _ \/ __ \/ / __ \
-          | |/ |/ / /_/ /| |/ /  __/ /_/ / / / / /
-          |__/|__/\__,_/ |___/\___/_.___/_/_/ /_/  v2.1
-        
-                     vksdr.com/wavebin
-        
-        
-        usage: wavebin [-h] [-i FILE] [-v] [--no-opengl] [--no-limit]
-        
-        Waveform capture viewer for Keysight oscilloscopes.
-        
-        optional arguments:
-          -h, --help   show this help message and exit
-          -i FILE      path to Keysight waveform capturefile (.bin)
-          -v           enable verbose logging mode
-          --no-opengl  disable hardware accelerated rendering with OpenGL
-          --no-limit   disable subsampling limit (may cause slow frame rates with large captures)
-        ```
-        
-        ## Features
-        ### Export to PulseView
-        [PulseView](https://sigrok.org/wiki/PulseView) by [sigrok](https://sigrok.org) is a logic analysis tool typically used with hardware logic analyser devices. It is capable of decoding many serial and parallel protocols with its built-in decoders.
-        
-        Below is a 115200bd UART waveform captured on a **DSO-X 1102G**, loaded into **wavebin** with [clipping](#clipping) enabled to create a clean digital waveform, exported to PulseView and decoded using the PulseView UART protocol decoder.
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/pulseview.png)
-        
-        To export waveforms to PulseView, click *File* &#8594; *Export to PulseView* then navigate to a save location. The produced [`.sr` file](https://sigrok.org/wiki/File_format:Sigrok/v2) can then be opened directly in PulseView.
-        
-        ### Export to WAV
-        WAV files can be opened in most media players (e.g. [VLC](https://www.videolan.org/vlc/)) and audio editors (e.g. [Audacity](https://www.audacityteam.org/)).
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/wav.png)
-        
-        To export waveforms to WAV files, click *File* &#8594; *Export to WAV file* then navigate to a save location. This will produce a mono `.wav` file for each waveform. The WAV files names follow the format `*_[n].wav`, where `n` is the waveform number starting at `0`.
-        
-        
-        ### Filtering
-        A [Savitzky-Golay low pass filter](https://en.wikipedia.org/wiki/Savitzky%E2%80%93Golay_filter) is included in **wavebin** for smoothing waveforms. This filter can be enabled using the *Filter Type* dropdown menu.
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/filtering.png)
-        
-        
-        ### Clipping
-        The clipping option converts analog waveforms to digital waveforms in a similar way to a Schmitt trigger.
-        
-        The [filtering](#filtering) and clipping options can be used simultaneously. Clipping is always applied after filtering.
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/clipping.png)
-        
-        
-        ### Subsampling
-        When a waveform capture is first loaded, all available sample points will be used to render the waveform.
-        The subsampling option renders the waveform using an equally-spaced subset of points.
-        
-        Below is a 62.5 MHz wave being rendered with all `20,000` points in the capture file, and then with only `1250` points.
-        
-        ![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/subsampling.png)
-        
-        By default, waveforms with over `50,000` points will automatically be subsampled. This can be overridden using the `--no-limit` switch.
-        
-        ## Resources
-          - [FaustinCarter/agilent_read_binary](https://github.com/FaustinCarter/agilent_read_binary)
-          - [yodalee/keysightBin](https://github.com/yodalee/keysightBin/)
-          - [Input output formats - sigrok](https://sigrok.org/wiki/Input_output_formats)
-          - [File format:sigrok/v2 - sigrok](https://sigrok.org/wiki/File_format:Sigrok/v2)
-        
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Environment :: Console
-Classifier: Environment :: X11 Applications :: Qt
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.6
-Description-Content-Type: text/markdown
+# <img src="https://raw.githubusercontent.com/sam210723/wavebin/master/icon.ico" width=24 /> Oscilloscope Waveform Capture Viewer
+
+[![GitHub release](https://img.shields.io/github/release/sam210723/wavebin.svg)](https://pypi.org/project/wavebin/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wavebin)](https://pypi.org/project/wavebin/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/wavebin)](https://pypi.org/project/wavebin/)
+[![GitHub license](https://img.shields.io/github/license/sam210723/wavebin.svg)](https://github.com/sam210723/wavebin/master/LICENSE)
+
+**wavebin** reads binary capture files generated by Agilent, Keysight and Rigol oscilloscopes and renders the waveforms in an interactive plot. Waveforms can be inspected, [filtered](#filtering), [clipped](#clipping), [subsampled](#subsampling) and exported to [sigrok PulseView](#export-to-pulseview) or [WAV files](#export-to-wav).
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/wavebin.png)
+
+**wavebin** has been tested with capture files from a [**Keysight DSO-X 1102G**](https://www.keysight.com/en/pdx-2766207-pn-DSOX1102G/oscilloscope-70-100-mhz-2-analog-channels), [**Keysight MSO-X 4154A**](https://www.keysight.com/en/pdx-x201943-pn-MSOX4154A/mixed-signal-oscilloscope-15-ghz-4-analog-plus-16-digital-channels) and [**Rigol MSO5074**](https://www.rigolna.com/products/digital-oscilloscopes/MSO5000/). If you have access to waveform files from other Agilent, Keysight or Rigol oscilloscopes, please submit them for testing through the [Sample Waveforms issue](https://github.com/sam210723/wavebin/issues/1).
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/console.png)
+
+
+## Getting Started
+**wavebin** is available via the [Python Package Index (PyPI)](https://pypi.org/project/wavebin/) and is installed using [pip](https://pip.pypa.io/en/stable/).
+
+```
+> pip3 install wavebin
+```
+
+Keysight oscilloscopes save capture files to external USB Mass Storage devices for easy transfer to a PC. These files use the `.bin` extension.
+To open a capture file in **wavebin**, start the application by running:
+
+```
+> python3 -m wavebin
+```
+
+Next, click *File* &#8594; *Open* and navigate to the `.bin` file.
+
+
+Alternatively a capture file path can be specified when running **wavebin** using the `-i` argument.
+
+```
+> python3 -m wavebin -i [PATH TO BIN FILE]
+```
+
+For more information about the **wavebin** command-line arguments run:
+
+```
+> python3 -m wavebin -h
+                              __    _
+   _      ______ __   _____  / /_  (_)___
+  | | /| / / __ `/ | / / _ \/ __ \/ / __ \
+  | |/ |/ / /_/ /| |/ /  __/ /_/ / / / / /
+  |__/|__/\__,_/ |___/\___/_.___/_/_/ /_/  v2.2
+
+             vksdr.com/wavebin
+
+
+usage: wavebin [-h] [-i FILE] [-v] [--no-opengl] [--no-limit]
+
+Waveform capture viewer for Keysight oscilloscopes.
+
+optional arguments:
+  -h, --help   show this help message and exit
+  -i FILE      path to Keysight waveform capturefile (.bin)
+  -v           enable verbose logging mode
+  --no-opengl  disable hardware accelerated rendering with OpenGL
+  --no-limit   disable subsampling limit (may cause slow frame rates with large captures)
+```
+
+## Features
+### Export to PulseView
+[PulseView](https://sigrok.org/wiki/PulseView) by [sigrok](https://sigrok.org) is a logic analysis tool typically used with hardware logic analyser devices. It is capable of decoding many serial and parallel protocols with its built-in decoders.
+
+Below is a 115200bd UART waveform captured on a **DSO-X 1102G**, loaded into **wavebin** with [clipping](#clipping) enabled to create a clean digital waveform, exported to PulseView and decoded using the PulseView UART protocol decoder.
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/pulseview.png)
+
+To export waveforms to PulseView, click *File* &#8594; *Export to PulseView* then navigate to a save location. The produced [`.sr` file](https://sigrok.org/wiki/File_format:Sigrok/v2) can then be opened directly in PulseView.
+
+### Export to WAV
+WAV files can be opened in most media players (e.g. [VLC](https://www.videolan.org/vlc/)) and audio editors (e.g. [Audacity](https://www.audacityteam.org/)).
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/wav.png)
+
+To export waveforms to WAV files, click *File* &#8594; *Export to WAV file* then navigate to a save location. This will produce a mono `.wav` file for each waveform. The WAV files names follow the format `*_[n].wav`, where `n` is the waveform number starting at `0`.
+
+
+### Filtering
+A [Savitzky-Golay low pass filter](https://en.wikipedia.org/wiki/Savitzky%E2%80%93Golay_filter) is included in **wavebin** for smoothing waveforms. This filter can be enabled using the *Filter Type* dropdown menu.
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/filtering.png)
+
+
+### Clipping
+The clipping option converts analog waveforms to digital waveforms in a similar way to a Schmitt trigger.
+
+The [filtering](#filtering) and clipping options can be used simultaneously. Clipping is always applied after filtering.
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/clipping.png)
+
+
+### Subsampling
+When a waveform capture is first loaded, all available sample points will be used to render the waveform.
+The subsampling option renders the waveform using an equally-spaced subset of points.
+
+Below is a 62.5 MHz wave being rendered with all `20,000` points in the capture file, and then with only `1250` points.
+
+![](https://raw.githubusercontent.com/sam210723/wavebin/master/screenshots/subsampling.png)
+
+By default, waveforms with over `50,000` points will automatically be subsampled. This can be overridden using the `--no-limit` switch.
+
+## Resources
+  - [FaustinCarter/agilent_read_binary](https://github.com/FaustinCarter/agilent_read_binary)
+  - [yodalee/keysightBin](https://github.com/yodalee/keysightBin/)
+  - [Input output formats - sigrok](https://sigrok.org/wiki/Input_output_formats)
+  - [File format:sigrok/v2 - sigrok](https://sigrok.org/wiki/File_format:Sigrok/v2)
```

### Comparing `wavebin-2.1/README.md` & `wavebin-2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: wavebin
+Version: 2.2
+Summary: Waveform capture viewer for Agilent, Keysight and Rigol oscilloscopes
+Home-page: https://github.com/sam210723/wavebin
+Author: sam210723
+Author-email: pypi@vksdr.com
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Environment :: Console
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # <img src="https://raw.githubusercontent.com/sam210723/wavebin/master/icon.ico" width=24 /> Oscilloscope Waveform Capture Viewer
 
 [![GitHub release](https://img.shields.io/github/release/sam210723/wavebin.svg)](https://pypi.org/project/wavebin/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wavebin)](https://pypi.org/project/wavebin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/wavebin)](https://pypi.org/project/wavebin/)
 [![GitHub license](https://img.shields.io/github/license/sam210723/wavebin.svg)](https://github.com/sam210723/wavebin/master/LICENSE)
 
@@ -41,15 +66,15 @@
 
 ```
 > python3 -m wavebin -h
                               __    _
    _      ______ __   _____  / /_  (_)___
   | | /| / / __ `/ | / / _ \/ __ \/ / __ \
   | |/ |/ / /_/ /| |/ /  __/ /_/ / / / / /
-  |__/|__/\__,_/ |___/\___/_.___/_/_/ /_/  v2.1
+  |__/|__/\__,_/ |___/\___/_.___/_/_/ /_/  v2.2
 
              vksdr.com/wavebin
 
 
 usage: wavebin [-h] [-i FILE] [-v] [--no-opengl] [--no-limit]
 
 Waveform capture viewer for Keysight oscilloscopes.
```

### Comparing `wavebin-2.1/setup.py` & `wavebin-2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='wavebin',
-    version='2.1',
+    version='2.2',
     packages=['wavebin'],
     author="sam210723",
     author_email="pypi@vksdr.com",
     description="Waveform capture viewer for Agilent, Keysight and Rigol oscilloscopes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sam210723/wavebin",
```

### Comparing `wavebin-2.1/wavebin/__main__.py` & `wavebin-2.2/wavebin/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 from pathlib import Path
 import sys
 
 from wavebin.interface import QtApp
 from wavebin.plot import QtPlot
 from wavebin.wave import WaveParser
 
-__version__ = 2.1
+__version__ = 2.2
 
 
 def init():
     print( "                              __    _        ")
     print( "   _      ______ __   _____  / /_  (_)___    ")
     print( "  | | /| / / __ `/ | / / _ \\/ __ \\/ / __ \\")
     print( "  | |/ |/ / /_/ /| |/ /  __/ /_/ / / / / /   ")
     print(f"  |__/|__/\\__,_/ |___/\\___/_.___/_/_/ /_/  v{__version__}\n")
     print( "             vksdr.com/wavebin\n\n")
 
     # Parse CLI arguments
     args = parse_args()
-    
+
     # Print startup info
     print_info(args)
 
     # Setup waveform capture parser
     wave = WaveParser({
         "verbose":     args.v
     })
 
     # Get subsampling limit
     if args.no_limit:
-        limit = 10e6
+        limit = int(10e6)
     else:
-        limit = 50e3
+        limit = int(50e3)
 
     # Create Qt application
     app = QtApp({
         "verbose": args.v,
         "version": __version__,
         "width":   1100,
         "height":  350,
```

### Comparing `wavebin-2.1/wavebin/export.py` & `wavebin-2.2/wavebin/export.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 Waveform capture viewer for oscilloscopes.
 """
 
 from pathlib import Path
 import numpy
 import wave
+import struct
 import zipfile
 
-
 class PulseView():
     def __init__(self, verbose, path, waveforms, clipped):
         self.verbose = verbose
         self.path = path
         self.waveforms = waveforms
         self.clipped = clipped
 
@@ -40,61 +40,75 @@
 
     def metadata(self):
         meta =   "[global]\r\n"
         meta +=  "sigrok version=0.5.2\r\n"
         meta +=  "\r\n"
 
         meta +=  "[device 1]\r\n"
-        meta +=  "capturefile=logic-1\r\n"
-        meta +=  "unitsize=1\r\n"
-        meta += f"total probes={len(self.waveforms)}\r\n"
-        meta += f"samplerate={round(self.get_sample_rate(), 4) / 1e6} MHz\r\n"
-        meta +=  "total analog=0\r\n"       #TODO: Use 'clipped' flag to export analog waveforms
-        
-        for i in range(len(self.waveforms)):
-            meta +=  f"probe{i + 1}=D{i}\r\n"
+        if self.clipped:
+            meta +=  "capturefile=logic-1\r\n"
+            meta +=  "unitsize=1\r\n"
+            meta += f"total probes={len(self.waveforms)}\r\n"
+        else:
+            meta += f"total analog={len(self.waveforms)}\r\n"
+        meta += f"samplerate={int(round(self.get_sample_rate(), 4) / 1e3)} kHz\r\n"
+
+        if self.clipped:
+            for i in range(len(self.waveforms)):
+                meta +=  f"probe{i + 1}=D{i}\r\n"
+        else:
+            for i in range(len(self.waveforms)):
+                meta += f"analog{i + 1}=A{i}\r\n"
+
         meta +=  "\r\n"
 
         return meta
 
 
     def write_data(self):
         num = len(self.waveforms[0]['data'])
-        data = bytearray(b'')
 
-        # Loop through waveform samples
-        for i in range(num):
-            sample = 0x00
-
-            # Loop through waveforms
-            for j, w in enumerate(self.waveforms):
-                # Get current sample
-                point = w['data'][i]
-
-                # Set bit for waveform
-                if point == 1: sample |= 1 << j
-            
-            # Add byte to data buffer
-            data.append(sample)
+        if self.clipped:
+            data = bytearray(b'')
+
+            # Loop through waveform samples
+            for i in range(num):
+                sample = 0x00
+
+                # Loop through waveforms
+                for j, w in enumerate(self.waveforms):
+                    # Get current sample
+                    point = w['data'][i]
 
-        # Write data to ZIP file
-        self.zipf.writestr(f"logic-1", bytes(data))
+                    # Set bit for waveform
+                    if point == 1: sample |= 1 << j
 
+                # Add byte to data buffer
+                data.append(sample)
+
+            # Write data to ZIP file
+            self.zipf.writestr(f"logic-1", bytes(data))
+        else:
+            for i, waveform in enumerate(self.waveforms):
+                data = bytearray(b'')
+                for point in waveform['data']:
+                    data.extend(struct.pack("f", point))
+                self.zipf.writestr(f"analog-1-{i + 1}-1", bytes(data))
 
     def get_sample_rate(self):
         # Check if waveform is subsampled
         if self.waveforms[0]['header'].points != len(self.waveforms[0]['data']):
             # Calculate new sample increment value
             dur = self.waveforms[0]['header'].x_increment * self.waveforms[0]['header'].points
             inc = dur / len(self.waveforms[0]['data'])
             sr = 1 / inc
         else:
             # Use increment value from waveform header
             sr  = 1 / self.waveforms[0]['header'].x_increment
-        
+
         return sr
 
 
     def log(self, msg):
         if self.verbose: print(msg)
 
 
@@ -128,24 +142,24 @@
             self.wavf.close()
 
         #TODO: Fix analog waveform exporting
         #TODO: Add max (ulong) data rate check
 
         self.log("Finished exporting")
 
-    
+
     def get_sample_rate(self, i):
         # Check if waveform is subsampled
         if self.waveforms[i]['header'].points != len(self.waveforms[i]['data']):
             # Calculate new sample increment value
             dur = self.waveforms[i]['header'].x_increment * self.waveforms[i]['header'].points
             inc = dur / len(self.waveforms[i]['data'])
             sr = 1 / inc
         else:
             # Use increment value from waveform header
             sr  = 1 / self.waveforms[i]['header'].x_increment
-        
+
         return sr
 
 
     def log(self, msg):
         if self.verbose: print(msg)
```

### Comparing `wavebin-2.1/wavebin/interface.py` & `wavebin-2.2/wavebin/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.window.show()
         self.exec_()
 
 
     def update(self):
         self.log("Updating UI")
         self.window.setWindowTitle(f"\"{self.config['file'].name}\"")
-        
+
         # Limit number of points for large captures
         points = len(self.config['wave'].waveforms[0]['data'])
         if points > self.config['limit']:
             subsampling = self.config['limit']
         else:
             subsampling = points
 
@@ -128,15 +128,15 @@
         # Add actions to menu items
         for a in self.menu_actions:
             if a.split("_")[1] == "----":
                 self.menus[a.split("_")[0]].addSeparator()
                 continue
             self.menu_actions[a].triggered.connect(eval(f"self.menu_{a}"))
             self.menus[a.split("_")[0]].addAction(self.menu_actions[a])
-        
+
         # Attach keyboard event handler
         self.window.keyPressEvent = self.keyPressEvent
 
 
     def instances(self, wave, plot):
         self.config['wave'] = wave
         self.config['plot'] = plot
@@ -147,15 +147,15 @@
     def keyPressEvent(self, event):
         key = event.key()
 
         try:
             char = chr(key)
         except ValueError:
             char = None
-        
+
         if char == 'B':
             self.menu_actions['view_sidebar'].toggle()
             self.sidebar.toggle()
 
 
     def menu_file_open(self):
         # Get initial path
@@ -172,15 +172,15 @@
             "Waveform files (*.bin);;All files (*.*)"
         )[0]
 
         # Handle cancelled dialog
         if file_path == "":
             self.log("Open file dialog cancelled")
             return
-        
+
         # Reset sidebar controls
         self.sidebar.update(0, False, -1)
 
         # Parse waveform capture
         if not self.config['wave'].parse(file_path):
             msgbox = qt.QMessageBox()
             msgbox.setWindowTitle("Error")
@@ -189,24 +189,14 @@
             msgbox.setText(
                 f"Error opening \"{Path(file_path).name}\": Unknown file format"
             )
             msgbox.exec_()
 
 
     def menu_file_export_pv(self):
-        # Check waveform has been clipped
-        if not self.sidebar.config['parts'][1]['widget'].isChecked():
-            msgbox = qt.QMessageBox()
-            msgbox.setWindowTitle("Error")
-            msgbox.setIcon(qt.QMessageBox.Critical)
-            msgbox.setStandardButtons(qt.QMessageBox.Ok)
-            msgbox.setText("Enable waveform clipping before exporting to PulseView")
-            msgbox.exec_()
-            return
-
         # Show save file dialog
         file_path = self.sfd.getSaveFileName(
             self.window,
             "Export to PulseView",
             f"./{self.config['file'].name.split('.')[0]}.sr",
             "sigrok Sessions (*.sr)"
         )[0]
@@ -219,15 +209,15 @@
         # Create PulseView session file
         PulseView(
             self.config['verbose'],
             file_path,
             self.config['plot'].processed_waveforms,
             self.sidebar.config['parts'][1]['widget'].isChecked()
         )
-    
+
 
     def menu_file_export_wav(self):
         # Check waveform has been clipped
         if not self.sidebar.config['parts'][1]['widget'].isChecked():
             msgbox = qt.QMessageBox()
             msgbox.setWindowTitle("Error")
             msgbox.setIcon(qt.QMessageBox.Critical)
@@ -304,24 +294,24 @@
             info += f"  - X Display Range:\t{rng} μs\n"
 
             dorigin = round(header.x_d_origin * float(10**6), 3)
             info += f"  - X Display Origin:\t{dorigin} μs\n"
 
             increment = round(header.x_increment * float(10**9), 3)
             info += f"  - X Increment:\t\t{increment} ns\n"
-            
+
             origin = round(header.x_origin * float(10**6), 3)
             info += f"  - X Origin:\t\t{origin} μs\n"
 
             frame = header.frame.decode().split(":")
             info += f"  - Frame Type:\t\t{frame[0]}\n"
             info += f"  - Frame Serial:\t\t{frame[1]}\n"
             info += f"  - Date:\t\t\t{header.date.decode()}\n"
             info += f"  - Time:\t\t\t{header.time.decode()}\n"
-            
+
             info += f"  - Waveform Label:\t{header.label.decode()}\n"
             info += f"  - Time Tags:\t\t{header.time_tags}\n"
             info += f"  - Segment Number:\t{header.segment}\n"
 
             info += "\n"
 
         # Show messagebox
@@ -396,15 +386,15 @@
             "font-weight: normal;"\
             "font-size: 17px;"
         )
 
         self.config = {}
         self.config['parts'] = []
         self.build()
-    
+
 
     def build(self):
         self.config['parts'].append({"name": "Filter Type", "widget": qt.QComboBox()})
         self.config['parts'].append({"name": "Clipping", "widget": qt.QPushButton("OFF")})
         self.config['parts'].append({"name": "Subsampling", "widget": qt.QSpinBox()})
 
         # Add filter dropdown options
@@ -424,36 +414,36 @@
         for i, p in enumerate(self.config['parts']):
             # Add new table row
             self.setRowCount(self.rowCount() + 1)
 
             # Set row name
             self.setItem(i, 0, qt.QTableWidgetItem(p['name']))
             self.setCellWidget(i, 1, p['widget'])
-        
+
         # Bold left column
         f = qtg.QFont()
         f.setBold(True)
         for i, p in enumerate(self.config['parts']):
             self.item(i, 0).setFont(f)
-        
+
         # Remove focus from sidebar widgets
         self.config['parts'][0]['widget'].clearFocus()
         self.config['parts'][1]['widget'].clearFocus()
         self.config['parts'][2]['widget'].clearFocus()
 
 
     def update(self, f, c, p):
         if f != None:
             self.config['parts'][0]['widget'].setCurrentIndex(f)
             self.filter_changed(f)
-        
+
         if c != None:
             self.config['parts'][1]['widget'].setChecked(c)
             self.clipping_changed(c)
-        
+
         if p != None:
             # Set subsampling spin box min/max
             self.config['parts'][2]['widget'].setMinimum(2)
             self.config['parts'][2]['widget'].setMaximum(p)
             self.config['parts'][2]['widget'].setValue(p)
             self.subsampling_changed(p)
 
@@ -473,27 +463,27 @@
 
         if btn.isChecked():
             btn.setText("ON")
             btn.setStyleSheet("background: green; color: white;")
         else:
             btn.setStyleSheet("background: red; color: white;")
             btn.setText("OFF")
-        
+
         self.config['plot'].config['clipping'] = btn.isChecked()
         btn.clearFocus()
 
         try:
             self.config['plot'].update()
         except AttributeError:
             return
 
 
     def subsampling_changed(self, value):
         self.config['plot'].config['subsampling'] = value
-        
+
         try:
             self.config['plot'].update()
         except AttributeError:
             return
 
 
     def toggle(self):
```

### Comparing `wavebin-2.1/wavebin/plot.py` & `wavebin-2.2/wavebin/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             start = w['header'].x_d_origin
             stop = w['header'].x_d_origin + w['header'].x_d_range
             x = np.linspace(start, stop, len(y))
 
             # Filtering
             if self.config['filter_type'] == 1:
                 self.log(f"  Filtering (Savitzky-Golay)")
-                
+
                 # Calculate window length
                 window = round(len(y) * 0.025)
                 if window % 2 == 0: window += 1
 
                 # Catch filter exceptions
                 try:
                     # Apply filter
@@ -81,15 +81,15 @@
 
                 # Shift waveform to be centered around zero
                 y = (y - med) + 0
 
                 # Apply threshold to waveform values
                 y[y > 0] = 1
                 y[y < 0] = 0
-            
+
 
             # Make processed waveforms available for exporting
             self.processed_waveforms.append({
                 "header": w['header'],
                 "data": y
             })
 
@@ -164,15 +164,15 @@
         .. [1] A. Savitzky, M. J. E. Golay, Smoothing and Differentiation of
         Data by Simplified Least Squares Procedures. Analytical
         Chemistry, 1964, 36 (8), pp 1627-1639.
         .. [2] Numerical Recipes 3rd Edition: The Art of Scientific Computing
         W.H. Press, S.A. Teukolsky, W.T. Vetterling, B.P. Flannery
         Cambridge University Press ISBN-13: 9780521880688
         """
-        
+
         import numpy as np
         from math import factorial
 
         try:
             window_size = np.abs(np.int(window_size))
             order = np.abs(np.int(order))
         except ValueError:
@@ -186,19 +186,19 @@
 
         order_range = range(order+1)
         half_window = (window_size -1) // 2
 
         # Precompute coefficients
         b = np.mat([[k**i for i in order_range] for k in range(-half_window, half_window+1)])
         m = np.linalg.pinv(b).A[deriv] * rate**deriv * factorial(deriv)
-        
+
         # Pad the signal at the extremes with values taken from the signal itself
         firstvals = y[0] - np.abs( y[1:half_window+1][::-1] - y[0] )
         lastvals = y[-1] + np.abs(y[-half_window-1:-1][::-1] - y[-1])
-        
+
         y = np.concatenate((firstvals, y, lastvals))
 
         return np.convolve( m[::-1], y, mode='valid')
 
 
 class Units(Enum):
     """
```

### Comparing `wavebin-2.1/wavebin/wave.py` & `wavebin-2.2/wavebin/wave.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         print(f"Opening \"{self.config['file'].name}\"")
         self.log(f"Full path \"{self.config['file']}\"\n")
         self.file = open(self.config['file'], mode="rb")
 
         # Parse file header
         if not self.parse_file_header(self.file.read(0x0C)):
             return False
-        
+
         # Loop through waveforms
         self.waveforms = []
         for i in range(self.file_header.waveforms):
             self.log(f"Waveform {i + 1}:")
 
             # Parse waveform header
             header = self.parse_waveform_header()
@@ -138,34 +138,34 @@
 
         # Unpack waveform data header
         waveform_data_header_tuple = namedtuple(
             "WaveformDataHeader",
             "size data_type bpp length"
         )
         fields = struct.unpack("i2hi", data)
-        
+
         return waveform_data_header_tuple(*fields)
 
 
     def instances(self, app, plot):
         self.config['app'] = app
         self.config['plot'] = plot
 
 
     def human_format(self, num, binary=False, sep=""):
         if binary:
             div = 1024.0
         else:
             div = 1000.0
-        
+
         num = float('{:.3g}'.format(num))
         mag = 0
         while abs(num) >= div:
             mag += 1
             num /= div
-        
+
         digits = '{:f}'.format(round(num, 2)).rstrip('0').rstrip('.')
         return f"{digits}{sep}{['', 'k', 'M', 'G', 'T'][mag]}"
 
 
     def log(self, msg):
         if self.config['verbose']: print(msg)
```

