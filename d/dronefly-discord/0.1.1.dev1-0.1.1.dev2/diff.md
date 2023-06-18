# Comparing `tmp/dronefly_discord-0.1.1.dev1.tar.gz` & `tmp/dronefly_discord-0.1.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_discord-0.1.1.dev1.tar", max compression
+gzip compressed data, was "dronefly_discord-0.1.1.dev2.tar", max compression
```

## Comparing `dronefly_discord-0.1.1.dev1.tar` & `dronefly_discord-0.1.1.dev2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev1/LICENSE
--rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev1/README.md
--rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev1/dronefly/discord/__init__.py
--rw-r--r--   0        0        0     3430 2023-05-27 08:05:17.585923 dronefly_discord-0.1.1.dev1/dronefly/discord/embeds.py
--rw-r--r--   0        0        0      700 2023-06-03 21:17:43.151019 dronefly_discord-0.1.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev1/setup.py
--rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev2/LICENSE
+-rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev2/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev2/dronefly/discord/__init__.py
+-rw-r--r--   0        0        0     3500 2023-06-18 10:38:56.459872 dronefly_discord-0.1.1.dev2/dronefly/discord/embeds.py
+-rw-r--r--   0        0        0      722 2023-06-18 12:36:18.677638 dronefly_discord-0.1.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev2/setup.py
+-rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev2/PKG-INFO
```

### Comparing `dronefly_discord-0.1.1.dev1/LICENSE` & `dronefly_discord-0.1.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev1/README.md` & `dronefly_discord-0.1.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev1/dronefly/discord/embeds.py` & `dronefly_discord-0.1.1.dev2/dronefly/discord/embeds.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,34 +62,38 @@
     return format_taxon_names(*args, **kwargs)
 
 
 def make_embed(**kwargs):
     """Make a standard embed."""
     return discord.Embed(color=EMBED_COLOR, **kwargs)
 
+
 def make_taxa_embed(taxon: Taxon, formatter: TaxonFormatter, description: str):
     """Make a taxon embed."""
     embed = make_embed(
         url=f"{WWW_BASE_URL}/taxa/{taxon.id}",
         title=formatter.format_title(),
         description=description,
     )
     embed.set_thumbnail(
-        url=taxon.default_photo.square_url
-        if taxon.default_photo
-        else taxon.icon.url
+        url=taxon.default_photo.square_url if taxon.default_photo else taxon.icon.url
     )
     return embed
 
+
 def make_image_embed(taxon: Taxon, index, lang: str):
     formatter = TaxonFormatter(taxon, lang=lang, with_url=False)
     title = formatter.format_title()
 
     taxon_photo = None
-    if index == 1 and taxon.default_photo and not isinstance(taxon.default_photo, IconPhoto):
+    if (
+        index == 1
+        and taxon.default_photo
+        and not isinstance(taxon.default_photo, IconPhoto)
+    ):
         taxon_photo = taxon.default_photo
     elif index >= 1 and index <= len(taxon.taxon_photos):
         taxon_photo = taxon.taxon_photos[index - 1]
 
     embed = make_embed(url=f"{WWW_BASE_URL}/taxa/{taxon.id}")
     embed.title = title
 
@@ -98,9 +102,12 @@
         embed.set_footer(text=taxon_photo.attribution)
         embed.description = f"Photo {index} of {len(taxon.taxon_photos)}"
     else:
         if index == 1:
             embed.description = "This taxon has no default photo."
         else:
             count = len(taxon.taxon_photos)
-            embed.description = f"Photo number {index} not found.\nTaxon has {count} {p.plural('photo', count)}."
+            embed.description = (
+                f"Photo number {index} not found.\n"
+                f"Taxon has {count} {p.plural('photo', count)}."
+            )
     return embed
```

### Comparing `dronefly_discord-0.1.1.dev1/setup.py` & `dronefly_discord-0.1.1.dev2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 packages = \
 ['discord']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dronefly-core>=0.3.6.dev0,<0.4.0',
+['discord-py>=2.2.3,<3.0.0',
+ 'dronefly-core>=0.3.6.dev2,<0.4.0',
  'inflect>=5.3.0,<6.0.0',
  'pyinaturalist>=0.19.0.dev2,<0.20']
 
 setup_kwargs = {
     'name': 'dronefly-discord',
-    'version': '0.1.1.dev1',
+    'version': '0.1.1.dev2',
     'description': 'Dronefly Discord library',
     'long_description': "# Dronefly Discord\n\nThis library will support writing Discord cogs based on\n[dronefly-core](https://github.com/dronefly-garden/dronefly-core). It is\nderived from the Discord-specific code extracted from the original\n[Dronefly](https://dronefly.readthedocs.io) bot codebase. We aim to keep\nthe library general enough to work with any bot based on\n[discord.py](https://discordpy.readthedocs.io), as well as on bots using\nthe [Red-DiscordBot](https://docs.discord.red) framework.\n\n# Related packages\n\n## Dronefly core\n\nThe [dronefly-core](https://github.com/dronefly-garden/dronefly-core)\npackage is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io/)\nDiscord bot's core components.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_discord-0.1.1.dev1/PKG-INFO` & `dronefly_discord-0.1.1.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dronefly-discord
-Version: 0.1.1.dev1
+Version: 0.1.1.dev2
 Summary: Dronefly Discord library
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dronefly-core (>=0.3.6.dev0,<0.4.0)
+Requires-Dist: discord-py (>=2.2.3,<3.0.0)
+Requires-Dist: dronefly-core (>=0.3.6.dev2,<0.4.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
 Requires-Dist: pyinaturalist (>=0.19.0.dev2,<0.20)
 Description-Content-Type: text/markdown
 
 # Dronefly Discord
 
 This library will support writing Discord cogs based on
```

