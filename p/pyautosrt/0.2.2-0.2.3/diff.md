# Comparing `tmp/pyautosrt-0.2.2.tar.gz` & `tmp/pyautosrt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.2.2.tar", last modified: Wed Jun 14 10:35:22 2023, max compression
+gzip compressed data, was "pyautosrt-0.2.3.tar", last modified: Sun Jun 18 04:14:48 2023, max compression
```

## Comparing `pyautosrt-0.2.2.tar` & `pyautosrt-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 10:35:22.192966 pyautosrt-0.2.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-06-14 10:35:22.193714 pyautosrt-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 10:35:22.136940 pyautosrt-0.2.2/pyautosrt/
--rw-rw-rw-   0        0        0   219161 2023-06-14 10:34:46.000000 pyautosrt-0.2.2/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 10:35:22.169739 pyautosrt-0.2.2/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-06-14 10:35:21.000000 pyautosrt-0.2.2/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-14 10:35:21.000000 pyautosrt-0.2.2/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 10:35:21.000000 pyautosrt-0.2.2/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-14 10:35:21.000000 pyautosrt-0.2.2/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-14 10:35:21.000000 pyautosrt-0.2.2/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 10:35:21.000000 pyautosrt-0.2.2/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-14 10:35:22.197461 pyautosrt-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 10:35:22.190717 pyautosrt-0.2.2/test/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:14:48.279353 pyautosrt-0.2.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-06-18 04:14:48.280100 pyautosrt-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 04:14:48.225869 pyautosrt-0.2.3/pyautosrt/
+-rw-rw-rw-   0        0        0   225245 2023-06-18 04:14:17.000000 pyautosrt-0.2.3/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:14:48.262583 pyautosrt-0.2.3/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-06-18 04:14:47.000000 pyautosrt-0.2.3/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-18 04:14:48.000000 pyautosrt-0.2.3/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 04:14:47.000000 pyautosrt-0.2.3/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-18 04:14:47.000000 pyautosrt-0.2.3/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-18 04:14:47.000000 pyautosrt-0.2.3/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 04:14:47.000000 pyautosrt-0.2.3/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-18 04:14:48.283856 pyautosrt-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:14:48.277854 pyautosrt-0.2.3/test/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.3/test/__init__.py
```

### Comparing `pyautosrt-0.2.2/LICENSE` & `pyautosrt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.2/PKG-INFO` & `pyautosrt-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.2
+Version: 0.2.3
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.2/README.md` & `pyautosrt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.2/pyautosrt/__init__.py` & `pyautosrt-0.2.3/pyautosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import shlex
 
 #import warnings
 #warnings.filterwarnings("ignore", category=DeprecationWarning)
 #warnings.filterwarnings("ignore", category=RuntimeWarning)
 #sys.tracebacklimit = 0
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 
 
 #======================================================== ffmpeg_progress_yield ========================================================#
 
 
 import re
 #import subprocess
@@ -217,15 +217,15 @@
         )
 
         stderr = []
         base_popen_kwargs = self.base_popen_kwargs.copy()
         if popen_kwargs is not None:
             base_popen_kwargs.update(popen_kwargs)
 
-        if sys.platform == "wind32":
+        if sys.platform == "win32":
             self.process = subprocess.Popen(
                 cmd_with_progress,
                 **base_popen_kwargs,
                 creationflags=subprocess.CREATE_NO_WINDOW,
             )  # type: ignore
         else:
             self.process = subprocess.Popen(
@@ -1176,33 +1176,71 @@
                             "ffmpeg",
                             "-y",
                             "-i", media_filepath,
                             "-ac", str(self.channels),
                             "-ar", str(self.rate),
                             "-loglevel", "error",
                             "-hide_banner",
+                            "-progress", "-", "-nostats",
                             temp.name
                          ]
 
         try:
             # RUNNING ffmpeg WITHOUT SHOWING PROGRESSS
             #use_shell = True if os.name == "nt" else False
             #subprocess.check_output(command, stdin=open(os.devnull), shell=use_shell)
 
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
             info = f"Converting '{media_file_display_name}' to a temporary WAV file"
             start_time = time.time()
 
+            '''
             # RUNNING ffmpeg WITH PROGRESSS
             ff = FfmpegProgress(ffmpeg_command)
             percentage = 0
             for progress in ff.run_command_with_progress():
                 percentage = progress
                 if self.progress_callback:
                     self.progress_callback(info, media_file_display_name, percentage, start_time)
+            '''
+
+            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
+            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+
+                    if current_duration>0:
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                        if self.progress_callback:
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
+
             temp.close()
 
             return temp.name, self.rate
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
@@ -1900,28 +1938,65 @@
                                 "-y",
                                 "-i", media_filepath,
                                 "-vf", f"subtitles={shlex.quote(subtitle_path_str)},scale={scale_switch}",
                                 "-c:v", "libx264",
                                 "-crf", "23",
                                 "-preset", "medium",
                                 "-c:a", "copy",
+                                "-progress", "-", "-nostats",
                                 self.output_path
                              ]
 
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
-            info = f"Rendering subtitles file into {media_file_display_name}"
+            info = f"Rendering subtitles file into '{media_file_display_name}'"
             start_time = time.time()
 
-            # RUNNING ffmpeg WITH PROGRESSS
+            '''
+            # RUNNING ffmpeg WITH ffmpeg_progress_yield
             ff = FfmpegProgress(ffmpeg_command)
             percentage = 0
             for progress in ff.run_command_with_progress():
                 percentage = progress
                 if self.progress_callback:
                     self.progress_callback(info, media_file_display_name, percentage, start_time)
+            '''
+
+            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
+            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+
+                    if current_duration>0:
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                        if self.progress_callback:
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
         except KeyboardInterrupt:
@@ -1960,15 +2035,15 @@
     def ffmpeg_check():
         if MediaSubtitleEmbedder.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleEmbedder.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, subtitle_path=None, language="eng", output_path=None, progress_callback=None, error_messages_callback=None):
+    def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def get_existing_subtitle_language(self, media_filepath):
@@ -2048,28 +2123,65 @@
                                     '-i', self.subtitle_path,
                                     '-c:v', 'copy',
                                     '-c:a', 'copy',
                                     '-scodec', 'mov_text',
                                     '-metadata:s:s:' + str(next_index), f'language={shlex.quote(self.language)}',
                                     '-map', '0',
                                     '-map', '1',
+                                    '-progress', '-', '-nostats',
                                     self.output_path
                                  ]
 
                 media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
-                info = f"Embedding subtitles file into {media_file_display_name}"
+                info = f"Embedding subtitles file into '{media_file_display_name}'"
                 start_time = time.time()
 
+                '''
                 # USING ffmpeg_progress_yield MODULE
                 ff = FfmpegProgress(ffmpeg_command)
                 percentage = 0
                 for progress in ff.run_command_with_progress():
                     percentage = progress
                     if self.progress_callback:
                         self.progress_callback(info, media_file_display_name, percentage, start_time)
+                '''
+
+                # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
+                ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+
+                if sys.platform == "win32":
+                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                else:
+                    ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+                total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+
+                if sys.platform == "win32":
+                    process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                else:
+                    process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+                while True:
+                    if process.stdout is None:
+                        continue
+
+                    stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                    if stderr_line == '' and process.poll() is not None:
+                        break
+
+                    if "out_time=" in stderr_line:
+                        time_str = stderr_line.split('time=')[1].split()[0]
+                        current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+
+                        if current_duration>0:
+                            percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                            if self.progress_callback:
+                                self.progress_callback(info, media_file_display_name, percentage, start_time)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
                 if os.path.isfile(self.output_path):
@@ -2145,57 +2257,66 @@
         try:
             ffmpeg_command = [
                                 'ffmpeg',
                                 '-y',
                                 '-i', media_filepath,
                                 '-c', 'copy',
                                 '-sn',
+                                '-progress', '-', '-nostats',
                                 self.output_path
                              ]
 
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
-            info = f"Removing subtitle streams from {media_file_display_name}"
+            info = f"Removing subtitle streams from '{media_file_display_name}'"
             start_time = time.time()
 
+            '''
             # USING ffmpeg_progress_yield MODULE
             ff = FfmpegProgress(ffmpeg_command)
             percentage = 0
             for progress in ff.run_command_with_progress():
                 percentage = progress
                 if self.progress_callback:
                     self.progress_callback(info, media_file_display_name, percentage, start_time)
-
             '''
-            # WITHOUT USING ffmpeg_progress_yield MODULE
+
+
+            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
             ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+
             if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
             total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
 
+
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
-            info = "Removing subtitle streams from file"
-            for line in process.stdout:
-                if "time=" in line:
-                    #print(line)
-                    time_str = line.split("time=")[1].split()[0]
-                    #print("time_str = %s" %time_str)
-                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    #print("current_duration = %s" %current_duration)
                     if current_duration>0:
-                        percentage = int(current_duration*100/total_duration)
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         if self.progress_callback:
                             self.progress_callback(info, media_file_display_name, percentage, start_time)
-            '''
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
             if os.path.isfile(self.output_path):
@@ -2219,21 +2340,14 @@
 
 
 #=======================================================================================================================================#
 
 #----------------------------------------------------------- MISC FUNCTIONS -----------------------------------------------------------#
 
 
-'''
-from autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
-    SubtitleFormatter,  SubtitleWriter, \
-    stop_ffmpeg_windows, stop_ffmpeg_linux, remove_temp_files, is_same_language, is_video_file, is_audio_file
-'''
-
-
 def stop_thread(thread):
     global main_window
     exc = ctypes.py_object(SystemExit)
     res = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(thread.ident), exc)
     if res == 0:
         main_window.write_event_value("-EXCEPTION-", "nonexistent thread id")
         #raise ValueError("nonexistent thread id")
@@ -2421,16 +2535,29 @@
         return False
 
 
 def record_streaming_windows(hls_url, media_filepath, error_messages_callback=None):
     global not_recording, main_window
 
     try:
-        ffmpeg_cmd = ['ffmpeg', '-y', '-i', hls_url,  '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov', '-fflags', 'nobuffer', media_filepath]
-        process = subprocess.Popen(ffmpeg_cmd, stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW)
+        ffmpeg_cmd = [
+                        'ffmpeg',
+                        '-y',
+                        '-i', hls_url,
+                        '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov',
+                        '-fflags', 'nobuffer',
+                        '-loglevel', '-1',
+                        media_filepath
+                     ]
+
+        if sys.platform == "win32":
+            process = subprocess.Popen(ffmpeg_cmd, shell=True, stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            process = subprocess.Popen(ffmpeg_cmd, stderr=subprocess.PIPE)
+
         msg = "RECORDING"
         main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
 
         while not not_recording:
             if not_recording:
                 break
 
@@ -2656,64 +2783,64 @@
 
             ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             window_key = '-PROGRESS-LOG-'
-            msg = f"Checking {media_file_display_name}\n"
+            msg = f"Checking '{media_file_display_name}'\n"
             append_flag = True
             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
             if not_transcribing: return
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
                     if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Is %s has '%s' subtitle stream : Yes\n" %(media_file_display_name, ffmpeg_src_language_code.center(3))
+                    msg = f"Is '{media_file_display_name}' has '{ffmpeg_src_language_code}' subtitle stream : Yes\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in src_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+                    src_subtitle_filepath = f"{base}.{src}.{subtitle_format}"
 
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     writer.write(src_subtitle_filepath)
 
                     if os.path.isfile(src_subtitle_filepath) and src_subtitle_filepath not in results:
                         results.append(src_subtitle_filepath)
 
                     if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"Extracting {media_file_display_name} '{ffmpeg_src_language_code}' subtitle stream as :\n  {src_subtitle_filepath}\n"
+                    msg = f"Extracting '{media_file_display_name}' '{ffmpeg_src_language_code}' subtitle stream as :\n  '{src_subtitle_filepath}'\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if not_transcribing: return
 
                     # no translate process
 
                     # print overall results
                     if os.path.isfile(src_subtitle_filepath):
 
                         window_key = '-RESULTS-'
-                        msg = f"Results for {media_file_display_name} :\n"
+                        msg = f"Results for '{media_file_display_name}' :\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         for result in results:
                             window_key = '-RESULTS-'
                             msg = f"{result}\n"
                             append_flag = True
@@ -2730,21 +2857,21 @@
                                 removed_media_filepaths.append(media_filepath)
 
                         completed_tasks += 1
                         main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
                     if embed_src == True:
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"No need to embed '{ffmpeg_src_language_code}' subtitle into {media_file_display_name} because it's already existed\n"
+                        msg = f"No need to embed '{ffmpeg_src_language_code}' subtitle into '{media_file_display_name}' because it's already existed\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 else:
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Is %s has '%s' subtitle stream : No\n" %(media_file_display_name, ffmpeg_src_language_code.center(3))
+                    msg = f"Is '{media_file_display_name}' has '{ffmpeg_src_language_code}' subtitle stream : No\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if not_transcribing: return
 
             if not_transcribing: return
 
@@ -2761,15 +2888,15 @@
 
             subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
             subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
             if not_transcribing: return
 
             window_key = '-PROGRESS-LOG-'
-            msg = f"Checking {media_file_display_name}\n"
+            msg = f"Checking '{media_file_display_name}'\n"
             append_flag = True
             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
             if subtitle_streams_data and subtitle_streams_data != []:
 
                 if not_transcribing: return
 
@@ -2778,101 +2905,101 @@
 
                 # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
                     if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Is %s has '%s' subtitle stream : Yes\n" %(media_file_display_name, ffmpeg_src_language_code.center(3))
+                    msg = f"Is '{media_file_display_name}' has '{ffmpeg_src_language_code}' subtitle stream : Yes\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in src_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                         if not_transcribing: return
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+                    src_subtitle_filepath = f"{base}.{src}.{subtitle_format}"
 
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     writer.write(src_subtitle_filepath)
 
                     if os.path.isfile(src_subtitle_filepath) and src_subtitle_filepath not in results:
                         results.append(src_subtitle_filepath)
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"Extracting {media_file_display_name} '{ffmpeg_src_language_code}' subtitle stream as :\n  {src_subtitle_filepath}\n"
+                    msg = f"Extracting '{media_file_display_name}' '{ffmpeg_src_language_code}' subtitle stream as :\n  '{src_subtitle_filepath}'\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if not_transcribing: return
 
                     if embed_src == True:
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"No need to embed '{ffmpeg_src_language_code}' subtitle into {media_file_display_name} because it's already existed\n"
+                        msg = f"No need to embed '{ffmpeg_src_language_code}' subtitle into '{media_file_display_name}' because it's already existed\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 # ffmpeg_src_language_code subtitle stream not exist, just print it
                 else:
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Is %s has '%s' subtitle stream : No\n" %(media_file_display_name, ffmpeg_src_language_code.center(3))
+                    msg = f"Is '{media_file_display_name}' has '{ffmpeg_src_language_code}' subtitle stream : No\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if not_transcribing: return
 
                 # ffmpeg_dst_language_code subtitle stream exist, so we print it and extract it
                 if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
 
                     if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Is %s has '%s' subtitle stream : Yes\n" %(media_file_display_name, ffmpeg_dst_language_code.center(3))
+                    msg = f"Is '{media_file_display_name}' has '{ffmpeg_dst_language_code}' subtitle stream : Yes\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     subtitle_stream_regions = []
                     subtitle_stream_transcripts = []
                     for entry in dst_subtitle_stream_timed_subtitles:
                         subtitle_stream_regions.append(entry[0])
                         subtitle_stream_transcripts.append(entry[1])
                         if not_transcribing: return
 
                     base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+                    dst_subtitle_filepath = f"{base}.{dst}.{subtitle_format}"
 
                     writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                     writer.write(dst_subtitle_filepath)
 
                     if os.path.isfile(dst_subtitle_filepath) and dst_subtitle_filepath not in results:
                         results.append(dst_subtitle_filepath)
 
                     if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"Extracting {media_file_display_name} '{ffmpeg_dst_language_code}' subtitle stream as :\n  {dst_subtitle_filepath}\n"
+                    msg = f"Extracting '{media_file_display_name}' '{ffmpeg_dst_language_code}' subtitle stream as :\n  '{dst_subtitle_filepath}'\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if embed_dst == True:
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"No need to embed '{ffmpeg_dst_language_code}' subtitle into {media_file_display_name} because it's already existed\n"
+                        msg = f"No need to embed '{ffmpeg_dst_language_code}' subtitle into '{media_file_display_name}' because it's already existed\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if not_transcribing: return
 
                 # ffmpeg_dst_language_code subtitle stream not exist, just print it
                 else:
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Is %s has '%s' subtitle stream : No\n" %(media_file_display_name, ffmpeg_dst_language_code.center(3))
+                    msg = f"Is '{media_file_display_name}' has '{ffmpeg_dst_language_code}' subtitle stream : No\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if not_transcribing: return
 
                 # ffmpeg_src_language_code subtitle stream = not exist,
                 # ffmpeg_dst_language_code subtitle stream = exist
@@ -2880,19 +3007,19 @@
                 if ffmpeg_src_language_code not in subtitle_stream_parser.languages() and ffmpeg_dst_language_code in subtitle_stream_parser.languages():
 
                     if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
 
                         if not_transcribing: return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f'Translating {media_file_display_name} subtitles from {language.name_of_code[dst]} ({dst}) to {language.name_of_code[src]} ({src})...\n'
+                        msg = f"Translating '{media_file_display_name}' subtitles from {language.name_of_code[dst]} ({dst}) to {language.name_of_code[src]} ({src})...\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[dst], dst, language.name_of_code[src], src)
+                        info = f"Translating '{media_file_display_name}' subtitles from {language.name_of_code[dst]} ({dst}) to {language.name_of_code[src]} ({src})"
                         total = 100
                         start_time = time.time()
 
                         transcript_translator = SentenceTranslator(src=dst, dst=src, error_messages_callback=show_error_messages)
 
                         if not_transcribing: return
 
@@ -2934,20 +3061,20 @@
                                 pool[media_filepath].terminate()
                                 pool[media_filepath].close()
                                 pool[media_filepath].join()
                                 pool[media_filepath] = None
                             return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"Writing {media_file_display_name} translated subtitles file...\n"
+                        msg = f"Writing '{media_file_display_name}' translated subtitles file...\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         base, ext = os.path.splitext(media_filepath)
-                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+                        src_subtitle_filepath = f"{base}.{src}.{subtitle_format}"
 
                         translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         translation_writer.write(src_subtitle_filepath)
 
                         if os.path.isfile(src_subtitle_filepath) and src_subtitle_filepath not in results:
                             results.append(src_subtitle_filepath)
 
@@ -2956,15 +3083,15 @@
                                 pool[media_filepath].terminate()
                                 pool[media_filepath].close()
                                 pool[media_filepath].join()
                                 pool[media_filepath] = None
                             return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"{media_file_display_name} translated subtitles file saved as :\n  {src_subtitle_filepath}\n"
+                        msg = f"'{media_file_display_name}' translated subtitles file saved as :\n  '{src_subtitle_filepath}'\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         # if embed_src is True then we embed that translated srt (from dst to src) above into media_filepath
                         if embed_src == True:
 
                             if not_transcribing:
@@ -2974,19 +3101,19 @@
                                     pool[media_filepath].join()
                                     pool[media_filepath] = None
                                 return
 
                             ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
 
                             base, ext = os.path.splitext(media_filepath)
-                            src_tmp_embedded_media_filepath = "{base}.src.tmp.embedded.{format}".format(base=base, format=ext[1:])
-                            src_embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                            src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                            src_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
 
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_file_display_name}"
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into '{media_file_display_name}'"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                             if not_transcribing:
                                 if pool[media_filepath]:
                                     pool[media_filepath].terminate()
                                     pool[media_filepath].close()
@@ -3015,28 +3142,28 @@
                                 os.remove(src_tmp_output)
 
                                 if src_embedded_media_filepath not in results:
                                     results.append(src_embedded_media_filepath)
 
                             if os.path.isfile(src_embedded_media_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"{media_file_display_name} subtitle embedded {media_type} file saved as :\n  {src_embedded_media_filepath}\n"
+                                msg = f"'{media_file_display_name}' subtitle embedded {media_type} file saved as :\n  '{src_embedded_media_filepath}'\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                             else:
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"Unknown error\n"
+                                msg = "Unknown error\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         # if args.embed_dst is True we can't embed it because dst subtitle stream already exist
                         if embed_dst == True:
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"No need to embed '{ffmpeg_dst_language_code}' subtitle into {media_file_display_name} because it's already existed\n"
+                            msg = f"No need to embed '{ffmpeg_dst_language_code}' subtitle into '{media_file_display_name}' because it's already existed\n"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         if not_transcribing:
                             if pool[media_filepath]:
                                 pool[media_filepath].terminate()
                                 pool[media_filepath].close()
@@ -3055,19 +3182,19 @@
                 elif ffmpeg_src_language_code in subtitle_stream_parser.languages() and ffmpeg_dst_language_code not in subtitle_stream_parser.languages():
 
                     if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
 
                         if not_transcribing: return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f'Translating {media_file_display_name} subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})...\n'
+                        msg = f"Translating '{media_file_display_name}' subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})...\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[src], src, language.name_of_code[dst], dst)
+                        info = f"Translating '{media_file_display_name}' subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})"
                         total = 100
                         start_time = time.time()
 
                         transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
 
                         if not_transcribing: return
 
@@ -3108,40 +3235,40 @@
                                 pool[media_filepath].terminate()
                                 pool[media_filepath].close()
                                 pool[media_filepath].join()
                                 pool[media_filepath] = None
                             return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"Writing {media_file_display_name} translated subtitles file...\n"
+                        msg = f"Writing '{media_file_display_name}' translated subtitles file...\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         base, ext = os.path.splitext(media_filepath)
-                        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+                        dst_subtitle_filepath = f"{base}.{dst}.{subtitle_format}"
 
                         translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         translation_writer.write(dst_subtitle_filepath)
 
                         if os.path.isfile(dst_subtitle_filepath) and dst_subtitle_filepath not in results:
                             results.append(dst_subtitle_filepath)
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"{media_file_display_name} translated subtitles file saved as :\n  {dst_subtitle_filepath}\n"
+                        msg = f"'{media_file_display_name}' translated subtitles file saved as :\n  '{dst_subtitle_filepath}'\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         if force_recognize == False:
                             if media_filepath not in removed_media_filepaths:
                                 removed_media_filepaths.append(media_filepath)
 
                         # if args.embed_src is True we can't embed it because src subtitle stream already exist
                         if embed_src == True:
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"No need to embed '{ffmpeg_src_language_code}' subtitle into {media_file_display_name} because it's already existed\n"
+                            msg = f"No need to embed '{ffmpeg_src_language_code}' subtitle into '{media_file_display_name}' because it's already existed\n"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
 
                         # if embed_dst is True we embed the translated srt (from src to dst) above into media_filepath
                         if embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
 
@@ -3149,34 +3276,35 @@
                                 if pool[media_filepath]:
                                     pool[media_filepath].terminate()
                                     pool[media_filepath].close()
                                     pool[media_filepath].join()
                                     pool[media_filepath] = None
                                 return
 
-                            base, ext = os.path.splitext(media_filepath)
-                            src_tmp_embedded_media_filepath = "{base}.src.tmp.embedded.{format}".format(base=base, format=ext[1:])
                             ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
-                            dst_embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                            base, ext = os.path.splitext(media_filepath)
+                            dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                            dst_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
 
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles file into {media_file_display_name}"
+                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles file into '{media_file_display_name}'"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                             if not_transcribing:
                                 if pool[media_filepath]:
                                     pool[media_filepath].terminate()
                                     pool[media_filepath].close()
                                     pool[media_filepath].join()
                                     pool[media_filepath] = None
                                 return
 
                             try:
-                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                 dst_tmp_output = subtitle_embedder(media_filepath)
                             except Exception as e:
                                 not_transcribing = True
                                 main_window.write_event_value("-EXCEPTION-", e)
                                 return
 
                             if not_transcribing:
@@ -3189,39 +3317,39 @@
 
                             if os.path.isfile(dst_tmp_output):
                                 shutil.copy(dst_tmp_output, dst_embedded_media_filepath)
                                 os.remove(dst_tmp_output)
 
                             if os.path.isfile(dst_embedded_media_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"{media_file_display_name} subtitle embedded {media_type} file saved as :\n  {dst_embedded_media_filepath}\n"
+                                msg = f"'{media_file_display_name}' subtitle embedded {media_type} file saved as :\n  '{dst_embedded_media_filepath}'\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 if dst_embedded_media_filepath not in results:
                                     results.append(dst_embedded_media_filepath)
 
                             else:
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"Unknown error\n"
+                                msg = "Unknown error\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 if not_transcribing:
                     if pool[media_filepath]:
                         pool[media_filepath].terminate()
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
                 # print overall results
                 if (src_subtitle_filepath and os.path.isfile(src_subtitle_filepath)) or (dst_subtitle_filepath and os.path.isfile(dst_subtitle_filepath)):
                     window_key = '-RESULTS-'
-                    msg = f"Results for {media_file_display_name} :\n"
+                    msg = f"Results for '{media_file_display_name}' :\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     for result in results:
                         window_key = '-RESULTS-'
                         msg = f"{result}\n"
                         append_flag = True
@@ -3259,31 +3387,31 @@
         if not_transcribing: return
 
         language = Language()
         wav_filepath = None
         sample_rate = None
 
         base, ext = os.path.splitext(media_filepath)
-        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+        src_subtitle_filepath = f"{base}.{src}.{subtitle_format}"
         if os.path.isfile(src_subtitle_filepath): os.remove(src_subtitle_filepath)
 
         if not is_same_language(src, dst, error_messages_callback=show_error_messages):
             base, ext = os.path.splitext(media_filepath)
-            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+            dst_subtitle_filepath = f"{base}.{dst}.{subtitle_format}"
             if os.path.isfile(dst_subtitle_filepath): os.remove(dst_subtitle_filepath)
 
         regions = None
 
         window_key = '-PROGRESS-LOG-'
-        msg = f"Processing {media_file_display_name} :\n"
+        msg = f"Processing '{media_file_display_name}' :\n"
         append_flag = True
         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
         window_key = '-PROGRESS-LOG-'
-        msg = f"Converting {media_file_display_name} to a temporary WAV file...\n"
+        msg = f"Converting '{media_file_display_name}' to a temporary WAV file...\n"
         append_flag = True
         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
         start_time = time.time()
 
         try:
             wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
@@ -3292,34 +3420,34 @@
             not_transcribing = True
             main_window.write_event_value("-EXCEPTION-", e)
             return
 
         if not_transcribing: return
 
         window_key = '-PROGRESS-LOG-'
-        msg = f"{media_file_display_name} converted WAV file is :\n  {wav_filepath}\n"
+        msg = f"'{media_file_display_name}' converted WAV file is :\n  {wav_filepath}\n"
         append_flag = True
         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
         window_key = '-PROGRESS-LOG-'
-        msg = f"Finding speech regions of {media_file_display_name} WAV file...\n"
+        msg = f"Finding speech regions of '{media_file_display_name}' WAV file...\n"
         append_flag = True
         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
         try:
             region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
             regions = region_finder(wav_filepath)
             num = len(regions)
         except Exception as e:
             not_transcribing = True
             main_window.write_event_value("-EXCEPTION-", e)
             return
 
         window_key = '-PROGRESS-LOG-'
-        msg = f"{media_file_display_name} speech regions found = {len(regions)}\n"
+        msg = f"'{media_file_display_name}' speech regions found = {len(regions)}\n"
         append_flag = True
 
         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
         try:
             converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
             recognizer = SpeechRecognizer(language=src, rate=sample_rate, error_messages_callback=show_error_messages)
@@ -3332,21 +3460,21 @@
         translated_transcriptions = []
 
         if not_transcribing: return
 
         if regions:
             try:
                 window_key = '-PROGRESS-LOG-'
-                msg = f"Converting {media_file_display_name} speech regions to FLAC files...\n"
+                msg = f"Converting '{media_file_display_name}' speech regions to FLAC files...\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
 
-                info = f"Converting {media_file_display_name} speech regions to FLAC files"
+                info = f"Converting '{media_file_display_name}' speech regions to FLAC files"
                 total = 100
 
                 start_time = time.time()
 
                 extracted_regions = []
 
                 for i, extracted_region in enumerate(pool[media_filepath].imap(converter, regions)):
@@ -3385,21 +3513,21 @@
                         pool[media_filepath].terminate()
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
                 window_key = '-PROGRESS-LOG-'
-                msg = f"Creating {media_file_display_name} transcriptions...\n"
+                msg = f"Creating '{media_file_display_name}' transcriptions...\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
 
-                info = f"Creating {media_file_display_name} transcriptions"
+                info = f"Creating '{media_file_display_name}' transcriptions"
                 total = 100
 
                 start_time = time.time()
 
                 for i, transcription in enumerate(pool[media_filepath].imap(recognizer, extracted_regions)):
 
                     if not_transcribing:
@@ -3436,15 +3564,15 @@
                         pool[media_filepath].terminate()
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
                 window_key = '-PROGRESS-LOG-'
-                msg = f"Writing {media_file_display_name} subtitles file...\n"
+                msg = f"Writing '{media_file_display_name}' subtitles file...\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 writer = SubtitleWriter(regions, transcriptions, subtitle_format, error_messages_callback=show_error_messages)
                 writer.write(src_subtitle_filepath)
 
                 if os.path.isfile(src_subtitle_filepath) and src_subtitle_filepath not in results:
@@ -3456,15 +3584,15 @@
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
                 if not is_same_language(src, dst, error_messages_callback=show_error_messages):
                     base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+                    dst_subtitle_filepath = f"{base}.{dst}.{subtitle_format}"
                 
                     if not_transcribing:
                         if pool[media_filepath]:
                             pool[media_filepath].terminate()
                             pool[media_filepath].close()
                             pool[media_filepath].join()
                             pool[media_filepath] = None
@@ -3483,21 +3611,21 @@
                             pool[media_filepath].terminate()
                             pool[media_filepath].close()
                             pool[media_filepath].join()
                             pool[media_filepath] = None
                         return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"Translating {media_file_display_name} subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})...\n"
+                    msg = f"Translating '{media_file_display_name}' subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})...\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
 
-                    info = "Translating %s subtitles from %s (%s) to %s (%s)" %(media_file_display_name, language.name_of_code[src], src, language.name_of_code[dst], dst)
+                    info = f"Translating '{media_file_display_name}' subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})"
                     total = 100
 
                     start_time = time.time()
 
                     transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
                     translated_transcriptions = []
 
@@ -3537,15 +3665,15 @@
                             pool[media_filepath].terminate()
                             pool[media_filepath].close()
                             pool[media_filepath].join()
                             pool[media_filepath] = None
                         return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"Writing {media_file_display_name} translated subtitles file...\n"
+                    msg = f"Writing '{media_file_display_name}' translated subtitles file...\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     translation_writer = SubtitleWriter(created_regions, translated_transcriptions, subtitle_format, error_messages_callback=show_error_messages)
                     translation_writer.write(dst_subtitle_filepath)
 
                     if os.path.isfile(dst_subtitle_filepath) and dst_subtitle_filepath not in results:
@@ -3556,22 +3684,22 @@
                             pool[media_filepath].terminate()
                             pool[media_filepath].close()
                             pool[media_filepath].join()
                             pool[media_filepath] = None
                         return
 
                 window_key = '-PROGRESS-LOG-'
-                msg = f"{media_file_display_name} subtitles file saved as :\n  {src_subtitle_filepath}\n"
+                msg = f"'{media_file_display_name}' subtitles file saved as :\n  '{src_subtitle_filepath}'\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 if is_same_language(src, dst, error_messages_callback=show_error_messages) and embed_src == False:
 
                     window_key = '-RESULTS-'
-                    msg = f"Results for {media_file_display_name} :\n"
+                    msg = f"Results for '{media_file_display_name}' :\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     for result in results:
                         window_key = '-RESULTS-'
                         msg = f"{result}\n"
                         append_flag = True
@@ -3583,22 +3711,22 @@
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     completed_tasks += 1
                     main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
                 if not is_same_language(src, dst, error_messages_callback=show_error_messages):
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"{media_file_display_name} translated subtitles file saved as :\n  {dst_subtitle_filepath}\n"
+                    msg = f"'{media_file_display_name}' translated subtitles file saved as :\n  '{dst_subtitle_filepath}'\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                     if embed_src == False and embed_dst == False:
 
                         window_key = '-RESULTS-'
-                        msg = f"Results for {media_file_display_name} :\n"
+                        msg = f"Results for '{media_file_display_name}' :\n"
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         for result in results:
                             window_key = '-RESULTS-'
                             msg = f"{result}\n"
                             append_flag = True
@@ -3621,20 +3749,20 @@
                     return
 
                 # EMBEDDING subtitles file
                 ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
                 ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
 
                 base, ext = os.path.splitext(media_filepath)
-                src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-                src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
-                src_embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                dst_embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-                src_dst_embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
+                src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                src_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
+                dst_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
+                src_dst_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
 
                 if is_same_language(src, dst, error_messages_callback=show_error_messages):
 
                     if embed_src == True:
                         try:
                             window_key = '-PROGRESS-LOG-'
                             msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}...\n"
@@ -3649,20 +3777,20 @@
                                 os.remove(src_tmp_output)
 
                                 if src_embedded_media_filepath not in results:
                                     results.append(src_embedded_media_filepath)
 
                             if os.path.isfile(src_embedded_media_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"{media_file_display_name} subtitle embedded {media_type} file saved as :\n  {src_embedded_media_filepath}\n"
+                                msg = f"'{media_file_display_name}' subtitle embedded {media_type} file saved as :\n  '{src_embedded_media_filepath}'\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 window_key = '-RESULTS-'
-                                msg = f"Results for {media_file_display_name} :\n"
+                                msg = f"Results for '{media_file_display_name}' :\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 for result in results:
                                     window_key = '-RESULTS-'
                                     msg = f"{result}\n"
                                     append_flag = True
@@ -3674,39 +3802,39 @@
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 completed_tasks += 1
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
                             else:
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"Unknown error\n"
+                                msg = "Unknown error\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
 
                         except Exception as e:
                             not_transcribing = True
                             main_window.write_event_value("-EXCEPTION-", e)
                             return
 
                 elif not is_same_language(src, dst, error_messages_callback=show_error_messages):
 
                     if embed_src == True and embed_dst == True:
                         try:
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_file_display_name}...\n"
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into '{media_file_display_name}'...\n"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                             src_subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             src_tmp_output = src_subtitle_embedder(media_filepath)
 
                             if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_file_display_name}...\n"
+                                msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into '{media_file_display_name}'...\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 src_dst_subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                 src_dst_tmp_output = src_dst_subtitle_embedder(src_tmp_output)
 
                             if os.path.isfile(src_dst_tmp_output):
@@ -3718,21 +3846,21 @@
                                     os.remove(src_tmp_output)
 
                                 if src_dst_embedded_media_filepath not in results:
                                     results.append(src_dst_embedded_media_filepath)
 
                             if os.path.isfile(src_dst_embedded_media_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"{media_file_display_name} subtitle embedded {media_type} file saved as :\n  {src_dst_embedded_media_filepath}\n"
+                                msg = f"'{media_file_display_name}' subtitle embedded {media_type} file saved as :\n  '{src_dst_embedded_media_filepath}'\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
 
                                 window_key = '-RESULTS-'
-                                msg = f"Results for {media_file_display_name} :\n"
+                                msg = f"Results for '{media_file_display_name}' :\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 for result in results:
                                     window_key = '-RESULTS-'
                                     msg = f"{result}\n"
                                     append_flag = True
@@ -3744,29 +3872,29 @@
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 completed_tasks += 1
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
                             else:
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"Unknown error\n"
+                                msg = "Unknown error\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         except Exception as e:
                             not_transcribing = True
                             main_window.write_event_value("-EXCEPTION-", e)
                             return
 
                         if not_transcribing: return
 
                     elif embed_src == True and embed_dst == False:
                         try:
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_file_display_name}...\n"
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into '{media_file_display_name}'...\n"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                             src_subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             src_tmp_output = src_subtitle_embedder(media_filepath)
 
                             if os.path.isfile(src_tmp_output):
@@ -3774,20 +3902,20 @@
                                 os.remove(src_tmp_output)
 
                                 if src_embedded_media_filepath not in results:
                                     results.append(src_embedded_media_filepath)
 
                             if os.path.isfile(src_embedded_media_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"{media_file_display_name} subtitle embedded {media_type} file saved as :\n  {src_embedded_media_filepath}\n"
+                                msg = f"'{media_file_display_name}' subtitle embedded {media_type} file saved as :\n  '{src_embedded_media_filepath}'\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 window_key = '-RESULTS-'
-                                msg = f"Results for {media_file_display_name} :\n"
+                                msg = f"Results for '{media_file_display_name}' :\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 for result in results:
                                     window_key = '-RESULTS-'
                                     msg = f"{result}\n"
                                     append_flag = True
@@ -3799,29 +3927,29 @@
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 completed_tasks += 1
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
                             else:
                                 window_key = '-PROGRESS-LOG-'
-                                msg = "Unknown error"
+                                msg = "Unknown error\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         except Exception as e:
                             not_transcribing = True
                             main_window.write_event_value("-EXCEPTION-", e)
                             return
 
                             if not_transcribing: return
 
                     elif embed_src == False and embed_dst == True:
                         try:
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_file_display_name}...\n"
+                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into '{media_file_display_name}'...\n"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                             dst_subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             dst_tmp_output = dst_subtitle_embedder(media_filepath)
 
                             if os.path.isfile(dst_tmp_output):
@@ -3829,20 +3957,20 @@
                                 os.remove(dst_tmp_output)
 
                                 if dst_embedded_media_filepath not in results:
                                     results.append(dst_embedded_media_filepath)
 
                             if os.path.isfile(dst_embedded_media_filepath):
                                 window_key = '-PROGRESS-LOG-'
-                                msg = f"{media_file_display_name} subtitle embedded {media_type} file saved as :\n  {dst_embedded_media_filepath}\n"
+                                msg = f"'{media_file_display_name}' subtitle embedded {media_type} file saved as :\n  '{dst_embedded_media_filepath}'\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 window_key = '-RESULTS-'
-                                msg = f"Results for {media_file_display_name} :\n"
+                                msg = f"Results for '{media_file_display_name}' :\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 for result in results:
                                     window_key = '-RESULTS-'
                                     msg = f"{result}\n"
                                     append_flag = True
@@ -3854,15 +3982,15 @@
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                                 completed_tasks += 1
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
                             else:
                                 window_key = '-PROGRESS-LOG-'
-                                msg = "Unknown error"
+                                msg = "Unknown error\n"
                                 append_flag = True
                                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                         except Exception as e:
                             not_transcribing = True
                             main_window.write_event_value("-EXCEPTION-", e)
                             return
@@ -3890,37 +4018,39 @@
     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
     window_key = '-RESULTS-'
     msg = ''
     append_flag = False
     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
+    main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', ("...", "Progress info", 0, "0%", 0, "00", "00", "00"))
+
     removed_media_filepaths = []
     proceed_list = []
 
     for media_filepath in media_filepaths:
 
         media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
 
         if force_recognize == True:
             base, ext = os.path.splitext(media_filepath)
-            tmp_subtitle_removed_media_filepath = "{base}.tmp.subtitles.removed.{format}".format(base=base, format=ext[1:])
-            subtitle_removed_media_filepath = "{base}.force.recognize.{format}".format(base=base, format=ext[1:])
+            tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.{ext[1:]}"
+            subtitle_removed_media_filepath = f"{base}.force.recognize.{ext[1:]}"
 
             subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
             tmp_output = subtitle_remover(media_filepath)
 
             if os.path.isfile(tmp_output):
                 shutil.copy(tmp_output, subtitle_removed_media_filepath)
                 os.remove(tmp_output)
 
                 proceed_list.append(subtitle_removed_media_filepath)
 
                 window_key = '-PROGRESS-LOG-'
-                msg = f"Removing all subtitle streams from {media_file_display_name} and save as :\n  {subtitle_removed_media_filepath}\n"
+                msg = f"Removing all subtitle streams from '{media_file_display_name}' and save as :\n  '{subtitle_removed_media_filepath}'\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
         else:
             proceed_list = media_filepaths
 
 
@@ -4092,21 +4222,21 @@
                 else:
                     not_exist_filepaths.append(argpath)
                     media_type = None
 
             if invalid_media_filepaths:
                 msg = ""
                 for invalid_media_filepath in invalid_media_filepaths:
-                    msg = msg + "{} is not valid video or audio files\n".format(invalid_media_filepath)
+                    msg = msg + f"{invalid_media_filepath} is not valid video or audio files\n"
                 sg.Popup(msg, title="Info", line_width=100, any_key_closes=True)
 
         if not_exist_filepaths:
             msg = ""
             for not_exist_filepath in not_exist_filepaths:
-                msg = msg + "{} is not exist\n".format(not_exist_filepath)
+                msg = msg + f"{not_exist_filepath} is not exist\n"
             sg.Popup(msg, title="Info", line_width=100, any_key_closes=True)
 
         elif not filepaths and not not_exist_filepaths:
             msg = "No any files matching filenames you typed"
             sg.Popup(msg, title="Info", line_width=100, any_key_closes=True)
 
 
@@ -4141,43 +4271,14 @@
         if args.format not in SubtitleFormatter.supported_formats:
             msg = "Subtitle format you typed is not supported\nPlease select one from combobox"
             sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
         else:
             subtitle_format = args.format
             sg_combo_subtitle_format_values = subtitle_format
 
-    if str(args.embed_src) == "true":
-        args.embed_src = True
-    if str(args.embed_src) == "false":
-        args.embed_src = False
-
-    if args.embed_src:
-        embed_src = True
-    else:
-        embed_src = False
-
-    if str(args.embed_dst) == "true":
-        args.embed_dst = True
-    if str(args.embed_dst) == "false":
-        args.embed_dst = False
-
-    if args.embed_dst:
-        embed_dst = True
-    else:
-        embed_dst = False
-
-    if str(args.force_recognize) == "true":
-        args.force_recognize = True
-    if str(args.force_recognize) == "false":
-        args.force_recognize = False
-
-    if args.force_recognize:
-        force_recognize = True
-    else:
-        force_recognize = False
 
 #------------------------------------------------------------- MAIN WINDOW -------------------------------------------------------------#
 
 
     not_transcribing = True
     subtitle_format = None
     FONT=('Helvetica', 10)
@@ -4226,16 +4327,16 @@
                                     [sg.FilesBrowse("Add", size=(8,1), target='-INPUT-', file_types=(("All Files", "*.*"),), enable_events=True, key="-ADD-")],
                                     [sg.Button("Remove", key="-REMOVE-", size=(8,1), expand_x=True, expand_y=False,)],
                                     [sg.Button("Clear", key="-CLEAR-", size=(8,1), expand_x=True, expand_y=False,)],
                                 ],
                                 element_justification='c'
                              )
                 ],
-                [sg.Text("Filename", size=(110,1), expand_x=False, expand_y=False, key='-FILE-DISPLAY-NAME-')],
-                [sg.Text("Progress", size=(110,1), expand_x=False, expand_y=False, key='-INFO-')],
+                [sg.Text("File to procees", size=(110,1), expand_x=False, expand_y=False, key='-FILE-DISPLAY-NAME-')],
+                [sg.Text("Progress info", size=(110,1), expand_x=False, expand_y=False, key='-INFO-')],
                 [
                     sg.ProgressBar(100, size=(56,1), orientation='h', expand_x=True, expand_y=True, key='-PROGRESS-'),
                     sg.Text("0%", size=(5,1), expand_x=False, expand_y=False, key='-PERCENTAGE-'),
                     sg.Text(f"ETA  : 00:00:00", size=(14, 1), expand_x=False, expand_y=False, key='-ETA-', justification='r')
                 ],
                 [sg.Text('Progress log', expand_x=False, expand_y=False)],
                 [sg.Multiline(size=(50, 6), expand_x=True, expand_y=True, horizontal_scroll=True, enable_events=True, right_click_menu=['&Edit', ['&Copy','&Paste',]], key='-PROGRESS-LOG-')],
@@ -4472,19 +4573,19 @@
                                 media_type = None
                             input_string = input_string[:-1]
                         else:
                             media_type = None
 
                     if invalid_media_filepaths:
                         if len(invalid_media_filepaths) == 1:
-                            msg = "{} is not a valid video or audio file".format(invalid_media_filepaths[0])
+                            msg = f"{invalid_media_filepaths[0]} is not a valid video or audio file"
                         else:
                             msg = ""
                             for invalid_media_filepath in invalid_media_filepaths:
-                                msg = msg + "{} is not a valid video or audio file\n".format(invalid_media_filepath)
+                                msg = msg + f"{invalid_media_filepath} is not a valid video or audio file\n"
                         sg.Popup(msg, title="Info", line_width=100, any_key_closes=False)
 
                 else:
                     msg = "Invalid filename or file is not exist"
                     sg.Popup(msg, title="Info", line_width=50, any_key_closes=False)
 
                 main_window['-LIST-'].update(sg_listbox_values)
@@ -4602,15 +4703,20 @@
                 percentage = pb[3]
                 progress = pb[4]
                 time_str = None
                 if progress > 0 and progress < total:
                     time_str = "ETA  : " + pb[5] + ":" + pb[6] + ":" + pb[7] 
                 if progress == total:
                     time_str = "Time : " + pb[5] + ":" + pb[6] + ":" + pb[7] 
-                main_window['-FILE-DISPLAY-NAME-'].update("Processing " + media_file_display_name)
+                processing_string = ""
+                if media_file_display_name == "...":
+                    processing_string = "File to process"
+                else:
+                    processing_string = f"Processing '{media_file_display_name}'"
+                main_window['-FILE-DISPLAY-NAME-'].update(processing_string)
                 main_window['-INFO-'].update(info)
                 main_window['-PERCENTAGE-'].update(percentage)
                 main_window['-PROGRESS-'].update(progress)
                 main_window['-ETA-'].update(time_str)
 
 
         elif event == '-EVENT-TRANSCRIBE-TASKS-COMPLETED-':
@@ -4624,15 +4730,16 @@
                 not_transcribing = True
                 main_window['-START-'].update(('Cancel','Start')[not_transcribing], button_color=(('white', ('red', '#283b5b')[not_transcribing])))
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
-                msg = "Total running time : %s:%s:%s" %(hour.zfill(2), minute, second)
+                ##msg = "Total running time : %s:%s:%s" %(hour.zfill(2), minute, second)
+                msg = f"Total running time : {hour.zfill(2)}:{minute}:{second}"
                 main_window['-PROGRESS-LOG-'].update("\n", append=True)
                 main_window['-PROGRESS-LOG-'].update(msg, append=True)
                 scroll_to_last_line(main_window, main_window['-PROGRESS-LOG-'])
 
 
         elif event == '-EXCEPTION-':
 
@@ -4667,65 +4774,71 @@
             else:
                 main_window['-RECORD-STREAMING-STATUS-'].update(text_color='black', background_color='green1')
                 main_window['-STREAMING-DURATION-RECORDED-'].update(text_color='black', background_color='green1')
 
 
         elif event == '-RECORD-STREAMING-':
 
-            if not_recording == True:
-                is_valid_url_streaming = is_streaming_url(str(values['-URL-']).strip(), error_messages_callback=show_error_messages)
-
-            if not is_valid_url_streaming:
+            if str(values['-URL-']).strip() == "":
                 msg = "Invalid URL, please enter a valid URL"
                 sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
-                main_window['-URL-'].update('')
+                not_recording = True
+                main_window['-RECORD-STREAMING-'].update(('Stop Record Streaming','Start Record Streaming')[not_recording], button_color=(('white', ('red', '#283b5b')[not_recording])))
 
             else:
-                not_recording = not not_recording
-                main_window['-RECORD-STREAMING-'].update(('Stop Record Streaming','Start Record Streaming')[not_recording], button_color=(('white', ('red', '#283b5b')[not_recording])))
+                if not_recording == True:
+                    is_valid_url_streaming = is_streaming_url(str(values['-URL-']).strip(), error_messages_callback=show_error_messages)
 
-                if main_window['-URL-'].get() != (None or '') and not_recording == False:
+                if not is_valid_url_streaming:
+                    msg = "Invalid URL, please enter a valid URL"
+                    sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
+                    main_window['-URL-'].update('')
 
-                    if is_valid_url_streaming:
+                else:
+                    not_recording = not not_recording
+                    main_window['-RECORD-STREAMING-'].update(('Stop Record Streaming','Start Record Streaming')[not_recording], button_color=(('white', ('red', '#283b5b')[not_recording])))
 
-                        url = values['-URL-']
+                    if (main_window['-URL-'].get() != None or main_window['-URL-'].get() != '') and not_recording == False:
+                        if is_valid_url_streaming:
 
-                        #NEEDED FOR streamlink MODULE WHEN RUN AS PYINSTALLER COMPILED BINARY
-                        os.environ['STREAMLINK_DIR'] = './streamlink/'
-                        os.environ['STREAMLINK_PLUGINS'] = './streamlink/plugins/'
-                        os.environ['STREAMLINK_PLUGIN_DIR'] = './streamlink/plugins/'
+                            url = values['-URL-']
 
-                        streamlink = Streamlink()
-                        streams = streamlink.streams(url)
-                        stream_url = streams['360p']
+                            #NEEDED FOR streamlink MODULE WHEN RUN AS PYINSTALLER COMPILED BINARY
+                            os.environ['STREAMLINK_DIR'] = './streamlink/'
+                            os.environ['STREAMLINK_PLUGINS'] = './streamlink/plugins/'
+                            os.environ['STREAMLINK_PLUGIN_DIR'] = './streamlink/plugins/'
+
+                            streamlink = Streamlink()
+                            streams = streamlink.streams(url)
+                            stream_url = streams['360p']
+
+                            # WINDOWS AND LINUX HAS DIFFERENT BEHAVIOR WHEN RECORDING FFMPEG AS THREAD
+                            # EVEN thread_record_streaming WAS DECLARED FIRST, IT ALWAYS GET LOADED AT LAST
+                            if sys.platform == "win32":
+                                thread_record_streaming = Thread(target=record_streaming_windows, args=(stream_url.url, tmp_recorded_streaming_filepath, show_error_messages), daemon=True)
+                                thread_record_streaming.start()
+
+                            elif sys.platform == "linux":
+                                thread_record_streaming = Thread(target=record_streaming_linux, args=(stream_url.url, tmp_recorded_streaming_filepath))
+                                thread_record_streaming.start()
 
-                        # WINDOWS AND LINUX HAS DIFFERENT BEHAVIOR WHEN RECORDING FFMPEG AS THREAD
-                        # EVEN thread_record_streaming WAS DECLARED FIRST, IT ALWAYS GET LOADED AT LAST
-                        if sys.platform == "win32":
-                            thread_record_streaming = Thread(target=record_streaming_windows, args=(stream_url.url, tmp_recorded_streaming_filepath), daemon=True)
-                            thread_record_streaming.start()
-
-                        elif sys.platform == "linux":
-                            thread_record_streaming = Thread(target=record_streaming_linux, args=(stream_url.url, tmp_recorded_streaming_filepath))
-                            thread_record_streaming.start()
+                        else:
+                            msg = "Invalid URL, please enter a valid URL"
+                            sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
+                            not_recording = True
+                            main_window['-RECORD-STREAMING-'].update(('Stop Record Streaming','Start Record Streaming')[not_recording], button_color=(('white', ('red', '#283b5b')[not_recording])))
 
                     else:
-                        msg = "Invalid URL, please enter a valid URL"
-                        sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
-                        not_recording = True
-                        main_window['-RECORD-STREAMING-'].update(('Stop Record Streaming','Start Record Streaming')[not_recording], button_color=(('white', ('red', '#283b5b')[not_recording])))
+                        if sys.platform == "win32":
+                            #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
+                            stop_record_streaming_windows()
 
-                else:
-                    if sys.platform == "win32":
-                        #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
-                        stop_record_streaming_windows()
-
-                    elif sys.platform == "linux":
-                        #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
-                        stop_record_streaming_linux()
+                        elif sys.platform == "linux":
+                            #print("thread_record_streaming.is_alive() = {}".format(thread_record_streaming.is_alive()))
+                            stop_record_streaming_linux()
 
 
         elif event == '-SAVE-RECORDED-STREAMING-':
 
             tmp_recorded_streaming_filename = "record.mp4"
             tmp_recorded_streaming_filepath = os.path.join(tempfile.gettempdir(), tmp_recorded_streaming_filename)
```

### Comparing `pyautosrt-0.2.2/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.2.3/pyautosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.2
+Version: 0.2.3
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.2/setup.py` & `pyautosrt-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.2/test/__init__.py` & `pyautosrt-0.2.3/test/__init__.py`

 * *Files identical despite different names*

