# Comparing `tmp/ican-0.1.6.tar.gz` & `tmp/ican-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ican-0.1.6.tar", last modified: Wed Jun 29 23:28:00 2022, max compression
+gzip compressed data, was "ican-0.1.9.tar", last modified: Tue Jul  5 16:30:00 2022, max compression
```

## Comparing `ican-0.1.6.tar` & `ican-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 23:28:00.597082 ican-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-06-29 23:27:22.000000 ican-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2022-06-29 23:28:00.597082 ican-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2022-06-29 23:27:22.000000 ican-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 23:28:00.597082 ican-0.1.6/ican/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-06-29 23:27:22.000000 ican-0.1.6/ican/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4551 2022-06-29 23:27:22.000000 ican-0.1.6/ican/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-06-29 23:27:22.000000 ican-0.1.6/ican/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2022-06-29 23:27:22.000000 ican-0.1.6/ican/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    63645 2022-06-29 23:27:22.000000 ican-0.1.6/ican/emojis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-06-29 23:27:22.000000 ican-0.1.6/ican/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5146 2022-06-29 23:27:22.000000 ican-0.1.6/ican/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-06-29 23:27:22.000000 ican-0.1.6/ican/ican.py
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-06-29 23:27:22.000000 ican-0.1.6/ican/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-06-29 23:27:22.000000 ican-0.1.6/ican/source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-06-29 23:27:22.000000 ican-0.1.6/ican/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11176 2022-06-29 23:27:22.000000 ican-0.1.6/ican/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 23:28:00.597082 ican-0.1.6/ican.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2022-06-29 23:28:00.000000 ican-0.1.6/ican.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-06-29 23:28:00.000000 ican-0.1.6/ican.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 23:28:00.000000 ican-0.1.6/ican.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-29 23:28:00.000000 ican-0.1.6/ican.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-29 23:28:00.000000 ican-0.1.6/ican.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-29 23:28:00.000000 ican-0.1.6/ican.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-06-29 23:27:22.000000 ican-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-29 23:28:00.597082 ican-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 16:30:00.898919 ican-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-07-05 16:29:46.000000 ican-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-07-05 16:30:00.898919 ican-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-07-05 16:29:46.000000 ican-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 16:30:00.898919 ican-0.1.9/ican/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-05 16:29:46.000000 ican-0.1.9/ican/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5029 2022-07-05 16:29:46.000000 ican-0.1.9/ican/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-07-05 16:29:46.000000 ican-0.1.9/ican/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6465 2022-07-05 16:29:46.000000 ican-0.1.9/ican/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63645 2022-07-05 16:29:46.000000 ican-0.1.9/ican/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-07-05 16:29:46.000000 ican-0.1.9/ican/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-07-05 16:29:46.000000 ican-0.1.9/ican/git.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-07-05 16:29:46.000000 ican-0.1.9/ican/ican.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-07-05 16:29:46.000000 ican-0.1.9/ican/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-05 16:29:46.000000 ican-0.1.9/ican/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-07-05 16:29:46.000000 ican-0.1.9/ican/source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-07-05 16:29:46.000000 ican-0.1.9/ican/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-07-05 16:29:46.000000 ican-0.1.9/ican/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 16:30:00.898919 ican-0.1.9/ican.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-07-05 16:30:00.000000 ican-0.1.9/ican.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-07-05 16:30:00.000000 ican-0.1.9/ican.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 16:30:00.000000 ican-0.1.9/ican.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-07-05 16:30:00.000000 ican-0.1.9/ican.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-05 16:30:00.000000 ican-0.1.9/ican.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-05 16:30:00.000000 ican-0.1.9/ican.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-07-05 16:29:46.000000 ican-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-05 16:30:00.898919 ican-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-07-05 16:29:46.000000 ican-0.1.9/setup.py
```

### Comparing `ican-0.1.6/LICENSE` & `ican-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ican-0.1.6/ican/config.py` & `ican-0.1.9/ican/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,206 +1,219 @@
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
 from configparser import ConfigParser
+from types import SimpleNamespace
 
 from .source import SourceCode
+from .pipeline import PipeLine
 from .log import logger
+from .log import ok_to_write
+from .log import setup_file_handler
+
 
 #######################################
 #
 #   Config Class
 #
 #######################################
 
 
 class Config(object):
     """
     Object which will orchestrate entire program
     """
 
-    ver = dict(current = '0.1.0')
-    opt = dict(
-        auto_tag = False,
-        auto_commit = False,
-        auto_push = False,
-        signature = False)
-    file = dict(file = '*.py',
+    default_ver = dict(current = '0.1.0')
+    default_file = dict(file = '*.py',
         style = 'semantic',
         variable = '__version__')
 
     CONFIG_FILE = '.ican'
-    DEFAULT_CONFIG = dict(version=ver, options=opt, file1=file)
+    DEFAULT_CONFIG = dict(
+        version=default_ver,
+        file1=default_file
+    )
 
-    def __init__(self, parent=None):
+    def __init__(self, git_root=None):
         self.config_file = None
-        self.parent = parent
-
-        self.parser = ConfigParser()
+        self.git_root = git_root
         self.ran_from = Path.cwd()
+        self.parser = ConfigParser()
 
         self.current_version = None
-        self.auto_sign = None
-        self.auto_commit = None
-        self.auto_push = None
-        self.signature = None
+        self.log_to_disk = False
+        self.log_file = ''
         self.source_files = []
+        self.pipelines = {}
+        self.aliases = {}
 
     @property
     def path(self):
         if self.config_file:
             return self.config_file.parent
         return None
 
     def ch_dir_root(self):
         """chdir to the config root, so if we run from another dir, relative
         file paths, etc still work as expected.
         """
-        if self.parent.git.root:
-            os.chdir(str(self.parent.git.root).rstrip('\n'))
+        if self.git_root:
+            os.chdir(str(self.git_root).rstrip('\n'))
         elif self.path:
             os.chdir(str(self.path).rstrip('\n'))
 
     def persist_version(self, version_str):
         """
         Update the version in the config file then write it so we know the
         new version next time
         """
-        logger.debug(f'Persisting version {version_str} in config file.')
-        
+        logger.debug(f'persisting version - {version_str}')
+
         self.parser.set('version', 'current', version_str)
-        if not self.parent.dry_run:
+        if ok_to_write():
             self.parser.write(open(self.config_file, "w"))
 
         return None
 
     def init(self):
         """
         Set default config and save
         """
+        logger.debug(f'command init - setting default config')
         self.parser.read_dict(Config.DEFAULT_CONFIG)
 
         file = Path(self.ran_from, Config.CONFIG_FILE)
-        if not self.parent.dry_run:
+        if not ok_to_write():
             config.write(open(file, "w"))
         self.config_file = file
         return
 
     def search_for_config(self):
+        logger.debug(f'searching for config file')
         f = Config.CONFIG_FILE
         dirs = [
-            self.parent.git.root,
-            self.ran_from, 
-            self.ran_from.parent, 
+            self.git_root,
+            self.ran_from,
+            self.ran_from.parent,
             self.ran_from.parent.parent
         ]
         for d in dirs:
             if d is None:
                 continue
             c = Path(d, f)
             if c.exists():
                 self.parser.read(c)
                 self.config_file = c
+                logger.debug(f'config found @ {c}')
                 break
         else:
             msg = f"Could not find config file [{f}]  " \
             "Try using a default config with '--init',"
             raise ValueError(msg)
         return
 
     def parse(self):
         """
-        We search for a config in several locations.  Also, the user may 
+        We search for a config in several locations.  Also, the user may
         specify default config, which we load here as well.
         """
 
         # By now we may have git_root or config_root
         self.ch_dir_root()
 
-        # Loop through config to debug it if --verbose
-        for section in self.parser.sections():
-            logger.debug(f'* Config section parsed: --== {section} ==--')
-            for name, value in self.parser.items(section):
-                logger.debug(f'* {name} = {value}')
-
         # Current version
         self.current_version = self.parser.get(
             'version', 'current', fallback='0.1.0'
         )
 
-        # OPTIONS
-        self.auto_tag = self.parser.getboolean('options', 'auto-tag', fallback=False)
-        self.auto_commit = self.parser.getboolean('options', 'auto-commit', fallback=False)
-        self.auto_push = self.parser.getboolean('options', 'auto-push', fallback=False)
-        self.signature = self.parser.getboolean('options', 'signature', fallback=False)
-
-        o = 'auto_tag={} auto_commit={} auto_push={} signature={}'.format(
-            self.auto_tag,
-            self.auto_commit,
-            self.auto_push,
-            self.signature
-        )
-        logger.debug(f'Options parsed.  {o}')
-
-        # We need to verify sections are there, especially before we blindly remove
+        # OPTIONS - log file setup
+        self.log_to_disk = self.parser.getboolean('options', 'log_to_disk', fallback=False)
+        self.log_file = self.parser.get('options', 'log_file', fallback='ican.log')
+        if self.log_to_disk:
+            setup_file_handler(self.log_file)
 
         self.parse_source_files()
+        self.parse_pipelines()
+        self.parse_aliases()
 
-        return None
+        return
+
+    def parse_aliases(self):
+        # aliases
+        if not self.parser.has_section('aliases'):
+            return
+
+        for alias, built_in in self.parser.items('aliases'):
+            cmd_with_args = built_in.strip().split(' ')
+            self.aliases[alias] = cmd_with_args
+        return
+
+    def parse_pipelines(self):
+        # Pipelines
+        for s in self.parser.sections():
+            if not s.startswith('pipeline:'):
+                # Not interested in this section
+                continue
+
+            label = s.split(':')[1].strip().lower()
+            logger.debug(f'parsing {label.upper()} pipeline')
+            list_tuples = self.parser.items(s)
+
+            pl = PipeLine(label=label, steps=list_tuples)
+            self.pipelines[label] = pl
+
+        return
 
     def parse_source_files(self):
         # FILES TO WRITE
-        sections = self.parser.sections().copy()
-        sections.remove('version')
-        sections.remove('options')
-        for s in sections:
+        for s in self.parser.sections():
+            if not s.startswith('file:'):
+                # Not interested in this section
+                continue
+
+            label = s.split(':')[1].strip().lower()
             file = self.parser.get(s, 'file', fallback=None)
             variable = self.parser.get(s, 'variable', fallback=None)
             style = self.parser.get(s, 'style', fallback='semantic')
             regex = self.parser.get(s, 'regex', fallback=None)
 
             # Instead of raising exp, we can just look for more files
-            if file is None :
-                logger.debug(f'Skipping {s}, missing file reference')
+            if file is None:
+                logger.debug(f'skipping source - missing file ({label})')
                 continue
             elif variable is None and regex is None:
-                logger.debug(f'Skipping {s}, found no variable or regex config')
+                logger.debug(f'skipping source - missing variable/regex')
                 continue
 
+            logger.debug(f'parsing version file {label.upper()}[{file}]')
+
             # Case with *.py for all python files
             if '*' in file:
                 files = self.search_for_files(file)
-                for f in files:
-                    u = SourceCode(
-                        self,
-                        f,
-                        style=style,
-                        variable=variable,
-                        regex=regex
-                    )
-                    self.source_files.append(u)
-            # This is the normal case, 1 file per section
             else:
+                files = [file]
+            for f in files:
                 u = SourceCode(
-                    self,
-                    file,
+                    label,
+                    f,
                     style=style,
                     variable=variable,
                     regex=regex
                 )
                 self.source_files.append(u)
 
     def search_for_files(self, f):
         """
         First we look in current_dir + all subdirs
         """
 
-        logger.debug(f'Config parser searching for: {f}')
+        logger.debug(f'* CONFIG: searching for - {f}')
 
         root = self.path
         #self.debug(f'Searching for {f} in dir {root}')
         matches = [x for x in Path(root).rglob(f)]
         if len(matches) > 0:
-            logger.debug(f'Config parser found: {len(matches)} files')
+            logger.debug(f'found: {len(matches)} files')
             return matches
         return None
```

### Comparing `ican-0.1.6/ican/emojis.py` & `ican-0.1.9/ican/emojis.py`

 * *Files identical despite different names*

### Comparing `ican-0.1.6/ican/exceptions.py` & `ican-0.1.9/ican/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,14 @@
     INVALID_CONFIG = 2
     CONFIG_WRITE_ERROR = 3
     NO_CURRENT_VERSION = 4
     
     GIT_UNUSABLE = 10
     GIT_ROOT_ERROR = 11
     GIT_DESCRIBE_ERROR = 12
-    GIT_ADD_ERROR = 13
-    GIT_COMMIT_ERROR = 14
-    GIT_TAG_ERROR = 15
-    GIT_PUSH_ERROR = 16
-    GPG_SIGNING_ERROR = 17
     
     VERSION_PARSE_ERROR = 20
     VERSION_METADATA_ERROR = 21
     VERSION_BUMP_ERROR = 22
     VERSION_PEP440_ERROR = 23
     VERSION_GIT_ERROR = 24
 
@@ -98,29 +93,14 @@
 
 class GitRootError(IcanException):
     exit_code = ExitCode.GIT_ROOT_ERROR
 
 class GitDescribeError(IcanException):
     exit_code = ExitCode.GIT_DESCRIBE_ERROR
 
-class GitAddError(IcanException):
-    exit_code = ExitCode.GIT_ADD_ERROR
-
-class GitCommitError(IcanException):
-    exit_code = ExitCode.GIT_COMMIT_ERROR
-
-class GitTagError(IcanException):
-    exit_code = ExitCode.GIT_TAG_ERROR
-
-class GitPushError(IcanException):
-    exit_code = ExitCode.GIT_PUSH_ERROR
-
-class GPGSigningError(IcanException):
-    exit_code = ExitCode.GPG_SIGNING_ERROR
-
 ########################
 
 class VersionParseError(IcanException):
     exit_code = ExitCode.VERSION_PARSE_ERROR
 
 class VersionMetadataError(IcanException):
     exit_code = ExitCode.VERSION_METADATA_ERROR
```

### Comparing `ican-0.1.6/ican/ican.py` & `ican-0.1.9/ican/ican.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
 
-from . import __version__
 from .config import Config
 from .version import Version
 from .git import Git
 from .log import logger
+from .log import ok_to_write
 from .emojis import rnd_good_emoji
 from .exceptions import GitDescribeError
 
 #######################################
 #
 #   Bump Class
 #
@@ -19,101 +19,91 @@
 
 
 class Ican(object):
     """
     Object which will orchestrate entire program
     """
 
-    @property
-    def dry_run(self):
-        if self.dryrun:
-            logger.info('Skipping file write due to --dry-run')
-            return True
-        return False
-
-    def __init__(self, dry_run=None, init=False):
-        self.dryrun = dry_run
-
+    def __init__(self, init=False):
         self.version = None
         self.git = None
         self.config = None
 
-        logger.debug(f'   ---=== Welcome to ican v{__version__} ===---')
         logger.debug('Verbose output selected.')
-        if self.dryrun:
-            logger.info('--dry-run detected.  No files will be written to.')
-        
+
         # Git init - Do this early incase we need git.root
-        logger.debug('Investigating a project git repo.')
         self.git = Git()
 
         # Create config obj.  If init, set defaults.
         # Otherwise, search for existing config file.
-        self.config = Config(parent=self)
+        self.config = Config(self.git.root)
         if init:
             self.config.init()
         else:
             self.config.search_for_config()
 
         # Now we have default or existing config, we can parse
         self.config.parse()
 
         # Now config is parsed.  We can parse from config
         self.version = Version.parse(self.config.current_version)
-        logger.debug(f'Parsed version {self.version.semantic} from config')
+        logger.debug(f'discovered {self.version.semantic} @ CONFIG.version')
 
         try:
             self.version._git_metadata = self.git.describe()
         except GitDescribeError as e:
             logger.info(e)
             logger.info('Git style versions will be disabled.')
             logger.info('Possibly this is a new repo with no tags.')
             self.git.disable()
-            
+
         else:
-            logger.debug(f'Set git-version metadata: {self.version.git}')
+            logger.debug(f'discovered {self.version.git} @ GIT.version')
 
         return
 
     def show(self, style):
         """
         Show the <STYLE> version
         """
 
         v = getattr(self.version, style)
         if v is None:
-            return f'version style: {style} not available'
+            return f'version STYLE: {style} not available'
         return v
 
-
     def bump(self, part):
         """
         This is pretty much the full process
         """
 
-        logger.debug(f'Beginning bump of `{part}`...')
+        logger.debug(f'beginning bump of <{part.upper()}>')
 
         # Use the Version API to bump 'part'
         self.version.bump(part)
-        logger.debug(f'+ New value of {part}: {getattr(self.version, part)}')
+        logger.debug(
+            f'new value of <{part.upper()}> - {getattr(self.version, part)}'
+        )
 
+        # Update the user's files with new version
         for file in self.config.source_files:
             file.update(self.version)
 
-        # Write the new version to config file
-        self.config.persist_version(self.version.semantic)
-
         # Pipeline
         if self.version.new_release:
-            # The actual auto_commit and auto_tag
-            if self.config.auto_commit and not self.dry_run:
-                self.git.add()
-                self.git.commit(f'auto-commit triggered by version bump')
-
-            if self.config.auto_tag and not self.dry_run:
-                msg = f'auto-generated release: {self.version.semantic}'
-                self.git.tag(self.version.tag, self.config.signature, msg)
+            if self.config.pipelines.get('release'):
+                self.run_pipeline('release')
+
 
-            if self.config.auto_push and not self.dry_run:
-                self.git.push(self.version.tag)
+        # Once all else is successful, persist the new version
+        self.config.persist_version(self.version.semantic)
 
         return self
+
+    def run_pipeline(self, label):
+        logger.debug('RELEASE pipeline triggered')
+
+        pl = self.config.pipelines.get(label)
+        ctx = {}
+        ctx['tag'] = self.version.tag
+        ctx['msg'] = f'auto commit for {self.version.tag}.'
+        pl.run(ctx)
```

### Comparing `ican-0.1.6/ican/source.py` & `ican-0.1.9/ican/source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 """
 import re
 from pathlib import Path
 
 from .log import logger
+from .log import ok_to_write
 from . import exceptions
 from .exceptions import UserSuppliedRegexError
 from .exceptions import SourceCodeFileOpenError
 from .exceptions import SourceCodeFileMissing
 
 #######################################
 #
@@ -18,16 +19,16 @@
 #######################################
 
 
 class SourceCode(object):
 
     VARIABLE_RE = r"{{var}}\s*=\s*(?P<quote>[\'\"])(?P<version>.+)(?P=quote)"
 
-    def __init__(self, parent, file, style='semantic', variable=None, regex=None):
-        self.parent = parent
+    def __init__(self, label, file, style='semantic', variable=None, regex=None):
+        self.label = f'{label.upper()}[{file}]'
         self.file = Path(file)
         self.variable = variable
         self.style = style
         self.regex = regex
 
         self.updated = False
         self.valid = False
@@ -36,15 +37,15 @@
             raise SourceCodeFileMissing(
                 f'config references non existant file: {self.file}'
             )
         self.valid = True
 
         if variable is not None:
             self.regex = SourceCode.VARIABLE_RE.replace("{{var}}", variable)
-            logger.debug(f'user supplied variable to regex: {self.regex}')
+            logger.debug(f'regex generated for {variable}')
 
         if self.regex:
             try:
                 self.compiled = re.compile(self.regex)
             except Exception as e:
                 msg = f'Error compiling regex: {self.regex}'
                 raise UserSuppliedRegexError(msg)
@@ -67,15 +68,15 @@
         Returns:
             True if all is successful.  Filename will be updated
             with new version if found.
         """
 
         self.new_version = getattr(version, self.style)
         logger.debug(
-            f'Updating `{self.file}` with {self.new_version}'
+            f'{self.label} - updating to {self.new_version}'
         )
 
         try:
             f = self.file.open('r+')
         except OSError:
             raise SourceCodeFileOpenError(f'Error opening {self.file}')
 
@@ -84,20 +85,20 @@
             original = f.read()
 
             # Regex search
             updated, n = self.compiled.subn(self._replacement, original, count=1)
 
             # Check if we found a match or not
             if n == 0:
-                logger.debug(f'No match found in {self.file}.')
+                logger.debug(f'{self.label} - NO MATCHES!')
                 return
-            logger.debug(f'Found {n} matches.')
+            logger.debug(f'{self.label} - found {n} matches')
 
             # Write the updated file
-            if not self.parent.parent.dry_run:
+            if ok_to_write():
                 f.seek(0)
                 f.write(updated)
                 f.truncate()
 
         self.updated = True
-        logger.debug(f'Rewrite of file `{self.file}` complete.')
+        logger.debug(f'{self.label} - update COMPLETE')
         return True
```

### Comparing `ican-0.1.6/ican/utils.py` & `ican-0.1.9/ican/utils.py`

 * *Files identical despite different names*

### Comparing `ican-0.1.6/ican/version.py` & `ican-0.1.9/ican/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import re
 from types import SimpleNamespace
+from .log import ok_to_write
 from .log import logger
 
+
+__version__ = '0.2'
+
+
 #######################################
 #
 #   Version Class
 #
 #######################################
 
 
@@ -306,15 +311,15 @@
     @property
     def new_release(self):
         if not self._frozen:
             return None
         
         part = self._frozen.part
         if part in ['major', 'minor', 'patch']:
-            logger.debug('release will trigger deployment pipeline')
+            logger.debug('* VERSION: release pipeline will trigger')
             return True
         return False
 
     @new_release.setter
     def new_release(self, value):
         raise AttributeError("new_release is readonly")
```

