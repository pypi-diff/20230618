# Comparing `tmp/drummachine-0.1.3.tar.gz` & `tmp/drummachine-0.4.5.tar.gz`

## Comparing `drummachine-0.1.3.tar` & `drummachine-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 drummachine-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 drummachine-0.1.3/demos/audio.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 drummachine-0.1.3/demos/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drummachine-0.1.3/src/drummachine/__init__.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 drummachine-0.1.3/src/drummachine/__main__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 drummachine-0.1.3/src/drummachine/waveforms.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 drummachine-0.1.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 drummachine-0.1.3/LICENSE
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 drummachine-0.1.3/README.md
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 drummachine-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 drummachine-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 drummachine-0.4.5/MANIFEST.in
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 drummachine-0.4.5/demos/audio.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 drummachine-0.4.5/demos/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drummachine-0.4.5/src/drummachine/__init__.py
+-rw-r--r--   0        0        0     9822 2020-02-02 00:00:00.000000 drummachine-0.4.5/src/drummachine/__main__.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 drummachine-0.4.5/src/drummachine/samples.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 drummachine-0.4.5/src/drummachine/waveforms.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 drummachine-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 drummachine-0.4.5/LICENSE
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 drummachine-0.4.5/README.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 drummachine-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 drummachine-0.4.5/PKG-INFO
```

### Comparing `drummachine-0.1.3/demos/audio.py` & `drummachine-0.4.5/demos/audio.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.1.3/demos/ui.py` & `drummachine-0.4.5/demos/ui.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.1.3/src/drummachine/__main__.py` & `drummachine-0.4.5/src/drummachine/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import sys, curses, threading
 import numpy as np
 import sounddevice as sd
-from . import waveforms as wfs
-import time
+from time import time, perf_counter_ns
+try:
+    from . import waveforms as wfs
+    from . import samples
+except ImportError: # running as script in development
+    import waveforms as wfs
+    import samples
 
 def get_grid(icon):
     hgap = ' ' * np.ones((icon.shape[0], 1), dtype=object)
     idx = 1 # using 0 for gaps
     grid_out, grid_map = [], []
     for layout_row in layout:
         out_row, map_row = [], []
@@ -74,15 +79,15 @@
     if i >= max_i:
         i = max_i
     if j >= max_j:
         j = max_j
     return i, j
 
 def blink_cursor(ui_grid, ui_map, i, j, icon, period_s = 0.25):
-    if time.time() % period_s < period_s / 2:
+    if time() % period_s < period_s / 2:
         ui_grid[ui_map[i, j] == ui_map] = np.array(icon.shape[0]*icon.shape[1]*[' '])
     return ui_grid
 
 def get_active_grid(icon, on_indices):
     ui_grid, ui_map = get_grid(icon)
     for m in range(ui_grid.shape[0]):
         for n in range(ui_grid.shape[1]):
@@ -142,20 +147,26 @@
     idx_i, row_idx = 1, 0
     indices = set()
     for row in sound_on:
         indices.update(np.where(row == 1)[0] + idx_i + row_idx)
         row_idx += len(row)
     return indices
 
+count, elapsed_total, elapsed = 1, 0, 0
 def display_help(stdscr, y0):
-    stdscr.addstr(y0 + 1, 0, 'MOVE CURSOR: ← / ↑ / → / ↓')
-    stdscr.addstr(y0 + 2, 0, '(DE)ACTIVATE SOUND: <spacebar>')
-    stdscr.addstr(y0 + 3, 0, 'CHANGE TEMPO: + / -')
-    stdscr.addstr(y0 + 4, 0, 'RANDOM BEAT: R')
-    stdscr.addstr(y0 + 5, 0, 'EXIT: CTRL + C')
+    global count, elapsed_total
+    elapsed_total += elapsed
+    stdscr.addstr(y0 + 1, 0, '(DE)ACTIVATE SOUND:   <spacebar>')
+    stdscr.addstr(y0 + 2, 0, 'CHANGE TEMPO:         + / -')
+    stdscr.addstr(y0 + 3, 0, 'RANDOM BEAT:          R')
+    stdscr.addstr(y0 + 4, 0, 'MOVE CURSOR:          ← / ↑ / → / ↓')
+    stdscr.addstr(y0 + 5, 0, 'EXIT:                 CTRL + C')
+    stdscr.addstr(y0 + 7, 0, f'AUDIO PLAYER STATUS:  {current_status}')
+    stdscr.addstr(y0 + 8, 0, f'MEAN CALLBACK TIME:   {int(elapsed_total/count)} [ns]')
+    count += 1
 
 def build_ui(stdscr):
     i, j = 0, 0
     icon = get_icon()
     threading.Thread(target=play_audio).start()
 
     while True:
@@ -198,63 +209,84 @@
 def init_colors(stdscr=None):
     curses.use_default_colors()
     for i in range(0, curses.COLORS):
         try:
             curses.init_pair(i + 1, i, -1)
         except ValueError:
             break
+        except Exception as ex: # windows-curses
+            if sys.platform != 'win32':
+                raise ex
     if stdscr:
         stdscr.nodelay(False)
         for i in range(0, 255):
             stdscr.addstr(f'{i} ', curses.color_pair(i))
         stdscr.getch()
         stdscr.nodelay(True)
         stdscr.erase()
 
-idx = 0
+idx, current_status, status_time = 0, '', None
 def callback(outdata, frames, time, status):
-    global idx
+    global idx, current_status, status_time, elapsed
+    st = perf_counter_ns()
+    if status:
+        current_status = status
+        status_time = time.currentTime
+    if status_time and status_display_time_s < time.currentTime - status_time:
+        current_status = ' '*16 # clear
     try:
         output_signal = get_superposition().sum(axis=0).reshape(-1, 1)
         outdata[:] = gain * output_signal[idx:idx+frames]
         idx += frames
         if idx > len(output_signal)-frames:
             idx = 0
     except ValueError: # extreme tempo changes
         outdata[:] = np.zeros((frames,1))
+    elapsed = perf_counter_ns() - st
 
-n_instruments, n_beats = 4, 4
-instr_color_idx = [14, 4, 11, 7]
+n_instruments, n_beats = 5, 4
+instr_color_idx = [14, 4, 11, 7, 5]
 single_instrument_layout = n_beats * [1, 1, 1, 1, 0, 0, 0, 0]
 layout = np.vstack([single_instrument_layout for _ in range(n_instruments)])
 sound_on = np.zeros((n_instruments, single_instrument_layout.count(1)), dtype=int)
+status_display_time_s = 3
 
 gain = 0.01
 n_channels = 2
 samplerate = get_samplerate()
 stream = sd.OutputStream(channels=n_channels, callback=callback, samplerate=samplerate)
 
 n_subdiv_samples = int(samplerate // 8) # 120 BPM, 16th note subdiv
-waveforms = [
-    wfs.get_kick(),
-    wfs.get_snare(Fs=samplerate),
-    wfs.get_hihat(),
-    wfs.get_click(Fs=samplerate),
-    wfs.get_modulated_sine(Fs=samplerate)
-]
 
+try:
+    if len(sys.argv) > 1:
+        waveforms = samples.get_waveforms()
+        gain = 0.1
+    else:
+        raise Exception('provide a command-line argument to download drum samples')
+except Exception as ex:
+    print(ex)
+    print('generating waveforms...')
+    waveforms = [
+        wfs.get_kick(),
+        wfs.get_snare(Fs=samplerate),
+        wfs.get_hihat(),
+        wfs.get_click(Fs=samplerate),
+        wfs.get_modulated_sine(Fs=samplerate)
+    ]
+
+#sys.exit(0)
 def main(stdscr):
     stdscr.nodelay(True)
     stdscr.keypad(True)
     if curses.has_colors():
         init_colors() # stdscr) # 
     try:
         build_ui(stdscr)
     except KeyboardInterrupt:
         stream.stop()
         curses.nocbreak()
         curses.echo()
         curses.endwin()
 
-#sys.exit(0)
 if __name__ == "__main__":
     curses.wrapper(main)
```

### Comparing `drummachine-0.1.3/src/drummachine/waveforms.py` & `drummachine-0.4.5/src/drummachine/waveforms.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.1.3/LICENSE` & `drummachine-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drummachine-0.1.3/pyproject.toml` & `drummachine-0.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "drummachine"
-version = "0.1.3"
+version = "0.4.5"
 authors = [
   { name="Guitar Dan", email="guitardanuk@gmail.com" },
 ]
 description = "A drum machine package for sequencing waveforms using numpy, curses and the sounddevice module."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,12 +18,14 @@
     "Environment :: Console :: Curses",
     "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis"
 ]
 keywords = ["music", "audio", "drums"]
 dependencies = [
     "numpy",
     "sounddevice",
+    "soundfile",
+    "windows-curses ; platform_system == 'Windows'"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/guitardan/realtime-audio"
 "Bug Tracker" = "https://github.com/guitardan/realtime-audio/issues"
```

