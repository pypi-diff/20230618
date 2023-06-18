# Comparing `tmp/pymino-1.1.9.9.tar.gz` & `tmp/pymino-1.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\subb\pymino\dist\.tmp-vtx59tf_\pymino-1.1.9.9.tar", last modified: Sat Jun 17 16:18:12 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\seb\pymino\dist\.tmp-9f8s1jm8\pymino-1.2.1.1.tar", last modified: Sun Jun 18 20:07:20 2023, max compression
```

## Comparing `pymino-1.1.9.9.tar` & `pymino-1.2.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.714582 pymino-1.1.9.9/
--rw-rw-rw-   0        0        0     1085 2023-06-17 16:15:11.000000 pymino-1.1.9.9/LICENSE
--rw-rw-rw-   0        0        0     7298 2023-06-17 16:18:12.715079 pymino-1.1.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     6580 2023-06-17 16:17:57.000000 pymino-1.1.9.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.642246 pymino-1.1.9.9/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-17 16:16:10.000000 pymino-1.1.9.9/pymino/__init__.py
--rw-rw-rw-   0        0        0     7986 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30208 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/bot.py
--rw-rw-rw-   0        0        0    65900 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.680357 pymino-1.1.9.9/pymino/ext/
--rw-rw-rw-   0        0        0      498 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    13871 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/account.py
--rw-rw-rw-   0        0        0   306780 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18079 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24095 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   305400 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/console.py
--rw-rw-rw-   0        0        0    42101 2023-06-17 16:16:22.000000 pymino-1.1.9.9/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.702678 pymino-1.1.9.9/pymino/ext/entities/
--rw-rw-rw-   0        0        0      355 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     1670 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    20322 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15638 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1847 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0     6185 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6729 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.713615 pymino-1.1.9.9/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6396 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10274 2023-06-17 16:15:11.000000 pymino-1.1.9.9/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:18:12.661589 pymino-1.1.9.9/pymino.egg-info/
--rw-rw-rw-   0        0        0     7298 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1433 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 16:18:12.000000 pymino-1.1.9.9/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-17 16:18:12.717062 pymino-1.1.9.9/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-06-17 16:15:11.000000 pymino-1.1.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.560312 pymino-1.2.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-06-18 20:03:12.000000 pymino-1.2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7426 2023-06-18 20:07:20.560312 pymino-1.2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6708 2023-06-18 20:03:12.000000 pymino-1.2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.492857 pymino-1.2.1.1/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-18 20:05:18.000000 pymino-1.2.1.1/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7986 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30208 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/bot.py
+-rw-rw-rw-   0        0        0    65900 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.526088 pymino-1.2.1.1/pymino/ext/
+-rw-rw-rw-   0        0        0      498 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    13871 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   328859 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18079 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24095 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   327444 2023-06-18 20:06:03.000000 pymino-1.2.1.1/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    42101 2023-06-18 20:06:09.000000 pymino-1.2.1.1/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.546920 pymino-1.2.1.1/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      355 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     1670 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20322 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15638 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0     6185 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-06-18 20:06:18.000000 pymino-1.2.1.1/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6729 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.558825 pymino-1.2.1.1/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6396 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10274 2023-06-18 20:03:12.000000 pymino-1.2.1.1/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:07:20.507765 pymino-1.2.1.1/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7426 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1433 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 20:07:20.000000 pymino-1.2.1.1/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-18 20:07:20.562296 pymino-1.2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-06-18 20:03:12.000000 pymino-1.2.1.1/setup.py
```

### Comparing `pymino-1.1.9.9/LICENSE` & `pymino-1.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/PKG-INFO` & `pymino-1.2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.9
+Version: 1.2.1.1
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
     <a href="https://discord.gg/JMJpzpsMNJ"><img src="https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server" alt="Discord"></a>
     <a href="https://libraries.io/github/forevercynical/pymino"><img src="https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet" alt="Libraries.io dependency status for GitHub repo"></a>
     <a href="https://github.com/forevercynical/pymino/commits/main"><img src="https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet" alt="GitHub last commit"></a>
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
-  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
+  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
     <h3 style="color: red;"><strong> WARNING </strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
@@ -98,32 +98,37 @@
 >>> from pymino import Bot
 >>> from pymino.ext import *
 
 >>> # Initialize the bot
 >>> bot = Bot(
 ...     command_prefix="!",
 ...     community_id=00000000,
-... ) # You can set proxies and device_id here
+...     console_enabled=True,
+...     device_id=None,
+...     intents=True,
+...     online_status=True,
+...     proxy="http://127.0.0.1:8080" # Must be a string.
+... ) 
 
 >>> # The on_ready event is called when the bot has logged in.
 >>> @bot.on_ready()
 ... def ready():
 ...     print(f"{bot.profile.username} has logged in!")
 
 >>> # The on_text_message event is called when a message is received.
 >>> @bot.on_text_message()
-... def message(ctx: Context):
-...     print(f"{ctx.author.username}: {ctx.message.content}")
-...     if ctx.message.content.startswith("hi"):
+... def message(ctx: Context, member: Member, message: str):
+...     print(f"{member.username}: {message}")
+...     if message.startswith("hi"):
 ...         ctx.reply("Hello!")
 
 >>> # The on_member_join event is called when a member joins a chat.
 >>> @bot.on_member_join()
-... def join(ctx: Context):
-...     ctx.reply(f"Welcome to the chat, {ctx.author.username}!")
+... def join(ctx: Context, member: Member):
+...     ctx.reply(f"Welcome to the chat, {member.username}!")
 
 >>> # The on_member_leave event is called when a member leaves a chat.
 >>> @bot.on_member_leave()
 ... def leave(ctx: Context):
 ...     ctx.reply(f"Goodbye!")
 
 >>> # This is how you create a command.
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.9 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.1 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
-  Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous
-                                   library.
+    Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
   violating the Amino Apps' Terms of Service. This could lead to your account
   being suspended or permanently banned. Please use Pymino responsibly and at
                                 your own risk.
  Understand that the developers and maintainers of Pymino are not responsible
  for any actions taken against your account as a result of using this client.
@@ -68,32 +67,37 @@
 >>> from pymino import Bot
 >>> from pymino.ext import *
 
 >>> # Initialize the bot
 >>> bot = Bot(
 ...     command_prefix="!",
 ...     community_id=00000000,
-... ) # You can set proxies and device_id here
+...     console_enabled=True,
+...     device_id=None,
+...     intents=True,
+...     online_status=True,
+...     proxy="http://127.0.0.1:8080" # Must be a string.
+... )
 
 >>> # The on_ready event is called when the bot has logged in.
 >>> @bot.on_ready()
 ... def ready():
 ...     print(f"{bot.profile.username} has logged in!")
 
 >>> # The on_text_message event is called when a message is received.
 >>> @bot.on_text_message()
-... def message(ctx: Context):
-...     print(f"{ctx.author.username}: {ctx.message.content}")
-...     if ctx.message.content.startswith("hi"):
+... def message(ctx: Context, member: Member, message: str):
+...     print(f"{member.username}: {message}")
+...     if message.startswith("hi"):
 ...         ctx.reply("Hello!")
 
 >>> # The on_member_join event is called when a member joins a chat.
 >>> @bot.on_member_join()
-... def join(ctx: Context):
-...     ctx.reply(f"Welcome to the chat, {ctx.author.username}!")
+... def join(ctx: Context, member: Member):
+...     ctx.reply(f"Welcome to the chat, {member.username}!")
 
 >>> # The on_member_leave event is called when a member leaves a chat.
 >>> @bot.on_member_leave()
 ... def leave(ctx: Context):
 ...     ctx.reply(f"Goodbye!")
 
 >>> # This is how you create a command.
```

### Comparing `pymino-1.1.9.9/README.md` & `pymino-1.2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <a href="https://discord.gg/JMJpzpsMNJ"><img src="https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server" alt="Discord"></a>
     <a href="https://libraries.io/github/forevercynical/pymino"><img src="https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet" alt="Libraries.io dependency status for GitHub repo"></a>
     <a href="https://github.com/forevercynical/pymino/commits/main"><img src="https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet" alt="GitHub last commit"></a>
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
-  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
+  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
     <h3 style="color: red;"><strong> WARNING </strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
@@ -80,32 +80,37 @@
 >>> from pymino import Bot
 >>> from pymino.ext import *
 
 >>> # Initialize the bot
 >>> bot = Bot(
 ...     command_prefix="!",
 ...     community_id=00000000,
-... ) # You can set proxies and device_id here
+...     console_enabled=True,
+...     device_id=None,
+...     intents=True,
+...     online_status=True,
+...     proxy="http://127.0.0.1:8080" # Must be a string.
+... ) 
 
 >>> # The on_ready event is called when the bot has logged in.
 >>> @bot.on_ready()
 ... def ready():
 ...     print(f"{bot.profile.username} has logged in!")
 
 >>> # The on_text_message event is called when a message is received.
 >>> @bot.on_text_message()
-... def message(ctx: Context):
-...     print(f"{ctx.author.username}: {ctx.message.content}")
-...     if ctx.message.content.startswith("hi"):
+... def message(ctx: Context, member: Member, message: str):
+...     print(f"{member.username}: {message}")
+...     if message.startswith("hi"):
 ...         ctx.reply("Hello!")
 
 >>> # The on_member_join event is called when a member joins a chat.
 >>> @bot.on_member_join()
-... def join(ctx: Context):
-...     ctx.reply(f"Welcome to the chat, {ctx.author.username}!")
+... def join(ctx: Context, member: Member):
+...     ctx.reply(f"Welcome to the chat, {member.username}!")
 
 >>> # The on_member_leave event is called when a member leaves a chat.
 >>> @bot.on_member_leave()
 ... def leave(ctx: Context):
 ...     ctx.reply(f"Goodbye!")
 
 >>> # This is how you create a command.
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
-  Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous
-                                   library.
+    Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
   violating the Amino Apps' Terms of Service. This could lead to your account
   being suspended or permanently banned. Please use Pymino responsibly and at
                                 your own risk.
  Understand that the developers and maintainers of Pymino are not responsible
  for any actions taken against your account as a result of using this client.
@@ -58,32 +57,37 @@
 >>> from pymino import Bot
 >>> from pymino.ext import *
 
 >>> # Initialize the bot
 >>> bot = Bot(
 ...     command_prefix="!",
 ...     community_id=00000000,
-... ) # You can set proxies and device_id here
+...     console_enabled=True,
+...     device_id=None,
+...     intents=True,
+...     online_status=True,
+...     proxy="http://127.0.0.1:8080" # Must be a string.
+... )
 
 >>> # The on_ready event is called when the bot has logged in.
 >>> @bot.on_ready()
 ... def ready():
 ...     print(f"{bot.profile.username} has logged in!")
 
 >>> # The on_text_message event is called when a message is received.
 >>> @bot.on_text_message()
-... def message(ctx: Context):
-...     print(f"{ctx.author.username}: {ctx.message.content}")
-...     if ctx.message.content.startswith("hi"):
+... def message(ctx: Context, member: Member, message: str):
+...     print(f"{member.username}: {message}")
+...     if message.startswith("hi"):
 ...         ctx.reply("Hello!")
 
 >>> # The on_member_join event is called when a member joins a chat.
 >>> @bot.on_member_join()
-... def join(ctx: Context):
-...     ctx.reply(f"Welcome to the chat, {ctx.author.username}!")
+... def join(ctx: Context, member: Member):
+...     ctx.reply(f"Welcome to the chat, {member.username}!")
 
 >>> # The on_member_leave event is called when a member leaves a chat.
 >>> @bot.on_member_leave()
 ... def leave(ctx: Context):
 ...     ctx.reply(f"Goodbye!")
 
 >>> # This is how you create a command.
```

### Comparing `pymino-1.1.9.9/pymino/__init__.py` & `pymino-1.2.1.1/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.9.9'
+__version__ = '1.2.1.1'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.9.9/pymino/async_bot.py` & `pymino-1.2.1.1/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/bot.py` & `pymino-1.2.1.1/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/client.py` & `pymino-1.2.1.1/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/account.py` & `pymino-1.2.1.1/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/async_community.py` & `pymino-1.2.1.1/pymino/ext/async_community.py`

 * *Files 2% similar despite different names*

```diff
@@ -2392,68 +2392,101 @@
             await self.session.handler(
             method="DELETE",
             url=f"/x{self.community_id if comId is None else comId}/s/blog/{blogId}"
             ))
 
 
     @community
-    async def post_wiki(self, title: str, content: str, fansOnly: bool=False, comId: Union[str, int] = None) -> ApiResponse:
+    async def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None,fansOnly: bool=False, comId: Union[str, int] = None) -> ApiResponse:
         """
         Posts a new wiki article in the specified community.
 
         :param title: The title of the wiki article.
         :type title: str
         :param content: The content of the wiki article.
         :type content: str
-        :param fansOnly: Whether the wiki article should be for fans only. Must be either `True` or `False`.
-        :type fansOnly: bool
+        :param icon: The icon image file for the wiki article.
+        :type icon: str, optional
+        :param imageList: A list of image files to include in the wiki article.
+        :type imageList: list, optional
+        :param keywords: Keywords associated with the wiki article.
+        :type keywords: str, optional
+        :param backgroundColor: The background color for the wiki article.
+        :type backgroundColor: str, optional
+        :param fansOnly: Whether the wiki article should be for fans only. Default is False.
+        :type fansOnly: bool, optional
         :param comId: The ID of the community to post the wiki article in. If not provided, the current community ID is used.
-        :type comId: Union[str, int]
+        :type comId: Union[str, int], optional
         :return: An `ApiResponse` object representing the response from the server.
         :rtype: ApiResponse
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
-        The function sends a POST request to the API to post a new wiki article with the specified title, content, and fans-only setting.
+        This method allows the authenticated user to post a new wiki article in the specified community. The `title` parameter specifies
+        the title of the article, and the `content` parameter contains the content of the article.
+
+        Additional optional parameters can be provided to customize the wiki article. The `icon` parameter is used to specify an icon
+        image for the article, and the `imageList` parameter can be used to include multiple image files in the article.
+
+        The `keywords` parameter allows specifying keywords associated with the article, and the `backgroundColor` parameter sets the
+        background color of the article.
+
+        The `fansOnly` parameter determines whether the article should be accessible only to fans. By default, it is set to False.
+
+        The `comId` parameter is used to specify the ID of the community where the article should be posted. If not provided, the
+        current community ID is used.
 
         The response from the server is returned as an `ApiResponse` object.
-        
+
         `ApiResponse`:
 
-        - `message`: A message indicating whether the blog was successfully deleted.
+        - `message`: A message indicating the status of the wiki article posting.
         - `statuscode`: The status code of the API response.
         - `duration`: The duration of the API request.
         - `timestamp`: The timestamp of the API request.
-        - `mediaValue`: The media value of the deleted blog.
+        - `mediaValue`: The media value of the wiki article.
 
         **Example usage:**
 
         To post a new wiki article with the title "My First Wiki Article" and the content "This is my first wiki article.":
 
         >>> response = client.community.post_wiki(title="My First Wiki Article", content="This is my first wiki article.")
-        ... if response.statuscode == 0:
+        ... try:
         ...     print("Wiki article successfully posted!")
-        ... else:
+        ... except:
         ...     print("Wiki article could not be posted.")
         """
-        return ApiResponse(
-            await self.session.handler(
-            method="POST",
-            url=f"/x{self.community_id if comId is None else comId}/s/item",
-            data={
+        media = []
+
+        if imageList is not None:
+            media.append([100, await self.upload_media(open(image, "rb").read(), "image/jpg"), None] for image in imageList)
+
+
+        data = {
+            "mediaList": media,
+        }
+        if icon: data["icon"] = await self.upload_media(open(icon, "rb").read(), "image/jpg")
+        if keywords: data["keywords"] = keywords
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style":{"backgroundColor": backgroundColor if backgroundColor.startswith("#") else f"#{backgroundColor}"}}
+
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/item",
+            data = {
             "extensions": {"fansOnly": fansOnly},
             "content": content,
             "latitude": 0,
             "longitude": 0,
-            "title": title,
+            "label": title,
             "type": 0,
             "contentLanguage": "en",
             "eventSource": "GlobalComposeMenu",
             "timestamp": int(time() * 1000),
-            }))
+            }.update(data)))
 
 
     @community
     async def delete_wiki(self, wikiId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Deletes a wiki item with the given ID.
 
@@ -4784,50 +4817,46 @@
         :type title: Optional[str]
         :param message: The message to send to the users when inviting them to the chat. Defaults to `None`.
         :type message: Optional[str]
         :param content: The content of the chat. Defaults to `None`.
         :type content: Optional[str]
         :param comId: The ID of the community where the chat will be created. If not provided, the current community ID is used.
         :type comId: Optional[Union[str, int]]
-        :return: An `ApiResponse` object containing information about the request status.
-        :rtype: ApiResponse
+        :return: An `ChatThread` object containing information about the request status.
+        :rtype: ChatThread
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
-        `ApiResponse`: TODO: Update this to reflect the new return type.
-
         - `message`: A message indicating whether the chat was successfully created.
         - `statuscode`: The status code of the API response.
         - `duration`: The duration of the API request.
         - `timestamp`: The timestamp of the API request.
 
         **Example usage:**
 
         To create a new chat with users "0000-0000-0000-0000" and "1111-1111-1111-1111":
 
         >>> response = client.community.start_chat(userIds=["0000-0000-0000-0000", "1111-1111-1111-1111"], title="New chat", message="Join my chat!", content="Hello, world!")
-        ... if response.statuscode == 0:
+        ... if response.status_code == 200:
         ...     print("Chat created successfully!")
         ... else:
         ...     print("Failed to create chat.")
         """
-        return ChatThread(
-            await self.session.handler(
-            method="POST",
-            url=f"/x{self.community_id if comId is None else comId}/s/chat/thread",
-            data={
-                "title": title,
-                "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
-                "initialMessageContent": message,
-                "content": content,
-                "type": 0,
-                "publishToGlobal": 0,
-                "timestamp": int(time() * 1000)
-                }
-            ))
+        return ChatThread(await self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread",
+            data = {
+            "title": title,
+            "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
+            "initialMessageContent": message,
+            "content": content,
+            "type": 0,
+            "publishToGlobal": 0,
+            "timestamp": int(time() * 1000)
+            })).status
 
 
     @community
     async def invite_chat(self, chatId: str, userIds: Union[str, List[str]], comId: Union[str, int] = None) -> ApiResponse:
         """
         Invites one or more users to join a chat.
 
@@ -6641,8 +6670,436 @@
         ... print(community.new_members_today)
         ... print(community.total_members)
         """
         return CommunityStats(
             await self.session.handler(
                 method = "GET",
                 url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/stats"
+        ))
+    
+    @community
+    async def edit_blog(self, blogId: str,
+                  title: str = None,
+                  content: str = None,
+                  imageList: list = None,
+                  categoriesList: list = None,
+                  backgroundColor: str = None,
+                  fansOnly: bool = False,
+                  comId: str = None) -> CBlog:
+        """
+        Edits a blog post.
+
+        :param blogId: The ID of the blog post to edit.
+        :type blogId: str
+        :param title: The new title for the blog post.
+        :type title: str, optional
+        :param content: The new content for the blog post.
+        :type content: str, optional
+        :param imageList: A list of image file paths to add as media to the blog post.
+        :type imageList: list, optional
+        :param categoriesList: A list of category IDs to tag the blog post with.
+        :type categoriesList: list, optional
+        :param backgroundColor: The new background color for the blog post.
+        :type backgroundColor: str, optional
+        :param fansOnly: Specifies whether the blog post should be available to fans only. Default is False.
+        :type fansOnly: bool, optional
+        :param comId: The ID of the community where the blog post is located. If not provided, the current community ID will be used.
+        :type comId: str, optional
+        :return: The edited blog post as a `CBlog` object.
+        :rtype: CBlog
+
+        This method allows the user to edit a blog post. The `blogId` parameter specifies the ID of the blog post to edit.
+        The `title`, `content`, `imageList`, `categoriesList`, `backgroundColor`, `fansOnly`, and `comId` parameters are used to
+        update the corresponding properties of the blog post. Only the specified parameters will be updated.
+
+        The `imageList` parameter accepts a list of image file paths, which will be uploaded as media for the blog post.
+        The `categoriesList` parameter accepts a list of category IDs, which will be used to tag the blog post.
+
+        **Example usage:**
+
+        To edit a blog post with a new title, content, and image:
+
+        >>> response = client.edit_blog(
+        ...     blogId="blog123",
+        ...     title="New Title",
+        ...     content="New Content",
+        ...     imageList=["path/to/image1.jpg", "path/to/image2.jpg"]
+        ... )
+        ... if response.status == 200:
+        ...     print("Blog post edited successfully!")
+        ... else:
+        ...     print("Failed to edit blog post.")
+        """
+        media = []
+        if imageList is not None: media = [[100, await self.upload_media(open(image, "rb").read(), "image/jpg"), None] for image in imageList]
+        
+        data = {
+            "address": None,
+            "mediaList": media,
+            "latitude": 0,
+            "longitude": 0,
+            "eventSource": "PostDetailView",
+            "timestamp": int(time() * 1000)
+        }
+
+        if title: data["title"] = title
+        if content: data["content"] = content
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style0": {
+            "backgroundColor": backgroundColor if backgroundColor.startswith("#") else f"#{backgroundColor}"
+        }}
+        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
+        
+        return CBlog(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/blog/{blogId}",
+            data = data
+        ))
+    
+    @community
+    async def delete_notification(self, notificationId: str, comId: str = None) -> ApiResponse:
+        """
+        Deletes a notification.
+
+        :param notificationId: The ID of the notification to delete.
+        :type notificationId: str
+        :param comId: The ID of the community (optional). If not provided, the current community ID will be used.
+        :type comId: str, optional
+        :return: The response from the API after deleting the notification.
+        :rtype: ApiResponse
+
+        This method allows the authenticated user to delete a notification with the specified notification ID.
+        Optionally, you can provide the community ID (`comId`) if the notification belongs to a specific community.
+        If `comId` is not provided, the notification will be deleted from the current community.
+
+        The method sends a DELETE request to the API endpoint responsible for deleting the notification. The response
+        from the API is returned as an `ApiResponse` object.
+
+        **Example usage:**
+
+        To delete a notification with ID "notif123" from the current community:
+
+        >>> response = client.delete_notification(notificationId="notif123")
+        >>> try:
+        ...     print("Notification deleted successfully!")
+        ... except:
+        ...     print("Failed to delete notification.")
+        """
+        return ApiResponse(await self.session.handler(
+            method = "DELETE",
+            url = f"/x{comId or self.community_id}/s/notification/{notificationId}"
+        ))
+    
+    @community
+    async def flag(self,
+             reason: str,
+             flagType: int,
+             userId: str = None,
+             blogId: str = None,
+             wikiId: str = None,
+             asGuest: bool = False,
+             comId: str = None) -> ApiResponse:
+        """
+        Flags content in the community.
+
+        :param reason: The reason for flagging the content.
+        :type reason: str
+        :param flagType: The type of flag. (0: User, 1: Blog, 2: Wiki)
+        :type flagType: int
+        :param userId: The ID of the user to flag. Required if flagType is 0.
+        :type userId: str, optional
+        :param blogId: The ID of the blog to flag. Required if flagType is 1.
+        :type blogId: str, optional
+        :param wikiId: The ID of the wiki to flag. Required if flagType is 2.
+        :type wikiId: str, optional
+        :param asGuest: Flag as a guest user. Default is False.
+        :type asGuest: bool, optional
+        :param comId: The ID of the community where the flagging occurs.
+        :type comId: str, optional
+        :return: The API response from the flagging request.
+        :rtype: ApiResponse
+        :raises ValueError: If reason or flagType is None, or if none of the object IDs (userId, blogId, wikiId) is provided.
+
+        This method allows flagging content in the community with a specified reason and flag type. The reason parameter should provide
+        an explanation for flagging the content, and the flagType parameter determines the type of content being flagged (0: User, 1: Blog, 2: Wiki).
+        The appropriate object ID (userId, blogId, wikiId) must be provided based on the flagType. If asGuest is set to True, the flagging
+        is performed as a guest user. The comId parameter specifies the ID of the community where the flagging occurs.
+
+        **Example usage:**
+
+        To flag a user with a reason:
+
+        >>> response = client.flag(reason="Inappropriate behavior", flagType=0, userId="user123")
+        >>> try:
+        ...     print("Content flagged successfully!")
+        ... except:
+        ...     print("Failed to flag content.")
+        """
+        if reason is None: raise ValueError("Reason can't be None.")
+        if flagType is None: raise ValueError("flagType can't be None.")
+
+        data = {
+            "flagType": flagType,
+            "message": reason,
+            "timestamp": int(time() * 1000)
+        }
+
+        if userId: data.update({
+            "objectId": userId,
+            "objectType": 0
+        })
+
+        elif blogId: data.update({
+            "objectId": blogId,
+            "objectType": 1
+        })
+
+        elif wikiId: data.update({
+            "objectId": wikiId,
+            "objectType": 2
+        })
+
+        else: raise ValueError("There must be a value inside one of the following variables: userId, blogId, wikiId.")
+
+        flagMethod = "g-flag" if asGuest else "flag"
+
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId}/s/{flagMethod}",
+            data = data
+        ))
+    
+    @community
+    async def promotion(self, noticeId: str, type: str = "accept", comId: str = None) -> ApiResponse:
+        """
+        Promotes or performs an action on a community notice.
+
+        :param noticeId: The ID of the community notice to promote or perform an action on.
+        :type noticeId: str
+        :param type: The type of action to perform. Options: "accept" (default), "reject", "cancel".
+        :type type: str, optional
+        :param comId: The ID of the community in which the notice is located. If not provided, the current community ID is used.
+        :type comId: str, optional
+        :return: The API response from the promotion action.
+        :rtype: ApiResponse
+
+        This method allows the user to promote or perform an action on a community notice. The `noticeId` parameter specifies the ID
+        of the notice to act upon. The `type` parameter determines the action to perform, with options being "accept" (default),
+        "reject", or "cancel". The `comId` parameter is used to specify the community ID in which the notice is located. If `comId`
+        is not provided, the current community ID associated with the client is used.
+
+        The method returns an `ApiResponse` object containing the response from the promotion action.
+
+        **Example usage:**
+
+        To accept a community notice promotion:
+
+        >>> response = client.promotion(noticeId="notice123", type="accept")
+        >>> if response.status_code == 200:
+        ...     print("Notice promotion accepted successfully!")
+        ... else:
+        ...     print("Failed to accept notice promotion.")
+        """
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/notice/{noticeId}/{type}"
+        ))
+    
+    @community
+    async def change_vc_permission(self, chatId: str, permission: int, comId: Union[str, int]) -> ApiResponse:
+        """
+        Changes the voice chat permission for a chat in the community.
+
+        :param chatId: The ID of the chat for which the voice chat permission will be changed.
+        :type chatId: str
+        :param permission: The new voice chat permission to set. Options: 1 (Open), 2 (Approval required), 3 (Invite only).
+        :type permission: int
+        :param comId: The ID of the community where the chat belongs. Defaults to the current community ID if not specified.
+        :type comId: Union[str, int]
+        :return: The API response from changing the voice chat permission.
+        :rtype: ApiResponse
+        :raises ValueError: If an incorrect permission type is provided.
+
+        This method allows changing the voice chat permission for a specific chat within a community. The `chatId` parameter specifies
+        the ID of the chat, while the `permission` parameter indicates the new permission to be set. The available permission options
+        are: 1 (Open), 2 (Approval required), and 3 (Invite only).
+
+        If the `permission` value is one of the valid options, the method sends a POST request to update the permission. The response
+        is returned as an `ApiResponse` object.
+
+        **Example usage:**
+
+        To change the voice chat permission to "Approval required" for a chat in the current community:
+
+        >>> response = client.change_vc_permission(chatId="chat123", permission=2)
+        >>> if response.status_code == 200:
+        ...     print("Voice chat permission changed successfully!")
+        ... else:
+        ...     print("Failed to change voice chat permission.")
+        """
+        if permission in {1, 2, 3}:
+            return ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x/{comId or self.community_id}/chat/thread/{chatId}/vvchat-permission",
+                data = {
+                    "vvChatJoinType": permission,
+                    "timestamp": int(time() * 1000)
+                }
+            ))
+        else:
+            raise ValueError("Incorrect permission type.")
+        
+    @community
+    async def fetch_blocked_users(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
+        """
+        Fetches a list of blocked users in the community.
+
+        :param start: The starting index of the blocked users to fetch (pagination). Default is 0.
+        :type start: int, optional
+        :param size: The number of blocked users to fetch (pagination). Default is 25.
+        :type size: int, optional
+        :param comId: The ID of the community to fetch blocked users from. If not provided, the method uses the current community ID.
+        :type comId: Union[str, int], optional
+        :return: The list of blocked users in the community.
+        :rtype: UserProfileList
+
+        This method retrieves a list of blocked users in the community. The blocked users can be fetched in a paginated manner using
+        the `start` and `size` parameters. By default, it fetches the first 25 blocked users. If the `comId` parameter is not provided,
+        it uses the current community ID associated with the client instance.
+
+        **Example usage:**
+
+        To fetch the first 25 blocked users in the community:
+
+        >>> blocked_users = client.fetch_blocked_users()
+        >>> for user in blocked_users:
+        ...     print(user.username)
+        """
+        return UserProfileList(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/block?start={start}&size={size}"
+        ))
+    
+    @community
+    async def search_users(self, nickname: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
+        """
+        Searches for users based on their nickname.
+
+        :param nickname: The nickname to search for.
+        :type nickname: str
+        :param start: The starting index of the search results (pagination). Default is 0.
+        :type start: int, optional
+        :param size: The number of search results to retrieve (pagination). Default is 25.
+        :type size: int, optional
+        :param comId: The ID or name of the community to search within. If not provided, the search will be performed within the current community.
+        :type comId: Union[str, int], optional
+        :return: The list of user profiles matching the search criteria.
+        :rtype: UserProfileList
+
+        This method allows searching for users based on their nickname. The `nickname` parameter specifies the nickname to search for.
+        The search results can be paginated using the `start` and `size` parameters. The `comId` parameter is used to specify the ID or name
+        of the community within which the search should be performed. If `comId` is not provided, the search will be conducted within the current
+        community.
+
+        The search results are returned as a `UserProfileList` object.
+
+        **Example usage:**
+
+        To search for users with the nickname "John" within the current community:
+
+        >>> results = client.search_users(nickname="John")
+        >>> for profile in results:
+        ...     print(profile.nickname)
+        """
+        return UserProfileList(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/user-profile?type=name&q={nickname}&start={start}&size={size}"
+        ))
+
+    @community
+    async def fetch_message(self, chatId: str, messageId: str, comId: Union[str, int] = None) -> Message:
+        """
+        Fetches a specific message from a chat thread.
+
+        :param chatId: The ID of the chat thread where the message is located.
+        :type chatId: str
+        :param messageId: The ID of the message to fetch.
+        :type messageId: str
+        :param comId: The ID of the community where the chat thread is located. If not provided, the default community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The fetched message.
+        :rtype: Message
+
+        This method fetches a specific message from a chat thread. The `chatId` parameter specifies the ID of the chat thread, while
+        the `messageId` parameter determines the ID of the message to retrieve. The `comId` parameter is the ID of the community where
+        the chat thread is located. If it is not provided, the default community ID is used.
+
+        The fetched message is returned as a `Message` object.
+
+        **Example usage:**
+
+        To fetch a specific message from a chat thread:
+
+        >>> message = client.fetch_message(chatId="chat123", messageId="message456")
+        >>> print(message.text)
+        """
+        return Message(await self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/message/{messageId}"
+        ))
+
+    @community
+    async def purchase(self,
+                 objectId: str,
+                 objectType: int,
+                 aminoPlus: bool = True,
+                 autoRenew: bool = False,
+                 comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Purchases an object from the store.
+
+        :param objectId: The ID of the object to purchase.
+        :type objectId: str
+        :param objectType: The type of the object to purchase.
+        :type objectType: int
+        :param aminoPlus: Indicates whether the purchase includes Amino Plus subscription. Default is True.
+        :type aminoPlus: bool, optional
+        :param autoRenew: Indicates whether the purchase should be set to auto-renew. Default is False.
+        :type autoRenew: bool, optional
+        :param comId: The ID or alias of the community where the purchase will be made. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The response from the store's purchase endpoint.
+        :rtype: ApiResponse
+
+        This method allows the user to purchase an object from the store. The `objectId` parameter specifies the ID of the object
+        to purchase, while the `objectType` parameter indicates the type of the object. The `aminoPlus` parameter determines whether
+        the purchase includes an Amino Plus subscription. By default, it is set to True. The `autoRenew` parameter specifies whether
+        the purchase should be set to auto-renew, with a default value of False. The `comId` parameter can be used to specify a
+        different community where the purchase will be made. If not provided, the current community ID is used.
+
+        **Note:** The request is made to the store's purchase endpoint and the response is returned as an `ApiResponse` object.
+
+        **Example usage:**
+
+        To purchase an object with Amino Plus and auto-renewal disabled:
+
+        >>> response = client.purchase(objectId="object123", objectType=1, aminoPlus=True, autoRenew=False)
+        >>> try:
+        ...     print("Purchase successful!")
+        ... except:
+        ...     print("Failed to make the purchase.")
+        """
+        return ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/store/purchase",
+            data = {
+                "objectId": objectId,
+                "objectType": objectType,
+                "v": 1,
+                "timestamp": int(time() * 1000),
+                "paymentContext": {
+                    "discountStatus": 1 if aminoPlus else 0,
+                    "discountValue": 1,
+                    "isAutoRenew": autoRenew
+                }
+            }
         ))
```

### Comparing `pymino-1.1.9.9/pymino/ext/async_context.py` & `pymino-1.2.1.1/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/async_event_handler.py` & `pymino-1.2.1.1/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/async_socket.py` & `pymino-1.2.1.1/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/community.py` & `pymino-1.2.1.1/pymino/ext/community.py`

 * *Files 2% similar despite different names*

```diff
@@ -2357,67 +2357,101 @@
         return ApiResponse(self.session.handler(
             method="DELETE",
             url=f"/x{self.community_id if comId is None else comId}/s/blog/{blogId}"
             ))
 
 
     @community
-    def post_wiki(self, title: str, content: str, fansOnly: bool=False, comId: Union[str, int] = None) -> ApiResponse:
+    def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None,fansOnly: bool=False, comId: Union[str, int] = None) -> ApiResponse:
         """
         Posts a new wiki article in the specified community.
 
         :param title: The title of the wiki article.
         :type title: str
         :param content: The content of the wiki article.
         :type content: str
-        :param fansOnly: Whether the wiki article should be for fans only. Must be either `True` or `False`.
-        :type fansOnly: bool
+        :param icon: The icon image file for the wiki article.
+        :type icon: str, optional
+        :param imageList: A list of image files to include in the wiki article.
+        :type imageList: list, optional
+        :param keywords: Keywords associated with the wiki article.
+        :type keywords: str, optional
+        :param backgroundColor: The background color for the wiki article.
+        :type backgroundColor: str, optional
+        :param fansOnly: Whether the wiki article should be for fans only. Default is False.
+        :type fansOnly: bool, optional
         :param comId: The ID of the community to post the wiki article in. If not provided, the current community ID is used.
-        :type comId: Union[str, int]
+        :type comId: Union[str, int], optional
         :return: An `ApiResponse` object representing the response from the server.
         :rtype: ApiResponse
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
-        The function sends a POST request to the API to post a new wiki article with the specified title, content, and fans-only setting.
+        This method allows the authenticated user to post a new wiki article in the specified community. The `title` parameter specifies
+        the title of the article, and the `content` parameter contains the content of the article.
+
+        Additional optional parameters can be provided to customize the wiki article. The `icon` parameter is used to specify an icon
+        image for the article, and the `imageList` parameter can be used to include multiple image files in the article.
+
+        The `keywords` parameter allows specifying keywords associated with the article, and the `backgroundColor` parameter sets the
+        background color of the article.
+
+        The `fansOnly` parameter determines whether the article should be accessible only to fans. By default, it is set to False.
+
+        The `comId` parameter is used to specify the ID of the community where the article should be posted. If not provided, the
+        current community ID is used.
 
         The response from the server is returned as an `ApiResponse` object.
-        
+
         `ApiResponse`:
 
-        - `message`: A message indicating whether the blog was successfully deleted.
+        - `message`: A message indicating the status of the wiki article posting.
         - `statuscode`: The status code of the API response.
         - `duration`: The duration of the API request.
         - `timestamp`: The timestamp of the API request.
-        - `mediaValue`: The media value of the deleted blog.
+        - `mediaValue`: The media value of the wiki article.
 
         **Example usage:**
 
         To post a new wiki article with the title "My First Wiki Article" and the content "This is my first wiki article.":
 
         >>> response = client.community.post_wiki(title="My First Wiki Article", content="This is my first wiki article.")
-        ... if response.statuscode == 0:
+        ... try:
         ...     print("Wiki article successfully posted!")
-        ... else:
+        ... except:
         ...     print("Wiki article could not be posted.")
         """
+        media = []
+
+        if imageList is not None:
+            media.append([100, self.upload_media(open(image, "rb").read(), "image/jpg"), None] for image in imageList)
+
+
+        data = {
+            "mediaList": media,
+        }
+        if icon: data["icon"] = self.upload_media(open(icon, "rb").read(), "image/jpg")
+        if keywords: data["keywords"] = keywords
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style":{"backgroundColor": backgroundColor if backgroundColor.startswith("#") else f"#{backgroundColor}"}}
+
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/item",
             data = {
             "extensions": {"fansOnly": fansOnly},
             "content": content,
             "latitude": 0,
             "longitude": 0,
-            "title": title,
+            "label": title,
             "type": 0,
             "contentLanguage": "en",
             "eventSource": "GlobalComposeMenu",
             "timestamp": int(time() * 1000),
-            }))
+            }.update(data)))
 
 
     @community
     def delete_wiki(self, wikiId: str, comId: Union[str, int] = None) -> ApiResponse:
         """
         Deletes a wiki item with the given ID.
 
@@ -4704,32 +4738,30 @@
         :type title: Optional[str]
         :param message: The message to send to the users when inviting them to the chat. Defaults to `None`.
         :type message: Optional[str]
         :param content: The content of the chat. Defaults to `None`.
         :type content: Optional[str]
         :param comId: The ID of the community where the chat will be created. If not provided, the current community ID is used.
         :type comId: Optional[Union[str, int]]
-        :return: An `ApiResponse` object containing information about the request status.
-        :rtype: ApiResponse
+        :return: An `ChatThread` object containing information about the request status.
+        :rtype: ChatThread
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
-        `ApiResponse`: TODO: Update this to reflect the new return type.
-
         - `message`: A message indicating whether the chat was successfully created.
         - `statuscode`: The status code of the API response.
         - `duration`: The duration of the API request.
         - `timestamp`: The timestamp of the API request.
 
         **Example usage:**
 
         To create a new chat with users "0000-0000-0000-0000" and "1111-1111-1111-1111":
 
         >>> response = client.community.start_chat(userIds=["0000-0000-0000-0000", "1111-1111-1111-1111"], title="New chat", message="Join my chat!", content="Hello, world!")
-        ... if response.statuscode == 0:
+        ... if response.status_code == 200:
         ...     print("Chat created successfully!")
         ... else:
         ...     print("Failed to create chat.")
         """
         return ChatThread(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread",
@@ -4737,15 +4769,15 @@
             "title": title,
             "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
             "initialMessageContent": message,
             "content": content,
             "type": 0,
             "publishToGlobal": 0,
             "timestamp": int(time() * 1000)
-            }))
+            })).status
 
 
     @community
     def invite_chat(self, chatId: str, userIds: Union[str, List[str]], comId: Union[str, int] = None) -> ApiResponse:
         """
         Invites one or more users to join a chat.
 
@@ -6555,8 +6587,436 @@
         try:
             return CommunityStats(
                 self.session.handler(
                     method = "GET",
                     url = f"http://service.aminoapps.com/api/v1/x{comId or self.community_id}/s/community/stats"
             ))
         except AccessDenied as e:
-            raise AccessDenied("You must be a leader to fetch community statistics.") from e
+            raise AccessDenied("You must be a leader to fetch community statistics.") from e
+    
+    @community
+    def edit_blog(self, blogId: str,
+                  title: str = None,
+                  content: str = None,
+                  imageList: list = None,
+                  categoriesList: list = None,
+                  backgroundColor: str = None,
+                  fansOnly: bool = False,
+                  comId: Union[str, int] = None) -> CBlog:
+        """
+        Edits a blog post.
+
+        :param blogId: The ID of the blog post to edit.
+        :type blogId: str
+        :param title: The new title for the blog post.
+        :type title: str, optional
+        :param content: The new content for the blog post.
+        :type content: str, optional
+        :param imageList: A list of image file paths to add as media to the blog post.
+        :type imageList: list, optional
+        :param categoriesList: A list of category IDs to tag the blog post with.
+        :type categoriesList: list, optional
+        :param backgroundColor: The new background color for the blog post.
+        :type backgroundColor: str, optional
+        :param fansOnly: Specifies whether the blog post should be available to fans only. Default is False.
+        :type fansOnly: bool, optional
+        :param comId: The ID of the community where the blog post is located. If not provided, the current community ID will be used.
+        :type comId: str, optional
+        :return: The edited blog post as a `CBlog` object.
+        :rtype: CBlog
+
+        This method allows the user to edit a blog post. The `blogId` parameter specifies the ID of the blog post to edit.
+        The `title`, `content`, `imageList`, `categoriesList`, `backgroundColor`, `fansOnly`, and `comId` parameters are used to
+        update the corresponding properties of the blog post. Only the specified parameters will be updated.
+
+        The `imageList` parameter accepts a list of image file paths, which will be uploaded as media for the blog post.
+        The `categoriesList` parameter accepts a list of category IDs, which will be used to tag the blog post.
+
+        **Example usage:**
+
+        To edit a blog post with a new title, content, and image:
+
+        >>> response = client.edit_blog(
+        ...     blogId="blog123",
+        ...     title="New Title",
+        ...     content="New Content",
+        ...     imageList=["path/to/image1.jpg", "path/to/image2.jpg"]
+        ... )
+        ... if response.status == 200:
+        ...     print("Blog post edited successfully!")
+        ... else:
+        ...     print("Failed to edit blog post.")
+        """
+        media = []
+        if imageList is not None: media = [[100, self.upload_media(open(image, "rb").read(), "image/jpg"), None] for image in imageList]
+        
+        data = {
+            "address": None,
+            "mediaList": media,
+            "latitude": 0,
+            "longitude": 0,
+            "eventSource": "PostDetailView",
+            "timestamp": int(time() * 1000)
+        }
+
+        if title: data["title"] = title
+        if content: data["content"] = content
+        if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+        if backgroundColor: data["extensions"] = {"style0": {
+            "backgroundColor": backgroundColor if backgroundColor.startswith("#") else f"#{backgroundColor}"
+        }}
+        if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
+        
+        return CBlog(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/blog/{blogId}",
+            data = data
+        ))
+
+    @community
+    def delete_notification(self, notificationId: str, comId: Union[str, int]= None) -> ApiResponse:
+        """
+        Deletes a notification.
+
+        :param notificationId: The ID of the notification to delete.
+        :type notificationId: str
+        :param comId: The ID of the community (optional). If not provided, the current community ID will be used.
+        :type comId: str, optional
+        :return: The response from the API after deleting the notification.
+        :rtype: ApiResponse
+
+        This method allows the authenticated user to delete a notification with the specified notification ID.
+        Optionally, you can provide the community ID (`comId`) if the notification belongs to a specific community.
+        If `comId` is not provided, the notification will be deleted from the current community.
+
+        The method sends a DELETE request to the API endpoint responsible for deleting the notification. The response
+        from the API is returned as an `ApiResponse` object.
+
+        **Example usage:**
+
+        To delete a notification with ID "notif123" from the current community:
+
+        >>> response = client.delete_notification(notificationId="notif123")
+        >>> try:
+        ...     print("Notification deleted successfully!")
+        ... except:
+        ...     print("Failed to delete notification.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "DELETE",
+            url = f"/x{comId or self.community_id}/s/notification/{notificationId}"
+        ))
+    
+    @community
+    def flag(self,
+             reason: str,
+             flagType: int,
+             userId: str = None,
+             blogId: str = None,
+             wikiId: str = None,
+             asGuest: bool = False,
+             comId: Union[str, int]= None) -> ApiResponse:
+        """
+        Flags content in the community.
+
+        :param reason: The reason for flagging the content.
+        :type reason: str
+        :param flagType: The type of flag. (0: User, 1: Blog, 2: Wiki)
+        :type flagType: int
+        :param userId: The ID of the user to flag. Required if flagType is 0.
+        :type userId: str, optional
+        :param blogId: The ID of the blog to flag. Required if flagType is 1.
+        :type blogId: str, optional
+        :param wikiId: The ID of the wiki to flag. Required if flagType is 2.
+        :type wikiId: str, optional
+        :param asGuest: Flag as a guest user. Default is False.
+        :type asGuest: bool, optional
+        :param comId: The ID of the community where the flagging occurs.
+        :type comId: str, optional
+        :return: The API response from the flagging request.
+        :rtype: ApiResponse
+        :raises ValueError: If reason or flagType is None, or if none of the object IDs (userId, blogId, wikiId) is provided.
+
+        This method allows flagging content in the community with a specified reason and flag type. The reason parameter should provide
+        an explanation for flagging the content, and the flagType parameter determines the type of content being flagged (0: User, 1: Blog, 2: Wiki).
+        The appropriate object ID (userId, blogId, wikiId) must be provided based on the flagType. If asGuest is set to True, the flagging
+        is performed as a guest user. The comId parameter specifies the ID of the community where the flagging occurs.
+
+        **Example usage:**
+
+        To flag a user with a reason:
+
+        >>> response = client.flag(reason="Inappropriate behavior", flagType=0, userId="user123")
+        >>> try:
+        ...     print("Content flagged successfully!")
+        ... except:
+        ...     print("Failed to flag content.")
+        """
+        if reason is None: raise ValueError("Reason can't be None.")
+        if flagType is None: raise ValueError("flagType can't be None.")
+
+        data = {
+            "flagType": flagType,
+            "message": reason,
+            "timestamp": int(time() * 1000)
+        }
+
+        if userId: data.update({
+            "objectId": userId,
+            "objectType": 0
+        })
+
+        elif blogId: data.update({
+            "objectId": blogId,
+            "objectType": 1
+        })
+
+        elif wikiId: data.update({
+            "objectId": wikiId,
+            "objectType": 2
+        })
+
+        else: raise ValueError("There must be a value inside one of the following variables: userId, blogId, wikiId.")
+
+        flagMethod = "g-flag" if asGuest else "flag"
+
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId}/s/{flagMethod}",
+            data = data
+        ))
+    
+    @community
+    def promotion(self, noticeId: str, type: str = "accept", comId: Union[str, int]= None) -> ApiResponse:
+        """
+        Promotes or performs an action on a community notice.
+
+        :param noticeId: The ID of the community notice to promote or perform an action on.
+        :type noticeId: str
+        :param type: The type of action to perform. Options: "accept" (default), "reject", "cancel".
+        :type type: str, optional
+        :param comId: The ID of the community in which the notice is located. If not provided, the current community ID is used.
+        :type comId: str, optional
+        :return: The API response from the promotion action.
+        :rtype: ApiResponse
+
+        This method allows the user to promote or perform an action on a community notice. The `noticeId` parameter specifies the ID
+        of the notice to act upon. The `type` parameter determines the action to perform, with options being "accept" (default),
+        "reject", or "cancel". The `comId` parameter is used to specify the community ID in which the notice is located. If `comId`
+        is not provided, the current community ID associated with the client is used.
+
+        The method returns an `ApiResponse` object containing the response from the promotion action.
+
+        **Example usage:**
+
+        To accept a community notice promotion:
+
+        >>> response = client.promotion(noticeId="notice123", type="accept")
+        >>> if response.status_code == 200:
+        ...     print("Notice promotion accepted successfully!")
+        ... else:
+        ...     print("Failed to accept notice promotion.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/notice/{noticeId}/{type}"
+        ))
+
+    @community
+    def change_vc_permission(self, chatId: str, permission: int, comId: Union[str, int]) -> ApiResponse:
+        """
+        Changes the voice chat permission for a chat in the community.
+
+        :param chatId: The ID of the chat for which the voice chat permission will be changed.
+        :type chatId: str
+        :param permission: The new voice chat permission to set. Options: 1 (Open), 2 (Approval required), 3 (Invite only).
+        :type permission: int
+        :param comId: The ID of the community where the chat belongs. Defaults to the current community ID if not specified.
+        :type comId: Union[str, int]
+        :return: The API response from changing the voice chat permission.
+        :rtype: ApiResponse
+        :raises ValueError: If an incorrect permission type is provided.
+
+        This method allows changing the voice chat permission for a specific chat within a community. The `chatId` parameter specifies
+        the ID of the chat, while the `permission` parameter indicates the new permission to be set. The available permission options
+        are: 1 (Open), 2 (Approval required), and 3 (Invite only).
+
+        If the `permission` value is one of the valid options, the method sends a POST request to update the permission. The response
+        is returned as an `ApiResponse` object.
+
+        **Example usage:**
+
+        To change the voice chat permission to "Approval required" for a chat in the current community:
+
+        >>> response = client.change_vc_permission(chatId="chat123", permission=2)
+        >>> if response.status_code == 200:
+        ...     print("Voice chat permission changed successfully!")
+        ... else:
+        ...     print("Failed to change voice chat permission.")
+        """
+        if permission in {1, 2, 3}:
+            return ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x/{comId or self.community_id}/chat/thread/{chatId}/vvchat-permission",
+                data = {
+                    "vvChatJoinType": permission,
+                    "timestamp": int(time() * 1000)
+                }
+            ))
+        else:
+            raise ValueError("Incorrect permission type.")
+    
+    @community
+    def fetch_blocked_users(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
+        """
+        Fetches a list of blocked users in the community.
+
+        :param start: The starting index of the blocked users to fetch (pagination). Default is 0.
+        :type start: int, optional
+        :param size: The number of blocked users to fetch (pagination). Default is 25.
+        :type size: int, optional
+        :param comId: The ID of the community to fetch blocked users from. If not provided, the method uses the current community ID.
+        :type comId: Union[str, int], optional
+        :return: The list of blocked users in the community.
+        :rtype: UserProfileList
+
+        This method retrieves a list of blocked users in the community. The blocked users can be fetched in a paginated manner using
+        the `start` and `size` parameters. By default, it fetches the first 25 blocked users. If the `comId` parameter is not provided,
+        it uses the current community ID associated with the client instance.
+
+        **Example usage:**
+
+        To fetch the first 25 blocked users in the community:
+
+        >>> blocked_users = client.fetch_blocked_users()
+        >>> for user in blocked_users:
+        ...     print(user.username)
+        """
+        return UserProfileList(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/block?start={start}&size={size}"
+        ))
+
+    @community
+    def search_users(self, nickname: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
+        """
+        Searches for users based on their nickname.
+
+        :param nickname: The nickname to search for.
+        :type nickname: str
+        :param start: The starting index of the search results (pagination). Default is 0.
+        :type start: int, optional
+        :param size: The number of search results to retrieve (pagination). Default is 25.
+        :type size: int, optional
+        :param comId: The ID or name of the community to search within. If not provided, the search will be performed within the current community.
+        :type comId: Union[str, int], optional
+        :return: The list of user profiles matching the search criteria.
+        :rtype: UserProfileList
+
+        This method allows searching for users based on their nickname. The `nickname` parameter specifies the nickname to search for.
+        The search results can be paginated using the `start` and `size` parameters. The `comId` parameter is used to specify the ID or name
+        of the community within which the search should be performed. If `comId` is not provided, the search will be conducted within the current
+        community.
+
+        The search results are returned as a `UserProfileList` object.
+
+        **Example usage:**
+
+        To search for users with the nickname "John" within the current community:
+
+        >>> results = client.search_users(nickname="John")
+        >>> for profile in results:
+        ...     print(profile.nickname)
+        """
+        return UserProfileList(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/user-profile?type=name&q={nickname}&start={start}&size={size}"
+        ))
+
+    @community
+    def fetch_message(self, chatId: str, messageId: str, comId: Union[str, int] = None) -> Message:
+        """
+        Fetches a specific message from a chat thread.
+
+        :param chatId: The ID of the chat thread where the message is located.
+        :type chatId: str
+        :param messageId: The ID of the message to fetch.
+        :type messageId: str
+        :param comId: The ID of the community where the chat thread is located. If not provided, the default community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The fetched message.
+        :rtype: Message
+
+        This method fetches a specific message from a chat thread. The `chatId` parameter specifies the ID of the chat thread, while
+        the `messageId` parameter determines the ID of the message to retrieve. The `comId` parameter is the ID of the community where
+        the chat thread is located. If it is not provided, the default community ID is used.
+
+        The fetched message is returned as a `Message` object.
+
+        **Example usage:**
+
+        To fetch a specific message from a chat thread:
+
+        >>> message = client.fetch_message(chatId="chat123", messageId="message456")
+        >>> print(message.text)
+        """
+        return Message(self.session.handler(
+            method = "GET",
+            url = f"/x{comId or self.community_id}/s/chat/thread/{chatId}/message/{messageId}"
+        ))
+
+    @community
+    def purchase(self,
+                 objectId: str,
+                 objectType: int,
+                 aminoPlus: bool = True,
+                 autoRenew: bool = False,
+                 comId: Union[str, int] = None) -> ApiResponse:
+        """
+        Purchases an object from the store.
+
+        :param objectId: The ID of the object to purchase.
+        :type objectId: str
+        :param objectType: The type of the object to purchase.
+        :type objectType: int
+        :param aminoPlus: Indicates whether the purchase includes Amino Plus subscription. Default is True.
+        :type aminoPlus: bool, optional
+        :param autoRenew: Indicates whether the purchase should be set to auto-renew. Default is False.
+        :type autoRenew: bool, optional
+        :param comId: The ID or alias of the community where the purchase will be made. If not provided, the current community ID is used.
+        :type comId: Union[str, int], optional
+        :return: The response from the store's purchase endpoint.
+        :rtype: ApiResponse
+
+        This method allows the user to purchase an object from the store. The `objectId` parameter specifies the ID of the object
+        to purchase, while the `objectType` parameter indicates the type of the object. The `aminoPlus` parameter determines whether
+        the purchase includes an Amino Plus subscription. By default, it is set to True. The `autoRenew` parameter specifies whether
+        the purchase should be set to auto-renew, with a default value of False. The `comId` parameter can be used to specify a
+        different community where the purchase will be made. If not provided, the current community ID is used.
+
+        **Note:** The request is made to the store's purchase endpoint and the response is returned as an `ApiResponse` object.
+
+        **Example usage:**
+
+        To purchase an object with Amino Plus and auto-renewal disabled:
+
+        >>> response = client.purchase(objectId="object123", objectType=1, aminoPlus=True, autoRenew=False)
+        >>> try:
+        ...     print("Purchase successful!")
+        ... except:
+        ...     print("Failed to make the purchase.")
+        """
+        return ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{comId or self.community_id}/s/store/purchase",
+            data = {
+                "objectId": objectId,
+                "objectType": objectType,
+                "v": 1,
+                "timestamp": int(time() * 1000),
+                "paymentContext": {
+                    "discountStatus": 1 if aminoPlus else 0,
+                    "discountValue": 1,
+                    "isAutoRenew": autoRenew
+                }
+            }
+        ))
```

### Comparing `pymino-1.1.9.9/pymino/ext/console.py` & `pymino-1.2.1.1/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/context.py` & `pymino-1.2.1.1/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/dispatcher.py` & `pymino-1.2.1.1/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/acm.py` & `pymino-1.2.1.1/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/api_response.py` & `pymino-1.2.1.1/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/chat_threads.py` & `pymino-1.2.1.1/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/comments.py` & `pymino-1.2.1.1/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/enums.py` & `pymino-1.2.1.1/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/exceptions.py` & `pymino-1.2.1.1/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/general.py` & `pymino-1.2.1.1/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/handlers.py` & `pymino-1.2.1.1/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/link_info.py` & `pymino-1.2.1.1/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/member.py` & `pymino-1.2.1.1/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/messages.py` & `pymino-1.2.1.1/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/notification.py` & `pymino-1.2.1.1/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/threads.py` & `pymino-1.2.1.1/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/userprofile.py` & `pymino-1.2.1.1/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/entities/wsevents.py` & `pymino-1.2.1.1/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/handle_queue.py` & `pymino-1.2.1.1/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/socket.py` & `pymino-1.2.1.1/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.1.1/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/chat_console.py` & `pymino-1.2.1.1/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/commands.py` & `pymino-1.2.1.1/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/community_console.py` & `pymino-1.2.1.1/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/generate.py` & `pymino-1.2.1.1/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/menu.py` & `pymino-1.2.1.1/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/profile_console.py` & `pymino-1.2.1.1/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino/ext/utilities/request_handler.py` & `pymino-1.2.1.1/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/pymino.egg-info/PKG-INFO` & `pymino-1.2.1.1/pymino.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.9.9
+Version: 1.2.1.1
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
     <a href="https://discord.gg/JMJpzpsMNJ"><img src="https://img.shields.io/discord/926853226152755280?color=blueviolet&label=discord%20server" alt="Discord"></a>
     <a href="https://libraries.io/github/forevercynical/pymino"><img src="https://img.shields.io/librariesio/github/forevercynical/pymino?color=blueviolet" alt="Libraries.io dependency status for GitHub repo"></a>
     <a href="https://github.com/forevercynical/pymino/commits/main"><img src="https://img.shields.io/github/last-commit/forevercynical/pymino?label=last%20updated&color=blueviolet" alt="GitHub last commit"></a>
     <a href="https://pypi.org/project/pymino/"><img src="https://img.shields.io/pypi/dw/pymino?color=blueviolet" alt="PyPI - Downloads"></a>
   </p>
 
   <p style="font-size: 1.2em; color: #424242;">A Python wrapper to communicate with the Amino Apps API.</p>
-  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous library.</p>
+  <p style="font-size: 1.2em; color: #424242;">Easily create a bot for Amino Apps using a modern, easy-to-use library.</p>
 
   <div style="border: 3px solid red; padding: 10px; margin: 15px 0;">
     <h3 style="color: red;"><strong> WARNING </strong></h3>
     <p><strong>Pymino is a fully reverse-engineered client. By using this client, you may be violating the Amino Apps' Terms of Service. This could lead to your account being suspended or permanently banned. Please use Pymino responsibly and at your own risk.</strong></p>
     <p><strong>Understand that the developers and maintainers of Pymino are not responsible for any actions taken against your account as a result of using this client. Proceed with caution.</strong></p>
   </div>
 
@@ -98,32 +98,37 @@
 >>> from pymino import Bot
 >>> from pymino.ext import *
 
 >>> # Initialize the bot
 >>> bot = Bot(
 ...     command_prefix="!",
 ...     community_id=00000000,
-... ) # You can set proxies and device_id here
+...     console_enabled=True,
+...     device_id=None,
+...     intents=True,
+...     online_status=True,
+...     proxy="http://127.0.0.1:8080" # Must be a string.
+... ) 
 
 >>> # The on_ready event is called when the bot has logged in.
 >>> @bot.on_ready()
 ... def ready():
 ...     print(f"{bot.profile.username} has logged in!")
 
 >>> # The on_text_message event is called when a message is received.
 >>> @bot.on_text_message()
-... def message(ctx: Context):
-...     print(f"{ctx.author.username}: {ctx.message.content}")
-...     if ctx.message.content.startswith("hi"):
+... def message(ctx: Context, member: Member, message: str):
+...     print(f"{member.username}: {message}")
+...     if message.startswith("hi"):
 ...         ctx.reply("Hello!")
 
 >>> # The on_member_join event is called when a member joins a chat.
 >>> @bot.on_member_join()
-... def join(ctx: Context):
-...     ctx.reply(f"Welcome to the chat, {ctx.author.username}!")
+... def join(ctx: Context, member: Member):
+...     ctx.reply(f"Welcome to the chat, {member.username}!")
 
 >>> # The on_member_leave event is called when a member leaves a chat.
 >>> @bot.on_member_leave()
 ... def leave(ctx: Context):
 ...     ctx.reply(f"Goodbye!")
 
 >>> # This is how you create a command.
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.9.9 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.1.1 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                              ****** pymino ******
 [Discord] [Libraries.io_dependency_status_for_GitHub_repo] [GitHub_last_commit]
                               [PyPI_-_Downloads]
            A Python wrapper to communicate with the Amino Apps API.
-  Easily create a bot for Amino Apps using a modern, easy-to-use, synchronous
-                                   library.
+    Easily create a bot for Amino Apps using a modern, easy-to-use library.
                                **** WARNING ****
  Pymino is a fully reverse-engineered client. By using this client, you may be
   violating the Amino Apps' Terms of Service. This could lead to your account
   being suspended or permanently banned. Please use Pymino responsibly and at
                                 your own risk.
  Understand that the developers and maintainers of Pymino are not responsible
  for any actions taken against your account as a result of using this client.
@@ -68,32 +67,37 @@
 >>> from pymino import Bot
 >>> from pymino.ext import *
 
 >>> # Initialize the bot
 >>> bot = Bot(
 ...     command_prefix="!",
 ...     community_id=00000000,
-... ) # You can set proxies and device_id here
+...     console_enabled=True,
+...     device_id=None,
+...     intents=True,
+...     online_status=True,
+...     proxy="http://127.0.0.1:8080" # Must be a string.
+... )
 
 >>> # The on_ready event is called when the bot has logged in.
 >>> @bot.on_ready()
 ... def ready():
 ...     print(f"{bot.profile.username} has logged in!")
 
 >>> # The on_text_message event is called when a message is received.
 >>> @bot.on_text_message()
-... def message(ctx: Context):
-...     print(f"{ctx.author.username}: {ctx.message.content}")
-...     if ctx.message.content.startswith("hi"):
+... def message(ctx: Context, member: Member, message: str):
+...     print(f"{member.username}: {message}")
+...     if message.startswith("hi"):
 ...         ctx.reply("Hello!")
 
 >>> # The on_member_join event is called when a member joins a chat.
 >>> @bot.on_member_join()
-... def join(ctx: Context):
-...     ctx.reply(f"Welcome to the chat, {ctx.author.username}!")
+... def join(ctx: Context, member: Member):
+...     ctx.reply(f"Welcome to the chat, {member.username}!")
 
 >>> # The on_member_leave event is called when a member leaves a chat.
 >>> @bot.on_member_leave()
 ... def leave(ctx: Context):
 ...     ctx.reply(f"Goodbye!")
 
 >>> # This is how you create a command.
```

### Comparing `pymino-1.1.9.9/pymino.egg-info/SOURCES.txt` & `pymino-1.2.1.1/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.9.9/setup.cfg` & `pymino-1.2.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e39 2e39 0d0a 6175  on = 1.1.9.9..au
+00000020: 6f6e 203d 2031 2e32 2e31 2e31 0d0a 6175  on = 1.2.1.1..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.9.9/setup.py` & `pymino-1.2.1.1/setup.py`

 * *Files identical despite different names*

