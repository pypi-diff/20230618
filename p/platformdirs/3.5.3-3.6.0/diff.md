# Comparing `tmp/platformdirs-3.5.3.tar.gz` & `tmp/platformdirs-3.6.0.tar.gz`

## Comparing `platformdirs-3.5.3.tar` & `platformdirs-3.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tox.ini
--rw-r--r--   0        0        0    19758 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/android.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/api.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/py.typed
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/version.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 platformdirs-3.5.3/src/platformdirs/windows.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/conftest.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_android.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_main.py
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 platformdirs-3.5.3/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.5.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.5.3/LICENSE
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 platformdirs-3.5.3/README.rst
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.5.3/pyproject.toml
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 platformdirs-3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tox.ini
+-rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/android.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 platformdirs-3.6.0/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/test_android.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/test_main.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 platformdirs-3.6.0/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.6.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.6.0/LICENSE
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 platformdirs-3.6.0/README.rst
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 platformdirs-3.6.0/PKG-INFO
```

### Comparing `platformdirs-3.5.3/tox.ini` & `platformdirs-3.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.3/src/platformdirs/__init__.py` & `platformdirs-3.6.0/src/platformdirs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,19 @@
 
 
 def user_documents_dir() -> str:
     """:returns: documents directory tied to the user"""
     return PlatformDirs().user_documents_dir
 
 
+def user_downloads_dir() -> str:
+    """:returns: downloads directory tied to the user"""
+    return PlatformDirs().user_downloads_dir
+
+
 def user_pictures_dir() -> str:
     """:returns: pictures directory tied to the user"""
     return PlatformDirs().user_pictures_dir
 
 
 def user_videos_dir() -> str:
     """:returns: videos directory tied to the user"""
@@ -476,14 +481,19 @@
 
 
 def user_documents_path() -> Path:
     """:returns: documents path tied to the user"""
     return PlatformDirs().user_documents_path
 
 
+def user_downloads_path() -> Path:
+    """:returns: downloads path tied to the user"""
+    return PlatformDirs().user_downloads_path
+
+
 def user_pictures_path() -> Path:
     """:returns: pictures path tied to the user"""
     return PlatformDirs().user_pictures_path
 
 
 def user_videos_path() -> Path:
     """:returns: videos path tied to the user"""
@@ -527,27 +537,29 @@
     "PlatformDirsABC",
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
+    "user_downloads_dir",
     "user_pictures_dir",
     "user_videos_dir",
     "user_music_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
     "user_data_path",
     "user_config_path",
     "user_cache_path",
     "user_state_path",
     "user_log_path",
     "user_documents_path",
+    "user_downloads_path",
     "user_pictures_path",
     "user_videos_path",
     "user_music_path",
     "user_runtime_path",
     "site_data_path",
     "site_config_path",
     "site_cache_path",
```

### Comparing `platformdirs-3.5.3/src/platformdirs/__main__.py` & `platformdirs-3.6.0/src/platformdirs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 PROPS = (
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
+    "user_downloads_dir",
     "user_pictures_dir",
     "user_videos_dir",
     "user_music_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
```

### Comparing `platformdirs-3.5.3/src/platformdirs/android.py` & `platformdirs-3.6.0/src/platformdirs/android.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user e.g. ``/storage/emulated/0/Documents``"""
         return _android_documents_folder()
 
     @property
+    def user_downloads_dir(self) -> str:
+        """:return: downloads directory tied to the user e.g. ``/storage/emulated/0/Downloads``"""
+        return _android_downloads_folder()
+
+    @property
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user e.g. ``/storage/emulated/0/Pictures``"""
         return _android_pictures_folder()
 
     @property
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user e.g. ``/storage/emulated/0/DCIM/Camera``"""
@@ -133,14 +138,30 @@
     except Exception:  # noqa: BLE001
         documents_dir = "/storage/emulated/0/Documents"
 
     return documents_dir
 
 
 @lru_cache(maxsize=1)
+def _android_downloads_folder() -> str:
+    """:return: downloads folder for the Android OS"""
+    # Get directories with pyjnius
+    try:
+        from jnius import autoclass
+
+        context = autoclass("android.content.Context")
+        environment = autoclass("android.os.Environment")
+        downloads_dir: str = context.getExternalFilesDir(environment.DIRECTORY_DOWNLOADS).getAbsolutePath()
+    except Exception:  # noqa: BLE001
+        downloads_dir = "/storage/emulated/0/Downloads"
+
+    return downloads_dir
+
+
+@lru_cache(maxsize=1)
 def _android_pictures_folder() -> str:
     """:return: pictures folder for the Android OS"""
     # Get directories with pyjnius
     try:
         from jnius import autoclass
 
         context = autoclass("android.content.Context")
```

### Comparing `platformdirs-3.5.3/src/platformdirs/api.py` & `platformdirs-3.6.0/src/platformdirs/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -125,14 +125,19 @@
     @property
     @abstractmethod
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user"""
 
     @property
     @abstractmethod
+    def user_downloads_dir(self) -> str:
+        """:return: downloads directory tied to the user"""
+
+    @property
+    @abstractmethod
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user"""
 
     @property
     @abstractmethod
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user"""
@@ -189,14 +194,19 @@
 
     @property
     def user_documents_path(self) -> Path:
         """:return: documents path tied to the user"""
         return Path(self.user_documents_dir)
 
     @property
+    def user_downloads_path(self) -> Path:
+        """:return: downloads path tied to the user"""
+        return Path(self.user_downloads_dir)
+
+    @property
     def user_pictures_path(self) -> Path:
         """:return: pictures path tied to the user"""
         return Path(self.user_pictures_dir)
 
     @property
     def user_videos_path(self) -> Path:
         """:return: videos path tied to the user"""
```

### Comparing `platformdirs-3.5.3/src/platformdirs/macos.py` & `platformdirs-3.6.0/src/platformdirs/macos.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,19 @@
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user, e.g. ``~/Documents``"""
         return os.path.expanduser("~/Documents")  # noqa: PTH111
 
     @property
+    def user_downloads_dir(self) -> str:
+        """:return: downloads directory tied to the user, e.g. ``~/Downloads``"""
+        return os.path.expanduser("~/Downloads")  # noqa: PTH111
+
+    @property
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user, e.g. ``~/Pictures``"""
         return os.path.expanduser("~/Pictures")  # noqa: PTH111
 
     @property
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user, e.g. ``~/Movies``"""
```

### Comparing `platformdirs-3.5.3/src/platformdirs/unix.py` & `platformdirs-3.6.0/src/platformdirs/unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,19 @@
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user, e.g. ``~/Documents``"""
         return _get_user_media_dir("XDG_DOCUMENTS_DIR", "~/Documents")
 
     @property
+    def user_downloads_dir(self) -> str:
+        """:return: downloads directory tied to the user, e.g. ``~/Downloads``"""
+        return _get_user_media_dir("XDG_DOWNLOAD_DIR", "~/Downloads")
+
+    @property
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user, e.g. ``~/Pictures``"""
         return _get_user_media_dir("XDG_PICTURES_DIR", "~/Pictures")
 
     @property
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user, e.g. ``~/Videos``"""
```

### Comparing `platformdirs-3.5.3/src/platformdirs/windows.py` & `platformdirs-3.6.0/src/platformdirs/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,19 @@
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user e.g. ``%USERPROFILE%\\Documents``"""
         return os.path.normpath(get_win_folder("CSIDL_PERSONAL"))
 
     @property
+    def user_downloads_dir(self) -> str:
+        """:return: downloads directory tied to the user e.g. ``%USERPROFILE%\\Downloads``"""
+        return os.path.normpath(get_win_folder("CSIDL_DOWNLOADS"))
+
+    @property
     def user_pictures_dir(self) -> str:
         """:return: pictures directory tied to the user e.g. ``%USERPROFILE%\\Pictures``"""
         return os.path.normpath(get_win_folder("CSIDL_MYPICTURES"))
 
     @property
     def user_videos_dir(self) -> str:
         """:return: videos directory tied to the user e.g. ``%USERPROFILE%\\Videos``"""
@@ -149,14 +154,17 @@
 
 
 def get_win_folder_if_csidl_name_not_env_var(csidl_name: str) -> str | None:
     """Get folder for a CSIDL name that does not exist as an environment variable."""
     if csidl_name == "CSIDL_PERSONAL":
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")  # noqa: PTH118
 
+    if csidl_name == "CSIDL_DOWNLOADS":
+        return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Downloads")  # noqa: PTH118
+
     if csidl_name == "CSIDL_MYPICTURES":
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Pictures")  # noqa: PTH118
 
     if csidl_name == "CSIDL_MYVIDEO":
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Videos")  # noqa: PTH118
 
     if csidl_name == "CSIDL_MYMUSIC":
@@ -172,14 +180,15 @@
     for all CSIDL_* names.
     """
     shell_folder_name = {
         "CSIDL_APPDATA": "AppData",
         "CSIDL_COMMON_APPDATA": "Common AppData",
         "CSIDL_LOCAL_APPDATA": "Local AppData",
         "CSIDL_PERSONAL": "Personal",
+        "CSIDL_DOWNLOADS": "{374DE290-123F-4565-9164-39C4925E467B}",
         "CSIDL_MYPICTURES": "My Pictures",
         "CSIDL_MYVIDEO": "My Video",
         "CSIDL_MYMUSIC": "My Music",
     }.get(csidl_name)
     if shell_folder_name is None:
         msg = f"Unknown CSIDL name: {csidl_name}"
         raise ValueError(msg)
@@ -190,22 +199,27 @@
     key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders")
     directory, _ = winreg.QueryValueEx(key, shell_folder_name)
     return str(directory)
 
 
 def get_win_folder_via_ctypes(csidl_name: str) -> str:
     """Get folder with ctypes."""
+    # There is no 'CSIDL_DOWNLOADS'.
+    # Use 'CSIDL_PROFILE' (40) and append the default folder 'Downloads' instead.
+    # https://learn.microsoft.com/en-us/windows/win32/shell/knownfolderid
+
     csidl_const = {
         "CSIDL_APPDATA": 26,
         "CSIDL_COMMON_APPDATA": 35,
         "CSIDL_LOCAL_APPDATA": 28,
         "CSIDL_PERSONAL": 5,
         "CSIDL_MYPICTURES": 39,
         "CSIDL_MYVIDEO": 14,
         "CSIDL_MYMUSIC": 13,
+        "CSIDL_DOWNLOADS": 40,
     }.get(csidl_name)
     if csidl_const is None:
         msg = f"Unknown CSIDL name: {csidl_name}"
         raise ValueError(msg)
 
     buf = ctypes.create_unicode_buffer(1024)
     windll = getattr(ctypes, "windll")  # noqa: B009 # using getattr to avoid false positive with mypy type checker
@@ -213,14 +227,17 @@
 
     # Downgrade to short path name if it has highbit chars.
     if any(ord(c) > 255 for c in buf):  # noqa: PLR2004
         buf2 = ctypes.create_unicode_buffer(1024)
         if windll.kernel32.GetShortPathNameW(buf.value, buf2, 1024):
             buf = buf2
 
+    if csidl_name == "CSIDL_DOWNLOADS":
+        return os.path.join(buf.value, "Downloads")  # noqa: PTH118
+
     return buf.value
 
 
 def _pick_get_win_folder() -> Callable[[str], str]:
     if hasattr(ctypes, "windll"):
         return get_win_folder_via_ctypes
     try:
```

### Comparing `platformdirs-3.5.3/tests/conftest.py` & `platformdirs-3.6.0/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 PROPS = (
     "user_data_dir",
     "user_config_dir",
     "user_cache_dir",
     "user_state_dir",
     "user_log_dir",
     "user_documents_dir",
+    "user_downloads_dir",
     "user_pictures_dir",
     "user_videos_dir",
     "user_music_dir",
     "user_runtime_dir",
     "site_data_dir",
     "site_config_dir",
     "site_cache_dir",
```

### Comparing `platformdirs-3.5.3/tests/test_android.py` & `platformdirs-3.6.0/tests/test_android.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         "user_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "site_config_dir": f"/data/data/com.example/shared_prefs{suffix}",
         "user_cache_dir": f"/data/data/com.example/cache{suffix}",
         "site_cache_dir": f"/data/data/com.example/cache{suffix}",
         "user_state_dir": f"/data/data/com.example/files{suffix}",
         "user_log_dir": f"/data/data/com.example/cache{suffix}{'' if params.get('opinion', True) is False else '/log'}",
         "user_documents_dir": "/storage/emulated/0/Documents",
+        "user_downloads_dir": "/storage/emulated/0/Downloads",
         "user_pictures_dir": "/storage/emulated/0/Pictures",
         "user_videos_dir": "/storage/emulated/0/DCIM/Camera",
         "user_music_dir": "/storage/emulated/0/Music",
         "user_runtime_dir": f"/data/data/com.example/cache{suffix}{'' if not params.get('opinion', True) else val}",
     }
     expected = expected_map[func]
```

### Comparing `platformdirs-3.5.3/tests/test_api.py` & `platformdirs-3.6.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.3/tests/test_comp_with_appdirs.py` & `platformdirs-3.6.0/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.3/tests/test_macos.py` & `platformdirs-3.6.0/tests/test_macos.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "user_config_dir": f"{home}/Library/Application Support{suffix}",
         "site_config_dir": f"/Library/Application Support{suffix}",
         "user_cache_dir": f"{home}/Library/Caches{suffix}",
         "site_cache_dir": f"/Library/Caches{suffix}",
         "user_state_dir": f"{home}/Library/Application Support{suffix}",
         "user_log_dir": f"{home}/Library/Logs{suffix}",
         "user_documents_dir": f"{home}/Documents",
+        "user_downloads_dir": f"{home}/Downloads",
         "user_pictures_dir": f"{home}/Pictures",
         "user_videos_dir": f"{home}/Movies",
         "user_music_dir": f"{home}/Music",
         "user_runtime_dir": f"{home}/Library/Caches/TemporaryItems{suffix}",
     }
     expected = expected_map[func]
```

### Comparing `platformdirs-3.5.3/tests/test_unix.py` & `platformdirs-3.6.0/tests/test_unix.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,36 @@
 
 if typing.TYPE_CHECKING:
     from pathlib import Path
 
     from pytest_mock import MockerFixture
 
 
-@pytest.mark.parametrize("prop", ["user_documents_dir", "user_pictures_dir", "user_videos_dir", "user_music_dir"])
+@pytest.mark.parametrize(
+    "prop",
+    [
+        "user_documents_dir",
+        "user_downloads_dir",
+        "user_pictures_dir",
+        "user_videos_dir",
+        "user_music_dir",
+    ],
+)
 def test_user_media_dir(mocker: MockerFixture, prop: str) -> None:
     example_path = "/home/example/ExampleMediaFolder"
     mock = mocker.patch("platformdirs.unix._get_user_dirs_folder")
     mock.return_value = example_path
     assert getattr(Unix(), prop) == example_path
 
 
 @pytest.mark.parametrize(
     ("env_var", "prop"),
     [
         pytest.param("XDG_DOCUMENTS_DIR", "user_documents_dir", id="user_documents_dir"),
+        pytest.param("XDG_DOWNLOAD_DIR", "user_downloads_dir", id="user_downloads_dir"),
         pytest.param("XDG_PICTURES_DIR", "user_pictures_dir", id="user_pictures_dir"),
         pytest.param("XDG_VIDEOS_DIR", "user_videos_dir", id="user_videos_dir"),
         pytest.param("XDG_MUSIC_DIR", "user_music_dir", id="user_music_dir"),
     ],
 )
 def test_user_media_dir_env_var(mocker: MockerFixture, env_var: str, prop: str) -> None:
     # Mock media dir not being in user-dirs.dirs file
@@ -44,14 +54,15 @@
     assert getattr(Unix(), prop) == example_path
 
 
 @pytest.mark.parametrize(
     ("env_var", "prop", "default_abs_path"),
     [
         pytest.param("XDG_DOCUMENTS_DIR", "user_documents_dir", "/home/example/Documents", id="user_documents_dir"),
+        pytest.param("XDG_DOWNLOAD_DIR", "user_downloads_dir", "/home/example/Downloads", id="user_downloads_dir"),
         pytest.param("XDG_PICTURES_DIR", "user_pictures_dir", "/home/example/Pictures", id="user_pictures_dir"),
         pytest.param("XDG_VIDEOS_DIR", "user_videos_dir", "/home/example/Videos", id="user_videos_dir"),
         pytest.param("XDG_MUSIC_DIR", "user_music_dir", "/home/example/Music", id="user_music_dir"),
     ],
 )
 def test_user_media_dir_default(mocker: MockerFixture, env_var: str, prop: str, default_abs_path: str) -> None:
     # Mock media dir not being in user-dirs.dirs file
```

### Comparing `platformdirs-3.5.3/LICENSE` & `platformdirs-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.3/README.rst` & `platformdirs-3.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 - user data dir (``user_data_dir``)
 - user config dir (``user_config_dir``)
 - user cache dir (``user_cache_dir``)
 - site data dir (``site_data_dir``)
 - site config dir (``site_config_dir``)
 - user log dir (``user_log_dir``)
 - user documents dir (``user_documents_dir``)
+- user downloads dir (``user_downloads_dir``)
 - user runtime dir (``user_runtime_dir``)
 
 And also:
 
 - Is slightly opinionated on the directory names used. Look for "OPINION" in
   documentation and code for when an opinion is being applied.
 
@@ -64,14 +65,16 @@
     '/Library/Application Support/SuperApp'
     >>> user_cache_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/Users/trentm/Library/Logs/SuperApp'
     >>> user_documents_dir()
     '/Users/trentm/Documents'
+    >>> user_downloads_dir()
+    '/Users/trentm/Downloads'
     >>> user_runtime_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 On Windows:
 
 .. code-block:: pycon
 
@@ -84,14 +87,16 @@
     'C:\\Users\\trentm\\AppData\\Roaming\\Acme\\SuperApp'
     >>> user_cache_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Cache'
     >>> user_log_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Logs'
     >>> user_documents_dir()
     'C:\\Users\\trentm\\Documents'
+    >>> user_downloads_dir()
+    'C:\\Users\\trentm\\Downloads'
     >>> user_runtime_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Temp\\Acme\\SuperApp'
 
 On Linux:
 
 .. code-block:: pycon
 
@@ -108,14 +113,16 @@
     '/home/trentm/.cache/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/home/trentm/.cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/home/trentm/.config/SuperApp'
     >>> user_documents_dir()
     '/home/trentm/Documents'
+    >>> user_downloads_dir()
+    '/home/trentm/Downloads'
     >>> user_runtime_dir(appname, appauthor)
     '/run/user/{os.getuid()}/SuperApp'
     >>> site_config_dir(appname)
     '/etc/xdg/SuperApp'
     >>> os.environ["XDG_CONFIG_DIRS"] = "/etc:/usr/local/etc"
     >>> site_config_dir(appname, multipath=True)
     '/etc/SuperApp:/usr/local/etc/SuperApp'
@@ -131,14 +138,16 @@
     '/data/data/com.myApp/cache/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/data/data/com.myApp/cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/data/data/com.myApp/shared_prefs/SuperApp'
     >>> user_documents_dir()
     '/storage/emulated/0/Documents'
+    >>> user_downloads_dir()
+    '/storage/emulated/0/Downloads'
     >>> user_runtime_dir(appname, appauthor)
     '/data/data/com.myApp/cache/SuperApp/tmp'
 
 Note: Some android apps like Termux and Pydroid are used as shells. These
 apps are used by the end user to emulate Linux environment. Presence of
 ``SHELL`` environment variable is used by Platformdirs to differentiate
 between general android apps and android apps used as shells. Shell android
@@ -158,14 +167,16 @@
     '/Library/Application Support/SuperApp'
     >>> dirs.user_cache_dir
     '/Users/trentm/Library/Caches/SuperApp'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
+    >>> dirs.user_downloads_dir
+    '/Users/trentm/Downloads'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 Per-version isolation
 =====================
 
 If you have multiple versions of your app in use that you want to be
@@ -180,14 +191,16 @@
     '/Library/Application Support/SuperApp/1.0'
     >>> dirs.user_cache_dir
     '/Users/trentm/Library/Caches/SuperApp/1.0'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp/1.0'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
+    >>> dirs.user_downloads_dir
+    '/Users/trentm/Downloads'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp/1.0'
 
 Be wary of using this for configuration files though; you'll need to handle
 migrating configuration files manually.
 
 Why this Fork?
```

### Comparing `platformdirs-3.5.3/pyproject.toml` & `platformdirs-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `platformdirs-3.5.3/PKG-INFO` & `platformdirs-3.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.5.3
+Version: 3.6.0
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
@@ -79,14 +79,15 @@
 - user data dir (``user_data_dir``)
 - user config dir (``user_config_dir``)
 - user cache dir (``user_cache_dir``)
 - site data dir (``site_data_dir``)
 - site config dir (``site_config_dir``)
 - user log dir (``user_log_dir``)
 - user documents dir (``user_documents_dir``)
+- user downloads dir (``user_downloads_dir``)
 - user runtime dir (``user_runtime_dir``)
 
 And also:
 
 - Is slightly opinionated on the directory names used. Look for "OPINION" in
   documentation and code for when an opinion is being applied.
 
@@ -106,14 +107,16 @@
     '/Library/Application Support/SuperApp'
     >>> user_cache_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/Users/trentm/Library/Logs/SuperApp'
     >>> user_documents_dir()
     '/Users/trentm/Documents'
+    >>> user_downloads_dir()
+    '/Users/trentm/Downloads'
     >>> user_runtime_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 On Windows:
 
 .. code-block:: pycon
 
@@ -126,14 +129,16 @@
     'C:\\Users\\trentm\\AppData\\Roaming\\Acme\\SuperApp'
     >>> user_cache_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Cache'
     >>> user_log_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Logs'
     >>> user_documents_dir()
     'C:\\Users\\trentm\\Documents'
+    >>> user_downloads_dir()
+    'C:\\Users\\trentm\\Downloads'
     >>> user_runtime_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Temp\\Acme\\SuperApp'
 
 On Linux:
 
 .. code-block:: pycon
 
@@ -150,14 +155,16 @@
     '/home/trentm/.cache/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/home/trentm/.cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/home/trentm/.config/SuperApp'
     >>> user_documents_dir()
     '/home/trentm/Documents'
+    >>> user_downloads_dir()
+    '/home/trentm/Downloads'
     >>> user_runtime_dir(appname, appauthor)
     '/run/user/{os.getuid()}/SuperApp'
     >>> site_config_dir(appname)
     '/etc/xdg/SuperApp'
     >>> os.environ["XDG_CONFIG_DIRS"] = "/etc:/usr/local/etc"
     >>> site_config_dir(appname, multipath=True)
     '/etc/SuperApp:/usr/local/etc/SuperApp'
@@ -173,14 +180,16 @@
     '/data/data/com.myApp/cache/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/data/data/com.myApp/cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/data/data/com.myApp/shared_prefs/SuperApp'
     >>> user_documents_dir()
     '/storage/emulated/0/Documents'
+    >>> user_downloads_dir()
+    '/storage/emulated/0/Downloads'
     >>> user_runtime_dir(appname, appauthor)
     '/data/data/com.myApp/cache/SuperApp/tmp'
 
 Note: Some android apps like Termux and Pydroid are used as shells. These
 apps are used by the end user to emulate Linux environment. Presence of
 ``SHELL`` environment variable is used by Platformdirs to differentiate
 between general android apps and android apps used as shells. Shell android
@@ -200,14 +209,16 @@
     '/Library/Application Support/SuperApp'
     >>> dirs.user_cache_dir
     '/Users/trentm/Library/Caches/SuperApp'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
+    >>> dirs.user_downloads_dir
+    '/Users/trentm/Downloads'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 Per-version isolation
 =====================
 
 If you have multiple versions of your app in use that you want to be
@@ -222,14 +233,16 @@
     '/Library/Application Support/SuperApp/1.0'
     >>> dirs.user_cache_dir
     '/Users/trentm/Library/Caches/SuperApp/1.0'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp/1.0'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
+    >>> dirs.user_downloads_dir
+    '/Users/trentm/Downloads'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp/1.0'
 
 Be wary of using this for configuration files though; you'll need to handle
 migrating configuration files manually.
 
 Why this Fork?
```

