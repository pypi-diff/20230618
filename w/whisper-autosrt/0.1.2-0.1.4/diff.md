# Comparing `tmp/whisper_autosrt-0.1.2.tar.gz` & `tmp/whisper_autosrt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.2.tar", last modified: Fri Jun  9 01:38:23 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.4.tar", last modified: Sat Jun 17 22:22:22 2023, max compression
```

## Comparing `whisper_autosrt-0.1.2.tar` & `whisper_autosrt-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.281040 whisper_autosrt-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1956 2023-06-09 01:38:23.281789 whisper_autosrt-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.2/README.md
--rw-rw-rw-   0        0        0      147 2023-06-09 01:38:23.284787 whisper_autosrt-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.251074 whisper_autosrt-0.1.2/whisper_autosrt/
--rw-rw-rw-   0        0        0   136062 2023-06-09 01:37:23.000000 whisper_autosrt-0.1.2/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 01:38:23.279541 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 01:38:23.000000 whisper_autosrt-0.1.2/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:22.940557 whisper_autosrt-0.1.4/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1956 2023-06-17 22:22:22.940557 whisper_autosrt-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.4/README.md
+-rw-rw-rw-   0        0        0      147 2023-06-17 22:22:22.943556 whisper_autosrt-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:22.902349 whisper_autosrt-0.1.4/whisper_autosrt/
+-rw-rw-rw-   0        0        0   151532 2023-06-17 22:21:48.000000 whisper_autosrt-0.1.4/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:22:22.938309 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-06-17 22:22:22.000000 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-17 22:22:22.000000 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 22:22:22.000000 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-17 22:22:22.000000 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-06-17 22:22:22.000000 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-17 22:22:22.000000 whisper_autosrt-0.1.4/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.2/LICENSE` & `whisper_autosrt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.2/PKG-INFO` & `whisper_autosrt-0.1.4/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whisper_autosrt
-Version: 0.1.2
+Name: whisper-autosrt
+Version: 0.1.4
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.2/README.md` & `whisper_autosrt-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.2/setup.py` & `whisper_autosrt-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.2/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.4/whisper_autosrt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,17 @@
 from pathlib import Path
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
-
-VERSION = "0.1.2"
+VERSION = "0.1.4"
 #marker='█'
 
-
 class WhisperLanguage:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("auto")
         self.list_codes.append("af")
         self.list_codes.append("sq")
         self.list_codes.append("am")
@@ -624,14 +622,17 @@
         self.list_names.append("Vietnamese")
         self.list_names.append("Welsh")
         self.list_names.append("Xhosa")
         self.list_names.append("Yiddish")
         self.list_names.append("Yoruba")
         self.list_names.append("Zulu")
 
+        # NOTE THAT Google Translate AND Whisper Speech Recognition API USE ISO-639-1 STANDARD CODE ('al', 'af', 'as', ETC)
+        # WHEN ffmpeg SUBTITLES STREAMS USE ISO 639-2 STANDARD CODE ('afr', 'alb', 'amh', ETC)
+
         self.list_ffmpeg_codes = []
         self.list_ffmpeg_codes.append("afr")  # Afrikaans
         self.list_ffmpeg_codes.append("alb")  # Albanian
         self.list_ffmpeg_codes.append("amh")  # Amharic
         self.list_ffmpeg_codes.append("ara")  # Arabic
         self.list_ffmpeg_codes.append("hye")  # Armenian
         self.list_ffmpeg_codes.append("asm")  # Assamese
@@ -1038,25 +1039,14 @@
                                 'cy': 'wel', # Welsh
                                 'xh': 'xho', # Xhosa
                                 'yi': 'yid', # Yiddish
                                 'yo': 'yor', # Yoruba
                                 'zu': 'zul', # Zulu
                            }
 
-    '''
-    def get_name(self, get_code):
-        return self.dict.get(get_code.lower(), "")
-
-    def get_code(self, language):
-        for get_code, lang in self.dict.items():
-            if lang.lower() == language.lower():
-                return get_code
-        return ""
-    '''
-
     def get_name(self, code):
         return self.name_of_code[code]
 
     def get_code(self, language):
         return self.code_of_name[language]
 
     def get_ffmpeg_code(self, code):
@@ -1120,58 +1110,72 @@
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
 
+
         try:
+            info = f"Converting to a temporary WAV file"
+
             # RUNNING ffmpeg WITHOUT SHOWING PROGRESSS
             #use_shell = True if os.name == "nt" else False
             #subprocess.check_output(command, stdin=open(os.devnull), shell=use_shell)
 
+
+            # RUNNING ffmpeg WITH SHOWING PROGRESSS
             '''
             # RUNNING ffmpeg WITH ffmpeg_progress_yield
             ff = FfmpegProgress(command)
             percentage = 0
             for progress in ff.run_command_with_progress():
                 percentage = progress
                 if self.progress_callback:
-                    self.progress_callback(media_filepath, percentage)
+                    self.progress_callback(info, media_filepath, percentage)
             temp.close()
             '''
 
-            # RUNNING ffmpeg WITH SIMPPLE PROGRESSS
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
-                            self.progress_callback(media_filepath, percentage)
+                            self.progress_callback(info, media_filepath, percentage)
 
             temp.close()
 
             return temp.name, self.rate
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
@@ -1391,69 +1395,14 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
-class SRTFileReader:
-    def __init__(self, srt_file_path, error_messages_callback=None):
-        self.timed_subtitles = self(srt_file_path)
-        self.error_messages_callback = error_messages_callback
-
-    @staticmethod
-    def __call__(srt_file_path):
-        try:
-            """
-            Read SRT formatted subtitle file and return subtitles as list of tuples
-            """
-            timed_subtitles = []
-            with open(srt_file_path, 'r') as srt_file:
-                lines = srt_file.readlines()
-                # Split the subtitle file into subtitle blocks
-                subtitle_blocks = []
-                block = []
-                for line in lines:
-                    if line.strip() == '':
-                        subtitle_blocks.append(block)
-                        block = []
-                    else:
-                        block.append(line.strip())
-                subtitle_blocks.append(block)
-
-                # Parse each subtitle block and store as tuple in timed_subtitles list
-                for block in subtitle_blocks:
-                    if block:
-                        # Extract start and end times from subtitle block
-                        start_time_str, end_time_str = block[1].split(' --> ')
-                        time_format = '%H:%M:%S,%f'
-                        start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
-                        start_time_total_seconds = start_time_time_delta.total_seconds()
-                        end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
-                        end_time_total_seconds = end_time_time_delta.total_seconds()
-                        # Extract subtitle text from subtitle block
-                        subtitle = ' '.join(block[2:])
-                        timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitle))
-                return timed_subtitles
-
-        except KeyboardInterrupt:
-            if self.error_messages_callback:
-                self.error_messages_callback("Cancelling all tasks")
-            else:
-                print("Cancelling all tasks")
-            return
-
-        except Exception as e:
-            if self.error_messages_callback:
-                self.error_messages_callback(e)
-            else:
-                print(e)
-            return
-
-
 class SubtitleStreamParser:
     def __init__(self, error_messages_callback=None):
         self.error_messages_callback = error_messages_callback
         self._indexes = []
         self._languages = []
         self._timed_subtitles = []
         self._number_of_streams = 0
@@ -1546,38 +1495,38 @@
 			#print(output)
 
             timed_subtitles = []
             subtitle_data = []
             lines = output.strip().split('\n')
             #print(lines)
             subtitles = []
-            subtitle = None
+            subtitles = None
             subtitle_blocks = []
             block = []
             for line in lines:
                 if line.strip() == '':
                     subtitle_blocks.append(block)
                     block = []
                 else:
                     block.append(line.strip())
             subtitle_blocks.append(block)
 
-            # Parse each subtitle block and store as tuple in timed_subtitles list
+            # Parse each subtitles block and store as tuple in timed_subtitles list
             for block in subtitle_blocks:
                 if block:
-                    # Extract start and end times from subtitle block
+                    # Extract start and end times from subtitles block
                     start_time_str, end_time_str = block[1].split(' --> ')
                     time_format = '%H:%M:%S,%f'
                     start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                     start_time_total_seconds = start_time_time_delta.total_seconds()
                     end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                     end_time_total_seconds = end_time_time_delta.total_seconds()
-                    # Extract subtitle text from subtitle block
-                    subtitle = ' '.join(block[2:])
-                    timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitle))
+                    # Extract subtitles text from subtitles block
+                    subtitles = ' '.join(block[2:])
+                    timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
             return timed_subtitles
 
         except FileNotFoundError:
             if self.error_messages_callback:
                 msg = 'ffmpeg not found. Make sure it is installed and added to the system PATH.'
                 self.error_messages_callback(msg)
             else:
@@ -1642,17 +1591,16 @@
     def ffmpeg_check():
         if MediaSubtitleRenderer.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleRenderer.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
+    def __init__(self, subtitle_path=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
-        self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def __call__(self, media_filepath):
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
@@ -1661,74 +1609,85 @@
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
-                print(f"The given file does not exist: '{media_filepath}'")
-                raise Exception(f"Invalid file: '{media_filepath}'")
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
         if not self.ffmpeg_check():
             if self.error_messages_callback:
-                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+                self.error_messages_callback("Cannot find ffmpeg executable on this machine")
             else:
-                print("ffmpeg: Executable not found on machine.")
+                print("Cannot find ffmpeg executable on this machine")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
-            '''
-            ffmpeg_command = [
-                                "ffmpeg",
-                                "-y",
-                                "-i", media_filepath,
-                                "-vf", f"subtitles={shlex.quote(self.subtitle_path)}",
-                                "-y", self.output_path
-                             ]
-            '''
-
             scale_switch = "'trunc(iw/2)*2':'trunc(ih/2)*2'"
             ffmpeg_command = [
                                 "ffmpeg",
                                 "-y",
                                 "-i", media_filepath,
                                 "-vf", f"subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}",
                                 "-c:v", "libx264",
                                 "-crf", "23",
                                 "-preset", "medium",
                                 "-c:a", "copy",
+                                "-progress", "-", "-nostats",
                                 self.output_path
                              ]
 
+            info = f"Rendering subtitles file into {media_type} file : "
+
+            '''
+            # RUNNING ffmpeg_command USING ffmpeg_progress_yield MODULE
+            ff = FfmpegProgress(ffmpeg_command)
+            percentage = 0
+            for progress in ff.run_command_with_progress():
+                percentage = progress
+                if self.progress_callback:
+                    self.progress_callback(info, media_filepath, percentage)
+            '''
+
+            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield MODULE
             ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
 
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
-                            self.progress_callback(media_filepath, percentage)
+                            self.progress_callback(info, media_filepath, percentage)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
         except KeyboardInterrupt:
@@ -1796,18 +1755,18 @@
             output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
         else:
             output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
         metadata = json.loads(output.stdout)
         streams = metadata['streams']
 
-        # Find the subtitle stream with language metadata
+        # Find the subtitles stream with language metadata
         subtitle_languages = []
         for stream in streams:
-            if stream['codec_type'] == 'subtitle' and 'tags' in stream and 'language' in stream['tags']:
+            if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
                 language = stream['tags']['language']
                 subtitle_languages.append(language)
 
         return subtitle_languages
 
     def __call__(self, media_filepath):
         if "\\" in media_filepath:
@@ -1817,91 +1776,101 @@
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
-                print(f"The given file does not exist: '{media_filepath}'")
-                raise Exception(f"Invalid file: '{media_filepath}'")
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
         if not self.ffmpeg_check():
             if self.error_messages_callback:
-                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+                self.error_messages_callback("Cannot find ffmpeg executable on this machine")
             else:
-                print("ffmpeg: Executable not found on machine.")
+                print("Cannot find ffmpeg executable on this machine")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             existing_languages = self.get_existing_subtitle_language(media_filepath)
             if self.language in existing_languages:
                 # THIS 'print' THINGS WILL MAKE progresbar screwed up!
-                #msg = (f"'{self.language}' subtitle stream already existed in {media_filepath}")
+                #msg = (f"'{self.language}' subtitles stream already existed in {media_filepath}")
                 #if self.error_messages_callback:
                 #    self.error_messages_callback(msg)
                 #else:
                 #    print(msg)
                 return
 
             else:
-                # Determine the next available subtitle index
+                # Determine the next available subtitles index
                 next_index = len(existing_languages)
 
                 ffmpeg_command = [
                                     'ffmpeg',
                                     '-y',
                                     '-i', media_filepath,
                                     '-sub_charenc', 'UTF-8',
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
 
+                info = f"Embedding subtitles file into {media_filepath}"
 
                 '''
                 # USING ffmpeg_progress_yield MODULE
                 ff = FfmpegProgress(ffmpeg_command)
                 percentage = 0
                 for progress in ff.run_command_with_progress():
                     percentage = progress
                     if self.progress_callback:
-                        self.progress_callback(media_filepath, percentage)
+                        self.progress_callback(info, media_filepath, percentage)
                 '''
 
-                # WITHOUT USING ffmpeg_progress_yield MODULE
+                # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield MODULE
                 ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+
                 if sys.platform == "win32":
-                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
                     ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
                 total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
 
+
                 if sys.platform == "win32":
-                    process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                    process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
-                    process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
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
 
-                for line in process.stdout:
-                    if "time=" in line:
-                        #print(line)
-                        time_str = line.split("time=")[1].split()[0]
-                        #print("time_str = %s" %time_str)
-                        current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                        #print("current_duration = %s" %current_duration)
                         if current_duration>0:
-                            percentage = int(current_duration*100/total_duration)
+                            percentage = int(current_duration*100/(int(float(total_duration))*1000))
                             if self.progress_callback:
-                                self.progress_callback(media_filepath, percentage)
+                                self.progress_callback(info, media_filepath, percentage)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
                 if os.path.isfile(self.output_path):
@@ -1920,14 +1889,200 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
+class MediaSubtitleRemover:
+    @staticmethod
+    def which(program):
+        def is_exe(media_filepath):
+            return os.path.isfile(media_filepath) and os.access(media_filepath, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    @staticmethod
+    def ffmpeg_check():
+        if MediaSubtitleRemover.which("ffmpeg"):
+            return "ffmpeg"
+        if MediaSubtitleRemover.which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
+    def __init__(self, output_path=None, progress_callback=None, error_messages_callback=None):
+        self.output_path = output_path
+        self.progress_callback = progress_callback
+        self.error_messages_callback = error_messages_callback
+
+    def __call__(self, media_filepath):
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if "\\" in self.output_path:
+            self.output_path = self.output_path.replace("\\", "/")
+
+        if not os.path.isfile(media_filepath):
+            if self.error_messages_callback:
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+            else:
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+        if not self.ffmpeg_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffmpeg executable on this machine")
+            else:
+                print("Cannot find ffmpeg executable on this machine")
+                raise Exception("Dependency not found: ffmpeg")
+
+        try:
+            ffmpeg_command = [
+                                'ffmpeg',
+                                '-y',
+                                '-i', media_filepath,
+                                '-c', 'copy',
+                                '-sn',
+                                "-progress", "-", "-nostats",
+                                self.output_path
+                             ]
+
+            info = "Removing subtitles streams from file"
+
+            '''
+            # USING ffmpeg_progress_yield MODULE
+            ff = FfmpegProgress(ffmpeg_command)
+            percentage = 0
+            for progress in ff.run_command_with_progress():
+                percentage = progress
+                if self.progress_callback:
+                    self.progress_callback(info, media_filepath, percentage)
+            '''
+
+            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield MODULE
+            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
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
+                            self.progress_callback(info, media_filepath, percentage)
+
+            if os.path.isfile(self.output_path):
+                return self.output_path
+            else:
+                return None
+
+            if os.path.isfile(self.output_path):
+                return self.output_path
+            else:
+                return None
+
+        except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
+            return
+
+        except Exception as e:
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
+            return
+
+
+class SRTFileReader:
+    def __init__(self, srt_file_path, error_messages_callback=None):
+        self.timed_subtitles = self(srt_file_path)
+        self.error_messages_callback = error_messages_callback
+
+    @staticmethod
+    def __call__(srt_file_path):
+        try:
+            """
+            Read SRT formatted subtitles file and return subtitles as list of tuples
+            """
+            timed_subtitles = []
+            with open(srt_file_path, 'r') as srt_file:
+                lines = srt_file.readlines()
+                # Split the subtitles file into subtitles blocks
+                subtitle_blocks = []
+                block = []
+                for line in lines:
+                    if line.strip() == '':
+                        subtitle_blocks.append(block)
+                        block = []
+                    else:
+                        block.append(line.strip())
+                subtitle_blocks.append(block)
+
+                # Parse each subtitles block and store as tuple in timed_subtitles list
+                for block in subtitle_blocks:
+                    if block:
+                        # Extract start and end times from subtitles block
+                        start_time_str, end_time_str = block[1].split(' --> ')
+                        time_format = '%H:%M:%S,%f'
+                        start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
+                        start_time_total_seconds = start_time_time_delta.total_seconds()
+                        end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
+                        end_time_total_seconds = end_time_time_delta.total_seconds()
+                        # Extract subtitles text from subtitles block
+                        subtitles = ' '.join(block[2:])
+                        timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
+                return timed_subtitles
+
+        except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
+            return
+
+        except Exception as e:
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
+            return
+
+
 def change_code_page(code_page):
     kernel32 = ctypes.windll.kernel32
     kernel32.SetConsoleOutputCP(code_page)
     kernel32.SetConsoleCP(code_page)
 
 
 def stop_ffmpeg_windows(error_messages_callback=None):
@@ -2075,18 +2230,18 @@
                 media_path
     ]
 
     output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
     metadata = json.loads(output.stdout)
     streams = metadata['streams']
 
-    # Find the subtitle stream with language metadata
+    # Find the subtitles stream with language metadata
     subtitle_languages = []
     for stream in streams:
-        if stream['codec_type'] == 'subtitle' and 'tags' in stream and 'language' in stream['tags']:
+        if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
             language = stream['tags']['language']
             subtitle_languages.append(language)
 
     return subtitle_languages
 
 
 def render_subtitle_to_media(media_filepath, media_type, media_ext, subtitle_path, output_path, error_messages_callback=None):
@@ -2139,20 +2294,20 @@
         else:
             process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
 
         for line in process.stdout:
             if "time=" in line:
                 #print(line)
                 time_str = line.split("time=")[1].split()[0]
-                #print("time_str = %s" %time_str)
+                #print(f"time_str = {time_str})
                 current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                #print("current_duration = %s" %current_duration)
+                #print(f"current_duration = {current_duration}")
                 if current_duration>0:
                     percentage = int(current_duration*100/total_duration)
-                    #print("percentage = {}%".format(percentage))
+                    #print(f"percentage = {percentage}%")
                     pbar.update(percentage)
         pbar.finish()
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
@@ -2170,19 +2325,19 @@
             subtitle_path = subtitle_path.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
         existing_languages = get_existing_subtitle_language(media_filepath)
         if language_code in existing_languages:
-            #print(f"'{language_code}' subtitle stream already existed in {media_filepath}")
+            #print(f"'{language_code}' subtitles stream already existed in {media_filepath}")
             return
 
         else:
-            # Determine the next available subtitle index
+            # Determine the next available subtitles index
             next_index = len(existing_languages)
 
             ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
             if sys.platform == "win32":
                 ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
             else:
                 ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
@@ -2213,34 +2368,34 @@
             else:
                 process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
 
             for line in process.stdout:
                 if "time=" in line:
                     #print(line)
                     time_str = line.split("time=")[1].split()[0]
-                    #print("time_str = %s" %time_str)
+                    #print(f"time_str = {time_str}")
                     current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    #print("current_duration = %s" %current_duration)
+                    #print(f"current_duration = {current_duration}")
                     if current_duration>0:
                         percentage = int(current_duration*100/total_duration)
-                        #print("percentage = {}%".format(percentage))
+                        #print(f"percentage = {percentage}%")
                         pbar.update(percentage)
             pbar.finish()
             return output_path
         return
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
         return None
 
 
-def show_progress(media_filepath, progress):
+def show_progress(info, media_filepath, progress):
     global pbar
     pbar.update(progress)
 
 
 def show_error_messages(messages):
     print(messages)
 
@@ -2284,18 +2439,19 @@
     parser.add_argument('-lct', '--list-compute-types', help="List of supported compute types", action='store_true')
     parser.add_argument('-t', '--cpu-threads', default=0, help="Number of threads to use when running on CPU")
     parser.add_argument('-nw', '--num-workers', default=1, help="Number of concurrent calls when running whisper model")
     parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="auto")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-lS', '--list-src-languages', help="List all available src_languages (whisper supported languages)", action='store_true')
     parser.add_argument('-lD', '--list-dst-languages', help="List all available dst_languages (google translate supported languages)", action='store_true')
-    parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
-    parser.add_argument('-lF', '--list-formats', help="List all supported subtitle formats", action='store_true')
+    parser.add_argument('-F', '--format', help="Desired subtitles format", default="srt")
+    parser.add_argument('-lF', '--list-formats', help="List all supported subtitles formats", action='store_true')
     parser.add_argument('-c', '--concurrency', help="Number of concurrent calls for Google Translate API", type=int, default=10)
-    parser.add_argument('-e', '--embed', help="Boolean value (True or False) for embedding subtitle file into video file", type=bool, default=False)
+    parser.add_argument('-es', '--embed-src', help="Boolean value (True or False) for embedding original language subtitles file into video file", type=bool, default=False)
+    parser.add_argument('-ed', '--embed-dst', help="Boolean value (True or False) for embedding translated subtitles file into video file", type=bool, default=False)
     parser.add_argument('-fr', '--force-recognize', help="Boolean value (True or False) for re-recognize media file event if it's already has subtitles stream", type=bool, default=False)
     parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args()
 
     src_language = args.src_language
     dst_language = args.dst_language
@@ -2355,21 +2511,21 @@
             do_translate = True
         else:
             do_translate = False
     else:
         do_translate = False
 
     if args.list_formats:
-        print("List of supported subtitle formats:")
+        print("List of supported subtitles formats:")
         for subtitle_format in SubtitleFormatter.supported_formats:
-            print("{format}".format(format=subtitle_format))
+            print(f"{subtitle_format}")
         return 0
 
     if args.format not in SubtitleFormatter.supported_formats:
-        print("Subtitle format is not supported. Run with --list-formats to see all supported formats.")
+        print("Subtitles format is not supported. Run with --list-formats to see all supported formats.")
         return 1
 
     if not args.source_path:
         parser.print_help(sys.stderr)
         return 1
 
     completed_tasks = 0
@@ -2444,370 +2600,442 @@
     task = "transcribe"
     total_duration = 0
 
     if args.src_language in google_unsupported_languages and do_translate:
         task = "translate"
         src_language = "en"
 
-    if str(args.embed) == "true":
-        args.embed = True
-    if str(args.embed) == "false":
-        args.embed = False
-
     removed_media_filepaths = []
     dst_language = args.dst_language
 
-    print("CHECKING EXISTING SUBTITLES STREAMS")
-    print("===================================")
+    if args.force_recognize == False:
 
-    # CHECKING ffmpeg_src_language_code SUBTITLE STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
-    if do_translate == False:
+        print("CHECKING EXISTING SUBTITLES STREAMS")
+        print("===================================")
 
-        for media_filepath in media_filepaths:
-            print(f"Checking '{media_filepath}'")
+        # CHECKING ffmpeg_src_language_code SUBTITLES STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
+        if do_translate == False:
 
-            if args.src_language == "auto":
-                try:
-                    widgets =["Converting to WAV file                : ", Percentage(), ' ', Bar(), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    wav_filepath, sample_rate = wav_converter(media_filepath)
-                    pbar.finish()
-
-                    segments, info = model.transcribe(wav_filepath)
-                    src_language = info.language
-                    print("Detected language                     : %s (probability = %f)" %(info.language, info.language_probability))
+            for media_filepath in media_filepaths:
+                print(f"Checking '{media_filepath}'")
 
+                if args.src_language == "auto":
+                    try:
+                        widgets =["Converting to WAV file                     : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        wav_filepath, sample_rate = wav_converter(media_filepath)
+                        pbar.finish()
 
-                except KeyboardInterrupt:
-                    pbar.finish()
-                    pool.terminate()
-                    pool.close()
-                    pool.join()
-                    print("Cancelling all tasks")
-
-                    if sys.platform == "win32":
-                        stop_ffmpeg_windows(error_messages_callback=show_error_messages)
-                    else:
-                        stop_ffmpeg_linux(error_messages_callback=show_error_messages)
-
-                    remove_temp_files("wav")
-                    sys.exit(1)
+                        segments, info = model.transcribe(wav_filepath)
+                        src_language = info.language
+                        print(f"Detected language                          : {info.language} (probability = {info.language_probability})")
 
-                except Exception as e:
-                    if not KeyboardInterrupt in e:
+                    except KeyboardInterrupt:
                         pbar.finish()
                         pool.terminate()
                         pool.close()
                         pool.join()
-                        print(e)
+                        print("Cancelling all tasks")
 
                         if sys.platform == "win32":
                             stop_ffmpeg_windows(error_messages_callback=show_error_messages)
                         else:
                             stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
                         remove_temp_files("wav")
                         sys.exit(1)
 
-            else:
-                src_language = args.src_language
+                    except Exception as e:
+                        if not KeyboardInterrupt in str(e):
+                            pbar.finish()
+                            pool.terminate()
+                            pool.close()
+                            pool.join()
+                            print(e)
+
+                            if sys.platform == "win32":
+                                stop_ffmpeg_windows(error_messages_callback=show_error_messages)
+                            else:
+                                stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
-            if src_language in google_unsupported_languages and args.force_recognize==False:
-                removed_media_filepaths.append(media_filepath)
+                            remove_temp_files("wav")
+                            sys.exit(1)
 
-            else:
-                ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+                else:
+                    src_language = args.src_language
 
-                subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-                subtitle_streams_data = subtitle_stream_parser(media_filepath)
+                if src_language in google_unsupported_languages and args.force_recognize==False:
+                    print("Language is not supported by Google Translate API")
+                    removed_media_filepaths.append(media_filepath)
 
-                if subtitle_streams_data and subtitle_streams_data != []:
+                else:
+                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
-                    src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
+                    subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
+                    subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
-                    if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                        print("Is '%s' subtitle stream exist        : Yes" %(ffmpeg_src_language_code.center(3)))
-                        subtitle_stream_regions = []
-                        subtitle_stream_transcripts = []
-                        for entry in src_subtitle_stream_timed_subtitles:
-                            subtitle_stream_regions.append(entry[0])
-                            subtitle_stream_transcripts.append(entry[1])
-                        base, ext = os.path.splitext(media_filepath)
-                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
-                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                        print(f"Extracting '{ffmpeg_src_language_code}' subtitle stream as   : '{src_subtitle_filepath}'")
-                        writer.write(src_subtitle_filepath)
-                        if args.force_recognize == False:
-                            removed_media_filepaths.append(media_filepath)
+                    if subtitle_streams_data and subtitle_streams_data != []:
 
-                    else:
-                        print("Is '%s' subtitle stream exist        : No" %(ffmpeg_src_language_code.center(3)))
+                        src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
-            print("")
+                        if ffmpeg_src_language_code in subtitle_stream_parser.languages():
+                            print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_src_language_code.center(3)))
 
-        if removed_media_filepaths:
-            for removed_media_filepath in removed_media_filepaths:
-                media_filepaths.remove(removed_media_filepath)
-
-        if not media_filepaths:
-            transcribe_end_time = time.time()
-            transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
-            transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
-            transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
-            hour, minute, second = transcribe_elapsed_time_str.split(":")
-            msg = "Total running time                    : %s:%s:%s" %(hour.zfill(2), minute, second)
-            print(msg)
-            sys.exit(0)
+                            subtitle_stream_regions = []
+                            subtitle_stream_transcripts = []
+                            for entry in src_subtitle_stream_timed_subtitles:
+                                subtitle_stream_regions.append(entry[0])
+                                subtitle_stream_transcripts.append(entry[1])
 
-    # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLE STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
-    # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT AND THEN EMBED IT
-    elif do_translate == True:
-        for media_filepath in media_filepaths:
-            print(f"Checking '{media_filepath}'")
+                            base, ext = os.path.splitext(media_filepath)
+                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
 
-            if args.src_language == "auto":
-                try:
-                    widgets =["Converting to WAV file                : ", Percentage(), ' ', Bar(), ' ', ETA()]
-                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    wav_filepath, sample_rate = wav_converter(media_filepath)
-                    pbar.finish()
+                            print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as       : '{src_subtitle_filepath}'")
 
-                    segments, info = model.transcribe(wav_filepath)
-                    src_language = info.language
-                    print("Detected language                     : %s (probability = %f)" %(info.language, info.language_probability))
+                            writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                            writer.write(src_subtitle_filepath)
 
-                except KeyboardInterrupt:
-                    pbar.finish()
-                    pool.terminate()
-                    pool.close()
-                    pool.join()
-                    print("Cancelling all tasks")
+                            if args.force_recognize == False:
+                                removed_media_filepaths.append(media_filepath)
 
-                    if sys.platform == "win32":
-                        stop_ffmpeg_windows(error_messages_callback=show_error_messages)
-                    else:
-                        stop_ffmpeg_linux(error_messages_callback=show_error_messages)
+                            # no translate process as instructed in command arguments
+
+                            # if args.embed_src is True we can't embed it because dst subtitles stream already exist
+                            if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
+
+                        else:
+                            print("Is '%s' subtitles stream exist            : No" %(ffmpeg_src_language_code.center(3)))
+
+                print("")
+
+            if removed_media_filepaths:
+                for removed_media_filepath in removed_media_filepaths:
+                    media_filepaths.remove(removed_media_filepath)
+
+            if not media_filepaths:
+                transcribe_end_time = time.time()
+                transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
+                transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
+                transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
+                hour, minute, second = transcribe_elapsed_time_str.split(":")
+                msg = "Total running time                         : %s:%s:%s" %(hour.zfill(2), minute, second)
+                print(msg)
+                sys.exit(0)
 
-                    remove_temp_files("wav")
-                    sys.exit(1)
+        # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLES STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
+        # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT AND THEN EMBED IT
+        elif do_translate == True:
+            for media_filepath in media_filepaths:
+                print(f"Checking '{media_filepath}'")
+
+                if args.src_language == "auto":
+                    try:
+                        widgets =["Converting to WAV file                     : ", Percentage(), ' ', Bar(), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        wav_filepath, sample_rate = wav_converter(media_filepath)
+                        pbar.finish()
 
-                except Exception as e:
-                    if not KeyboardInterrupt in e:
+                        segments, info = model.transcribe(wav_filepath)
+                        src_language = info.language
+                        print(f"Detected language                          : {info.language} (probability = {info.language_probability})")
+
+                    except KeyboardInterrupt:
                         pbar.finish()
                         pool.terminate()
                         pool.close()
                         pool.join()
-                        print(e)
+                        print("Cancelling all tasks")
 
                         if sys.platform == "win32":
                             stop_ffmpeg_windows(error_messages_callback=show_error_messages)
                         else:
                             stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
                         remove_temp_files("wav")
                         sys.exit(1)
 
-            else:
-                src_language = args.src_language
+                    except Exception as e:
+                        if not KeyboardInterrupt in str(e):
+                            pbar.finish()
+                            pool.terminate()
+                            pool.close()
+                            pool.join()
+                            print(e)
+
+                            if sys.platform == "win32":
+                                stop_ffmpeg_windows(error_messages_callback=show_error_messages)
+                            else:
+                                stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
-            if src_language in google_unsupported_languages and args.force_recognize==False:
-                removed_media_filepaths.append(media_filepath)
+                            remove_temp_files("wav")
+                            sys.exit(1)
 
-            else:
-                ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
-                ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+                else:
+                    src_language = args.src_language
 
-                subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-                subtitle_streams_data = subtitle_stream_parser(media_filepath)
+                if src_language in google_unsupported_languages and args.force_recognize==False:
+                    print(f"Language '{src_language}' is not supported by Google Translate API")
+                    removed_media_filepaths.append(media_filepath)
 
-                if subtitle_streams_data and subtitle_streams_data != []:
+                else:
+                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+                    ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
-                    src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
-                    dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
-
-                    # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
-                    if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                        print("Is '%s' subtitle stream exist        : Yes" %(ffmpeg_src_language_code.center(3)))
-                        subtitle_stream_regions = []
-                        subtitle_stream_transcripts = []
-                        for entry in src_subtitle_stream_timed_subtitles:
-                            subtitle_stream_regions.append(entry[0])
-                            subtitle_stream_transcripts.append(entry[1])
-                        base, ext = os.path.splitext(media_filepath)
-                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
-                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                        print(f"Extracting '{ffmpeg_src_language_code}' subtitle stream as   : '{src_subtitle_filepath}'")
-                        writer.write(src_subtitle_filepath)
+                    subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
+                    subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
-                    # ffmpeg_src_language_code subtitle stream not exist, just print it
-                    else:
-                        print("Is '%s' subtitle stream exist        : No" %(ffmpeg_src_language_code.center(3)))
+                    if subtitle_streams_data and subtitle_streams_data != []:
 
-                    # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
-                    if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
-                        print("Is '%s' subtitle stream exist        : Yes" %(ffmpeg_dst_language_code.center(3)))
-                        subtitle_stream_regions = []
-                        subtitle_stream_transcripts = []
-                        for entry in dst_subtitle_stream_timed_subtitles:
-                            subtitle_stream_regions.append(entry[0])
-                            subtitle_stream_transcripts.append(entry[1])
-                        base, ext = os.path.splitext(media_filepath)
-                        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
-                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                        print(f"Extracting '{ffmpeg_dst_language_code}' subtitle stream as   : '{dst_subtitle_filepath}'")
-                        writer.write(dst_subtitle_filepath)
+                        src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
+                        dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
-                    # ffmpeg_dst_language_code subtitle stream not exist, just print it
-                    else:
-                        print("Is '%s' subtitle stream exist        : No" %(ffmpeg_dst_language_code.center(3)))
+                        # ffmpeg_src_language_code subtitles stream exist, we print it and extract it
+                        if ffmpeg_src_language_code in subtitle_stream_parser.languages():
+                            print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_src_language_code.center(3)))
+
+                            subtitle_stream_regions = []
+                            subtitle_stream_transcripts = []
+                            for entry in src_subtitle_stream_timed_subtitles:
+                                subtitle_stream_regions.append(entry[0])
+                                subtitle_stream_transcripts.append(entry[1])
 
-                    # ffmpeg_dst_language_code subtitle stream = exist,
-                    # ffmpeg_src_language_code subtitle stream = not exist,
-                    # so we translate it from 'dst_language' to 'src_language'
-                    if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
-
-                        if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
-                            prompt = "Translating from %s to %s : " %(dst_language.center(8), src_language.center(8))
-                            widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
-                            pbar = ProgressBar(widgets=widgets, maxval=len(dst_subtitle_stream_timed_subtitles)).start()
-
-                            transcript_translator = SentenceTranslator(src=dst_language, dst=src_language, error_messages_callback=show_error_messages)
-
-                            translated_subtitle_stream_transcripts = []
-                            for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
-                                translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
-                                pbar.update(i)
-                            pbar.finish()
+                            base, ext = os.path.splitext(media_filepath)
+                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+
+                            print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as       : '{src_subtitle_filepath}'")
+
+                            writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                            writer.write(src_subtitle_filepath)
+
+                        # ffmpeg_src_language_code subtitles stream not exist, just print it
+                        else:
+                            print("Is '%s' subtitles stream exist            : No" %(ffmpeg_src_language_code.center(3)))
 
+                        # ffmpeg_src_language_code subtitles stream exist, we print it and extract it
+                        if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
+                            print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_dst_language_code.center(3)))
+                            subtitle_stream_regions = []
+                            subtitle_stream_transcripts = []
+                            for entry in dst_subtitle_stream_timed_subtitles:
+                                subtitle_stream_regions.append(entry[0])
+                                subtitle_stream_transcripts.append(entry[1])
                             base, ext = os.path.splitext(media_filepath)
-                            dst_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
-                            translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                            translation_writer.write(dst_subtitle_filepath)
-                            print(f"Translated subtitles file saved as    : '{dst_subtitle_filepath}'")
-                            if args.force_recognize == False:
-                                removed_media_filepaths.append(media_filepath)
+                            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
+                            writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                            print(f"Extracting '{ffmpeg_dst_language_code}' subtitles stream as       : '{dst_subtitle_filepath}'")
+                            writer.write(dst_subtitle_filepath)
+
+                        # ffmpeg_dst_language_code subtitles stream not exist, just print it
+                        else:
+                            print("Is '%s' subtitles stream exist            : No" %(ffmpeg_dst_language_code.center(3)))
+
+                        # ffmpeg_src_language_code subtitles stream = not exist,
+                        # ffmpeg_dst_language_code subtitles stream = exist,
+                        # so we translate it from 'dst_language' to 'src_language'
+                        if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
+
+                            if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                                prompt = "Translating from %s to %s      : " %(dst_language.center(8), src_language.center(8))
+                                widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
+                                pbar = ProgressBar(widgets=widgets, maxval=len(dst_subtitle_stream_timed_subtitles)).start()
+
+                                transcript_translator = SentenceTranslator(src=dst_language, dst=src_language, error_messages_callback=show_error_messages)
+
+                                translated_subtitle_stream_transcripts = []
+                                for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
+                                    translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
+                                    pbar.update(i)
+                                pbar.finish()
 
-                            if args.embed and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                 base, ext = os.path.splitext(media_filepath)
-                                tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                                ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
-                                embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-
-                                widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                                pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                                result = subtitle_embedder(media_filepath)
+                                src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+
+                                translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                                translation_writer.write(src_subtitle_filepath)
+
+                                print(f"Translated subtitles file saved as         : '{src_subtitle_filepath}'")
+
+                                if args.force_recognize == False:
+                                    removed_media_filepaths.append(media_filepath)
+
+                                if args.embed_src and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+
+                                    base, ext = os.path.splitext(media_filepath)
+                                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                    src_tmp_output = subtitle_embedder(media_filepath)
+                                    pbar.finish()
+
+                                    if os.path.isfile(src_tmp_output):
+                                        shutil.copy(src_tmp_output, embedded_media_filepath)
+                                        os.remove(src_tmp_output)
+
+                                    if os.path.isfile(embedded_media_filepath):
+                                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+
+                                # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
+                                if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                                    print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
+
+                        # ffmpeg_src_language_code subtitles stream = exist,
+                        # ffmpeg_dst_language_code subtitles stream = not exist,
+                        # so we translate it from 'src_language' to 'dst_language'
+                        if ffmpeg_dst_language_code not in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
+
+                            if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                prompt = "Translating from %s to %s      : " %(src_language.center(8), dst_language.center(8))
+                                widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
+                                pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
+
+                                transcript_translator = SentenceTranslator(src=src_language, dst=dst_language, error_messages_callback=show_error_messages)
+
+                                translated_subtitle_stream_transcripts = []
+                                for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
+                                    translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
+                                    pbar.update(i)
                                 pbar.finish()
 
-                                if os.path.isfile(tmp_embedded_media_filepath_1):
-                                    shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                                    os.remove(tmp_embedded_media_filepath_1)
-                                if os.path.isfile(embedded_media_filepath):
-                                    print(f"Subtitle embedded {media_type} file saved as : '{embedded_media_filepath}'")
-
-                    # ffmpeg_dst_language_code subtitle stream = not exist,
-                    # ffmpeg_src_language_code subtitle stream = exist,
-                    # so we translate it from 'src_language' to 'dst_language'
-                    if ffmpeg_dst_language_code not in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
-
-                        if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
-                            prompt = "Translating from %s to %s : " %(src_language.center(8), dst_language.center(8))
-                            widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
-                            pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
-
-                            transcript_translator = SentenceTranslator(src=src_language, dst=dst_language, error_messages_callback=show_error_messages)
-
-                            translated_subtitle_stream_transcripts = []
-                            for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
-                                translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
-                                pbar.update(i)
-                            pbar.finish()
+                                base, ext = os.path.splitext(media_filepath)
+                                dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
 
-                            base, ext = os.path.splitext(media_filepath)
-                            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
-                            translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                            translation_writer.write(dst_subtitle_filepath)
-                            print(f"Translated subtitles file saved as    : '{dst_subtitle_filepath}'")
+                                translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                                translation_writer.write(dst_subtitle_filepath)
+
+                                print(f"Translated subtitles file saved as         : '{dst_subtitle_filepath}'")
+
+                                if args.force_recognize == False:
+                                    removed_media_filepaths.append(media_filepath)
+
+                                if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                    ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+
+                                    base, ext = os.path.splitext(media_filepath)
+                                    dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                                    embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                                    widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                    dst_tmp_output = subtitle_embedder(media_filepath)
+                                    pbar.finish()
+
+                                    if os.path.isfile(dst_tmp_output):
+                                        shutil.copy(dst_tmp_output, embedded_media_filepath)
+                                        os.remove(dst_tmp_output)
+
+                                    if os.path.isfile(embedded_media_filepath):
+                                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+
+                                # if args.embed_src is True then no need to embed it because src subtitles stream already exist
+                                if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                    print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
+
+                        # ffmpeg_dst_language_code subtitles stream = exist,
+                        # ffmpeg_src_language_code subtitles stream = exist,
+                        # so we remove media_filepath from the list of files to be proceed
+                        elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
                             if args.force_recognize == False:
                                 removed_media_filepaths.append(media_filepath)
 
-                        if args.embed and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
-                            ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
-                            base, ext = os.path.splitext(media_filepath)
-                            tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                            embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-
-                            widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(media_filepath)
-                            pbar.finish()
+                            # no need to translate becouse both languages subtitles files already saved
 
-                            if os.path.isfile(tmp_embedded_media_filepath_1):
-                                shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                                os.remove(tmp_embedded_media_filepath_1)
-                            if os.path.isfile(embedded_media_filepath):
-                                print(f"Subtitle embedded {media_type} file saved as : '{embedded_media_filepath}'")
-
-                    # ffmpeg_dst_language_code subtitle stream = exist,
-                    # ffmpeg_src_language_code subtitle stream = exist,
-                    # so we remove media_filepath from the list of files to be proceed
-                    elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                        if args.force_recognize == False:
-                            removed_media_filepaths.append(media_filepath)
+                            # if args.embed_src is True we can't embed it because dst subtitles stream already exist
+                            if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
+
+                            # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
+                            if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
 
                 print("")
 
-        if removed_media_filepaths:
-            for removed_media_filepath in removed_media_filepaths:
-                if removed_media_filepath in media_filepaths:
-                    media_filepaths.remove(removed_media_filepath)
+            if removed_media_filepaths:
+                for removed_media_filepath in removed_media_filepaths:
+                    if removed_media_filepath in media_filepaths:
+                        media_filepaths.remove(removed_media_filepath)
 
-        if not media_filepaths:
-            transcribe_end_time = time.time()
-            transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
-            transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
-            transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
-            hour, minute, second = transcribe_elapsed_time_str.split(":")
-            msg = "Total running time                    : %s:%s:%s" %(hour.zfill(2), minute, second)
-            print(msg)
-            sys.exit(0)
+            if not media_filepaths:
+                transcribe_end_time = time.time()
+                transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
+                transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
+                transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
+                hour, minute, second = transcribe_elapsed_time_str.split(":")
+                msg = "Total running time                         : %s:%s:%s" %(hour.zfill(2), minute, second)
+                print(msg)
+                sys.exit(0)
 
 
-    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLE STREAMS OR FORCED TO BE RE-RECOGNIZED")
+    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLES STREAMS OR FORCED TO BE RE-RECOGNIZED")
     print("=========================================================================================================")
 
-    for media_filepath in media_filepaths:
+    proceed_list = []
+    # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to proceed with transcribe
+    if args.force_recognize == True:
+        for media_filepath in media_filepaths:
+            base, ext = os.path.splitext(media_filepath)
+            tmp_subtitle_removed_media_filepath = "{base}.tmp.subtitles.removed.media_filepath.{format}".format(base=base, format=ext[1:])
+            subtitle_removed_media_filepath = "{base}.force.recognize.{format}".format(base=base, format=ext[1:])
+
+            #src_tmp_output = remove_subtitles_from_media(media_filepath, tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+
+            widgets = [f"Removing subtitles streams from {media_type} file : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+            subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+            tmp_output = subtitle_remover(media_filepath)
+            pbar.finish()
+
+            if os.path.isfile(tmp_output):
+                shutil.copy(tmp_output, subtitle_removed_media_filepath)
+                os.remove(tmp_output)
+
+                proceed_list.append(subtitle_removed_media_filepath)
+
+            print(f"Subtitles removed {media_type} file saved as      : '{subtitle_removed_media_filepath}'")
+            print("")
+
+    # if args.force_recognize is false then we just use modified media_filepaths list
+    else:
+        proceed_list = media_filepaths
+
+
+    # START THE TRANSCRIBE PROCESS
+    for media_filepath in proceed_list:
         print(f"Processing '{media_filepath}'")
 
         try:
-            widgets =["Converting to WAV file                : ", Percentage(), ' ', Bar(), ' ', ETA()]
+            widgets =["Converting to WAV file                     : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
             wav_filepath, sample_rate = wav_converter(media_filepath)
             pbar.finish()
 
             if args.src_language == "auto":
                 segments, info = model.transcribe(wav_filepath)
                 src_language = info.language
-                print("Detected language                     : %s (probability = %f)" %(info.language, info.language_probability))
+                print(f"Detected language                          : {info.language} (probability = {info.language_probability})")
                 total_duration = info.duration
                 ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                 if src_language in google_unsupported_languages and do_translate:
                     task = "translate"
                     src_language = "en"
 
             else:
                 segments, info = model.transcribe(wav_filepath, language=src_language, task=task)
                 total_duration = info.duration
 
-            widgets = ["Performing speech recognition         : ", Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
+            widgets = ["Performing speech recognition              : ", Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
 
             timed_subtitles = []
             regions = []
             transcripts = []
             for segment in segments:
                 progress = int(round(float(segment.end))*100/total_duration)
@@ -2815,117 +3043,177 @@
                 transcripts.append(segment.text)
                 pbar.update(progress)
             pbar.finish()
             timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
 
             base, ext = os.path.splitext(media_filepath)
             src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+
             writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
             writer.write(src_subtitle_filepath)
 
             if do_translate:
                 timed_subtitles = writer.timed_subtitles
                 created_regions = []
                 created_subtitles = []
                 for entry in timed_subtitles:
                     created_regions.append(entry[0])
                     created_subtitles.append(entry[1])
 
-                prompt = "Translating from %s to %s : " %(src_language.center(8), dst_language.center(8))
+                prompt = "Translating from %s to %s      : " %(src_language.center(8), dst_language.center(8))
                 widgets = [prompt, Percentage(), ' ', Bar(marker='#'), ' ', ETA()]
                 pbar = ProgressBar(widgets=widgets, maxval=len(timed_subtitles)).start()
 
                 transcript_translator = SentenceTranslator(src=src_language, dst=dst_language, error_messages_callback=show_error_messages)
 
                 translated_subtitles = []
                 for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                     translated_subtitles.append(translated_subtitle)
                     pbar.update(i)
                 pbar.finish()
 
                 base, ext = os.path.splitext(media_filepath)
                 dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+
                 translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
                 translation_writer.write(dst_subtitle_filepath)
 
             if do_translate:
-                print(f"Original subtitles file saved as      : '{src_subtitle_filepath}'")
-                print(f"Translated subtitles file saved as    : '{dst_subtitle_filepath}'")
+                print(f"Original subtitles file saved as           : '{src_subtitle_filepath}'")
+                print(f"Translated subtitles file saved as         : '{dst_subtitle_filepath}'")
             else:
-                print(f"Subtitles file saved as               : '{src_subtitle_filepath}'")
+                print(f"Subtitles file saved as                    : '{src_subtitle_filepath}'")
 
-            if args.embed:
-                base, ext = os.path.splitext(media_filepath)
-                tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
-                tmp_embedded_media_filepath_3 = "{base}.embedded3.{format}".format(base=base, format=ext[1:])
-                embedded_media_filepath = None
 
-                if do_translate:
+            # EMBEDDING SUBTITLES FILE
+
+            embedded_media_filepath = None
+
+            if do_translate == False:
+
+                if args.embed_src == True:
+
+                    ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    src_tmp_output = subtitle_embedder(media_filepath)
+                    pbar.finish()
+
+                    if os.path.isfile(src_tmp_output):
+                        shutil.copy(src_tmp_output, embedded_media_filepath)
+                        os.remove(src_tmp_output)
+                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+
+            elif do_translate == True:
+
+                if args.embed_src == True and args.embed_dst == True:
+
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                    src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
                     embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
 
-                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    result = subtitle_embedder(media_filepath)
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
-                    if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
-                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(tmp_embedded_media_filepath_1)
-                        pbar.finish()
-                    elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
-                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
+                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_dst_tmp_output = subtitle_embedder(src_tmp_embedded_media_filepath)
                         pbar.finish()
+                    else:
+                        print("Unknown error!")
 
-                    if os.path.isfile(tmp_embedded_media_filepath_2):
-                        shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
+                    if os.path.isfile(src_dst_tmp_output):
+                        shutil.copy(src_dst_tmp_output, embedded_media_filepath)
+                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
 
-                    if os.path.isfile(tmp_embedded_media_filepath_1):
-                        os.remove(tmp_embedded_media_filepath_1)
-                    if os.path.isfile(tmp_embedded_media_filepath_2):
-                        os.remove(tmp_embedded_media_filepath_2)
+                    if os.path.isfile(src_dst_tmp_output):
+                        os.remove(src_dst_tmp_output)
+
+                    if os.path.isfile(src_tmp_output):
+                        os.remove(src_tmp_output)
+
+                elif args.embed_src == True and args.embed_dst == False:
 
-                else:
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
                     embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
-                    #result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    src_tmp_output = subtitle_embedder(media_filepath)
+                    pbar.finish()
+
+                    if os.path.isfile(src_tmp_output):
+                        shutil.copy(src_tmp_output, embedded_media_filepath)
+                        os.remove(src_tmp_embedded_media_filepath)
+                        print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+                    else:
+                        print("Unknown error!")
+
+                elif args.embed_src == False and args.embed_dst == True:
+
+                    ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+
+                    base, ext = os.path.splitext(media_filepath)
+                    dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                    embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
 
-                    widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                    widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                    result = subtitle_embedder(media_filepath)
+                    subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    dst_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
-                    if tmp_embedded_media_filepath_1:
-                        shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                        os.remove(tmp_embedded_media_filepath_1)
+                    if os.path.isfile(dst_tmp_output):
+                        shutil.copy(dst_tmp_output, embedded_media_filepath)
+                        os.remove(dst_tmp_output)
+                        print(f"Subtitles embedded {media_type} file saved as     : {embedded_media_filepath}")
+                    else:
+                        print("Unknown error!")
 
-            if not args.embed:
-                completed_tasks += 1
-            else:
-                if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+            if do_translate == False:
+                if args.embed_src == True:
+                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                        completed_tasks += 1
+                else:
+                    completed_tasks += 1
+
+            elif do_translate == True:
+                if args.embed_src == True or args.embed_dst == True:
+                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                        completed_tasks += 1
+                else:
                     completed_tasks += 1
 
             print("")
             if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
-                msg = "Total running time                    : %s:%s:%s" %(hour.zfill(2), minute, second)
+                msg = "Total running time                         : %s:%s:%s" %(hour.zfill(2), minute, second)
                 print(msg)
 
 
         except KeyboardInterrupt:
             pbar.finish()
             pool.terminate()
             pool.close()
@@ -2937,15 +3225,15 @@
             else:
                 stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
             remove_temp_files("wav")
             return 1
 
         except Exception as e:
-            if not KeyboardInterrupt in e:
+            if not KeyboardInterrupt in str(e):
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
                 print(e)
 
                 if sys.platform == "win32":
```

### Comparing `whisper_autosrt-0.1.2/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whisper-autosrt
-Version: 0.1.2
+Name: whisper_autosrt
+Version: 0.1.4
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

