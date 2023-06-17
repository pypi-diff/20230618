# Comparing `tmp/legendary-gl-0.20.8.tar.gz` & `tmp/legendary-gl-0.20.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\legendary-gl-0.20.8.tar", last modified: Thu Sep  2 17:49:54 2021, max compression
+gzip compressed data, was "dist\legendary-gl-0.20.9.tar", last modified: Fri Sep  3 17:34:20 2021, max compression
```

## Comparing `legendary-gl-0.20.8.tar` & `legendary-gl-0.20.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.108707 legendary-gl-0.20.8/
--rw-rw-rw-   0        0        0    28310 2021-09-02 17:49:54.105707 legendary-gl-0.20.8/PKG-INFO
--rw-rw-rw-   0        0        0    22842 2021-09-02 17:47:00.000000 legendary-gl-0.20.8/README.md
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.050725 legendary-gl-0.20.8/legendary/
--rw-rw-rw-   0        0        0       71 2021-09-02 17:47:42.000000 legendary-gl-0.20.8/legendary/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.053725 legendary-gl-0.20.8/legendary/api/
--rw-rw-rw-   0        0        0        0 2020-03-25 09:37:16.000000 legendary-gl-0.20.8/legendary/api/__init__.py
--rw-rw-rw-   0        0        0     8379 2021-09-02 17:31:04.000000 legendary-gl-0.20.8/legendary/api/egs.py
--rw-rw-rw-   0        0        0      580 2021-09-02 17:31:04.000000 legendary-gl-0.20.8/legendary/api/lgd.py
--rw-rw-rw-   0        0        0    78966 2021-09-02 17:31:04.000000 legendary-gl-0.20.8/legendary/cli.py
--rw-rw-rw-   0        0        0    61436 2021-09-02 17:31:04.000000 legendary-gl-0.20.8/legendary/core.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.055725 legendary-gl-0.20.8/legendary/downloader/
--rw-rw-rw-   0        0        0        0 2020-03-25 09:45:18.000000 legendary-gl-0.20.8/legendary/downloader/__init__.py
--rw-rw-rw-   0        0        0        0 2021-08-12 00:50:35.000000 legendary-gl-0.20.8/legendary/downloader/analyser.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.058724 legendary-gl-0.20.8/legendary/downloader/mp/
--rw-rw-rw-   0        0        0        0 2021-08-12 00:49:56.000000 legendary-gl-0.20.8/legendary/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    35604 2021-09-01 00:37:49.000000 legendary-gl-0.20.8/legendary/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    11075 2021-09-01 00:36:12.000000 legendary-gl-0.20.8/legendary/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.065720 legendary-gl-0.20.8/legendary/lfs/
--rw-rw-rw-   0        0        0        0 2020-03-25 09:38:01.000000 legendary-gl-0.20.8/legendary/lfs/__init__.py
--rw-rw-rw-   0        0        0     2826 2020-06-01 18:41:52.000000 legendary-gl-0.20.8/legendary/lfs/egl.py
--rw-rw-rw-   0        0        0    12052 2021-09-02 17:31:04.000000 legendary-gl-0.20.8/legendary/lfs/lgndry.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.079716 legendary-gl-0.20.8/legendary/models/
--rw-rw-rw-   0        0        0        0 2020-03-25 09:37:45.000000 legendary-gl-0.20.8/legendary/models/__init__.py
--rw-rw-rw-   0        0        0     4487 2020-05-15 05:00:19.000000 legendary-gl-0.20.8/legendary/models/chunk.py
--rw-rw-rw-   0        0        0     3410 2021-08-14 03:00:51.000000 legendary-gl-0.20.8/legendary/models/downloading.py
--rw-rw-rw-   0        0        0     6588 2020-12-17 14:23:05.000000 legendary-gl-0.20.8/legendary/models/egl.py
--rw-rw-rw-   0        0        0      210 2020-05-15 05:00:19.000000 legendary-gl-0.20.8/legendary/models/exceptions.py
--rw-rw-rw-   0        0        0     5331 2021-09-01 12:46:35.000000 legendary-gl-0.20.8/legendary/models/game.py
--rw-rw-rw-   0        0        0     5704 2021-01-04 13:30:56.000000 legendary-gl-0.20.8/legendary/models/json_manifest.py
--rw-rw-rw-   0        0        0    24360 2021-01-04 13:38:04.000000 legendary-gl-0.20.8/legendary/models/manifest.py
--rw-rw-rw-   0        0        0     2241 2021-08-12 02:45:20.000000 legendary-gl-0.20.8/legendary/models/options.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.097710 legendary-gl-0.20.8/legendary/utils/
--rw-rw-rw-   0        0        0        0 2020-05-04 12:08:35.000000 legendary-gl-0.20.8/legendary/utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2020-12-16 10:54:05.000000 legendary-gl-0.20.8/legendary/utils/cli.py
--rw-rw-rw-   0        0        0     1256 2021-09-02 17:11:06.000000 legendary-gl-0.20.8/legendary/utils/config.py
--rw-rw-rw-   0        0        0     1107 2020-05-04 12:13:16.000000 legendary-gl-0.20.8/legendary/utils/custom_parser.py
--rw-rw-rw-   0        0        0      604 2020-12-16 10:52:52.000000 legendary-gl-0.20.8/legendary/utils/game_workarounds.py
--rw-rw-rw-   0        0        0     3809 2021-06-17 12:56:26.000000 legendary-gl-0.20.8/legendary/utils/lfs.py
--rw-rw-rw-   0        0        0     1684 2021-05-24 16:15:22.000000 legendary-gl-0.20.8/legendary/utils/manifests.py
--rw-rw-rw-   0        0        0      537 2020-05-09 05:22:43.000000 legendary-gl-0.20.8/legendary/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     6667 2021-01-04 13:38:49.000000 legendary-gl-0.20.8/legendary/utils/savegame_helper.py
--rw-rw-rw-   0        0        0     1579 2020-12-20 07:45:39.000000 legendary-gl-0.20.8/legendary/utils/selective_dl.py
--rw-rw-rw-   0        0        0      624 2020-12-16 10:15:26.000000 legendary-gl-0.20.8/legendary/utils/wine_helpers.py
-drwxrwxrwx   0        0        0        0 2021-09-02 17:49:54.104708 legendary-gl-0.20.8/legendary_gl.egg-info/
--rw-rw-rw-   0        0        0    28310 2021-09-02 17:49:53.000000 legendary-gl-0.20.8/legendary_gl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2021-09-02 17:49:53.000000 legendary-gl-0.20.8/legendary_gl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-02 17:49:53.000000 legendary-gl-0.20.8/legendary_gl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2021-09-02 17:49:53.000000 legendary-gl-0.20.8/legendary_gl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2021-09-02 17:49:53.000000 legendary-gl-0.20.8/legendary_gl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-09-02 17:49:53.000000 legendary-gl-0.20.8/legendary_gl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-02 17:49:54.109706 legendary-gl-0.20.8/setup.cfg
--rw-rw-rw-   0        0        0     1709 2021-09-01 17:05:03.000000 legendary-gl-0.20.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.534850 legendary-gl-0.20.9/
+-rw-rw-rw-   0        0        0    28310 2021-09-03 17:34:20.533850 legendary-gl-0.20.9/PKG-INFO
+-rw-rw-rw-   0        0        0    22842 2021-09-02 17:47:00.000000 legendary-gl-0.20.9/README.md
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.473871 legendary-gl-0.20.9/legendary/
+-rw-rw-rw-   0        0        0       71 2021-09-03 17:25:21.000000 legendary-gl-0.20.9/legendary/__init__.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.477870 legendary-gl-0.20.9/legendary/api/
+-rw-rw-rw-   0        0        0        0 2020-03-25 09:37:16.000000 legendary-gl-0.20.9/legendary/api/__init__.py
+-rw-rw-rw-   0        0        0     8379 2021-09-02 17:31:04.000000 legendary-gl-0.20.9/legendary/api/egs.py
+-rw-rw-rw-   0        0        0      629 2021-09-03 08:57:59.000000 legendary-gl-0.20.9/legendary/api/lgd.py
+-rw-rw-rw-   0        0        0    79270 2021-09-03 17:22:58.000000 legendary-gl-0.20.9/legendary/cli.py
+-rw-rw-rw-   0        0        0    61498 2021-09-03 17:16:15.000000 legendary-gl-0.20.9/legendary/core.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.480868 legendary-gl-0.20.9/legendary/downloader/
+-rw-rw-rw-   0        0        0        0 2020-03-25 09:45:18.000000 legendary-gl-0.20.9/legendary/downloader/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-08-12 00:50:35.000000 legendary-gl-0.20.9/legendary/downloader/analyser.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.485867 legendary-gl-0.20.9/legendary/downloader/mp/
+-rw-rw-rw-   0        0        0        0 2021-08-12 00:49:56.000000 legendary-gl-0.20.9/legendary/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    35604 2021-09-01 00:37:49.000000 legendary-gl-0.20.9/legendary/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    11075 2021-09-01 00:36:12.000000 legendary-gl-0.20.9/legendary/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.489866 legendary-gl-0.20.9/legendary/lfs/
+-rw-rw-rw-   0        0        0        0 2020-03-25 09:38:01.000000 legendary-gl-0.20.9/legendary/lfs/__init__.py
+-rw-rw-rw-   0        0        0     2826 2020-06-01 18:41:52.000000 legendary-gl-0.20.9/legendary/lfs/egl.py
+-rw-rw-rw-   0        0        0    12052 2021-09-02 17:31:04.000000 legendary-gl-0.20.9/legendary/lfs/lgndry.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.503861 legendary-gl-0.20.9/legendary/models/
+-rw-rw-rw-   0        0        0        0 2020-03-25 09:37:45.000000 legendary-gl-0.20.9/legendary/models/__init__.py
+-rw-rw-rw-   0        0        0     4487 2020-05-15 05:00:19.000000 legendary-gl-0.20.9/legendary/models/chunk.py
+-rw-rw-rw-   0        0        0     3410 2021-08-14 03:00:51.000000 legendary-gl-0.20.9/legendary/models/downloading.py
+-rw-rw-rw-   0        0        0     6588 2020-12-17 14:23:05.000000 legendary-gl-0.20.9/legendary/models/egl.py
+-rw-rw-rw-   0        0        0      210 2020-05-15 05:00:19.000000 legendary-gl-0.20.9/legendary/models/exceptions.py
+-rw-rw-rw-   0        0        0     5331 2021-09-01 12:46:35.000000 legendary-gl-0.20.9/legendary/models/game.py
+-rw-rw-rw-   0        0        0     5704 2021-01-04 13:30:56.000000 legendary-gl-0.20.9/legendary/models/json_manifest.py
+-rw-rw-rw-   0        0        0    24360 2021-01-04 13:38:04.000000 legendary-gl-0.20.9/legendary/models/manifest.py
+-rw-rw-rw-   0        0        0     2241 2021-08-12 02:45:20.000000 legendary-gl-0.20.9/legendary/models/options.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.521855 legendary-gl-0.20.9/legendary/utils/
+-rw-rw-rw-   0        0        0        0 2020-05-04 12:08:35.000000 legendary-gl-0.20.9/legendary/utils/__init__.py
+-rw-rw-rw-   0        0        0     1270 2020-12-16 10:54:05.000000 legendary-gl-0.20.9/legendary/utils/cli.py
+-rw-rw-rw-   0        0        0     1256 2021-09-02 17:11:06.000000 legendary-gl-0.20.9/legendary/utils/config.py
+-rw-rw-rw-   0        0        0     1107 2020-05-04 12:13:16.000000 legendary-gl-0.20.9/legendary/utils/custom_parser.py
+-rw-rw-rw-   0        0        0      604 2020-12-16 10:52:52.000000 legendary-gl-0.20.9/legendary/utils/game_workarounds.py
+-rw-rw-rw-   0        0        0     3809 2021-06-17 12:56:26.000000 legendary-gl-0.20.9/legendary/utils/lfs.py
+-rw-rw-rw-   0        0        0     1684 2021-05-24 16:15:22.000000 legendary-gl-0.20.9/legendary/utils/manifests.py
+-rw-rw-rw-   0        0        0      537 2020-05-09 05:22:43.000000 legendary-gl-0.20.9/legendary/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     6667 2021-01-04 13:38:49.000000 legendary-gl-0.20.9/legendary/utils/savegame_helper.py
+-rw-rw-rw-   0        0        0     1579 2020-12-20 07:45:39.000000 legendary-gl-0.20.9/legendary/utils/selective_dl.py
+-rw-rw-rw-   0        0        0      624 2020-12-16 10:15:26.000000 legendary-gl-0.20.9/legendary/utils/wine_helpers.py
+drwxrwxrwx   0        0        0        0 2021-09-03 17:34:20.531852 legendary-gl-0.20.9/legendary_gl.egg-info/
+-rw-rw-rw-   0        0        0    28310 2021-09-03 17:34:20.000000 legendary-gl-0.20.9/legendary_gl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2021-09-03 17:34:20.000000 legendary-gl-0.20.9/legendary_gl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-03 17:34:20.000000 legendary-gl-0.20.9/legendary_gl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2021-09-03 17:34:20.000000 legendary-gl-0.20.9/legendary_gl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2021-09-03 17:34:20.000000 legendary-gl-0.20.9/legendary_gl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-09-03 17:34:20.000000 legendary-gl-0.20.9/legendary_gl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-09-03 17:34:20.534850 legendary-gl-0.20.9/setup.cfg
+-rw-rw-rw-   0        0        0     1709 2021-09-01 17:05:03.000000 legendary-gl-0.20.9/setup.py
```

### Comparing `legendary-gl-0.20.8/PKG-INFO` & `legendary-gl-0.20.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legendary-gl
-Version: 0.20.8
+Version: 0.20.9
 Summary: Free and open-source replacement for the Epic Games Launcher application
 Home-page: https://github.com/derrod/legendary
 Author: Rodney
 Author-email: rodney@rodney.io
 License: GPL-3
 Description: # Legendary
         ## A free and open-source Epic Games Launcher alternative
```

### Comparing `legendary-gl-0.20.8/README.md` & `legendary-gl-0.20.9/README.md`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/api/egs.py` & `legendary-gl-0.20.9/legendary/api/egs.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/cli.py` & `legendary-gl-0.20.9/legendary/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from legendary.core import LegendaryCore
 from legendary.models.exceptions import InvalidCredentialsError
 from legendary.models.game import SaveGameStatus, VerifyResult
 from legendary.utils.cli import get_boolean_choice, sdl_prompt
 from legendary.utils.custom_parser import AliasedSubParsersAction
 from legendary.utils.lfs import validate_files
 from legendary.utils.selective_dl import get_sdl_appname
+from legendary.utils.wine_helpers import read_registry, get_shell_folders
 
 # todo custom formatter for cli logger (clean info, highlighted error/warning)
 logging.basicConfig(
     format='[%(name)s] %(levelname)s: %(message)s',
     level=logging.INFO
 )
 logger = logging.getLogger('cli')
@@ -65,42 +66,47 @@
         except InvalidCredentialsError:
             logger.error('Stored credentials were found but were no longer valid. Continuing with login...')
             self.core.lgd.invalidate_userdata()
 
         if args.import_egs_auth:
             # get appdata path on Linux
             if not self.core.egl.appdata_path:
-                wine_pfx_users = None
-                lutris_wine_users = os.path.expanduser('~/Games/epic-games-store/drive_c/users')
-                if os.path.exists(lutris_wine_users):
-                    logger.info(f'Found Lutris EGL WINE prefix at "{lutris_wine_users}"')
+                egl_wine_pfx = None
+                lutris_wine_pfx = os.path.expanduser('~/Games/epic-games-store')
+                if os.path.exists(lutris_wine_pfx):
+                    logger.info(f'Found Lutris EGL WINE prefix at "{lutris_wine_pfx}"')
                     if args.yes or get_boolean_choice('Do you want to use the Lutris install?'):
-                        wine_pfx_users = lutris_wine_users
+                        egl_wine_pfx = lutris_wine_pfx
 
-                if not wine_pfx_users:
+                if not egl_wine_pfx:
                     logger.info('Please enter the path to the Wine prefix that has EGL installed')
                     wine_pfx = input('Path [empty input to quit]: ').strip()
                     if not wine_pfx:
                         print('Empty input, quitting...')
                         exit(0)
-                    if not os.path.exists(wine_pfx):
+                    if not os.path.exists(wine_pfx) and os.path.isdir(wine_pfx):
                         print('Path is invalid (does not exist)!')
                         exit(1)
-                    wine_pfx_users = os.path.join(wine_pfx, 'drive_c/users')
 
-                # todo instead of getuser() this should read from the user.reg in the WINE prefix
-                appdata_dir = os.path.join(wine_pfx_users, getuser(),
-                                           'Local Settings/Application Data/EpicGamesLauncher',
-                                           'Saved/Config/Windows')
-                if not os.path.exists(appdata_dir):
-                    logger.error(f'Wine prefix does not have EGL appdata path at "{appdata_dir}"')
+                try:
+                    wine_folders = get_shell_folders(read_registry(egl_wine_pfx), egl_wine_pfx)
+                    egl_appdata = os.path.realpath(os.path.join(wine_folders['Local AppData'],
+                                                                'EpicGamesLauncher', 'Saved',
+                                                                'Config', 'Windows'))
+                except Exception as e:
+                    logger.error(f'Got exception when trying to read WINE registry: {e!r}')
+                    logger.error('Make sure you are specifying a valid wine prefix.')
+                    exit(1)
+
+                if not os.path.exists(egl_appdata):
+                    logger.error(f'Wine prefix does not have EGL appdata path at "{egl_appdata}"')
                     exit(0)
                 else:
-                    logger.info(f'Using EGL appdata path at "{appdata_dir}"')
-                    self.core.egl.appdata_path = appdata_dir
+                    logger.info(f'Using EGL appdata path at "{egl_appdata}"')
+                    self.core.egl.appdata_path = egl_appdata
 
             logger.info('Importing login session from the Epic Launcher...')
             try:
                 if self.core.auth_import():
                     logger.info('Successfully imported login session from EGS!')
                     logger.info(f'Now logged in as user "{self.core.lgd.userdata["displayName"]}"')
                     return
```

### Comparing `legendary-gl-0.20.8/legendary/core.py` & `legendary-gl-0.20.9/legendary/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
             'X-Requested-With': 'XMLHttpRequest',
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
                           'AppleWebKit/537.36 (KHTML, like Gecko) '
                           'EpicGamesLauncher/11.0.1-14907503+++Portal+Release-Live '
                           'UnrealEngine/4.23.0-14907503+++Portal+Release-Live '
                           'Chrome/84.0.4147.38 Safari/537.36'
         })
+        s.cookies['EPIC_COUNTRY'] = self.country_code.upper()
 
         # get first set of cookies (EPIC_BEARER_TOKEN etc.)
         _ = s.get('https://www.epicgames.com/id/api/set-sid', params=dict(sid=sid))
         # get XSRF-TOKEN and EPIC_SESSION_AP cookie
         _ = s.get('https://www.epicgames.com/id/api/csrf')
         # finally, get the exchange code
         r = s.post('https://www.epicgames.com/id/api/exchange/generate',
```

### Comparing `legendary-gl-0.20.8/legendary/downloader/mp/manager.py` & `legendary-gl-0.20.9/legendary/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/downloader/mp/workers.py` & `legendary-gl-0.20.9/legendary/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/lfs/egl.py` & `legendary-gl-0.20.9/legendary/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/lfs/lgndry.py` & `legendary-gl-0.20.9/legendary/lfs/lgndry.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/chunk.py` & `legendary-gl-0.20.9/legendary/models/chunk.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/downloading.py` & `legendary-gl-0.20.9/legendary/models/downloading.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/egl.py` & `legendary-gl-0.20.9/legendary/models/egl.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/game.py` & `legendary-gl-0.20.9/legendary/models/game.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/json_manifest.py` & `legendary-gl-0.20.9/legendary/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/manifest.py` & `legendary-gl-0.20.9/legendary/models/manifest.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/models/options.py` & `legendary-gl-0.20.9/legendary/models/options.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/cli.py` & `legendary-gl-0.20.9/legendary/utils/cli.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/config.py` & `legendary-gl-0.20.9/legendary/utils/config.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/custom_parser.py` & `legendary-gl-0.20.9/legendary/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/game_workarounds.py` & `legendary-gl-0.20.9/legendary/utils/game_workarounds.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/lfs.py` & `legendary-gl-0.20.9/legendary/utils/lfs.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/manifests.py` & `legendary-gl-0.20.9/legendary/utils/manifests.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/rolling_hash.py` & `legendary-gl-0.20.9/legendary/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/savegame_helper.py` & `legendary-gl-0.20.9/legendary/utils/savegame_helper.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/selective_dl.py` & `legendary-gl-0.20.9/legendary/utils/selective_dl.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary/utils/wine_helpers.py` & `legendary-gl-0.20.9/legendary/utils/wine_helpers.py`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/legendary_gl.egg-info/PKG-INFO` & `legendary-gl-0.20.9/legendary_gl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legendary-gl
-Version: 0.20.8
+Version: 0.20.9
 Summary: Free and open-source replacement for the Epic Games Launcher application
 Home-page: https://github.com/derrod/legendary
 Author: Rodney
 Author-email: rodney@rodney.io
 License: GPL-3
 Description: # Legendary
         ## A free and open-source Epic Games Launcher alternative
```

### Comparing `legendary-gl-0.20.8/legendary_gl.egg-info/SOURCES.txt` & `legendary-gl-0.20.9/legendary_gl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legendary-gl-0.20.8/setup.py` & `legendary-gl-0.20.9/setup.py`

 * *Files identical despite different names*

