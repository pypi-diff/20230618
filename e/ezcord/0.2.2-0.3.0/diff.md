# Comparing `tmp/ezcord-0.2.2.tar.gz` & `tmp/ezcord-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.2.2.tar", last modified: Thu Jun  1 16:03:30 2023, max compression
+gzip compressed data, was "ezcord-0.3.0.tar", last modified: Sun Jun 18 19:32:45 2023, max compression
```

## Comparing `ezcord-0.2.2.tar` & `ezcord-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.886761 ezcord-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 16:03:19.000000 ezcord-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 16:03:19.000000 ezcord-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-01 16:03:30.886761 ezcord-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-01 16:03:19.000000 ezcord-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 16:03:19.000000 ezcord-0.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 16:03:19.000000 ezcord-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 16:03:19.000000 ezcord-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 16:03:19.000000 ezcord-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:03:30.886761 ezcord-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.878760 ezcord-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.886761 ezcord-0.2.2/src/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 19:32:35.000000 ezcord-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 19:32:35.000000 ezcord-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-18 19:32:45.111140 ezcord-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-18 19:32:35.000000 ezcord-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 19:32:35.000000 ezcord-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 19:32:35.000000 ezcord-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-18 19:32:35.000000 ezcord-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 19:32:35.000000 ezcord-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 19:32:45.115140 ezcord-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.107140 ezcord-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/cogs/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.2.2/LICENSE` & `ezcord-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/PKG-INFO` & `ezcord-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.2.2
+Version: 0.3.0
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.2.2/README.md` & `ezcord-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/pyproject.toml` & `ezcord-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/bot.py` & `ezcord-0.3.0/src/ezcord/bot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
+import asyncio
 import logging
 import os
 from pathlib import Path
 from typing import Any
 
 import aiohttp
 import discord
 from discord.ext import bridge, commands
 
 from .emb import error as error_emb
-from .enums import CogLog, ReadyEvent
+from .enums import CogLog, HelpStyle, ReadyEvent
 from .logs import DEFAULT_LOG, custom_log, set_log
 from .times import dc_timestamp
 
 from .internal import (  # isort: skip
     READY_TITLE,
     load_lang,
     print_custom_ready,
@@ -84,27 +85,32 @@
 
         if debug:
             self.logger = set_log(DEFAULT_LOG)
         else:
             self.logger = logging.getLogger(DEFAULT_LOG)
             self.logger.addHandler(logging.NullHandler())
 
+        self.help: dict = {}
         self.error_handler = error_handler
         self.error_webhook_url = error_webhook_url
         self.ignored_errors = ignored_errors or []
         self.full_error_traceback = full_error_traceback
         load_lang(language)
         set_lang(language) if language != {} else set_lang("en")
 
         if error_handler or error_webhook_url:
             self.add_listener(self._error_event, "on_application_command_error")
 
         self.ready_event = ready_event
         if ready_event:
             self.add_listener(self._ready_event, "on_ready")
+        self.add_listener(self._check_cog_groups, "on_ready")
+
+        self.ready_event_adds: dict = {}
+        self.ready_event_removes: list[int | str] = []
 
     def _send_cog_log(
         self,
         custom_log_level: str | None,
         log_format: str,
         color: str | None,
     ):
@@ -229,14 +235,47 @@
                             )
 
                     self._cog_count_log(custom_log_level, log, loaded_dir_cogs, log_color, dirname)
                     loaded_cogs += loaded_dir_cogs
 
         self._cog_count_log(custom_log_level, log, loaded_cogs, log_color)
 
+    def add_ready_info(
+        self,
+        name: str,
+        value: str | int,
+        position: int | None = None,
+        color: str | None = None,
+    ):
+        """Adds an information to the ``on_ready`` message.
+
+        Parameters
+        ----------
+        name:
+            The name of the info to add. If this name already exists, the info will be updated.
+        value:
+            The value of the info.
+        position:
+            The position of the info. If this is ``None``, the info will be added at the end.
+        color:
+            The color of the info. If this is ``None``, a default color will be used.
+        """
+        self.ready_event_adds[name] = {"value": value, "position": position, "color": color}
+
+    def remove_ready_info(self, *elements: str | int):
+        """Removes an information from the ``on_ready`` message.
+
+        Parameters
+        ----------
+        *elements:
+            The names or positions of the infos to remove.
+        """
+        for element in elements:
+            self.ready_event_removes.append(element)
+
     def ready(
         self,
         *,
         title: str = READY_TITLE,
         style: ReadyEvent = ReadyEvent.default,
         default_info: bool = True,
         new_info: dict | None = None,
@@ -249,27 +288,61 @@
         title:
             The title of the ready message.
         style:
             The style of the ready message. Defaults to :attr:`.ReadyEvent.default`.
         default_info:
             Whether to include the default information. Defaults to ``True``.
         new_info:
-            A dictionary of information to include in the ready message.
+            A dictionary of additional information to include in the ready message.
             Defaults to ``None``.
+
+            .. note::
+                Information can also be added with :meth:`.add_ready_info` and removed with
+                :meth:`.remove_ready_info`.
         colors:
             A list of colors to use for the ready message. If no colors are given,
             default colors will be used.
 
             Colors can only be used with :attr:`.ReadyEvent.box_colorful` and all table styles.
         """
-        print_custom_ready(self, title, style, default_info, new_info, colors)
+        modifications = self.ready_event_adds, self.ready_event_removes
+        print_custom_ready(self, title, modifications, style, default_info, new_info, colors)
 
     async def _ready_event(self):
         """Prints the bot's information when it's ready."""
-        print_ready(self, self.ready_event)
+        if len(self.ready_event_adds) > 0 or len(self.ready_event_removes) > 0:
+            await asyncio.sleep(0.5)
+
+        modifications = self.ready_event_adds, self.ready_event_removes
+        print_ready(self, self.ready_event, modifications=modifications)
+
+    async def _check_cog_groups(self):
+        """Checks if all cog groups are valid."""
+        for cog in self.cogs.values():
+            if hasattr(cog, "group") and cog.group:
+                if cog.group not in self.cogs.keys():
+                    self.logger.warning(
+                        f"The cog group '{cog.group}' for cog '{cog.qualified_name}' does not exist."
+                    )
+
+    # This requires the following PR to be in a stable Pycord release:
+    # https://github.com/Pycord-Development/pycord/pull/1945
+    #
+    # async def on_error(
+    #     self, event_method: str, exception: Exception, *args: Any, **kwargs: Any
+    # ) -> None:
+    #     """This overrides the default ``on_error`` event to send an error webhook."""
+    #     description = format_error(exception)
+    #     webhook_sent = await self._send_error_webhook(description)
+    #
+    #     self.logger.exception(
+    #         f"Error while executing **{event_method}**",
+    #         exc_info=exception,
+    #         extra={"webhook_sent": webhook_sent},
+    #     )
 
     async def _error_event(self, ctx: discord.ApplicationContext, error: discord.DiscordException):
         """The event that handles application command errors."""
         if type(error) in self.ignored_errors:
             return
 
         if isinstance(error, commands.CommandOnCooldown):
@@ -335,14 +408,46 @@
                     "Please check if the URL is correct."
                 )
             else:
                 webhook_sent = True
 
         return webhook_sent
 
+    def add_help_command(
+        self,
+        *,
+        style: HelpStyle = HelpStyle.embed_description,
+        embed: discord.Embed | None = None,
+        show_categories: bool = True,
+        ephemeral: bool = True,
+    ):
+        """Add a help command that uses a select menu to group commands by cogs.
+
+        If you use :class:`Cog`, you can pass in emojis to use for the select menu.
+
+        Parameters
+        ----------
+        style:
+            The style to use for the help command. Defaults to :attr:`.HelpStyle.default`.
+        embed:
+            The embed to use for the help command. If this is ``None``, a default
+            embed will be used.
+        show_categories:
+            Whether to display the categories of the help command front page. Defaults to ``True``.
+        ephemeral:
+            Whether the help command should be ephemeral. Defaults to ``False``.
+        """
+        self.load_extension(f".cogs.help", package="src.ezcord")
+        self.help = {
+            "style": style,
+            "embed": embed,
+            "show_categories": show_categories,
+            "ephemeral": ephemeral,
+        }
+
 
 class PrefixBot(Bot, commands.Bot):
     """A subclass of :class:`discord.ext.commands.Bot` that implements the :class:`Bot` class.
 
     This class can be used if you want to use EzCord with prefix commands.
     """
 
@@ -354,7 +459,31 @@
     """A subclass of :class:`discord.ext.bridge.Bot` that implements the :class:`Bot` class.
 
     This class can be used if you want to use EzCord with bridge commands.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+
+
+class _CogMeta(discord.cog.CogMeta):
+    """A metaclass for cogs that adds an ``emoji`` attribute."""
+
+    def __new__(cls, *args, **kwargs) -> discord.cog.CogMeta:
+        name, bases, attrs = args
+        attrs["emoji"] = kwargs.pop("emoji", None)
+        attrs["group"] = kwargs.pop("group", None)
+        attrs["hidden"] = kwargs.pop("hidden", False)
+        return super().__new__(cls, *args, **kwargs)
+
+
+class Cog(commands.Cog, metaclass=_CogMeta):
+    """This can be used as a base class for all cogs.
+
+    Parameters
+    ----------
+    bot:
+        The bot instance.
+    """
+
+    def __init__(self, bot: Bot) -> None:
+        self.bot = bot
```

### Comparing `ezcord-0.2.2/src/ezcord/components.py` & `ezcord-0.3.0/src/ezcord/components.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/emb.py` & `ezcord-0.3.0/src/ezcord/emb.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/enums.py` & `ezcord-0.3.0/src/ezcord/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,14 +30,29 @@
     time = "%H:%M:%S"
     default = "%H:%M:%S"
 
     def __str__(self):
         return self.value
 
 
+class HelpStyle(Enum):
+    """Presets for the help command used in :func:`.add_help_command`."""
+
+    embed_fields = 0
+    embed_description = 1
+    markdown = 2
+    codeblocks = 3
+    codeblocks_inline = 4
+
+    default = embed_fields
+
+    def __str__(self):
+        return self.name
+
+
 class CogLog(str, Enum):
     """Presets for log messages in :meth:`.Bot.load_cogs`.
 
     - ``{cog}`` is the name of the cog.
     - ``{directory}`` is the directory where a cog was loaded from.
     - ``{path}`` is the path of a cog.
     - ``{sum}`` is the amount of cogs that were loaded.
```

### Comparing `ezcord-0.2.2/src/ezcord/internal/colors.py` & `ezcord-0.3.0/src/ezcord/internal/colors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/internal/embed_templates.py` & `ezcord-0.3.0/src/ezcord/internal/embed_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,19 @@
         if name in _TEMPLATES.keys():
             save_embeds()
             return load_embed()
         else:
             raise ValueError(f"Embed template '{name}' not found.")
 
 
+def format_error(error: Exception) -> str:
+    txt = "".join(traceback.format_exception(type(error), error, error.__traceback__))
+    return f"\n```py\n{txt[:3500]}```"
+
+
 def get_error_text(
     ctx: discord.ApplicationContext | discord.Interaction,
     error: Exception,
     item: discord.ui.Item | discord.ui.Modal | None = None,
 ):
     """Get the description for the webhook embed."""
     if item:
@@ -74,13 +79,12 @@
         elif ctx.type == discord.InteractionType.modal_submit:
             location = f"- **Modal:** {type(item).__name__}"
         else:
             location = f"- **Select Menu:** {type(item.view).__name__}"
     else:
         location = f"- **Command:** /{ctx.command.qualified_name}"
 
-    error_txt = "".join(traceback.format_exception(type(error), error, error.__traceback__))
     guild_txt = f"\n- **Guild:** {ctx.guild.name} - `{ctx.guild.id}`" if ctx.guild else ""
     user_txt = f"\n- **User:** {ctx.user} - `{ctx.user.id}`" if ctx.user else ""
 
-    description = location + guild_txt + user_txt + f"\n```py\n{error_txt[:3500]}```"
+    description = location + guild_txt + user_txt + format_error(error)
     return description
```

### Comparing `ezcord-0.2.2/src/ezcord/internal/language/languages.py` & `ezcord-0.3.0/src/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/internal/ready_style.py` & `ezcord-0.3.0/src/ezcord/internal/ready_style.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utility functions for the ready event."""
 
 from __future__ import annotations
 
+from collections import OrderedDict
 from itertools import cycle, islice
 
 import discord
 from colorama import Fore
 
 from .. import __version__
 from ..enums import ReadyEvent
@@ -31,58 +32,97 @@
     TL, TR, BL, BR, H, V, M, L, R, T, B = "╔", "╗", "╚", "╝", "═", "║", "╬", "╠", "╣", "╦", "╩"
 
 
 READY_TITLE: str = f"Bot is online with EzCord {__version__}"
 DEFAULT_COLORS: list[str] = [Fore.CYAN, Fore.MAGENTA, Fore.YELLOW, Fore.GREEN, Fore.BLUE, Fore.RED]
 
 
-def get_default_info(bot: discord.Bot):
+def get_default_info(bot: discord.Bot) -> list[tuple[str, str]]:
     cmds = [
         cmd for cmd in bot.walk_application_commands() if type(cmd) != discord.SlashCommandGroup
     ]
 
-    infos = {
-        "Bot": f"{bot.user}",
-        "ID": f"{bot.user.id}",
-        "Pycord": discord.__version__,
-        "Commands": f"{len(cmds):,}",
-        "Guilds": f"{len(bot.guilds):,}",
-        "Latency": f"{round(bot.latency * 1000):,}ms",
-    }
+    return [
+        ("Bot", f"{bot.user}"),
+        ("ID", f"{bot.user.id}"),
+        ("Pycord", discord.__version__),
+        ("Commands", f"{len(cmds):,}"),
+        ("Guilds", f"{len(bot.guilds):,}"),
+        ("Latency", f"{round(bot.latency * 1000):,}ms"),
+    ]
+
+
+def modify_info(
+    bot: discord.Bot, modifications: tuple, custom_color_list: list[str] | None = None
+) -> tuple[list[tuple[str, str]], list[str]]:
+    """Add or remove information from the default ready event."""
+
+    infos = get_default_info(bot)
+    additions, deletions = modifications
+    colors = custom_color_list or DEFAULT_COLORS
+
+    for key, settings in additions.items():
+        value, position, color = settings["value"], settings["position"], settings["color"]
+
+        if position is None:
+            position = len(infos)
+
+        infos.insert(position, (key, str(value)))
+        colors.insert(position, get_escape_code(color))
+
+    for key in deletions:
+        if isinstance(key, int):
+            try:
+                infos.pop(key)
+            except IndexError:
+                log.warning(f"Index {key} does not exist and could not be removed.")
+        else:
+            infos = [info for info in infos if info[0] != key]
 
-    return infos
+    return infos, colors
 
 
 def print_custom_ready(
     bot: discord.Bot,
     title: str,
+    modifications: tuple,
     style: ReadyEvent = ReadyEvent.default,
     default_info: bool = True,
     new_info: dict | None = None,
     colors: list[str] | None = None,
 ):
-    infos = get_default_info(bot) if default_info else {}
     colors = list(map(get_escape_code, colors or DEFAULT_COLORS))
 
+    if default_info:
+        infos, colors = modify_info(bot, modifications, colors)
+    else:
+        infos = get_default_info(bot)
+
     if new_info:
         for key, value in new_info.items():
-            infos[str(key)] = str(value)
+            infos.append((str(key), str(value)))
 
-    print_ready(bot, style, infos, title, colors)
+    print_ready(bot, style, OrderedDict(infos), title, colors)
 
 
 def print_ready(
     bot: discord.Bot,
     style: ReadyEvent,
-    infos: dict[str, str] | None = None,
+    infos: OrderedDict | None = None,
     title: str = READY_TITLE,
     colors: list[str] | None = None,
+    *,
+    modifications: tuple | None = None,
 ):
-    infos = infos or get_default_info(bot)
     colors = colors or DEFAULT_COLORS
+    infos = infos or OrderedDict(get_default_info(bot))
+
+    if modifications:
+        infos_list, colors = modify_info(bot, modifications, colors)
+        infos = OrderedDict(infos_list)
 
     info_count = len(infos.items())
     colors = list(islice(cycle(colors), info_count))
 
     colon_infos = {key + ":": value for key, value in infos.items()}
 
     style_cls = Style()
```

### Comparing `ezcord-0.2.2/src/ezcord/internal/translation.py` & `ezcord-0.3.0/src/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/logs.py` & `ezcord-0.3.0/src/ezcord/logs.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/times.py` & `ezcord-0.3.0/src/ezcord/times.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord/utils.py` & `ezcord-0.3.0/src/ezcord/utils.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.2/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.3.0/src/ezcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.2.2
+Version: 0.3.0
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.2.2/src/ezcord.egg-info/SOURCES.txt` & `ezcord-0.3.0/src/ezcord.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 docs/requirements.txt
 src/ezcord/__init__.py
 src/ezcord/bot.py
 src/ezcord/components.py
 src/ezcord/emb.py
 src/ezcord/enums.py
 src/ezcord/logs.py
+src/ezcord/sql.py
 src/ezcord/times.py
 src/ezcord/utils.py
 src/ezcord.egg-info/PKG-INFO
 src/ezcord.egg-info/SOURCES.txt
 src/ezcord.egg-info/dependency_links.txt
 src/ezcord.egg-info/requires.txt
 src/ezcord.egg-info/top_level.txt
+src/ezcord/cogs/help.py
 src/ezcord/internal/__init__.py
 src/ezcord/internal/colors.py
 src/ezcord/internal/embed_templates.py
 src/ezcord/internal/funcutils.py
 src/ezcord/internal/ready_style.py
 src/ezcord/internal/translation.py
 src/ezcord/internal/language/de.json
```

