# Comparing `tmp/WaveLinkCord-2.2.3.tar.gz` & `tmp/WavelinkCord-2.5.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveLinkCord-2.2.3.tar", last modified: Thu Apr 13 21:27:26 2023, max compression
+gzip compressed data, was "WavelinkCord-2.5.2b0.tar", last modified: Sun Jun 18 13:22:59 2023, max compression
```

## Comparing `WaveLinkCord-2.2.3.tar` & `WavelinkCord-2.5.2b0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.270708 WaveLinkCord-2.2.3/
--rw-rw-rw-   0        0        0     1108 2023-03-11 18:03:30.000000 WaveLinkCord-2.2.3/LICENSE
--rw-rw-rw-   0        0        0     6010 2023-04-13 21:27:26.271554 WaveLinkCord-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5123 2023-04-12 16:20:02.000000 WaveLinkCord-2.2.3/README.rst
--rw-rw-rw-   0        0        0     1015 2023-04-13 21:26:50.000000 WaveLinkCord-2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       30 2023-03-11 18:15:49.000000 WaveLinkCord-2.2.3/requirements.txt
--rw-rw-rw-   0        0        0      672 2023-04-13 21:27:26.287807 WaveLinkCord-2.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.102752 WaveLinkCord-2.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.176991 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/
--rw-rw-rw-   0        0        0     6010 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 21:27:26.000000 WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.224517 WaveLinkCord-2.2.3/src/wavelinkcord/
--rw-rw-rw-   0        0        0     1495 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/backoff.py
--rw-rw-rw-   0        0        0     1731 2023-04-12 15:43:17.000000 WaveLinkCord-2.2.3/src/wavelinkcord/enums.py
--rw-rw-rw-   0        0        0     1995 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.106935 WaveLinkCord-2.2.3/src/wavelinkcord/ext/
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.227518 WaveLinkCord-2.2.3/src/wavelinkcord/ext/spotify/
--rw-rw-rw-   0        0        0    16472 2023-04-13 21:21:23.000000 WaveLinkCord-2.2.3/src/wavelinkcord/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/filters.py
--rw-rw-rw-   0        0        0    17775 2023-04-12 16:19:22.000000 WaveLinkCord-2.2.3/src/wavelinkcord/node.py
--rw-rw-rw-   0        0        0     2474 2023-04-12 15:46:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/payloads.py
--rw-rw-rw-   0        0        0    20778 2023-04-12 15:44:18.000000 WaveLinkCord-2.2.3/src/wavelinkcord/player.py
--rw-rw-rw-   0        0        0    12384 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/queue.py
--rw-rw-rw-   0        0        0    10104 2023-04-12 15:44:29.000000 WaveLinkCord-2.2.3/src/wavelinkcord/tracks.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:27:26.267720 WaveLinkCord-2.2.3/src/wavelinkcord/types/
--rw-rw-rw-   0        0        0      860 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/events.py
--rw-rw-rw-   0        0        0      635 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/request.py
--rw-rw-rw-   0        0        0      424 2023-04-12 15:42:28.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/state.py
--rw-rw-rw-   0        0        0      343 2023-04-12 15:42:21.000000 WaveLinkCord-2.2.3/src/wavelinkcord/types/track.py
--rw-rw-rw-   0        0        0     9098 2023-04-12 16:19:03.000000 WaveLinkCord-2.2.3/src/wavelinkcord/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.579206 WavelinkCord-2.5.2b0/
+-rw-rw-rw-   0        0        0     1108 2023-06-18 12:59:01.000000 WavelinkCord-2.5.2b0/LICENSE
+-rw-rw-rw-   0        0        0     5873 2023-06-18 13:22:59.576205 WavelinkCord-2.5.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     5064 2023-06-18 12:59:01.000000 WavelinkCord-2.5.2b0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.447175 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/
+-rw-rw-rw-   0        0        0     5873 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 13:22:59.000000 WavelinkCord-2.5.2b0/WavelinkCord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1011 2023-06-18 13:00:25.000000 WavelinkCord-2.5.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0       30 2023-06-18 13:00:12.000000 WavelinkCord-2.5.2b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:22:59.580206 WavelinkCord-2.5.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.540197 WavelinkCord-2.5.2b0/wavelink/
+-rw-rw-rw-   0        0        0     1463 2023-06-18 12:57:31.000000 WavelinkCord-2.5.2b0/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2630 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     3539 2023-06-18 12:23:34.000000 WavelinkCord-2.5.2b0/wavelink/enums.py
+-rw-rw-rw-   0        0        0     2936 2023-06-18 12:23:33.000000 WavelinkCord-2.5.2b0/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.366157 WavelinkCord-2.5.2b0/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.545199 WavelinkCord-2.5.2b0/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    17299 2023-06-18 12:23:27.000000 WavelinkCord-2.5.2b0/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    19586 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17308 2023-06-18 12:23:32.000000 WavelinkCord-2.5.2b0/wavelink/node.py
+-rw-rw-rw-   0        0        0     3369 2023-06-18 12:23:32.000000 WavelinkCord-2.5.2b0/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    21638 2023-06-18 12:23:31.000000 WavelinkCord-2.5.2b0/wavelink/player.py
+-rw-rw-rw-   0        0        0    12123 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/queue.py
+-rw-rw-rw-   0        0        0     9628 2023-06-18 12:23:30.000000 WavelinkCord-2.5.2b0/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:22:59.570204 WavelinkCord-2.5.2b0/wavelink/types/
+-rw-rw-rw-   0        0        0      825 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      602 2023-06-18 12:18:37.000000 WavelinkCord-2.5.2b0/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      409 2023-06-18 12:23:29.000000 WavelinkCord-2.5.2b0/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      325 2023-06-18 12:18:37.000000 WavelinkCord-2.5.2b0/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9311 2023-06-18 12:18:36.000000 WavelinkCord-2.5.2b0/wavelink/websocket.py
```

### Comparing `WaveLinkCord-2.2.3/LICENSE` & `WavelinkCord-2.5.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `WaveLinkCord-2.2.3/PKG-INFO` & `WavelinkCord-2.5.2b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
-Name: WaveLinkCord
-Version: 2.2.3
-Summary: A robust and powerful Lavalink wrapper for Nextcord
-Home-page: https://github.com/Zyb3rWolfi/Wavelinkcord
-Author: Zyb3rWolfi
-Author-email: Zyb3rWolfi  <Zyb3rWolfi@proton.me>
+Name: WavelinkCord
+Version: 2.5.2b0
+Summary: A robust and powerful Lavalink wrapper for discord.py
+Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -42,31 +40,30 @@
 
 .. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
     :target: https://github.com/PythonistaGuild/Wavelink/commits/main
     :alt: Maintenance
 
 
 
-Wavelink is a robust and powerful Lavalink wrapper for `Nextcord <https://github.com/nextcord/nextcord>`_.
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
 Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-This is a Fork of `WaveLink <https://github.com/PythonistaGuild/Wavelink>`_ which was modified to allow it to run on Nextcord.
 
 
 **Features:**
 
 - Fully Asynchronous
 - Auto-Play and Looping (With the inbuilt Queue system)
 - Spotify Support
 - Node Balancing and Fail-over
 - Supports Lavalink 3.7+
 
 
 Documentation
 ---------------------------
-`Official Documentation <https://wavelink.readthedocs.io/en/latest/index.html>`_
+`Official Documentation <https://wavelink.dev/>`_
 
 Support
 ---------------------------
 For support using WaveLink, please join the official `support server
 <https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
 
 .. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
@@ -94,56 +91,65 @@
 Getting Started
 ----------------------------
 
 **See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
 
 .. code:: py
 
-    import nextcord
+    import discord
     import wavelink
-    from nextcord.ext import commands
+    from discord.ext import commands
 
-    intents = nextcord.intents.all()
-    client = nextcord.Client()
-    bot = commands.Bot(command_prefix="?", intents=intents)
-
-    @bot.event
-    async def on_ready():
-        print(f'Logged in {self.user} | {self.user.id}')
-        bot.loop.create_task(on_node())
-
-    async def setup_hook():
-        # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-        # and pass it to NodePool.connect with the client/bot.
-        node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-        await wavelink.NodePool.connect(client=self, nodes=[node])
 
-    @bot.slash_command()
-    async def play(interaction : nextcord.Interaction, search : str):
-        """Simple play command."""
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
 
-        query = await wavelink.YoutubeTrack.search(search, return_first=True)
 
-        destination = interaction.user.voice.channel
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
 
-        if not interaction.guild.voice_client:
-            vc: wavelink.Player = await destination.connect(cls=wavelink.Player)
-        elif interaction.guild.voice_client:
-            vc: wavelink.Player = interaction.guild.voice_client
-        
-        await vc.play(query)
+        track = tracks[0]
+        await vc.play(track)
 
 
-    @bot.slash_command()
-    async def disconnect(interaction : nextcord.Interaction):
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
         """Simple disconnect command.
 
         This command assumes there is a currently connected Player.
         """
-        vc: wavelink.Player = interaction.guild.voice_client
+        vc: wavelink.Player = ctx.voice_client
         await vc.disconnect()
 
 
 Lavalink Installation
 ---------------------
 
 Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
```

### Comparing `WaveLinkCord-2.2.3/README.rst` & `WavelinkCord-2.5.2b0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -20,31 +20,30 @@
 
 .. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
     :target: https://github.com/PythonistaGuild/Wavelink/commits/main
     :alt: Maintenance
 
 
 
-Wavelink is a robust and powerful Lavalink wrapper for `Nextcord <https://github.com/nextcord/nextcord>`_.
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
 Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-This is a Fork of `WaveLink <https://github.com/PythonistaGuild/Wavelink>`_ which was modified to allow it to run on Nextcord.
 
 
 **Features:**
 
 - Fully Asynchronous
 - Auto-Play and Looping (With the inbuilt Queue system)
 - Spotify Support
 - Node Balancing and Fail-over
 - Supports Lavalink 3.7+
 
 
 Documentation
 ---------------------------
-`Official Documentation <https://wavelink.readthedocs.io/en/latest/index.html>`_
+`Official Documentation <https://wavelink.dev/>`_
 
 Support
 ---------------------------
 For support using WaveLink, please join the official `support server
 <https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
 
 .. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
@@ -72,56 +71,65 @@
 Getting Started
 ----------------------------
 
 **See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
 
 .. code:: py
 
-    import nextcord
+    import discord
     import wavelink
-    from nextcord.ext import commands
+    from discord.ext import commands
 
-    intents = nextcord.intents.all()
-    client = nextcord.Client()
-    bot = commands.Bot(command_prefix="?", intents=intents)
-
-    @bot.event
-    async def on_ready():
-        print(f'Logged in {self.user} | {self.user.id}')
-        bot.loop.create_task(on_node())
-
-    async def setup_hook():
-        # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-        # and pass it to NodePool.connect with the client/bot.
-        node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-        await wavelink.NodePool.connect(client=self, nodes=[node])
 
-    @bot.slash_command()
-    async def play(interaction : nextcord.Interaction, search : str):
-        """Simple play command."""
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
 
-        query = await wavelink.YoutubeTrack.search(search, return_first=True)
 
-        destination = interaction.user.voice.channel
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
 
-        if not interaction.guild.voice_client:
-            vc: wavelink.Player = await destination.connect(cls=wavelink.Player)
-        elif interaction.guild.voice_client:
-            vc: wavelink.Player = interaction.guild.voice_client
-        
-        await vc.play(query)
+        track = tracks[0]
+        await vc.play(track)
 
 
-    @bot.slash_command()
-    async def disconnect(interaction : nextcord.Interaction):
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
         """Simple disconnect command.
 
         This command assumes there is a currently connected Player.
         """
-        vc: wavelink.Player = interaction.guild.voice_client
+        vc: wavelink.Player = ctx.voice_client
         await vc.disconnect()
 
 
 Lavalink Installation
 ---------------------
 
 Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
```

### Comparing `WaveLinkCord-2.2.3/pyproject.toml` & `WavelinkCord-2.5.2b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "WaveLinkCord"
-version = "2.2.3"
+name = "WavelinkCord"
+version = "2.5.2b"
 authors = [
-  { name="Zyb3rWolfi ", email="Zyb3rWolfi@proton.me" },
+  { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
-description = "A robust and powerful Lavalink wrapper for Nextcord"
+description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
 classifiers = [
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `WaveLinkCord-2.2.3/src/WaveLinkCord.egg-info/PKG-INFO` & `WavelinkCord-2.5.2b0/WavelinkCord.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
-Name: WaveLinkCord
-Version: 2.2.3
-Summary: A robust and powerful Lavalink wrapper for Nextcord
-Home-page: https://github.com/Zyb3rWolfi/Wavelinkcord
-Author: Zyb3rWolfi
-Author-email: Zyb3rWolfi  <Zyb3rWolfi@proton.me>
+Name: WavelinkCord
+Version: 2.5.2b0
+Summary: A robust and powerful Lavalink wrapper for discord.py
+Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -42,31 +40,30 @@
 
 .. image:: https://img.shields.io/maintenance/yes/2023?color=pink&style=for-the-badge
     :target: https://github.com/PythonistaGuild/Wavelink/commits/main
     :alt: Maintenance
 
 
 
-Wavelink is a robust and powerful Lavalink wrapper for `Nextcord <https://github.com/nextcord/nextcord>`_.
+Wavelink is a robust and powerful Lavalink wrapper for `Discord.py <https://github.com/Rapptz/discord.py>`_.
 Wavelink features a fully asynchronous API that's intuitive and easy to use with built in Spotify Support and Node Pool Balancing.
-This is a Fork of `WaveLink <https://github.com/PythonistaGuild/Wavelink>`_ which was modified to allow it to run on Nextcord.
 
 
 **Features:**
 
 - Fully Asynchronous
 - Auto-Play and Looping (With the inbuilt Queue system)
 - Spotify Support
 - Node Balancing and Fail-over
 - Supports Lavalink 3.7+
 
 
 Documentation
 ---------------------------
-`Official Documentation <https://wavelink.readthedocs.io/en/latest/index.html>`_
+`Official Documentation <https://wavelink.dev/>`_
 
 Support
 ---------------------------
 For support using WaveLink, please join the official `support server
 <https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
 
 .. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
@@ -94,56 +91,65 @@
 Getting Started
 ----------------------------
 
 **See also:** `Examples <https://github.com/PythonistaGuild/Wavelink/tree/main/examples>`_
 
 .. code:: py
 
-    import nextcord
+    import discord
     import wavelink
-    from nextcord.ext import commands
+    from discord.ext import commands
 
-    intents = nextcord.intents.all()
-    client = nextcord.Client()
-    bot = commands.Bot(command_prefix="?", intents=intents)
-
-    @bot.event
-    async def on_ready():
-        print(f'Logged in {self.user} | {self.user.id}')
-        bot.loop.create_task(on_node())
-
-    async def setup_hook():
-        # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
-        # and pass it to NodePool.connect with the client/bot.
-        node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
-        await wavelink.NodePool.connect(client=self, nodes=[node])
 
-    @bot.slash_command()
-    async def play(interaction : nextcord.Interaction, search : str):
-        """Simple play command."""
+    class Bot(commands.Bot):
+
+        def __init__(self) -> None:
+            intents = discord.Intents.default()
+            intents.message_content = True
+
+            super().__init__(intents=intents, command_prefix='?')
+
+        async def on_ready(self) -> None:
+            print(f'Logged in {self.user} | {self.user.id}')
+
+        async def setup_hook(self) -> None:
+            # Wavelink 2.0 has made connecting Nodes easier... Simply create each Node
+            # and pass it to NodePool.connect with the client/bot.
+            node: wavelink.Node = wavelink.Node(uri='http://localhost:2333', password='youshallnotpass')
+            await wavelink.NodePool.connect(client=self, nodes=[node])
 
-        query = await wavelink.YoutubeTrack.search(search, return_first=True)
 
-        destination = interaction.user.voice.channel
+    bot = Bot()
+
+
+    @bot.command()
+    async def play(ctx: commands.Context, *, search: str) -> None:
+        """Simple play command."""
+
+        if not ctx.voice_client:
+            vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+        else:
+            vc: wavelink.Player = ctx.voice_client
+
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
 
-        if not interaction.guild.voice_client:
-            vc: wavelink.Player = await destination.connect(cls=wavelink.Player)
-        elif interaction.guild.voice_client:
-            vc: wavelink.Player = interaction.guild.voice_client
-        
-        await vc.play(query)
+        track = tracks[0]
+        await vc.play(track)
 
 
-    @bot.slash_command()
-    async def disconnect(interaction : nextcord.Interaction):
+    @bot.command()
+    async def disconnect(ctx: commands.Context) -> None:
         """Simple disconnect command.
 
         This command assumes there is a currently connected Player.
         """
-        vc: wavelink.Player = interaction.guild.voice_client
+        vc: wavelink.Player = ctx.voice_client
         await vc.disconnect()
 
 
 Lavalink Installation
 ---------------------
 
 Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/__init__.py` & `WavelinkCord-2.5.2b0/wavelink/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-__title__ = "WaveLink"
-__author__ = "PythonistaGuild, EvieePy"
-__license__ = "MIT"
-__copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.2.1"
-
-from .enums import *
-from .exceptions import *
-from .node import *
-from .payloads import *
-from .player import Player as Player
-from .tracks import *
-from .queue import *
-from .filters import *
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+__title__ = "WaveLinkCord"
+__author__ = "PythonistaGuild, EvieePy"
+__license__ = "MIT"
+__copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
+__version__ = "2.5.2b"
+
+from .enums import *
+from .exceptions import *
+from .node import *
+from .payloads import *
+from .player import Player as Player
+from .tracks import *
+from .queue import *
+from .filters import *
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/backoff.py` & `WavelinkCord-2.5.2b0/wavelink/backoff.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-"""
-The MIT License (MIT)
-Copyright (c) 2021-Present PythonistaGuild, EvieePy, Rapptz
-Permission is hereby granted, free of charge, to any person obtaining a
-copy of this software and associated documentation files (the "Software"),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
-OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-"""
-from __future__ import annotations
-
-import random
-from collections.abc import Callable
-
-
-class Backoff:
-    """An implementation of an Exponential Backoff.
-    Parameters
-    ----------
-    base: int
-        The base time to multiply exponentially. Defaults to 1.
-    maximum_time: float
-        The maximum wait time. Defaults to 30.0
-    maximum_tries: Optional[int]
-        The amount of times to backoff before resetting. Defaults to 5. If set to None, backoff will run indefinitely.
-    """
-
-    def __init__(self, *, base: int = 1, maximum_time: float = 30.0, maximum_tries: int | None = 5) -> None:
-        self._base: int = base
-        self._maximum_time: float = maximum_time
-        self._maximum_tries: int | None = maximum_tries
-        self._retries: int = 1
-
-        rand = random.Random()
-        rand.seed()
-
-        self._rand: Callable[[float, float], float] = rand.uniform
-
-        self._last_wait: float = 0
-
-    def calculate(self) -> float:
-        exponent = min((self._retries ** 2), self._maximum_time)
-        wait = self._rand(0, (self._base * 2) * exponent)
-
-        if wait <= self._last_wait:
-            wait = self._last_wait * 2
-
-        self._last_wait = wait
-
-        if wait > self._maximum_time:
-            wait = self._maximum_time
-            self._retries = 0
-            self._last_wait = 0
-
-        if self._maximum_tries and self._retries >= self._maximum_tries:
-            self._retries = 0
-            self._last_wait = 0
-
-        self._retries += 1
-
-        return wait
+"""
+The MIT License (MIT)
+Copyright (c) 2021-Present PythonistaGuild, EvieePy, Rapptz
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+"""
+from __future__ import annotations
+
+import random
+from collections.abc import Callable
+
+
+class Backoff:
+    """An implementation of an Exponential Backoff.
+    Parameters
+    ----------
+    base: int
+        The base time to multiply exponentially. Defaults to 1.
+    maximum_time: float
+        The maximum wait time. Defaults to 30.0
+    maximum_tries: Optional[int]
+        The amount of times to backoff before resetting. Defaults to 5. If set to None, backoff will run indefinitely.
+    """
+
+    def __init__(self, *, base: int = 1, maximum_time: float = 30.0, maximum_tries: int | None = 5) -> None:
+        self._base: int = base
+        self._maximum_time: float = maximum_time
+        self._maximum_tries: int | None = maximum_tries
+        self._retries: int = 1
+
+        rand = random.Random()
+        rand.seed()
+
+        self._rand: Callable[[float, float], float] = rand.uniform
+
+        self._last_wait: float = 0
+
+    def calculate(self) -> float:
+        exponent = min((self._retries ** 2), self._maximum_time)
+        wait = self._rand(0, (self._base * 2) * exponent)
+
+        if wait <= self._last_wait:
+            wait = self._last_wait * 2
+
+        self._last_wait = wait
+
+        if wait > self._maximum_time:
+            wait = self._maximum_time
+            self._retries = 0
+            self._last_wait = 0
+
+        if self._maximum_tries and self._retries >= self._maximum_tries:
+            self._retries = 0
+            self._last_wait = 0
+
+        self._retries += 1
+
+        return wait
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/ext/spotify/__init__.py` & `WavelinkCord-2.5.2b0/wavelink/ext/spotify/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,493 +1,539 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import asyncio
-import base64
-import enum
-import re
-import time
-from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
-
-import aiohttp
-from nextcord.ext import commands
-
-import wavelinkcord
-from wavelinkcord import Node, NodePool
-
-if TYPE_CHECKING:
-    from wavelinkcord import Player, Playable
-
-
-__all__ = ('SpotifySearchType',
-           'SpotifyClient',
-           'SpotifyTrack',
-           'SpotifyRequestError',
-           'decode_url')
-
-
-GRANTURL = 'https://accounts.spotify.com/api/token?grant_type=client_credentials'
-URLREGEX = re.compile(r'(https?://open.)?(spotify)(.com/|:)'
-                      r'(?P<type>album|playlist|track|artist)([/:])'
-                      r'(?P<id>[a-zA-Z0-9]+)(\?si=[a-zA-Z0-9]+)?(&dl_branch=[0-9]+)?')
-BASEURL = 'https://api.spotify.com/v1/{entity}s/{identifier}'
-RECURL = 'https://api.spotify.com/v1/recommendations?seed_tracks={tracks}'
-
-
-ST = TypeVar("ST", bound="Playable")
-
-
-def decode_url(url: str) -> Optional[dict]:
-    """Check whether the given URL is a valid Spotify URL and return it's type and ID.
-
-    Parameters
-    ----------
-    url: str
-        The URL to check.
-
-    Returns
-    -------
-    Optional[dict]
-        An mapping of :class:`SpotifySearchType` and Spotify ID. Type will be either track, album or playlist.
-        If type is not track, album or playlist, a special unusable type is returned.
-
-        Could return None if the URL is invalid.
-
-    Examples
-    --------
-
-    .. code:: python3
-
-        from wavelink.ext import spotify
-
-        ...
-
-        decoded = spotify.decode_url("https://open.spotify.com/track/6BDLcvvtyJD2vnXRDi1IjQ?si=e2e5bd7aaf3d4a2a")
-
-        if decoded and decoded['type'] is spotify.SpotifySearchType.track:
-            track = await spotify.SpotifyTrack.search(query=decoded["id"], type=decoded["type"])
-    """
-    match = URLREGEX.match(url)
-    if match:
-        try:
-            type_ = SpotifySearchType[match['type']]
-        except KeyError:
-            type_ = SpotifySearchType.unusable
-
-        return {'type': type_, 'id': match['id']}
-
-    return None
-
-
-class SpotifySearchType(enum.Enum):
-    """An enum specifying which type to search for with a given Spotify ID.
-
-    track
-        Default search type. Unless specified otherwise this will always be the search type.
-    album
-        Search for an album.
-    playlist
-        Search for a playlist.
-    """
-    track = 0
-    album = 1
-    playlist = 2
-    unusable = 3
-
-
-class SpotifyAsyncIterator:
-
-    def __init__(self, *, query: str, limit: int, type: SpotifySearchType, node: Node):
-        self._query = query
-        self._limit = limit
-        self._type = type
-        self._node = node
-
-        self._first = True
-        self._count = 0
-        self._queue = asyncio.Queue()
-
-    def __aiter__(self):
-        return self
-
-    async def fill_queue(self):
-        tracks = await self._node._spotify._search(query=self._query, iterator=True, type=self._type)
-
-        for track in tracks:
-            await self._queue.put(track)
-
-    async def __anext__(self):
-        if self._first:
-            await self.fill_queue()
-            self._first = False
-
-        if self._limit is not None and self._count == self._limit:
-            raise StopAsyncIteration
-
-        try:
-            track = self._queue.get_nowait()
-        except asyncio.QueueEmpty as e:
-            raise StopAsyncIteration from e
-
-        if track is None:
-            return await self.__anext__()
-
-        track = SpotifyTrack(track)
-
-        self._count += 1
-        return track
-
-
-class SpotifyRequestError(Exception):
-    """Base error for Spotify requests.
-
-    Attributes
-    ----------
-    status: int
-        The status code returned from the request.
-    reason: Optional[str]
-        The reason the request failed. Could be None.
-    """
-
-    def __init__(self, status: int, reason: Optional[str] = None):
-        self.status = status
-        self.reason = reason
-
-
-class SpotifyTrack:
-    """A track retrieved via Spotify.
-
-    Attributes
-    ----------
-    raw: dict[str, Any]
-        The raw payload from Spotify for this track.
-    album: str
-        The album name this track belongs to.
-    images: list[str]
-        A list of URLs to images associated with this track.
-    artists: list[str]
-        A list of artists for this track.
-    genres: list[str]
-        A list of genres associated with this tracks artist.
-    name: str
-        The track name.
-    title: str
-        An alias to name.
-    uri: str
-        The URI for this spotify track.
-    id: str
-        The spotify ID for this track.
-    isrc: str | None
-        The International Standard Recording Code associated with this track if given.
-    length: int
-        The track length in milliseconds.
-    duration: int
-        Alias to length.
-    """
-
-    __slots__ = (
-        'raw',
-        'album',
-        'images',
-        'artists',
-        'name',
-        'title',
-        'uri',
-        'id',
-        'length',
-        'duration',
-        'isrc',
-        '__dict__'
-    )
-
-    def __init__(self, data: dict[str, Any]) -> None:
-        self.raw: dict[str, Any] = data
-
-        album = data['album']
-        self.album: str = album['name']
-        self.images: list[str] = [i['url'] for i in album['images']]
-
-        artists = data['artists']
-        self.artists: list[str] = [a['name'] for a in artists]
-        # self.genres: list[str] = [a['genres'] for a in artists]
-
-        self.name: str = data['name']
-        self.title: str = self.name
-        self.uri: str = data['uri']
-        self.id: str = data['id']
-        self.length: int = data['duration_ms']
-        self.duration: int = self.length
-
-        self.isrc: str | None = data["external_ids"].get("isrc")
-
-    def __eq__(self, other) -> bool:
-        return self.id == other.id
-
-    @classmethod
-    async def search(
-        cls: Type[ST],
-            query: str,
-            *,
-            type: SpotifySearchType = SpotifySearchType.track,
-            node: Node | None = None,
-            return_first: bool = False,
-    ) -> Union[Optional[ST], List[ST]]:
-        """|coro|
-
-        Search for tracks with the given query.
-
-        Parameters
-        ----------
-        query: str
-            The song to search for.
-        type: Optional[:class:`spotify.SpotifySearchType`]
-            An optional enum value to use when searching with Spotify. Defaults to track.
-        node: Optional[:class:`wavelink.Node`]
-            An optional Node to use to make the search with.
-        return_first: Optional[bool]
-            An optional bool which when set to True will return only the first track found. Defaults to False.
-
-        Returns
-        -------
-        Union[Optional[Track], List[Track]]
-        """
-        if node is None:
-            node: Node = NodePool.get_connected_node()
-
-        if type == SpotifySearchType.track:
-            tracks = await node._spotify._search(query=query, type=type)
-
-            return tracks[0] if return_first else tracks
-        return await node._spotify._search(query=query, type=type)
-
-    @classmethod
-    def iterator(cls,
-                 *,
-                 query: str,
-                 limit: int | None = None,
-                 type: SpotifySearchType = SpotifySearchType.playlist,
-                 node: Node | None = None,
-                 ):
-        """An async iterator version of search.
-
-        This can be useful when searching for large playlists or albums with Spotify.
-
-        Parameters
-        ----------
-        query: str
-            The Spotify URL or ID to search for. Must be of type Playlist or Album.
-        limit: Optional[int]
-            Limit the amount of tracks returned.
-        type: :class:`SpotifySearchType`
-            The type of search. Must be either playlist or album. Defaults to playlist.
-        node: Optional[:class:`Node`]
-            An optional node to use when querying for tracks. Defaults to best available.
-
-        Examples
-        --------
-
-        .. code:: python3
-
-                async for track in spotify.SpotifyTrack.iterator(query=..., type=spotify.SpotifySearchType.playlist):
-                    ...
-        """
-
-        if type is not SpotifySearchType.album and type is not SpotifySearchType.playlist:
-            raise TypeError("Iterator search type must be either album or playlist.")
-
-        if node is None:
-            node = NodePool.get_connected_node()
-
-        return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=type)
-
-    @classmethod
-    async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
-        """Converter which searches for and returns the first track.
-
-        Used as a type hint in a discord.py command.
-        """
-        results = await cls.search(argument)
-
-        if not results:
-            raise commands.BadArgument("Could not find any songs matching that query.")
-
-        return results[0]
-
-    async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
-        """
-        Parameters
-        ----------
-        player: :class:`wavelink.player.Player`
-            If Player.autoplay is enabled, this search will fill the AutoPlay Queue.
-        cls
-            The class to convert this Spotify Track to.
-        """
-        try:
-            tracks: list[cls] = await cls.search(f'"{self.isrc}"')
-        except wavelinkcord.NoTracksError:
-            tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
-
-        if not player.autoplay or not populate:
-            return tracks[0]
-
-        node: Node = player.current_node
-        sc: SpotifyClient | None = node._spotify
-
-        if not sc:
-            raise RuntimeError(f"There is no spotify client associated with <{node:!r}>")
-
-        if len(player._track_seeds) == 5:
-            player._track_seeds.pop(0)
-
-        player._track_seeds.append(self.id)
-
-        url: str = RECURL.format(tracks=','.join(player._track_seeds))
-        async with node._session.get(url=url, headers=sc.bearer_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestError(resp.status, resp.reason)
-
-            data = await resp.json()
-
-        recos = [SpotifyTrack(t) for t in data['tracks']]
-        for reco in recos:
-            if reco in player.auto_queue or reco in player.auto_queue.history:
-                pass
-
-            await player.auto_queue.put_wait(reco)
-
-        return tracks[0]
-
-
-class SpotifyClient:
-    """Spotify client passed to Nodes for searching via Spotify.
-
-    Parameters
-    ----------
-    client_id: str
-        Your spotify application client ID.
-    client_secret: str
-        Your spotify application secret.
-    """
-
-    def __init__(self, *, client_id: str, client_secret: str):
-        self._client_id = client_id
-        self._client_secret = client_secret
-
-        self.session = aiohttp.ClientSession()
-
-        self._bearer_token: str = None  # type: ignore
-        self._expiry: int = 0
-
-    @property
-    def grant_headers(self) -> dict:
-        authbytes = f'{self._client_id}:{self._client_secret}'.encode()
-        return {'Authorization': f'Basic {base64.b64encode(authbytes).decode()}',
-                'Content-Type': 'application/x-www-form-urlencoded'}
-
-    @property
-    def bearer_headers(self) -> dict:
-        return {'Authorization': f'Bearer {self._bearer_token}'}
-
-    async def _get_bearer_token(self) -> None:
-        async with self.session.post(GRANTURL, headers=self.grant_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestError(resp.status, resp.reason)
-
-            data = await resp.json()
-            self._bearer_token = data['access_token']
-            self._expiry = time.time() + (int(data['expires_in']) - 10)
-
-    async def _search(self,
-                      query: str,
-                      type: SpotifySearchType = SpotifySearchType.track,
-                      iterator: bool = False,
-                      ) -> SpotifyTrack | list[SpotifyTrack]:
-
-        if not self._bearer_token or time.time() >= self._expiry:
-            await self._get_bearer_token()
-
-        regex_result = URLREGEX.match(query)
-
-        url = (
-            BASEURL.format(
-                entity=regex_result['type'], identifier=regex_result['id']
-            )
-            if regex_result
-            else BASEURL.format(entity=type.name, identifier=query)
-        )
-        async with self.session.get(url, headers=self.bearer_headers) as resp:
-            if resp.status != 200:
-                raise SpotifyRequestError(resp.status, resp.reason)
-
-            data = await resp.json()
-
-        if data['type'] == 'track':
-            return SpotifyTrack(data)
-
-        elif data['type'] == 'album':
-            album_data: dict[str, Any]= {
-                                        'album_type': data['album_type'],
-                                        'artists': data['artists'],
-                                        'available_markets': data['available_markets'],
-                                        'external_urls': data['external_urls'],
-                                        'href': data['href'],
-                                        'id': data['id'],
-                                        'images': data['images'],
-                                        'name': data['name'],
-                                        'release_date': data['release_date'],
-                                        'release_date_precision': data['release_date_precision'],
-                                        'total_tracks': data['total_tracks'],
-                                        'type': data['type'],
-                                        'uri': data['uri'],
-                                        }
-            tracks = []
-            for track in data['tracks']['items']:
-                track['album'] = album_data
-                if iterator:
-                    tracks.append(track)
-                else:
-                    tracks.append(SpotifyTrack(track))
-
-            return tracks
-
-        elif data['type'] == 'playlist':
-            if iterator:
-                if not data['tracks']['next']:
-                    return [t['track'] for t in data['tracks']['items']]
-
-                url = data['tracks']['next']
-
-                items = [t['track'] for t in data['tracks']['items']]
-                while True:
-                    async with self.session.get(url, headers=self.bearer_headers) as resp:
-                        data = await resp.json()
-
-                        items.extend([t['track'] for t in data['items']])
-                        if not data['next']:
-                            return items
-
-                        url = data['next']
-            else:
-                tracks = data['tracks']['items']
-                return [SpotifyTrack(t) for t in tracks]
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import asyncio
+import base64
+import enum
+import re
+import time
+from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
+
+import aiohttp
+from nextcord.ext import commands
+
+import wavelink
+from wavelink import Node, NodePool
+
+if TYPE_CHECKING:
+    from wavelink import Player, Playable
+
+
+__all__ = ('SpotifySearchType',
+           'SpotifyClient',
+           'SpotifyTrack',
+           'SpotifyRequestError',
+           'decode_url')
+
+
+GRANTURL = 'https://accounts.spotify.com/api/token?grant_type=client_credentials'
+URLREGEX = re.compile(r'(https?://open.)?(spotify)(.com/|:)'
+                      r'(?P<type>album|playlist|track|artist)([/:])'
+                      r'(?P<id>[a-zA-Z0-9]+)(\?si=[a-zA-Z0-9]+)?(&dl_branch=[0-9]+)?')
+BASEURL = 'https://api.spotify.com/v1/{entity}s/{identifier}'
+RECURL = 'https://api.spotify.com/v1/recommendations?seed_tracks={tracks}'
+
+
+ST = TypeVar("ST", bound="Playable")
+
+
+def decode_url(url: str) -> Optional[dict]:
+    """Check whether the given URL is a valid Spotify URL and return it's type and ID.
+
+    Parameters
+    ----------
+    url: str
+        The URL to check.
+
+    Returns
+    -------
+    Optional[dict]
+        An mapping of :class:`SpotifySearchType` and Spotify ID. Type will be either track, album or playlist.
+        If type is not track, album or playlist, a special unusable type is returned.
+
+        Could return None if the URL is invalid.
+
+    Examples
+    --------
+
+    .. code:: python3
+
+        from wavelink.ext import spotify
+
+        ...
+
+        decoded = spotify.decode_url("https://open.spotify.com/track/6BDLcvvtyJD2vnXRDi1IjQ?si=e2e5bd7aaf3d4a2a")
+
+        if decoded and decoded['type'] is spotify.SpotifySearchType.track:
+            track = await spotify.SpotifyTrack.search(query=decoded["id"], type=decoded["type"])
+    """
+    match = URLREGEX.match(url)
+    if match:
+        try:
+            type_ = SpotifySearchType[match['type']]
+        except KeyError:
+            type_ = SpotifySearchType.unusable
+
+        return {'type': type_, 'id': match['id']}
+
+    return None
+
+
+class SpotifySearchType(enum.Enum):
+    """An enum specifying which type to search for with a given Spotify ID.
+
+    Attributes
+    ----------
+    track
+        Default search type. Unless specified otherwise this will always be the search type.
+    album
+        Album search type.
+    playlist
+        Playlist search type.
+    unusable
+        Unusable type. This type is returned when Wavelink can not be used to play this track.
+    """
+    track = 0
+    album = 1
+    playlist = 2
+    unusable = 3
+
+
+class SpotifyAsyncIterator:
+
+    def __init__(self, *, query: str, limit: int, type: SpotifySearchType, node: Node):
+        self._query = query
+        self._limit = limit
+        self._type = type
+        self._node = node
+
+        self._first = True
+        self._count = 0
+        self._queue = asyncio.Queue()
+
+    def __aiter__(self):
+        return self
+
+    async def fill_queue(self):
+        tracks = await self._node._spotify._search(query=self._query, iterator=True, type=self._type)
+
+        for track in tracks:
+            await self._queue.put(track)
+
+    async def __anext__(self):
+        if self._first:
+            await self.fill_queue()
+            self._first = False
+
+        if self._limit is not None and self._count == self._limit:
+            raise StopAsyncIteration
+
+        try:
+            track = self._queue.get_nowait()
+        except asyncio.QueueEmpty as e:
+            raise StopAsyncIteration from e
+
+        if track is None:
+            return await self.__anext__()
+
+        track = SpotifyTrack(track)
+
+        self._count += 1
+        return track
+
+
+class SpotifyRequestError(Exception):
+    """Base error for Spotify requests.
+
+    Attributes
+    ----------
+    status: int
+        The status code returned from the request.
+    reason: Optional[str]
+        The reason the request failed. Could be None.
+    """
+
+    def __init__(self, status: int, reason: Optional[str] = None):
+        self.status = status
+        self.reason = reason
+
+
+class SpotifyTrack:
+    """A track retrieved via Spotify.
+
+    Attributes
+    ----------
+    raw: dict[str, Any]
+        The raw payload from Spotify for this track.
+    album: str
+        The album name this track belongs to.
+    images: list[str]
+        A list of URLs to images associated with this track.
+    artists: list[str]
+        A list of artists for this track.
+    genres: list[str]
+        A list of genres associated with this tracks artist.
+    name: str
+        The track name.
+    title: str
+        An alias to name.
+    uri: str
+        The URI for this spotify track.
+    id: str
+        The spotify ID for this track.
+    isrc: str | None
+        The International Standard Recording Code associated with this track if given.
+    length: int
+        The track length in milliseconds.
+    duration: int
+        Alias to length.
+    """
+
+    __slots__ = (
+        'raw',
+        'album',
+        'images',
+        'artists',
+        'name',
+        'title',
+        'uri',
+        'id',
+        'length',
+        'duration',
+        'isrc',
+        '__dict__'
+    )
+
+    def __init__(self, data: dict[str, Any]) -> None:
+        self.raw: dict[str, Any] = data
+
+        album = data['album']
+        self.album: str = album['name']
+        self.images: list[str] = [i['url'] for i in album['images']]
+
+        artists = data['artists']
+        self.artists: list[str] = [a['name'] for a in artists]
+        # self.genres: list[str] = [a['genres'] for a in artists]
+
+        self.name: str = data['name']
+        self.title: str = self.name
+        self.uri: str = data['uri']
+        self.id: str = data['id']
+        self.length: int = data['duration_ms']
+        self.duration: int = self.length
+
+        self.isrc: str | None = data["external_ids"].get("isrc")
+
+    def __str__(self) -> str:
+        return f'{self.name} - {self.artists[0]}'
+
+    def __repr__(self) -> str:
+        return f'SpotifyTrack(id={self.id}, isrc={self.isrc}, name={self.name}, duration={self.duration})'
+
+    def __eq__(self, other) -> bool:
+        if isinstance(other, SpotifyTrack):
+            return self.id == other.id
+        raise NotImplemented
+
+    @classmethod
+    async def search(
+        cls: Type[ST],
+            query: str,
+            *,
+            type: SpotifySearchType = SpotifySearchType.track,
+            node: Node | None = None,
+    ) -> Union[Optional[ST], List[ST]]:
+        """|coro|
+
+        Search for tracks with the given query.
+
+        Parameters
+        ----------
+        query: str
+            The song to search for.
+        type: Optional[:class:`~SpotifySearchType`]
+            An optional enum value to use when searching with Spotify. Defaults to track.
+        node: Optional[:class:`wavelink.Node`]
+            An optional Node to use to make the search with.
+
+        Returns
+        -------
+        List[:class:`SpotifyTrack`]
+
+        Examples
+        --------
+        Searching for a singular tack to play...
+
+        .. code:: python3
+
+            track: spotify.SpotifyTrack = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+
+
+        Searching for all tracks in an album...
+
+        .. code:: python3
+
+            tracks: list[spotify.SpotifyTrack] =
+            await spotify.SpotifyTrack.search(query=SPOTIFY_URL, type=spotify.SpotifySearchType.album)
+
+
+        .. note::
+
+            See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
+            Before using this method.
+        """
+        if node is None:
+            node: Node = NodePool.get_connected_node()
+
+        return await node._spotify._search(query=query, type=type)
+
+    @classmethod
+    def iterator(cls,
+                 *,
+                 query: str,
+                 limit: int | None = None,
+                 type: SpotifySearchType = SpotifySearchType.playlist,
+                 node: Node | None = None,
+                 ):
+        """An async iterator version of search.
+
+        This can be useful when searching for large playlists or albums with Spotify.
+
+        Parameters
+        ----------
+        query: str
+            The Spotify URL or ID to search for. Must be of type Playlist or Album.
+        limit: Optional[int]
+            Limit the amount of tracks returned.
+        type: :class:`~SpotifySearchType`
+            The type of search. Must be either playlist or album. Defaults to playlist.
+        node: Optional[:class:`wavelink.Node`]
+            An optional node to use when querying for tracks. Defaults to the best available.
+
+        Examples
+        --------
+
+        .. code:: python3
+
+                async for track in spotify.SpotifyTrack.iterator(query=..., type=spotify.SpotifySearchType.playlist):
+                    ...
+
+
+        .. note::
+
+            See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
+            Before using this method.
+        """
+
+        if type is not SpotifySearchType.album and type is not SpotifySearchType.playlist:
+            raise TypeError("Iterator search type must be either album or playlist.")
+
+        if node is None:
+            node = NodePool.get_connected_node()
+
+        return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=type)
+
+    @classmethod
+    async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
+        """Converter which searches for and returns the first track.
+
+        Used as a type hint in a
+        `nextcord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
+        """
+        results = await cls.search(argument)
+
+        if not results:
+            raise commands.BadArgument(f"Could not find any songs matching query: {argument}")
+
+        return results[0]
+
+    async def fulfill(self, *, player: Player, cls: Playable, populate: bool) -> Playable:
+        """Used to fulfill the :class:`wavelink.Player` Auto Play Queue.
+
+        .. warning::
+
+            Usually you would not call this directly. Instead you would set :attr:`wavelink.Player.autoplay` to true,
+            and allow the player to fulfill this request automatically.
+
+
+        Parameters
+        ----------
+        player: :class:`wavelink.player.Player`
+            If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
+        cls
+            The class to convert this Spotify Track to.
+        """
+        tracks: list[cls] = await cls.search(f'"{self.isrc}"')
+        if not tracks:
+            tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
+
+        if not player.autoplay or not populate:
+            return tracks[0]
+
+        node: Node = player.current_node
+        sc: SpotifyClient | None = node._spotify
+
+        if not sc:
+            raise RuntimeError(f"There is no spotify client associated with <{node:!r}>")
+
+        if sc.is_token_expired():
+            await sc._get_bearer_token()
+
+        if len(player._track_seeds) == 5:
+            player._track_seeds.pop(0)
+
+        player._track_seeds.append(self.id)
+
+        url: str = RECURL.format(tracks=','.join(player._track_seeds))
+        async with node._session.get(url=url, headers=sc.bearer_headers) as resp:
+            if resp.status != 200:
+                raise SpotifyRequestError(resp.status, resp.reason)
+
+            data = await resp.json()
+
+        recos = [SpotifyTrack(t) for t in data['tracks']]
+        for reco in recos:
+            if reco in player.auto_queue or reco in player.auto_queue.history:
+                pass
+
+            await player.auto_queue.put_wait(reco)
+
+        return tracks[0]
+
+
+class SpotifyClient:
+    """Spotify client passed to :class:`wavelink.Node` for searching via Spotify.
+
+    Parameters
+    ----------
+    client_id: str
+        Your spotify application client ID.
+    client_secret: str
+        Your spotify application secret.
+    """
+
+    def __init__(self, *, client_id: str, client_secret: str):
+        self._client_id = client_id
+        self._client_secret = client_secret
+
+        self.session = aiohttp.ClientSession()
+
+        self._bearer_token: str | None = None
+        self._expiry: int = 0
+
+    @property
+    def grant_headers(self) -> dict:
+        authbytes = f'{self._client_id}:{self._client_secret}'.encode()
+        return {'Authorization': f'Basic {base64.b64encode(authbytes).decode()}',
+                'Content-Type': 'application/x-www-form-urlencoded'}
+
+    @property
+    def bearer_headers(self) -> dict:
+        return {'Authorization': f'Bearer {self._bearer_token}'}
+
+    async def _get_bearer_token(self) -> None:
+        async with self.session.post(GRANTURL, headers=self.grant_headers) as resp:
+            if resp.status != 200:
+                raise SpotifyRequestError(resp.status, resp.reason)
+
+            data = await resp.json()
+            self._bearer_token = data['access_token']
+            self._expiry = time.time() + (int(data['expires_in']) - 10)
+
+    def is_token_expired(self) -> bool:
+        return time.time() >= self._expiry
+
+    async def _search(self,
+                      query: str,
+                      type: SpotifySearchType = SpotifySearchType.track,
+                      iterator: bool = False,
+                      ) -> list[SpotifyTrack]:
+
+        if self.is_token_expired():
+            await self._get_bearer_token()
+
+        regex_result = URLREGEX.match(query)
+
+        url = (
+            BASEURL.format(
+                entity=regex_result['type'], identifier=regex_result['id']
+            )
+            if regex_result
+            else BASEURL.format(entity=type.name, identifier=query)
+        )
+        async with self.session.get(url, headers=self.bearer_headers) as resp:
+            if resp.status != 200:
+                raise SpotifyRequestError(resp.status, resp.reason)
+
+            data = await resp.json()
+
+        if data['type'] == 'track':
+            return [SpotifyTrack(data)]
+
+        elif data['type'] == 'album':
+            album_data: dict[str, Any]= {
+                                        'album_type': data['album_type'],
+                                        'artists': data['artists'],
+                                        'available_markets': data['available_markets'],
+                                        'external_urls': data['external_urls'],
+                                        'href': data['href'],
+                                        'id': data['id'],
+                                        'images': data['images'],
+                                        'name': data['name'],
+                                        'release_date': data['release_date'],
+                                        'release_date_precision': data['release_date_precision'],
+                                        'total_tracks': data['total_tracks'],
+                                        'type': data['type'],
+                                        'uri': data['uri'],
+                                        }
+            tracks = []
+            for track in data['tracks']['items']:
+                track['album'] = album_data
+                if iterator:
+                    tracks.append(track)
+                else:
+                    tracks.append(SpotifyTrack(track))
+
+            return tracks
+
+        elif data['type'] == 'playlist':
+            if iterator:
+                if not data['tracks']['next']:
+                    return [t['track'] for t in data['tracks']['items']]
+
+                url = data['tracks']['next']
+
+                items = [t['track'] for t in data['tracks']['items']]
+                while True:
+                    async with self.session.get(url, headers=self.bearer_headers) as resp:
+                        data = await resp.json()
+
+                        items.extend([t['track'] for t in data['items']])
+                        if not data['next']:
+                            return items
+
+                        url = data['next']
+            else:
+                tracks = data['tracks']['items']
+                return [SpotifyTrack(t) for t in tracks]
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/node.py` & `WavelinkCord-2.5.2b0/wavelink/node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,537 +1,538 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import logging
-import random
-import re
-import string
-from typing import TYPE_CHECKING, Any, TypeVar
-
-import aiohttp
-import nextcord
-from nextcord.enums import try_enum
-from nextcord.utils import MISSING, classproperty
-import urllib.parse
-
-from .enums import LoadType, NodeStatus
-from .exceptions import *
-from .websocket import Websocket
-
-if TYPE_CHECKING:
-    from .player import Player
-    from .tracks import *
-    from .types.request import Request
-    from .ext import spotify as spotify_
-
-    PlayableT = TypeVar('PlayableT', bound=Playable)
-    
-
-__all__ = ('Node', 'NodePool')
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-# noinspection PyShadowingBuiltins
-class Node:
-    """The base Wavelink Node.
-
-    The Node is responsible for keeping the Websocket alive, tracking the state of Players
-    and fetching/decoding Tracks and Playlists.
-
-    .. note::
-
-        The Node class should only be created once per Lavalink connection.
-        To retrieve a Node use the appropriate :class:`NodePool` methods instead.
-
-    .. warning::
-
-        The Node will not be connected until passed to :meth:`NodePool.connect`.
-
-    Parameters
-    ----------
-    id: Optional[str]
-        The unique identifier for this Node. If not passed, one will be generated randomly.
-    uri: str
-        The uri to connect to your Lavalink server. E.g ``http://localhost:2333``.
-    password: str
-        The password used to connect to your Lavalink server.
-    secure: Optional[bool]
-        Whether the connection should use https/wss.
-    use_http: Optional[bool]
-        Whether to use http:// over ws:// when connecting to the Lavalink websocket. Defaults to False.
-    session: Optional[aiohttp.ClientSession]
-        The session to use for this Node. If no session is passed a default will be used.
-    heartbeat: float
-        The time in seconds to send a heartbeat ack. Defaults to 15.0.
-    retries: Optional[int]
-        The amount of times this Node will try to reconnect after a disconnect.
-        If not set the Node will try unlimited times.
-
-    Attributes
-    ----------
-    heartbeat: float
-        The time in seconds to send a heartbeat ack. Defaults to 15.0.
-    client: :class:`nextcord.Client`
-        The nextcord client used to connect this Node. Could be None if this Node has not been connected.
-    """
-
-    def __init__(
-            self,
-            *,
-            id: str | None = None,
-            uri: str,
-            password: str,
-            secure: bool = False,
-            use_http: bool = False,
-            session: aiohttp.ClientSession = MISSING,
-            heartbeat: float = 15.0,
-            retries: int | None = None,
-    ) -> None:
-        if id is None:
-            id = ''.join(random.sample(string.ascii_letters + string.digits, 12))
-
-        self._id: str = id
-        self._uri: str = uri
-        self._secure: bool = secure
-        self._use_http: bool = use_http
-        host: str = re.sub(r'(?:http|ws)s?://', '', self._uri)
-        self._host: str = f'{"https://" if secure else "http://"}{host}'
-        self._password: str = password
-
-        self._session: aiohttp.ClientSession = session
-        self.heartbeat: float = heartbeat
-        self._retries: int | None = retries
-
-        self.client: nextcord.Client | None = None
-        self._websocket: Websocket = MISSING
-        self._session_id: str | None = None
-
-        self._players: dict[int, Player] = {}
-
-        self._status: NodeStatus = NodeStatus.DISCONNECTED
-        self._major_version: int | None = None
-
-        self._spotify: spotify_.SpotifyClient | None = None
-
-    def __repr__(self) -> str:
-        return f'Node: id="{self._id}", uri="{self.uri}", status={self.status}'
-
-    def __eq__(self, other: object) -> bool:
-        return self.id == other.id if isinstance(other, Node) else NotImplemented
-
-    @property
-    def id(self) -> str:
-        """The Nodes unique identifier."""
-        return self._id
-
-    @property
-    def uri(self) -> str:
-        """The URI used to connect this Node to Lavalink."""
-        return self._host
-
-    @property
-    def password(self) -> str:
-        """The password used to connect this Node to Lavalink."""
-        return self._password
-
-    @property
-    def players(self) -> dict[int, Player]:
-        """A mapping of Guild ID to Player."""
-        return self._players
-
-    @property
-    def status(self) -> NodeStatus:
-        """The connection status of this Node.
-
-        DISCONNECTED
-        CONNECTING
-        CONNECTED
-        """
-        return self._status
-
-    def get_player(self, guild_id: int, /) -> Player | None:
-        """Return the :class:`player.Player` associated with the provided guild ID.
-
-        If no :class:`player.Player` is found, returns None.
-
-        Parameters
-        ----------
-        guild_id: int
-            The Guild ID to return a Player for.
-
-        Returns
-        -------
-        Optional[:class:`player.Player`]
-        """
-        return self._players.get(guild_id, None)
-
-    async def _connect(self, client: nextcord.Client) -> None:
-        if client.user is None:
-            raise RuntimeError('')
-
-        if not self._session:
-            self._session = aiohttp.ClientSession(headers={'Authorization': self._password})
-
-        self.client = client
-
-        self._websocket = Websocket(node=self)
-
-        await self._websocket.connect()
-
-        async with self._session.get(f'{self._host}/version') as resp:
-            version: str = await resp.text()
-
-            if version.endswith('-SNAPSHOT'):
-                self._major_version = 3
-                return
-
-            version_tuple = tuple(int(v) for v in version.split('.'))
-            if version_tuple[0] < 3:
-                raise InvalidLavalinkVersion(f'Wavelink 2 is not compatible with Lavalink "{version}".')
-
-            if version_tuple[0] == 3 and version_tuple[1] < 7:
-                raise InvalidLavalinkVersion('Wavelink 2 is not compatible with Lavalink versions under "3.7".')
-
-            self._major_version = version_tuple[0]
-
-    async def _send(self,
-                    *,
-                    method: str,
-                    path: str,
-                    guild_id: int | str | None = None,
-                    query: str | None = None,
-                    data: Request | None = None,
-                    ) -> dict[str, Any] | None:
-
-        uri: str = f'{self._host}/' \
-                   f'v{self._major_version}/' \
-                   f'{path}' \
-                   f'{f"/{guild_id}" if guild_id else ""}' \
-                   f'{f"?{query}" if query else ""}'
-
-        async with self._session.request(method=method, url=uri, json=data or {}) as resp:
-            if resp.status >= 300:
-                raise InvalidLavalinkResponse(f'An error occurred when attempting to reach: "{uri}".',
-                                              status=resp.status)
-
-            if resp.status == 204:
-                return
-
-            return await resp.json()
-
-    async def get_tracks(self, cls: type[PlayableT], query: str) -> list[PlayableT]:
-        """|coro|
-
-        Search for and retrieve Tracks based on the query and cls provided.
-
-        .. note::
-
-            If the query is not a Local search or direct URL, you will need to provide a search prefix.
-            E.g. ``ytsearch:`` for a YouTube search.
-
-        Parameters
-        ----------
-        cls: type[PlayableT]
-            The type of Playable tracks that should be returned.
-        query: str
-            The query to search for and return tracks.
-
-        Returns
-        -------
-        list[PlayableT]
-            A list of found tracks converted to the provided cls.
-        """
-        data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
-        load_type = try_enum(LoadType, data.get("loadType"))
-
-        if load_type is LoadType.load_failed:
-            # TODO - Proper Exception...
-
-            raise ValueError('Track Failed to load.')
-
-        if load_type is LoadType.no_matches:
-            return []
-
-        if load_type is LoadType.track_loaded:
-            track_data = data["tracks"][0]
-            return [cls(track_data)]
-
-        if load_type is not LoadType.search_result:
-            # TODO - Proper Exception...
-
-            raise ValueError('Track Failed to load.')
-
-        return [cls(track_data) for track_data in data["tracks"]]
-
-    async def get_playlist(self, cls: Playlist, query: str):
-        """|coro|
-
-        Search for and return a :class:`tracks.Playlist` given an identifier.
-
-        Parameters
-        ----------
-        cls: Type[:class:`tracks.Playlist`]
-            The type of which playlist should be returned, this must subclass :class:`tracks.Playlist`.
-        query: str
-            The playlist's identifier. This may be a YouTube playlist URL for example.
-
-        Returns
-        -------
-        Optional[:class:`tracks.Playlist`]:
-            The related wavelink track object or ``None`` if none was found.
-
-        Raises
-        ------
-        ValueError
-            Loading the playlist failed.
-        WavelinkException
-            An unspecified error occurred when loading the playlist.
-        """
-        data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
-
-        load_type = try_enum(LoadType, data.get("loadType"))
-
-        if load_type is LoadType.load_failed:
-            # TODO Proper exception...
-            raise ValueError('Tracks failed to Load.')
-
-        if load_type is LoadType.no_matches:
-            return None
-
-        if load_type is not LoadType.playlist_loaded:
-            raise WavelinkException("Track failed to load.")
-
-        return cls(data)
-
-    async def build_track(self, *, cls: type[PlayableT], encoded: str) -> PlayableT:
-        """|coro|
-
-        Build a track from the provided encoded string with the given Track class.
-
-        Parameters
-        ----------
-        cls: type[PlayableT]
-            The type of Playable track that should be returned.
-        encoded: str
-            The Tracks unique encoded string.
-        """
-        encoded = urllib.parse.quote(encoded)
-        data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded}')
-
-        return cls(data=data)
-
-
-# noinspection PyShadowingBuiltins
-class NodePool:
-    """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
-
-    Attributes
-    ----------
-    nodes: dict[str, :class:`Node`]
-        A mapping of :class:`Node` identifier to :class:`Node`.
-
-
-    .. warning::
-
-        This class should never be initialised. All methods are class methods.
-    """
-
-    __nodes: dict[str, Node] = {}
-
-    @classmethod
-    async def connect(
-            cls,
-            *,
-            client: nextcord.Client,
-            nodes: list[Node],
-            spotify: spotify_.SpotifyClient | None = None
-    ) -> dict[str, Node]:
-        """|coro|
-
-        Connect a list of Nodes.
-
-        Parameters
-        ----------
-        client: :class:`nextcord.Client`
-            The nextcord Client or Bot used to connect the Nodes.
-        nodes: list[:class:`Node`]
-            A list of Nodes to connect.
-        spotify: Optional[:class:`ext.spotify.SpotifyClient`]
-            The spotify Client to use when searching for Spotify Tracks.
-
-        Returns
-        -------
-        dict[str, :class:`Node`]
-            A mapping of :class:`Node` identifier to :class:`Node`.
-        """
-        if client.user is None:
-            raise RuntimeError('')
-
-        for node in nodes:
-
-            if spotify:
-                node._spotify = spotify
-
-            if node.id in cls.__nodes:
-                logger.error(f'A Node with the ID "{node.id}" already exists on the NodePool. Disregarding.')
-                continue
-
-            try:
-                await node._connect(client)
-            except AuthorizationFailed:
-                logger.error(f'The Node <{node!r}> failed to authenticate properly. '
-                             f'Please check your password and try again.')
-            else:
-                cls.__nodes[node.id] = node
-
-        return cls.nodes
-
-    @classproperty
-    def nodes(cls) -> dict[str, Node]:
-        """A mapping of :class:`Node` identifier to :class:`Node`."""
-        return cls.__nodes
-
-    @classmethod
-    def get_node(cls, id: str | None = None) -> Node:
-        """Retrieve a :class:`Node` with the given ID or best, if no ID was passed.
-
-        Parameters
-        ----------
-        id: Optional[str]
-            The unique identifier of the :class:`Node` to retrieve. If not passed the best :class:`Node`
-            will be fetched.
-
-        Returns
-        -------
-        :class:`Node`
-
-        Raises
-        ------
-        InvalidNode
-            The given id does nto resolve to a :class:`Node` or no :class:`Node` has been connected.
-        """
-        if id:
-            if id not in cls.__nodes:
-                raise InvalidNode(f'A Node with ID "{id}" does not exist on the Wavelink NodePool.')
-
-            return cls.__nodes[id]
-
-        if not cls.__nodes:
-            raise InvalidNode('No Node currently exists on the Wavelink NodePool.')
-
-        nodes = cls.__nodes.values()
-        return sorted(nodes, key=lambda n: len(n.players))[0]
-
-    @classmethod
-    def get_connected_node(cls) -> Node:
-        """Get the best available connected :class:`Node`.
-
-        Returns
-        -------
-        :class:`Node`
-            The best available connected Node.
-
-        Raises
-        ------
-        InvalidNode
-            No Nodes are currently in the connected state.
-        """
-
-        nodes: list[Node] = [n for n in cls.__nodes.values() if n.status is NodeStatus.CONNECTED]
-        if not nodes:
-            raise InvalidNode('There are no Nodes on the Wavelink NodePool that are currently in the connected state.')
-
-        return sorted(nodes, key=lambda n: len(n.players))[0]
-
-    @classmethod
-    async def get_tracks(cls_,  # type: ignore
-                         query: str,
-                         /,
-                         *,
-                         cls: type[PlayableT],
-                         node: Node | None = None
-                         ) -> list[PlayableT]:
-        """|coro|
-
-        Helper method to retrieve tracks from the NodePool without fetching a :class:`Node`.
-
-        Parameters
-        ----------
-        query: str
-            The query to search for and return tracks.
-        cls: type[PlayableT]
-            The type of Playable tracks that should be returned.
-        node: Optional[:class:`Node`]
-            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
-            Defaults to None.
-
-        Returns
-        -------
-        list[PlayableT]
-            A list of found tracks converted to the provided cls.
-        """
-        if not node:
-            node = cls_.get_connected_node()
-
-        return await node.get_tracks(cls=cls, query=query)
-
-    @classmethod
-    async def get_playlist(cls_,  # type: ignore
-                           query: str,
-                           /,
-                           *,
-                           cls: Playlist,
-                           node: Node | None = None
-                           ) -> Playlist:
-        """|coro|
-
-        Helper method to retrieve a playlist from the NodePool without fetching a :class:`Node`.
-
-
-        .. warning::
-
-            The only playlist currently supported is :class:`tracks.YouTubePlaylist`.
-
-
-        Parameters
-        ----------
-        query: str
-            The query to search for and return a playlist.
-        cls: type[PlayableT]
-            The type of Playlist that should be returned.
-        node: Optional[:class:`Node`]
-            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
-            Defaults to None.
-
-        Returns
-        -------
-        Playlist
-            A Playlist with its tracks.
-        """
-        if not node:
-            node = cls_.get_connected_node()
-
-        return await node.get_playlist(cls=cls, query=query)
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import logging
+import random
+import re
+import string
+from typing import TYPE_CHECKING, Any, TypeVar
+
+import aiohttp
+import nextcord
+from nextcord.enums import try_enum
+from nextcord.utils import MISSING, classproperty
+import urllib.parse
+
+from .enums import LoadType, NodeStatus
+from .exceptions import *
+from .websocket import Websocket
+
+if TYPE_CHECKING:
+    from .player import Player
+    from .tracks import *
+    from .types.request import Request
+    from .ext import spotify as spotify_
+
+    PlayableT = TypeVar('PlayableT', bound=Playable)
+    
+
+__all__ = ('Node', 'NodePool')
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+# noinspection PyShadowingBuiltins
+class Node:
+    """The base Wavelink Node.
+
+    The Node is responsible for keeping the Websocket alive, tracking the state of Players
+    and fetching/decoding Tracks and Playlists.
+
+    .. note::
+
+        The Node class should only be created once per Lavalink connection.
+        To retrieve a Node use the appropriate :class:`NodePool` methods instead.
+
+    .. warning::
+
+        The Node will not be connected until passed to :meth:`NodePool.connect`.
+
+    Parameters
+    ----------
+    id: Optional[str]
+        The unique identifier for this Node. If not passed, one will be generated randomly.
+    uri: str
+        The uri to connect to your Lavalink server. E.g ``http://localhost:2333``.
+    password: str
+        The password used to connect to your Lavalink server.
+    secure: Optional[bool]
+        Whether the connection should use https/wss.
+    use_http: Optional[bool]
+        Whether to use http:// over ws:// when connecting to the Lavalink websocket. Defaults to False.
+    session: Optional[aiohttp.ClientSession]
+        The session to use for this Node. If no session is passed a default will be used.
+    heartbeat: float
+        The time in seconds to send a heartbeat ack. Defaults to 15.0.
+    retries: Optional[int]
+        The amount of times this Node will try to reconnect after a disconnect.
+        If not set the Node will try unlimited times.
+
+    Attributes
+    ----------
+    heartbeat: float
+        The time in seconds to send a heartbeat ack. Defaults to 15.0.
+    client: :class:`nextcord.Client`
+        The nextcord client used to connect this Node. Could be None if this Node has not been connected.
+    """
+
+    def __init__(
+            self,
+            *,
+            id: str | None = None,
+            uri: str,
+            password: str,
+            secure: bool = False,
+            use_http: bool = False,
+            session: aiohttp.ClientSession = MISSING,
+            heartbeat: float = 15.0,
+            retries: int | None = None,
+    ) -> None:
+        if id is None:
+            id = ''.join(random.sample(string.ascii_letters + string.digits, 12))
+
+        self._id: str = id
+        self._uri: str = uri
+        self._secure: bool = secure
+        self._use_http: bool = use_http
+        host: str = re.sub(r'(?:http|ws)s?://', '', self._uri)
+        self._host: str = f'{"https://" if secure else "http://"}{host}'
+        self._password: str = password
+
+        self._session: aiohttp.ClientSession = session
+        self.heartbeat: float = heartbeat
+        self._retries: int | None = retries
+
+        self.client: nextcord.Client | None = None
+        self._websocket: Websocket = MISSING
+        self._session_id: str | None = None
+
+        self._players: dict[int, Player] = {}
+
+        self._status: NodeStatus = NodeStatus.DISCONNECTED
+        self._major_version: int | None = None
+
+        self._spotify: spotify_.SpotifyClient | None = None
+
+    def __repr__(self) -> str:
+        return f'Node: id="{self._id}", uri="{self.uri}", status={self.status}'
+
+    def __eq__(self, other: object) -> bool:
+        return self.id == other.id if isinstance(other, Node) else NotImplemented
+
+    @property
+    def id(self) -> str:
+        """The Nodes unique identifier."""
+        return self._id
+
+    @property
+    def uri(self) -> str:
+        """The URI used to connect this Node to Lavalink."""
+        return self._host
+
+    @property
+    def password(self) -> str:
+        """The password used to connect this Node to Lavalink."""
+        return self._password
+
+    @property
+    def players(self) -> dict[int, Player]:
+        """A mapping of Guild ID to Player."""
+        return self._players
+
+    @property
+    def status(self) -> NodeStatus:
+        """The connection status of this Node.
+
+        DISCONNECTED
+        CONNECTING
+        CONNECTED
+        """
+        return self._status
+
+    def get_player(self, guild_id: int, /) -> Player | None:
+        """Return the :class:`player.Player` associated with the provided guild ID.
+
+        If no :class:`player.Player` is found, returns None.
+
+        Parameters
+        ----------
+        guild_id: int
+            The Guild ID to return a Player for.
+
+        Returns
+        -------
+        Optional[:class:`player.Player`]
+        """
+        return self._players.get(guild_id, None)
+
+    async def _connect(self, client: nextcord.Client) -> None:
+        if client.user is None:
+            raise RuntimeError('')
+
+        if not self._session:
+            self._session = aiohttp.ClientSession(headers={'Authorization': self._password})
+
+        self.client = client
+
+        self._websocket = Websocket(node=self)
+
+        await self._websocket.connect()
+
+        async with self._session.get(f'{self._host}/version') as resp:
+            version: str = await resp.text()
+
+            if version.endswith('-SNAPSHOT'):
+                self._major_version = 3
+                return
+
+            version_tuple = tuple(int(v) for v in version.split('.'))
+            if version_tuple[0] < 3:
+                raise InvalidLavalinkVersion(f'Wavelink 2 is not compatible with Lavalink "{version}".')
+
+            if version_tuple[0] == 3 and version_tuple[1] < 7:
+                raise InvalidLavalinkVersion('Wavelink 2 is not compatible with Lavalink versions under "3.7".')
+
+            self._major_version = version_tuple[0]
+
+    async def _send(self,
+                    *,
+                    method: str,
+                    path: str,
+                    guild_id: int | str | None = None,
+                    query: str | None = None,
+                    data: Request | None = None,
+                    ) -> dict[str, Any] | None:
+
+        uri: str = f'{self._host}/' \
+                   f'v{self._major_version}/' \
+                   f'{path}' \
+                   f'{f"/{guild_id}" if guild_id else ""}' \
+                   f'{f"?{query}" if query else ""}'
+
+        async with self._session.request(method=method, url=uri, json=data or {}) as resp:
+            if resp.status >= 300:
+                raise InvalidLavalinkResponse(f'An error occurred when attempting to reach: "{uri}".',
+                                              status=resp.status)
+
+            if resp.status == 204:
+                return
+
+            return await resp.json()
+
+    async def get_tracks(self, cls: type[PlayableT], query: str) -> list[PlayableT]:
+        """|coro|
+
+        Search for and retrieve Tracks based on the query and cls provided.
+
+        .. note::
+
+            If the query is not a Local search or direct URL, you will need to provide a search prefix.
+            E.g. ``ytsearch:`` for a YouTube search.
+
+        Parameters
+        ----------
+        cls: type[PlayableT]
+            The type of Playable tracks that should be returned.
+        query: str
+            The query to search for and return tracks.
+
+        Returns
+        -------
+        list[PlayableT]
+            A list of found tracks converted to the provided cls.
+        """
+        data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
+        load_type = try_enum(LoadType, data.get("loadType"))
+
+        if load_type is LoadType.load_failed:
+            # TODO - Proper Exception...
+
+            raise ValueError('Track Failed to load.')
+
+        if load_type is LoadType.no_matches:
+            return []
+
+        if load_type is LoadType.track_loaded:
+            track_data = data["tracks"][0]
+            return [cls(track_data)]
+
+        if load_type is not LoadType.search_result:
+            # TODO - Proper Exception...
+
+            raise ValueError('Track Failed to load.')
+
+        return [cls(track_data) for track_data in data["tracks"]]
+
+    async def get_playlist(self, cls: Playlist, query: str):
+        """|coro|
+
+        Search for and return a :class:`tracks.Playlist` given an identifier.
+
+        Parameters
+        ----------
+        cls: Type[:class:`tracks.Playlist`]
+            The type of which playlist should be returned, this must subclass :class:`tracks.Playlist`.
+        query: str
+            The playlist's identifier. This may be a YouTube playlist URL for example.
+
+        Returns
+        -------
+        Optional[:class:`tracks.Playlist`]:
+            The related wavelink track object or ``None`` if none was found.
+
+        Raises
+        ------
+        ValueError
+            Loading the playlist failed.
+        WavelinkException
+            An unspecified error occurred when loading the playlist.
+        """
+        encoded_query = urllib.parse.quote(query)
+        data = await self._send(method='GET', path='loadtracks', query=f'identifier={encoded_query}')
+
+        load_type = try_enum(LoadType, data.get("loadType"))
+
+        if load_type is LoadType.load_failed:
+            # TODO Proper exception...
+            raise ValueError('Tracks failed to Load.')
+
+        if load_type is LoadType.no_matches:
+            return None
+
+        if load_type is not LoadType.playlist_loaded:
+            raise WavelinkException("Track failed to load.")
+
+        return cls(data)
+
+    async def build_track(self, *, cls: type[PlayableT], encoded: str) -> PlayableT:
+        """|coro|
+
+        Build a track from the provided encoded string with the given Track class.
+
+        Parameters
+        ----------
+        cls: type[PlayableT]
+            The type of Playable track that should be returned.
+        encoded: str
+            The Tracks unique encoded string.
+        """
+        encoded_query = urllib.parse.quote(encoded)
+        data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded_query}')
+
+        return cls(data=data)
+
+
+# noinspection PyShadowingBuiltins
+class NodePool:
+    """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
+
+    Attributes
+    ----------
+    nodes: dict[str, :class:`Node`]
+        A mapping of :class:`Node` identifier to :class:`Node`.
+
+
+    .. warning::
+
+        This class should never be initialised. All methods are class methods.
+    """
+
+    __nodes: dict[str, Node] = {}
+
+    @classmethod
+    async def connect(
+            cls,
+            *,
+            client: nextcord.Client,
+            nodes: list[Node],
+            spotify: spotify_.SpotifyClient | None = None
+    ) -> dict[str, Node]:
+        """|coro|
+
+        Connect a list of Nodes.
+
+        Parameters
+        ----------
+        client: :class:`nextcord.Client`
+            The nextcord Client or Bot used to connect the Nodes.
+        nodes: list[:class:`Node`]
+            A list of Nodes to connect.
+        spotify: Optional[:class:`ext.spotify.SpotifyClient`]
+            The spotify Client to use when searching for Spotify Tracks.
+
+        Returns
+        -------
+        dict[str, :class:`Node`]
+            A mapping of :class:`Node` identifier to :class:`Node`.
+        """
+        if client.user is None:
+            raise RuntimeError('')
+
+        for node in nodes:
+
+            if spotify:
+                node._spotify = spotify
+
+            if node.id in cls.__nodes:
+                logger.error(f'A Node with the ID "{node.id}" already exists on the NodePool. Disregarding.')
+                continue
+
+            try:
+                await node._connect(client)
+            except AuthorizationFailed:
+                logger.error(f'The Node <{node!r}> failed to authenticate properly. '
+                             f'Please check your password and try again.')
+            else:
+                cls.__nodes[node.id] = node
+
+        return cls.nodes
+
+    @classproperty
+    def nodes(cls) -> dict[str, Node]:
+        """A mapping of :class:`Node` identifier to :class:`Node`."""
+        return cls.__nodes
+
+    @classmethod
+    def get_node(cls, id: str | None = None) -> Node:
+        """Retrieve a :class:`Node` with the given ID or best, if no ID was passed.
+
+        Parameters
+        ----------
+        id: Optional[str]
+            The unique identifier of the :class:`Node` to retrieve. If not passed the best :class:`Node`
+            will be fetched.
+
+        Returns
+        -------
+        :class:`Node`
+
+        Raises
+        ------
+        InvalidNode
+            The given id does nto resolve to a :class:`Node` or no :class:`Node` has been connected.
+        """
+        if id:
+            if id not in cls.__nodes:
+                raise InvalidNode(f'A Node with ID "{id}" does not exist on the Wavelink NodePool.')
+
+            return cls.__nodes[id]
+
+        if not cls.__nodes:
+            raise InvalidNode('No Node currently exists on the Wavelink NodePool.')
+
+        nodes = cls.__nodes.values()
+        return sorted(nodes, key=lambda n: len(n.players))[0]
+
+    @classmethod
+    def get_connected_node(cls) -> Node:
+        """Get the best available connected :class:`Node`.
+
+        Returns
+        -------
+        :class:`Node`
+            The best available connected Node.
+
+        Raises
+        ------
+        InvalidNode
+            No Nodes are currently in the connected state.
+        """
+
+        nodes: list[Node] = [n for n in cls.__nodes.values() if n.status is NodeStatus.CONNECTED]
+        if not nodes:
+            raise InvalidNode('There are no Nodes on the Wavelink NodePool that are currently in the connected state.')
+
+        return sorted(nodes, key=lambda n: len(n.players))[0]
+
+    @classmethod
+    async def get_tracks(cls_,  # type: ignore
+                         query: str,
+                         /,
+                         *,
+                         cls: type[PlayableT],
+                         node: Node | None = None
+                         ) -> list[PlayableT]:
+        """|coro|
+
+        Helper method to retrieve tracks from the NodePool without fetching a :class:`Node`.
+
+        Parameters
+        ----------
+        query: str
+            The query to search for and return tracks.
+        cls: type[PlayableT]
+            The type of Playable tracks that should be returned.
+        node: Optional[:class:`Node`]
+            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
+            Defaults to None.
+
+        Returns
+        -------
+        list[PlayableT]
+            A list of found tracks converted to the provided cls.
+        """
+        if not node:
+            node = cls_.get_connected_node()
+
+        return await node.get_tracks(cls=cls, query=query)
+
+    @classmethod
+    async def get_playlist(cls_,  # type: ignore
+                           query: str,
+                           /,
+                           *,
+                           cls: Playlist,
+                           node: Node | None = None
+                           ) -> Playlist:
+        """|coro|
+
+        Helper method to retrieve a playlist from the NodePool without fetching a :class:`Node`.
+
+
+        .. warning::
+
+            The only playlist currently supported is :class:`tracks.YouTubePlaylist`.
+
+
+        Parameters
+        ----------
+        query: str
+            The query to search for and return a playlist.
+        cls: type[PlayableT]
+            The type of Playlist that should be returned.
+        node: Optional[:class:`Node`]
+            The node to use for retrieving tracks. If not passed, the best :class:`Node` will be used.
+            Defaults to None.
+
+        Returns
+        -------
+        Playlist
+            A Playlist with its tracks.
+        """
+        if not node:
+            node = cls_.get_connected_node()
+
+        return await node.get_playlist(cls=cls, query=query)
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/player.py` & `WavelinkCord-2.5.2b0/wavelink/player.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,589 +1,633 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import datetime
-import logging
-from typing import TYPE_CHECKING, Any, Union
-
-import nextcord
-from nextcord.utils import MISSING
-
-from .enums import *
-from .exceptions import InvalidLavalinkResponse, QueueEmpty
-from .ext import spotify
-from .filters import Filter
-from .node import Node, NodePool
-from .payloads import TrackEventPayload
-from .queue import Queue
-from .tracks import *
-
-
-if TYPE_CHECKING:
-    from nextcord.types.voice import GuildVoiceState, VoiceServerUpdate
-    from typing_extensions import Self
-
-    from .types.events import PlayerState, PlayerUpdateOp
-    from .types.request import EncodedTrackRequest, Request
-    from .types.state import DiscordVoiceState
-
-__all__ = ("Player",)
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-VoiceChannel = Union[
-    nextcord.VoiceChannel, nextcord.StageChannel
-]  # todo: VocalGuildChannel?
-
-
-class Player(nextcord.VoiceProtocol):
-    """Wavelink Player class.
-
-    This class is used as a :class:`nextcord.VoiceProtocol` and inherits all its members.
-
-
-    .. note::
-
-        The Player class come with an in-built queue. See :class:`queue.Queue`.
-
-    Parameters
-    ----------
-    nodes: Optional[list[:class:`node.Node`]]
-        An optional list of :class:`node.Node` to use with this Player. If no Nodes are provided
-        the best connected Node will be used.
-    swap_node_on_disconnect: bool
-        If a list of :class:`node.Node` is provided the Player will swap Nodes on Node disconnect.
-        Defaults to True.
-
-    Attributes
-    ----------
-    client: :class:nextcord.Client`
-        The nextcord Client or Bot associated with this Player.
-    channel: :class:`nextcord.VoiceChannel`
-        The channel this player is currently connected to.
-    nodes: list[:class:`node.Node`]
-        The list of Nodes this player is currently using.
-    current_node: :class:`node.Node`
-        The Node this player is currently using.
-    queue: :class:`queue.Queue`
-        The wavelink built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
-        Meaning any songs in this queue will be played before auto_queue songs.
-    auto_queue: :class:`queue.Queue`
-        The built-in AutoPlay Queue. This queue keeps track of recommended songs only.
-        When a song is retrieved from this queue in the AutoPlay event, it is added to the main Queue.history.
-    filter: dict[:class:`str`, :class:`Any`]
-        The current filters applied.
-    """
-
-    def __call__(self, client: nextcord.Client, channel: VoiceChannel) -> Self:
-        self.client = client
-        self.channel = channel
-
-        return self
-
-    def __init__(
-        self,
-        client: nextcord.Client = MISSING,
-        channel: VoiceChannel = MISSING,
-        *,
-        nodes: list[Node] | None = None,
-        swap_node_on_disconnect: bool = True
-    ) -> None:
-        self.client: nextcord.Client = client
-        self.channel: VoiceChannel | None = channel
-
-        self.nodes: list[Node]
-        self.current_node: Node
-
-        if swap_node_on_disconnect and not nodes:
-            self.nodes = list(NodePool.nodes.values())
-            self.current_node = self.nodes[0]
-        elif nodes:
-            self.current_node = nodes[0]
-            self.nodes = nodes
-        else:
-            self.current_node = NodePool.get_connected_node()
-            self.nodes = [self.current_node]
-
-        if not self.client:
-            if self.current_node.client is None:
-                raise RuntimeError('')
-            self.client = self.current_node.client
-
-        self._guild: nextcord.Guild | None = None
-        self._voice_state: DiscordVoiceState = {}
-        self._player_state: dict[str, Any] = {}
-
-        self.swap_on_disconnect: bool = swap_node_on_disconnect
-
-        self.last_update: datetime.datetime | None = None
-        self.last_position: int = 0
-
-        self._ping: int = 0
-
-        self.queue: Queue = Queue()
-        self._current: Playable | None = None
-        self._original: Playable | None = None
-
-        self._volume: int = 50
-        self._paused: bool = False
-
-        self._track_seeds: list[str] = []
-        self._autoplay: bool = False
-        self.auto_queue: Queue = Queue()
-        self._auto_threshold: int = 20
-        self._filter: Filter | None = None
-
-    async def _auto_play_event(self, payload: TrackEventPayload) -> None:
-        if not self.autoplay:
-            return
-
-        if payload.reason == 'REPLACED':
-            return
-
-        if self.queue.loop:
-            try:
-                track = self.queue.get()
-            except QueueEmpty:
-                return
-
-            await self.play(track)
-            return
-
-        if self.queue:
-            populate = len(self.auto_queue) < self._auto_threshold
-            await self.play(self.queue.get(), populate=populate)
-
-            return
-
-        if not self.auto_queue:
-            return
-
-        await self.queue.put_wait(await self.auto_queue.get_wait())
-        populate = self.auto_queue.is_empty
-
-        await self.play(await self.queue.get_wait(), populate=populate)
-
-    @property
-    def autoplay(self) -> bool:
-        """Bool whether the Player is in AutoPlay mode or not.
-
-        Can be set to True or False.
-        """
-        return self._autoplay
-
-    @autoplay.setter
-    def autoplay(self, value: bool) -> None:
-        """Set AutoPlay to True or False."""
-        self._autoplay = value
-
-    def is_playing(self) -> bool:
-        """Whether the Player is currently playing a track."""
-        return self.current is not None
-
-    def is_paused(self) -> bool:
-        """Whether the Player is currently paused."""
-        return self._paused
-
-    @property
-    def volume(self) -> int:
-        """The current volume of the Player."""
-        return self._volume
-
-    @property
-    def guild(self) -> nextcord.Guild | None:
-        """The nextcord Guild associated with the Player."""
-        return self._guild
-
-    @property
-    def position(self) -> float:
-        """The position of the currently playing track in milliseconds."""
-
-        if not self.is_playing():
-            return 0
-
-        if self.is_paused():
-            return min(self.last_position, self.current.duration)  # type: ignore
-
-        delta = (datetime.datetime.now(datetime.timezone.utc) - self.last_update).total_seconds() * 1000
-        position = self.last_position + delta
-
-        return min(position, self.current.duration)
-
-    @property
-    def ping(self) -> int:
-        """The ping to the nextcord endpoint in milliseconds."""
-        return self._ping
-
-    @property
-    def current(self) -> Playable | None:
-        """The currently playing Track if there is one.
-
-        Could be None if no Track is playing.
-        """
-        return self._current
-
-    @property
-    def filter(self) -> dict[str, Any]:
-        return self._filter._payload
-
-    async def _update_event(self, data: PlayerUpdateOp | None) -> None:
-        assert self._guild is not None
-
-        if data is None: 
-            if self.swap_on_disconnect:
-
-                if len(self.nodes) < 2:
-                    return
-
-                new: Node = [n for n in self.nodes if n != self.current_node and n.status is NodeStatus.CONNECTED][0]
-                del self.current_node._players[self._guild.id]
-
-                if not new:
-                    return
-
-                self.current_node: Node = new
-                new._players[self._guild.id] = self
-
-                await self._dispatch_voice_update()
-                await self._swap_state()
-            return
-
-        data.pop('op')  # type: ignore
-        self._player_state.update(**data)
-
-        state: PlayerState = data['state']
-        self.last_update = datetime.datetime.fromtimestamp(state.get("time", 0) / 1000, datetime.timezone.utc)
-        self.last_position = state.get('position', 0)
-
-        self._ping = state['ping']
-
-    async def on_voice_server_update(self, data: VoiceServerUpdate) -> None:
-        self._voice_state['token'] = data['token']
-        self._voice_state['endpoint'] = data['endpoint']
-
-        await self._dispatch_voice_update()
-
-    async def on_voice_state_update(self, data: GuildVoiceState) -> None:
-        assert self._guild is not None
-
-        channel_id = data["channel_id"]
-
-        if not channel_id:
-            await self._destroy()
-            return
-
-        self._voice_state['session_id'] = data['session_id']
-        self.channel = self.client.get_channel(int(channel_id))  # type: ignore
-
-        if not self._guild:
-            self._guild = self.channel.guild  # type: ignore
-            assert self._guild is not None
-            self.current_node._players[self._guild.id] = self
-
-    async def _dispatch_voice_update(self, data: DiscordVoiceState | None = None) -> None:
-        assert self._guild is not None
-
-        data = data or self._voice_state
-
-        try:
-            session_id: str = data['session_id']
-            token: str = data['token']
-            endpoint: str = data['endpoint']
-        except KeyError:
-            return
-
-        voice: Request = {'voice': {'sessionId': session_id, 'token': token, 'endpoint': endpoint}}
-        self._player_state.update(**voice)
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=voice)
-
-        logger.debug(f'Dispatching VOICE_UPDATE: {resp}')
-
-    async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
-        if self.channel is None:
-            raise RuntimeError('')
-
-        if not self._guild:
-            self._guild = self.channel.guild
-            self.current_node._players[self._guild.id] = self
-
-        await self.channel.guild.change_voice_state(channel=self.channel, **kwargs)
-
-    async def move_to(self, channel: nextcord.VoiceChannel) -> None:
-        """|coro|
-
-        Moves the player to a different voice channel.
-
-        Parameters
-        -----------
-        channel: :class:`nextcord.VoiceChannel`
-            The channel to move to. Must be a voice channel.
-        """
-        await self.guild.change_voice_state(channel=channel)
-        logger.info(f"Moving to voice channel:: {channel.id}")
-
-    async def play(self,
-                   track: Playable,
-                   replace: bool = True,
-                   start: int | None = None,
-                   end: int | None = None,
-                   volume: int | None = None,
-                   *,
-                   populate: bool = False
-                   ) -> Playable:
-        """|coro|
-
-        Play a WaveLink Track.
-
-        Parameters
-        ----------
-        track: :class:`tracks.Playable`
-            The :class:`tracks.Playable` track to start playing.
-        replace: bool
-            Whether this track should replace the current track. Defaults to ``True``.
-        start: Optional[int]
-            The position to start the track at in milliseconds.
-            Defaults to ``None`` which will start the track at the beginning.
-        end: Optional[int]
-            The position to end the track at in milliseconds.
-            Defaults to ``None`` which means it will play until the end.
-        volume: Optional[int]
-            Sets the volume of the player. Must be between ``0`` and ``1000``.
-            Defaults to ``None`` which will not change the volume.
-        populate: bool
-            Whether to populate the AutoPlay queue. This is done automatically when AutoPlay is on.
-            Defaults to False.
-
-        Returns
-        -------
-        :class:`tracks.Playable`
-            The track that is now playing.
-        """
-        assert self._guild is not None
-
-        if isinstance(track, spotify.SpotifyTrack):
-            original = track
-            track = await track.fulfill(player=self, cls=YouTubeTrack, populate=populate)
-
-            for attr, value in original.__dict__.items():
-                if hasattr(track, attr):
-                    logger.warning(f'Unable to set attribute "{attr}" as it conflicts with new track type.')
-                    continue
-
-                setattr(track, attr, value)
-
-        data = {
-            'encodedTrack': track.encoded,
-            'position': start or 0,
-            'volume': volume or self._volume
-        }
-
-        if end:
-            data['endTime'] = end
-
-        self._current = track
-        self._original = track
-
-        try:
-
-            resp: dict[str, Any] = await self.current_node._send(
-                method='PATCH',
-                path=f'sessions/{self.current_node._session_id}/players',
-                guild_id=self._guild.id,
-                data=data,
-                query=f'noReplace={not replace}'
-            )
-
-        except InvalidLavalinkResponse as e:
-            self._current = None
-            self._original = None
-            raise e
-
-        self._player_state['track'] = resp['track']['encoded']
-        self.queue._loaded = track
-
-        return track
-
-    async def set_volume(self, value: int) -> None:
-        """|coro|
-
-        Set the Player volume.
-
-        Parameters
-        ----------
-        value: int
-            A volume value between 0 and 1000.
-        """
-        assert self._guild is not None
-
-        self._volume = max(min(value, 1000), 0)
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'volume': self._volume})
-
-        logger.debug(f'Player {self.guild.id} volume was set to {self._volume}.')
-
-    async def seek(self, position: int) -> None:
-        """|coro|
-
-        Seek to the provided position, in milliseconds.
-
-        Parameters
-        ----------
-        position: int
-            The position to seek to in milliseconds.
-        """
-        if not self._current:
-            return
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'position': position})
-
-        logger.debug(f'Player {self.guild.id} seeked current track to position {position}.')
-
-    async def pause(self) -> None:
-        """|coro|
-
-        Pauses the Player.
-        """
-        assert self._guild is not None
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'paused': True})
-
-        self._paused = True
-        logger.debug(f'Player {self.guild.id} was paused.')
-
-    async def resume(self) -> None:
-        """|coro|
-
-        Resumes the Player.
-        """
-        assert self._guild is not None
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'paused': False})
-
-        self._paused = False
-        logger.debug(f'Player {self.guild.id} was resumed.')
-
-    async def stop(self) -> None:
-        """|coro|
-
-        Stops the currently playing Track.
-        """
-        assert self._guild is not None
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data={'encodedTrack': None})
-
-        self.queue._loaded = None
-
-        self._player_state['track'] = None
-        logger.debug(f'Player {self.guild.id} was stopped.')
-
-    async def set_filter(
-        self,
-        _filter: Filter,
-        /, *,
-        seek: bool = False
-    ) -> None:
-        """|coro|
-
-        Set the player's filter.
-
-        Parameters
-        ----------
-        filter: :class:`wavelink.Filter`
-            The filter to apply to the player.
-        seek: bool
-            Whether to seek the player to its current position
-            which will apply the filter immediately. Defaults to ``False``.
-        """
-
-        assert self._guild is not None
-
-        self._filter = _filter
-        data: Request = {"filters": _filter._payload}
-
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=data)        
-
-        if self.is_playing() and seek:
-            await self.seek(int(self.position))
-        logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
-
-    async def _destroy(self) -> None:
-        self.autoplay = False
-        self._voice_state = {}
-        self._player_state = {}
-        self.cleanup()
-
-        await self.current_node._send(method='DELETE',
-                                      path=f'sessions/{self.current_node._session_id}/players',
-                                      guild_id=self._guild.id)
-
-        del self.current_node._players[self.guild.id]
-        logger.debug(f'Player {self.guild.id} was destroyed.')
-
-    async def disconnect(self, **kwargs) -> None:
-        """|coro|
-
-        Disconnect the Player from voice and cleanup the Player state.
-        """
-        await self.guild.change_voice_state(channel=None)
-
-    async def _swap_state(self) -> None:
-        assert self._guild is not None
-
-        try:
-            self._player_state['track']
-        except KeyError:
-            return
-
-        data: EncodedTrackRequest = {'encodedTrack': self._player_state['track'], 'position': self.position}
-        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
-                                                             path=f'sessions/{self.current_node._session_id}/players',
-                                                             guild_id=self._guild.id,
-                                                             data=data)
-
-        logger.debug(f'Swapping State: {resp}')
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import datetime
+import logging
+from typing import TYPE_CHECKING, Any, Union
+
+import nextcord
+from nextcord.utils import MISSING
+
+from .enums import *
+from .exceptions import *
+from .ext import spotify
+from .filters import Filter
+from .node import Node, NodePool
+from .payloads import TrackEventPayload
+from .queue import Queue
+from .tracks import *
+
+
+if TYPE_CHECKING:
+    from nextcord.types.voice import GuildVoiceState, VoiceServerUpdate
+    from typing_extensions import Self
+
+    from .types.events import PlayerState, PlayerUpdateOp
+    from .types.request import EncodedTrackRequest, Request
+    from .types.state import DiscordVoiceState
+
+__all__ = ("Player",)
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+VoiceChannel = Union[
+    nextcord.VoiceChannel, nextcord.StageChannel
+]  # todo: VocalGuildChannel?
+
+
+class Player(nextcord.VoiceProtocol):
+    """Wavelink Player class.
+
+    This class is used as a :class:`~nextcord.VoiceProtocol` and inherits all its members.
+
+
+    .. note::
+
+        The Player class come with an in-built queue. See :class:`queue.Queue`.
+
+    Parameters
+    ----------
+    nodes: Optional[list[:class:`node.Node`]]
+        An optional list of :class:`node.Node` to use with this Player. If no Nodes are provided
+        the best connected Node will be used.
+    swap_node_on_disconnect: bool
+        If a list of :class:`node.Node` is provided the Player will swap Nodes on Node disconnect.
+        Defaults to True.
+
+    Attributes
+    ----------
+    client: :class:`nextcord.Client`
+        The nextcord Client or Bot associated with this Player.
+    channel: :class:`nextcord.VoiceChannel`
+        The channel this player is currently connected to.
+    nodes: list[:class:`node.Node`]
+        The list of Nodes this player is currently using.
+    current_node: :class:`node.Node`
+        The Node this player is currently using.
+    queue: :class:`queue.Queue`
+        The wavelink built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
+        Meaning any songs in this queue will be played before auto_queue songs.
+    auto_queue: :class:`queue.Queue`
+        The built-in AutoPlay Queue. This queue keeps track of recommended songs only.
+        When a song is retrieved from this queue in the AutoPlay event, it is added to the main Queue.history.
+    filter: dict[:class:`str`, :class:`Any`]
+        The current filters applied.
+    """
+
+    def __call__(self, client: nextcord.Client, channel: VoiceChannel) -> Self:
+        self.client = client
+        self.channel = channel
+
+        return self
+
+    def __init__(
+        self,
+        client: nextcord.Client = MISSING,
+        channel: VoiceChannel = MISSING,
+        *,
+        nodes: list[Node] | None = None,
+        swap_node_on_disconnect: bool = True
+    ) -> None:
+        self.client: nextcord.Client = client
+        self.channel: VoiceChannel | None = channel
+
+        self.nodes: list[Node]
+        self.current_node: Node
+
+        if swap_node_on_disconnect and not nodes:
+            nodes = list(NodePool.nodes.values())
+            self.nodes = sorted(nodes, key=lambda n: len(n.players))
+            self.current_node = self.nodes[0]
+        elif nodes:
+            nodes = sorted(nodes, key=lambda n: len(n.players))
+            self.current_node = nodes[0]
+            self.nodes = nodes
+        else:
+            self.current_node = NodePool.get_connected_node()
+            self.nodes = [self.current_node]
+
+        if not self.client:
+            if self.current_node.client is None:
+                raise RuntimeError('')
+            self.client = self.current_node.client
+
+        self._guild: nextcord.Guild | None = None
+        self._voice_state: DiscordVoiceState = {}
+        self._player_state: dict[str, Any] = {}
+
+        self.swap_on_disconnect: bool = swap_node_on_disconnect
+
+        self.last_update: datetime.datetime | None = None
+        self.last_position: int = 0
+
+        self._ping: int = 0
+
+        self.queue: Queue = Queue()
+        self._current: Playable | None = None
+        self._original: Playable | None = None
+
+        self._volume: int = 50
+        self._paused: bool = False
+
+        self._track_seeds: list[str] = []
+        self._autoplay: bool = False
+        self.auto_queue: Queue = Queue()
+        self._auto_threshold: int = 20
+        self._filter: Filter | None = None
+
+    async def _auto_play_event(self, payload: TrackEventPayload) -> None:
+        if not self.autoplay:
+            return
+
+        if payload.reason == 'REPLACED':
+            return
+
+        if self.queue.loop:
+            try:
+                track = self.queue.get()
+            except QueueEmpty:
+                return
+
+            await self.play(track)
+            return
+
+        if self.queue:
+            populate = len(self.auto_queue) < self._auto_threshold
+            await self.play(self.queue.get(), populate=populate)
+
+            return
+
+        if self.queue.loop_all:
+            await self.play(self.queue.get())
+            return
+
+        if not self.auto_queue:
+            return
+
+        await self.queue.put_wait(await self.auto_queue.get_wait())
+        populate = self.auto_queue.is_empty
+
+        await self.play(await self.queue.get_wait(), populate=populate)
+
+    @property
+    def autoplay(self) -> bool:
+        """Bool whether the Player is in AutoPlay mode or not.
+
+        Can be set to True or False.
+        """
+        return self._autoplay
+
+    @autoplay.setter
+    def autoplay(self, value: bool) -> None:
+        """Set AutoPlay to True or False."""
+        self._autoplay = value
+
+    def is_connected(self) -> bool:
+        """Whether the player is connected to a voice channel."""
+        return self.channel is not None and self.channel is not MISSING
+
+    def is_playing(self) -> bool:
+        """Whether the Player is currently playing a track."""
+        return self.current is not None
+
+    def is_paused(self) -> bool:
+        """Whether the Player is currently paused."""
+        return self._paused
+
+    @property
+    def volume(self) -> int:
+        """The current volume of the Player."""
+        return self._volume
+
+    @property
+    def guild(self) -> nextcord.Guild | None:
+        """The nextcord Guild associated with the Player."""
+        return self._guild
+
+    @property
+    def position(self) -> float:
+        """The position of the currently playing track in milliseconds."""
+
+        if not self.is_playing():
+            return 0
+
+        if self.is_paused():
+            return min(self.last_position, self.current.duration)  # type: ignore
+
+        delta = (datetime.datetime.now(datetime.timezone.utc) - self.last_update).total_seconds() * 1000
+        position = self.last_position + delta
+
+        return min(position, self.current.duration)
+
+    @property
+    def ping(self) -> int:
+        """The ping to the nextcord endpoint in milliseconds."""
+        return self._ping
+
+    @property
+    def current(self) -> Playable | None:
+        """The currently playing Track if there is one.
+
+        Could be None if no Track is playing.
+        """
+        return self._current
+
+    @property
+    def filter(self) -> dict[str, Any]:
+        return self._filter._payload
+
+    async def _update_event(self, data: PlayerUpdateOp | None) -> None:
+        assert self._guild is not None
+
+        if data is None: 
+            if self.swap_on_disconnect:
+
+                if len(self.nodes) < 2:
+                    return
+
+                new: Node = [n for n in self.nodes if n != self.current_node and n.status is NodeStatus.CONNECTED][0]
+                del self.current_node._players[self._guild.id]
+
+                if not new:
+                    return
+
+                self.current_node: Node = new
+                new._players[self._guild.id] = self
+
+                await self._dispatch_voice_update()
+                await self._swap_state()
+            return
+
+        data.pop('op')  # type: ignore
+        self._player_state.update(**data)
+
+        state: PlayerState = data['state']
+        self.last_update = datetime.datetime.fromtimestamp(state.get("time", 0) / 1000, datetime.timezone.utc)
+        self.last_position = state.get('position', 0)
+
+        self._ping = state['ping']
+
+    async def on_voice_server_update(self, data: VoiceServerUpdate) -> None:
+        self._voice_state['token'] = data['token']
+        self._voice_state['endpoint'] = data['endpoint']
+
+        await self._dispatch_voice_update()
+
+    async def on_voice_state_update(self, data: GuildVoiceState) -> None:
+        assert self._guild is not None
+
+        channel_id = data["channel_id"]
+
+        if not channel_id:
+            await self._destroy()
+            return
+
+        self._voice_state['session_id'] = data['session_id']
+        self.channel = self.client.get_channel(int(channel_id))  # type: ignore
+
+        if not self._guild:
+            self._guild = self.channel.guild  # type: ignore
+            assert self._guild is not None
+            self.current_node._players[self._guild.id] = self
+
+    async def _dispatch_voice_update(self, data: DiscordVoiceState | None = None) -> None:
+        assert self._guild is not None
+
+        data = data or self._voice_state
+
+        try:
+            session_id: str = data['session_id']
+            token: str = data['token']
+            endpoint: str = data['endpoint']
+        except KeyError:
+            return
+
+        voice: Request = {'voice': {'sessionId': session_id, 'token': token, 'endpoint': endpoint}}
+        self._player_state.update(**voice)
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data=voice)
+
+        logger.debug(f'Dispatching VOICE_UPDATE: {resp}')
+
+    async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
+        if self.channel is None:
+            self._invalidate()
+
+            msg: str = 'Please use the method "nextcord.VoiceChannel.connect" and pass this player to cls='
+            raise InvalidChannelStateError(msg)
+
+        if not self.channel.permissions_for(self.channel.guild.me).connect:
+            self._invalidate()
+
+            raise InvalidChannelPermissions('You do not have connect permissions to join this channel.')
+
+        limit: int = self.channel.user_limit
+        total: int = len(self.channel.members)
+
+        if limit == 0:
+            pass
+
+        elif total >= limit:
+            self._invalidate()
+
+            msg: str = f'There are currently too many users in this channel. <{total}/{limit}>'
+            raise InvalidChannelPermissions(msg)
+
+        if not self._guild:
+            self._guild = self.channel.guild
+            self.current_node._players[self._guild.id] = self
+
+        await self.channel.guild.change_voice_state(channel=self.channel, **kwargs)
+
+    async def move_to(self, channel: nextcord.VoiceChannel) -> None:
+        """|coro|
+
+        Moves the player to a different voice channel.
+
+        Parameters
+        -----------
+        channel: :class:`nextcord.VoiceChannel`
+            The channel to move to. Must be a voice channel.
+        """
+        await self.guild.change_voice_state(channel=channel)
+        logger.info(f"Moving to voice channel:: {channel.id}")
+
+    async def play(self,
+                   track: Playable,
+                   replace: bool = True,
+                   start: int | None = None,
+                   end: int | None = None,
+                   volume: int | None = None,
+                   *,
+                   populate: bool = False
+                   ) -> Playable:
+        """|coro|
+
+        Play a WaveLink Track.
+
+        Parameters
+        ----------
+        track: :class:`tracks.Playable`
+            The :class:`tracks.Playable` track to start playing.
+        replace: bool
+            Whether this track should replace the current track. Defaults to ``True``.
+        start: Optional[int]
+            The position to start the track at in milliseconds.
+            Defaults to ``None`` which will start the track at the beginning.
+        end: Optional[int]
+            The position to end the track at in milliseconds.
+            Defaults to ``None`` which means it will play until the end.
+        volume: Optional[int]
+            Sets the volume of the player. Must be between ``0`` and ``1000``.
+            Defaults to ``None`` which will not change the volume.
+        populate: bool
+            Whether to populate the AutoPlay queue. This is done automatically when AutoPlay is on.
+            Defaults to False.
+
+        Returns
+        -------
+        :class:`tracks.Playable`
+            The track that is now playing.
+        """
+        assert self._guild is not None
+
+        if isinstance(track, spotify.SpotifyTrack):
+            original = track
+            track = await track.fulfill(player=self, cls=YouTubeTrack, populate=populate)
+
+            for attr, value in original.__dict__.items():
+                if hasattr(track, attr):
+                    logger.warning(f'Unable to set attribute "{attr}" as it conflicts with new track type.')
+                    continue
+
+                setattr(track, attr, value)
+
+        data = {
+            'encodedTrack': track.encoded,
+            'position': start or 0,
+            'volume': volume or self._volume
+        }
+
+        if end:
+            data['endTime'] = end
+
+        self._current = track
+        self._original = track
+
+        try:
+
+            resp: dict[str, Any] = await self.current_node._send(
+                method='PATCH',
+                path=f'sessions/{self.current_node._session_id}/players',
+                guild_id=self._guild.id,
+                data=data,
+                query=f'noReplace={not replace}'
+            )
+
+        except InvalidLavalinkResponse as e:
+            self._current = None
+            self._original = None
+            raise e
+
+        self._player_state['track'] = resp['track']['encoded']
+
+        if self.queue.loop and self.queue._loaded:
+            pass
+        else:
+            self.queue.history.put(track)
+
+        self.queue._loaded = track
+
+        return track
+
+    async def set_volume(self, value: int) -> None:
+        """|coro|
+
+        Set the Player volume.
+
+        Parameters
+        ----------
+        value: int
+            A volume value between 0 and 1000.
+        """
+        assert self._guild is not None
+
+        self._volume = max(min(value, 1000), 0)
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'volume': self._volume})
+
+        logger.debug(f'Player {self.guild.id} volume was set to {self._volume}.')
+
+    async def seek(self, position: int) -> None:
+        """|coro|
+
+        Seek to the provided position, in milliseconds.
+
+        Parameters
+        ----------
+        position: int
+            The position to seek to in milliseconds.
+        """
+        if not self._current:
+            return
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'position': position})
+
+        logger.debug(f'Player {self.guild.id} seeked current track to position {position}.')
+
+    async def pause(self) -> None:
+        """|coro|
+
+        Pauses the Player.
+        """
+        assert self._guild is not None
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'paused': True})
+
+        self._paused = True
+        logger.debug(f'Player {self.guild.id} was paused.')
+
+    async def resume(self) -> None:
+        """|coro|
+
+        Resumes the Player.
+        """
+        assert self._guild is not None
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'paused': False})
+
+        self._paused = False
+        logger.debug(f'Player {self.guild.id} was resumed.')
+
+    async def stop(self) -> None:
+        """|coro|
+
+        Stops the currently playing Track.
+        """
+        assert self._guild is not None
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data={'encodedTrack': None})
+
+        self.queue._loaded = None
+
+        self._player_state['track'] = None
+        logger.debug(f'Player {self.guild.id} was stopped.')
+
+    async def set_filter(
+        self,
+        _filter: Filter,
+        /, *,
+        seek: bool = False
+    ) -> None:
+        """|coro|
+
+        Set the player's filter.
+
+        Parameters
+        ----------
+        filter: :class:`wavelink.Filter`
+            The filter to apply to the player.
+        seek: bool
+            Whether to seek the player to its current position
+            which will apply the filter immediately. Defaults to ``False``.
+        """
+
+        assert self._guild is not None
+
+        self._filter = _filter
+        data: Request = {"filters": _filter._payload}
+
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data=data)        
+
+        if self.is_playing() and seek:
+            await self.seek(int(self.position))
+        logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
+
+    def _invalidate(self) -> None:
+        try:
+            self.cleanup()
+        except Exception as e:
+            logger.debug(f'Failed to cleanup player, most likely due to never having been connected: {e}')
+
+        self._voice_state = {}
+        self._player_state = {}
+        self.channel = None
+
+    async def _destroy(self) -> None:
+        self._invalidate()
+
+        await self.current_node._send(method='DELETE',
+                                      path=f'sessions/{self.current_node._session_id}/players',
+                                      guild_id=self._guild.id)
+
+        del self.current_node._players[self._guild.id]
+        logger.debug(f'Player {self._guild.id} was destroyed.')
+
+    async def disconnect(self, **kwargs) -> None:
+        """|coro|
+
+        Disconnect the Player from voice and cleanup the Player state.
+        """
+        self._invalidate()
+        await self.guild.change_voice_state(channel=None)
+
+    async def _swap_state(self) -> None:
+        assert self._guild is not None
+
+        try:
+            self._player_state['track']
+        except KeyError:
+            return
+
+        data: EncodedTrackRequest = {'encodedTrack': self._player_state['track'], 'position': self.position}
+        resp: dict[str, Any] = await self.current_node._send(method='PATCH',
+                                                             path=f'sessions/{self.current_node._session_id}/players',
+                                                             guild_id=self._guild.id,
+                                                             data=data)
+
+        logger.debug(f'Swapping State: {resp}')
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/types/request.py` & `WavelinkCord-2.5.2b0/wavelink/types/request.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, TypedDict
-
-from .state import VoiceState
-
-if TYPE_CHECKING:
-    from typing_extensions import TypeAlias
-
-
-class Filters(TypedDict):
-    ...
-
-
-class _BaseRequest(TypedDict, total=False):
-    voice: VoiceState
-    position: int
-    endTime: int
-    volume: int
-    paused: bool
-    filters: Filters
-    voice: VoiceState
-
-
-class EncodedTrackRequest(_BaseRequest):
-    encodedTrack: str | None
-
-
-class IdentifierRequest(_BaseRequest):
-    identifier: str
-
-
-Request: TypeAlias = '_BaseRequest | EncodedTrackRequest | IdentifierRequest'
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, TypedDict
+
+from .state import VoiceState
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
+
+class Filters(TypedDict):
+    ...
+
+
+class _BaseRequest(TypedDict, total=False):
+    voice: VoiceState
+    position: int
+    endTime: int
+    volume: int
+    paused: bool
+    filters: Filters
+    voice: VoiceState
+
+
+class EncodedTrackRequest(_BaseRequest):
+    encodedTrack: str | None
+
+
+class IdentifierRequest(_BaseRequest):
+    identifier: str
+
+
+Request: TypeAlias = '_BaseRequest | EncodedTrackRequest | IdentifierRequest'
```

### Comparing `WaveLinkCord-2.2.3/src/wavelinkcord/websocket.py` & `WavelinkCord-2.5.2b0/wavelink/websocket.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,251 +1,259 @@
-"""
-MIT License
-
-Copyright (c) 2019-Present PythonistaGuild
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-"""
-from __future__ import annotations
-
-import asyncio
-import logging
-from typing import TYPE_CHECKING, Any, Optional
-
-import aiohttp
-
-import wavelinkcord
-
-from . import __version__
-from .backoff import Backoff
-from .enums import NodeStatus, TrackEventType
-from .exceptions import *
-from .payloads import TrackEventPayload
-
-if TYPE_CHECKING:
-    from .node import Node
-    from .player import Player
-
-
-logger: logging.Logger = logging.getLogger(__name__)
-
-
-class Websocket:
-
-    __slots__ = (
-        'node',
-        'socket',
-        'retries',
-        'retry',
-        '_original_attempts',
-        'backoff',
-        '_listener_task'
-    )
-
-    def __init__(self, *, node: Node) -> None:
-        self.node: Node = node
-        self.socket: aiohttp.ClientWebSocketResponse | None = None
-
-        self.retries: int | None = node._retries
-        self.retry: float = 1
-        self._original_attempts: int | None = node._retries
-
-        self.backoff: Backoff = Backoff()
-
-        self._listener_task: asyncio.Task | None = None
-
-    @property
-    def headers(self) -> dict[str, str]:
-        assert self.node.client is not None
-        assert self.node.client.user is not None
-
-        return {
-            'Authorization': self.node.password,
-            'User-Id': str(self.node.client.user.id),
-            'Client-Name': f'Wavelink/{__version__}'
-        }
-
-    def is_connected(self) -> bool:
-        return self.socket is not None and not self.socket.closed
-
-    async def connect(self) -> None:
-        if self.node.status is NodeStatus.CONNECTED:
-            logger.error(f'The Node <{self.node!r}> is already in a connected state. Disregarding.')
-            return
-
-        self.node._status = NodeStatus.CONNECTING
-
-        try:
-            self._listener_task.cancel()
-        except Exception as e:
-            logger.debug(f'An error was raised while cancelling the websocket listener. {e}')
-
-        uri: str = self.node._host.removeprefix('https://').removeprefix('http://')
-
-        if self.node._use_http:
-            uri: str = f'{"https://" if self.node._secure else "http://"}{uri}'
-        else:
-            uri: str = f'{"wss://" if self.node._secure else "ws://"}{uri}'
-
-        heartbeat: float = self.node.heartbeat
-
-        try:
-            self.socket = await self.node._session.ws_connect(url=uri, heartbeat=heartbeat, headers=self.headers)
-        except Exception as e:
-            if isinstance(e, aiohttp.WSServerHandshakeError) and e.status == 401:
-                raise AuthorizationFailed from e
-            else:
-                logger.error(f'An error occurred connecting to node: "{self.node}". {e}')
-
-        if self.is_connected():
-            self.retries = self._original_attempts
-            # TODO - Configure Resuming...
-        else:
-            await self._reconnect()
-            return
-
-        self._listener_task = asyncio.create_task(self._listen())
-
-    async def _reconnect(self) -> None:
-        self.node._status = NodeStatus.CONNECTING
-        self.retry = self.backoff.calculate()
-
-        if self.retries == 0:
-            logger.error('Wavelink 2.0 was unable to connect, and has exhausted the reconnection attempt limit. '
-                         'Please check your Lavalink Node is started and your connection details are correct.')
-
-            await self.cleanup()
-            return
-
-        retries = f'{self.retries} attempt(s) remaining.' if self.retries else ''
-        logger.error(f'Wavelink 2.0 was unable to connect, retrying connection in: "{self.retry}" seconds. {retries}')
-
-        if self.retries:
-            self.retries -= 1
-
-        await asyncio.sleep(self.retry)
-        await self.connect()
-
-    async def _listen(self) -> None:
-        while True:
-            message = await self.socket.receive()
-
-            if message.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
-
-                for player in self.node.players.copy().values():
-                    await player._update_event(data=None)
-
-                asyncio.create_task(self._reconnect())
-                return
-
-            if message.data == 1011:
-                logger.error('Lavalink encountered an internal error which can not be resolved. '
-                             'Make sure your Lavalink sever is up to date, and try restarting.')
-
-                await self.cleanup()
-                return
-
-            if message.data is None:
-                logger.info('Received a message from Lavalink with empty data. Disregarding.')
-                continue
-
-            data = message.json()
-            logger.debug(f'Received a message from Lavalink: {data}')
-
-            op = data.get('op', None)
-            if not op:
-                logger.info('Message "op" from Lavalink was None. Disregarding.')
-                continue
-
-            if op == 'ready':
-                self.node._status = NodeStatus.CONNECTED
-                self.node._session_id = data['sessionId']
-
-                self.dispatch('node_ready', self.node)
-
-            elif op == 'stats':
-                payload = ...
-                logger.debug(f'Stats Update: {data}')
-                self.dispatch('stats_update', data)
-
-            elif op == 'event':
-                logger.debug(f'Websocket Event: {data}')
-                player = self.get_player(data)
-
-                if player is None:
-                    logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
-                    continue
-
-                if data['type'] == 'WebSocketClosedEvent':
-                    if data['code'] == 4014:
-                        continue
-
-                track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
-                payload: TrackEventPayload = TrackEventPayload(
-                    data=data,
-                    track=track,
-                    player=player,
-                    original=player._original
-                )
-
-                if payload.event is TrackEventType.END and payload.reason != 'REPLACED':
-                    player._current = None
-
-                self.dispatch('track_event', payload)
-
-                if payload.event is TrackEventType.END:
-                    self.dispatch('track_end', payload)
-                    asyncio.create_task(player._auto_play_event(payload))
-
-                elif payload.event is TrackEventType.START:
-                    self.dispatch('track_start', payload)
-
-            elif op == 'playerUpdate':
-                player = self.get_player(data)
-                if player is None:
-                    logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
-                    continue
-
-                await player._update_event(data)
-                self.dispatch("player_update", data)
-                logger.debug(f'Websocket Player Update: {data}')
-
-            else:
-                logger.info(f'Received unknown payload from Lavalink: <{data}>. '
-                            f'If this continues consider making a ticket on the Wavelink GitHub. '
-                            f'https://github.com/PythonistaGuild/Wavelink')
-
-    def get_player(self, payload: dict[str, Any]) -> Optional['Player']:
-        return self.node.players.get(int(payload['guildId']), None)
-
-    def dispatch(self, event, *args: Any, **kwargs: Any) -> None:
-        self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
-
-    # noinspection PyBroadException
-    async def cleanup(self) -> None:
-        try:
-            await self.socket.close()
-        except AttributeError:
-            pass
-
-        try:
-            self._listener_task.cancel()
-        except Exception:
-            pass
-
-        self.node._status = NodeStatus.DISCONNECTED
+"""
+MIT License
+
+Copyright (c) 2019-Present PythonistaGuild
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+from __future__ import annotations
+
+import asyncio
+import logging
+from typing import TYPE_CHECKING, Any, Optional
+
+import aiohttp
+
+import wavelink
+
+from . import __version__
+from .backoff import Backoff
+from .enums import NodeStatus, TrackEventType
+from .exceptions import *
+from .payloads import TrackEventPayload, WebsocketClosedPayload
+
+if TYPE_CHECKING:
+    from .node import Node
+    from .player import Player
+
+
+logger: logging.Logger = logging.getLogger(__name__)
+
+
+class Websocket:
+
+    __slots__ = (
+        'node',
+        'socket',
+        'retries',
+        'retry',
+        '_original_attempts',
+        'backoff',
+        '_listener_task',
+        '_reconnect_task'
+    )
+
+    def __init__(self, *, node: Node) -> None:
+        self.node: Node = node
+        self.socket: aiohttp.ClientWebSocketResponse | None = None
+
+        self.retries: int | None = node._retries
+        self.retry: float = 1
+        self._original_attempts: int | None = node._retries
+
+        self.backoff: Backoff = Backoff()
+
+        self._listener_task: asyncio.Task | None = None
+        self._reconnect_task: asyncio.Task | None = None
+
+    @property
+    def headers(self) -> dict[str, str]:
+        assert self.node.client is not None
+        assert self.node.client.user is not None
+
+        return {
+            'Authorization': self.node.password,
+            'User-Id': str(self.node.client.user.id),
+            'Client-Name': f'Wavelink/{__version__}'
+        }
+
+    def is_connected(self) -> bool:
+        return self.socket is not None and not self.socket.closed
+
+    async def connect(self) -> None:
+        if self.node.status is NodeStatus.CONNECTED:
+            logger.error(f'The Node <{self.node!r}> is already in a connected state. Disregarding.')
+            return
+
+        self.node._status = NodeStatus.CONNECTING
+
+        try:
+            self._listener_task.cancel()
+        except Exception as e:
+            logger.debug(f'An error was raised while cancelling the websocket listener. {e}')
+
+        uri: str = self.node._host.removeprefix('https://').removeprefix('http://')
+
+        if self.node._use_http:
+            uri: str = f'{"https://" if self.node._secure else "http://"}{uri}'
+        else:
+            uri: str = f'{"wss://" if self.node._secure else "ws://"}{uri}'
+
+        heartbeat: float = self.node.heartbeat
+
+        try:
+            self.socket = await self.node._session.ws_connect(url=uri, heartbeat=heartbeat, headers=self.headers)
+        except Exception as e:
+            if isinstance(e, aiohttp.WSServerHandshakeError) and e.status == 401:
+                raise AuthorizationFailed from e
+            else:
+                logger.error(f'An error occurred connecting to node: "{self.node}". {e}')
+
+        if self.is_connected():
+            self.retries = self._original_attempts
+            self._reconnect_task = None
+            # TODO - Configure Resuming...
+        else:
+            await self._reconnect()
+            return
+
+        self._listener_task = asyncio.create_task(self._listen())
+
+    async def _reconnect(self) -> None:
+        self.node._status = NodeStatus.CONNECTING
+        self.retry = self.backoff.calculate()
+
+        if self.retries == 0:
+            logger.error('Wavelink 2.0 was unable to connect, and has exhausted the reconnection attempt limit. '
+                         'Please check your Lavalink Node is started and your connection details are correct.')
+
+            await self.cleanup()
+            return
+
+        retries = f'{self.retries} attempt(s) remaining.' if self.retries else ''
+        logger.error(f'Wavelink 2.0 was unable to connect, retrying connection in: "{self.retry}" seconds. {retries}')
+
+        if self.retries:
+            self.retries -= 1
+
+        await asyncio.sleep(self.retry)
+        await self.connect()
+
+    async def _listen(self) -> None:
+        while True:
+            message = await self.socket.receive()
+
+            if message.type in (aiohttp.WSMsgType.CLOSED, aiohttp.WSMsgType.CLOSING):
+
+                for player in self.node.players.copy().values():
+                    await player._update_event(data=None)
+
+                self._reconnect_task = asyncio.create_task(self._reconnect())
+                return
+
+            if message.data == 1011:
+                logger.error('Lavalink encountered an internal error which can not be resolved. '
+                             'Make sure your Lavalink sever is up to date, and try restarting.')
+
+                await self.cleanup()
+                return
+
+            if message.data is None:
+                logger.info('Received a message from Lavalink with empty data. Disregarding.')
+                continue
+
+            data = message.json()
+            logger.debug(f'Received a message from Lavalink: {data}')
+
+            op = data.get('op', None)
+            if not op:
+                logger.info('Message "op" from Lavalink was None. Disregarding.')
+                continue
+
+            if op == 'ready':
+                self.node._status = NodeStatus.CONNECTED
+                self.node._session_id = data['sessionId']
+
+                self.dispatch('node_ready', self.node)
+
+            elif op == 'stats':
+                payload = ...
+                logger.debug(f'Stats Update: {data}')
+                self.dispatch('stats_update', data)
+
+            elif op == 'event':
+                logger.debug(f'Websocket Event: {data}')
+                player = self.get_player(data)
+
+                if player is None:
+                    logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
+                    continue
+
+                if data['type'] == 'WebSocketClosedEvent':
+                    logger.debug(f'WebSocketClosed Event: '
+                                 f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>')
+
+                    payload: WebsocketClosedPayload = WebsocketClosedPayload(data=data, player=player)
+
+                    self.dispatch('websocket_closed', payload)
+                    continue
+
+                track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
+                payload: TrackEventPayload = TrackEventPayload(
+                    data=data,
+                    track=track,
+                    player=player,
+                    original=player._original
+                )
+
+                if payload.event is TrackEventType.END and payload.reason != 'REPLACED':
+                    player._current = None
+
+                self.dispatch('track_event', payload)
+
+                if payload.event is TrackEventType.END:
+                    self.dispatch('track_end', payload)
+                    asyncio.create_task(player._auto_play_event(payload))
+
+                elif payload.event is TrackEventType.START:
+                    self.dispatch('track_start', payload)
+
+            elif op == 'playerUpdate':
+                player = self.get_player(data)
+                if player is None:
+                    logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
+                    continue
+
+                await player._update_event(data)
+                self.dispatch("player_update", data)
+                logger.debug(f'Websocket Player Update: {data}')
+
+            else:
+                logger.info(f'Received unknown payload from Lavalink: <{data}>. '
+                            f'If this continues consider making a ticket on the Wavelink GitHub. '
+                            f'https://github.com/PythonistaGuild/Wavelink')
+
+    def get_player(self, payload: dict[str, Any]) -> Optional['Player']:
+        return self.node.players.get(int(payload['guildId']), None)
+
+    def dispatch(self, event, *args: Any, **kwargs: Any) -> None:
+        self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
+
+    # noinspection PyBroadException
+    async def cleanup(self) -> None:
+        try:
+            await self.socket.close()
+        except AttributeError:
+            pass
+
+        try:
+            self._listener_task.cancel()
+        except Exception:
+            pass
+
+        self.node._status = NodeStatus.DISCONNECTED
```

