# Comparing `tmp/harambot-0.3.0.tar.gz` & `tmp/harambot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harambot-0.3.0.tar", max compression
+gzip compressed data, was "harambot-0.3.1.tar", max compression
```

## Comparing `harambot-0.3.0.tar` & `harambot-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0     1071 2022-03-21 00:23:13.038328 harambot-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     5518 2023-04-23 00:10:11.637498 harambot-0.3.0/README.md
--rw-r--r--   0        0        0   205449 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/discord-add-bot.png
--rw-r--r--   0        0        0   297377 2022-09-30 15:15:31.381358 harambot-0.3.0/assests/discord-config-command.png
--rw-r--r--   0        0        0   172632 2022-09-30 15:15:31.381358 harambot-0.3.0/assests/discord-config-dm.png
--rw-r--r--   0        0        0   249813 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/discord-copy-token.png
--rw-r--r--   0        0        0   181891 2022-11-11 15:59:03.669059 harambot-0.3.0/assests/discord-intents.png
--rw-r--r--   0        0        0   177261 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/discord-new-application.png
--rw-r--r--   0        0        0   217621 2022-09-30 15:15:31.381358 harambot-0.3.0/assests/discord-oauth-generator.png
--rw-r--r--   0        0        0   251183 2022-09-30 15:15:31.381358 harambot-0.3.0/assests/discord-oauth-url-authorize-1.png
--rw-r--r--   0        0        0   264428 2022-09-30 15:15:31.381358 harambot-0.3.0/assests/discord-oauth-url-authorize-2.png
--rw-r--r--   0        0        0    40246 2023-04-22 23:37:19.512580 harambot-0.3.0/assests/harambot_configure_1.png
--rw-r--r--   0        0        0    65725 2023-04-22 23:37:22.672579 harambot-0.3.0/assests/harambot_configure_2.png
--rw-r--r--   0        0        0    49651 2023-04-22 23:37:25.512578 harambot-0.3.0/assests/harambot_configure_3.png
--rw-r--r--   0        0        0    36723 2023-04-22 23:41:51.442521 harambot-0.3.0/assests/harambot_configure_4.png
--rw-r--r--   0        0        0   207972 2022-09-30 15:15:31.381358 harambot-0.3.0/assests/heroku-deployment.png
--rw-r--r--   0        0        0   118091 2022-11-11 15:59:03.669059 harambot-0.3.0/assests/heroku-dyno.png
--rw-r--r--   0        0        0   156615 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/matchups.PNG
--rw-r--r--   0        0        0    74049 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/player_details.PNG
--rw-r--r--   0        0        0   530839 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/rip.PNG
--rw-r--r--   0        0        0    69062 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/roster.PNG
--rw-r--r--   0        0        0   104400 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/standings.PNG
--rw-r--r--   0        0        0   107130 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/trade.PNG
--rw-r--r--   0        0        0   478431 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/yahoo-app-details.png
--rw-r--r--   0        0        0    91598 2022-03-21 00:23:13.048328 harambot-0.3.0/assests/yahoo-app-secrets.png
--rw-r--r--   0        0        0   127686 2022-03-21 00:23:13.058328 harambot-0.3.0/assests/yahoo-create-app.png
--rw-r--r--   0        0        0  1808878 2022-03-21 00:23:13.058328 harambot-0.3.0/assests/yahoo-league-id.png
--rw-r--r--   0        0        0     1742 2023-04-21 17:55:04.551812 harambot-0.3.0/harambot/bot.py
--rw-r--r--   0        0        0     2666 2023-04-22 23:32:27.732642 harambot-0.3.0/harambot/cogs/meta.py
--rw-r--r--   0        0        0      953 2023-04-19 19:19:16.820119 harambot-0.3.0/harambot/cogs/misc.py
--rw-r--r--   0        0        0    12158 2023-04-19 19:19:19.440118 harambot-0.3.0/harambot/cogs/yahoo.py
--rw-r--r--   0        0        0      157 2023-04-19 19:19:16.820119 harambot-0.3.0/harambot/config.py
--rw-r--r--   0        0        0      980 2023-04-19 19:19:19.440118 harambot-0.3.0/harambot/database/migrations.py
--rw-r--r--   0        0        0      836 2023-04-19 19:19:19.450118 harambot-0.3.0/harambot/database/models.py
--rw-r--r--   0        0        0     2833 2023-04-19 19:19:19.450118 harambot-0.3.0/harambot/ui/modals.py
--rw-r--r--   0        0        0     1117 2023-04-19 19:19:19.450118 harambot-0.3.0/harambot/ui/views.py
--rw-r--r--   0        0        0      850 2023-04-19 19:19:19.450118 harambot-0.3.0/harambot/utils.py
--rw-r--r--   0        0        0     7634 2023-04-19 19:19:19.450118 harambot-0.3.0/harambot/yahoo_api.py
--rw-r--r--   0        0        0     1474 2023-04-22 23:59:38.223462 harambot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 harambot-0.3.0/setup.py
--rw-r--r--   0        0        0     6577 1970-01-01 00:00:00.000000 harambot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-03-21 00:23:13.038328 harambot-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     3861 2023-06-16 19:20:54.292979 harambot-0.3.1/README.md
+-rw-r--r--   0        0        0   205449 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/discord-add-bot.png
+-rw-r--r--   0        0        0   297377 2022-09-30 15:15:31.381358 harambot-0.3.1/assests/discord-config-command.png
+-rw-r--r--   0        0        0   172632 2022-09-30 15:15:31.381358 harambot-0.3.1/assests/discord-config-dm.png
+-rw-r--r--   0        0        0   249813 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/discord-copy-token.png
+-rw-r--r--   0        0        0   181891 2022-11-11 15:59:03.669059 harambot-0.3.1/assests/discord-intents.png
+-rw-r--r--   0        0        0   177261 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/discord-new-application.png
+-rw-r--r--   0        0        0   217621 2022-09-30 15:15:31.381358 harambot-0.3.1/assests/discord-oauth-generator.png
+-rw-r--r--   0        0        0   251183 2022-09-30 15:15:31.381358 harambot-0.3.1/assests/discord-oauth-url-authorize-1.png
+-rw-r--r--   0        0        0   264428 2022-09-30 15:15:31.381358 harambot-0.3.1/assests/discord-oauth-url-authorize-2.png
+-rw-r--r--   0        0        0   120953 2023-06-12 23:06:21.945077 harambot-0.3.1/assests/harambot-1.jpg
+-rw-r--r--   0        0        0    40246 2023-04-26 00:49:46.631473 harambot-0.3.1/assests/harambot_configure_1.png
+-rw-r--r--   0        0        0    65725 2023-04-26 00:49:46.631473 harambot-0.3.1/assests/harambot_configure_2.png
+-rw-r--r--   0        0        0    35656 2023-06-12 23:06:21.945077 harambot-0.3.1/assests/harambot_configure_3.png
+-rw-r--r--   0        0        0    36723 2023-04-26 00:49:46.631473 harambot-0.3.1/assests/harambot_configure_4.png
+-rw-r--r--   0        0        0   207972 2022-09-30 15:15:31.381358 harambot-0.3.1/assests/heroku-deployment.png
+-rw-r--r--   0        0        0   118091 2022-11-11 15:59:03.669059 harambot-0.3.1/assests/heroku-dyno.png
+-rw-r--r--   0        0        0   156615 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/matchups.PNG
+-rw-r--r--   0        0        0    74049 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/player_details.PNG
+-rw-r--r--   0        0        0   530839 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/rip.PNG
+-rw-r--r--   0        0        0    69062 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/roster.PNG
+-rw-r--r--   0        0        0   104400 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/standings.PNG
+-rw-r--r--   0        0        0   107130 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/trade.PNG
+-rw-r--r--   0        0        0   478431 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/yahoo-app-details.png
+-rw-r--r--   0        0        0    91598 2022-03-21 00:23:13.048328 harambot-0.3.1/assests/yahoo-app-secrets.png
+-rw-r--r--   0        0        0   127686 2022-03-21 00:23:13.058328 harambot-0.3.1/assests/yahoo-create-app.png
+-rw-r--r--   0        0        0  1808878 2022-03-21 00:23:13.058328 harambot-0.3.1/assests/yahoo-league-id.png
+-rw-r--r--   0        0        0     1899 2023-06-16 19:20:54.292979 harambot-0.3.1/harambot/bot.py
+-rw-r--r--   0        0        0     2666 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/cogs/meta.py
+-rw-r--r--   0        0        0      953 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/cogs/misc.py
+-rw-r--r--   0        0        0      999 2023-06-16 19:20:54.292979 harambot-0.3.1/harambot/cogs/webserver.py
+-rw-r--r--   0        0        0    12158 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/cogs/yahoo.py
+-rw-r--r--   0        0        0      157 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/config.py
+-rw-r--r--   0        0        0      980 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/database/migrations.py
+-rw-r--r--   0        0        0      836 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/database/models.py
+-rw-r--r--   0        0        0     2833 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/ui/modals.py
+-rw-r--r--   0        0        0     1117 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/ui/views.py
+-rw-r--r--   0        0        0      850 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/utils.py
+-rw-r--r--   0        0        0     7634 2023-04-26 00:49:46.631473 harambot-0.3.1/harambot/yahoo_api.py
+-rw-r--r--   0        0        0     1479 2023-06-16 19:20:54.292979 harambot-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 harambot-0.3.1/PKG-INFO
```

### Comparing `harambot-0.3.0/LICENSE.md` & `harambot-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-add-bot.png` & `harambot-0.3.1/assests/discord-add-bot.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-config-command.png` & `harambot-0.3.1/assests/discord-config-command.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-config-dm.png` & `harambot-0.3.1/assests/discord-config-dm.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-copy-token.png` & `harambot-0.3.1/assests/discord-copy-token.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-intents.png` & `harambot-0.3.1/assests/discord-intents.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-new-application.png` & `harambot-0.3.1/assests/discord-new-application.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-oauth-generator.png` & `harambot-0.3.1/assests/discord-oauth-generator.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-oauth-url-authorize-1.png` & `harambot-0.3.1/assests/discord-oauth-url-authorize-1.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/discord-oauth-url-authorize-2.png` & `harambot-0.3.1/assests/discord-oauth-url-authorize-2.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/harambot_configure_1.png` & `harambot-0.3.1/assests/harambot_configure_1.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/harambot_configure_2.png` & `harambot-0.3.1/assests/harambot_configure_2.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/harambot_configure_4.png` & `harambot-0.3.1/assests/harambot_configure_4.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/heroku-deployment.png` & `harambot-0.3.1/assests/heroku-deployment.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/heroku-dyno.png` & `harambot-0.3.1/assests/heroku-dyno.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/matchups.PNG` & `harambot-0.3.1/assests/matchups.PNG`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/player_details.PNG` & `harambot-0.3.1/assests/player_details.PNG`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/rip.PNG` & `harambot-0.3.1/assests/rip.PNG`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/roster.PNG` & `harambot-0.3.1/assests/roster.PNG`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/standings.PNG` & `harambot-0.3.1/assests/standings.PNG`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/trade.PNG` & `harambot-0.3.1/assests/trade.PNG`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/yahoo-app-details.png` & `harambot-0.3.1/assests/yahoo-app-details.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/yahoo-app-secrets.png` & `harambot-0.3.1/assests/yahoo-app-secrets.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/yahoo-create-app.png` & `harambot-0.3.1/assests/yahoo-create-app.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/assests/yahoo-league-id.png` & `harambot-0.3.1/assests/yahoo-league-id.png`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/bot.py` & `harambot-0.3.1/harambot/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import discord
 
 
 from discord.ext import commands
 from harambot.cogs.meta import Meta
 from harambot.cogs.misc import Misc
 from harambot.cogs.yahoo import YahooCog
+
+from harambot.cogs.webserver import WebServer
 from harambot.config import settings
 from harambot.database.models import Guild
 from harambot.database.migrations import migrations
 
 # logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("harambot.py")
 if "LOGLEVEL" in settings:
@@ -27,14 +29,18 @@
 
 
 @bot.event
 async def on_ready():
     await bot.add_cog(Meta(bot))
     await bot.add_cog(YahooCog(bot, settings.yahoo_key, settings.yahoo_secret))
     await bot.add_cog(Misc(bot))
+    server = WebServer(bot)
+    await bot.add_cog(server)
+    bot.loop.create_task(server.webserver())
+
     if not Guild.table_exists():
         Guild.create_table()
     if "RUN_MIGRATIONS" in settings and settings.run_migrations:
         migrations[settings.version]()
     for guild in bot.guilds:
         bot.tree.copy_global_to(guild=guild)
         await bot.tree.sync(guild=guild)
```

### Comparing `harambot-0.3.0/harambot/cogs/meta.py` & `harambot-0.3.1/harambot/cogs/meta.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/cogs/misc.py` & `harambot-0.3.1/harambot/cogs/misc.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/cogs/yahoo.py` & `harambot-0.3.1/harambot/cogs/yahoo.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/database/migrations.py` & `harambot-0.3.1/harambot/database/migrations.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/database/models.py` & `harambot-0.3.1/harambot/database/models.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/ui/modals.py` & `harambot-0.3.1/harambot/ui/modals.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/ui/views.py` & `harambot-0.3.1/harambot/ui/views.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/utils.py` & `harambot-0.3.1/harambot/utils.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/harambot/yahoo_api.py` & `harambot-0.3.1/harambot/yahoo_api.py`

 * *Files identical despite different names*

### Comparing `harambot-0.3.0/pyproject.toml` & `harambot-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harambot"
-version = "0.3.0"
+version = "0.3.1"
 description = "A Yahoo Fantasy Sports bot for Discord"
 authors = ["DMcP89 <davemcpherson@wochstudios.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DMcP89/harambot"
 repository = "https://github.com/DMcP89/harambot"
 keywords = [
@@ -25,15 +25,15 @@
 
 packages = [
     {include = "harambot"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-discord = "^2.1.0"
+"discord.py" = "^2.1.0"
 dynaconf = "^3.1.11"
 peewee = "^3.15.4"
 cachetools = "^5.2.0"
 psycopg2 = "^2.9.5"
 mysqlclient = "^2.1.1"
 yahoo_fantasy_api = "2.7.0"
```

