# Comparing `tmp/honkairail-1.0.6.tar.gz` & `tmp/honkairail-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkairail-1.0.6.tar", max compression
+gzip compressed data, was "honkairail-1.0.7.tar", max compression
```

## Comparing `honkairail-1.0.6.tar` & `honkairail-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-06-05 03:59:10.580471 honkairail-1.0.6/honkairail/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 04:03:31.753289 honkairail-1.0.6/honkairail/src/__init__.py
--rw-r--r--   0        0        0      148 2023-06-05 09:07:32.687441 honkairail-1.0.6/honkairail/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-06-05 03:58:24.588036 honkairail-1.0.6/honkairail/src/tools/__init__.py
--rw-r--r--   0        0        0      154 2023-06-05 09:07:32.690434 honkairail-1.0.6/honkairail/src/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2869 2023-06-13 09:02:25.940990 honkairail-1.0.6/honkairail/src/tools/__pycache__/api.cpython-310.pyc
--rw-r--r--   0        0        0    12087 2023-06-09 11:33:55.802274 honkairail-1.0.6/honkairail/src/tools/__pycache__/modal.cpython-310.pyc
--rw-r--r--   0        0        0     5919 2023-06-13 09:00:08.334290 honkairail-1.0.6/honkairail/src/tools/__pycache__/modalV1.cpython-310.pyc
--rw-r--r--   0        0        0     7344 2023-06-13 09:03:44.338257 honkairail-1.0.6/honkairail/src/tools/__pycache__/modalV2.cpython-310.pyc
--rw-r--r--   0        0        0     1310 2023-06-09 11:18:15.642417 honkairail-1.0.6/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc
--rw-r--r--   0        0        0     2941 2023-06-17 12:58:36.838347 honkairail-1.0.6/honkairail/src/tools/api.py
--rw-r--r--   0        0        0     4982 2023-06-13 08:54:13.093344 honkairail-1.0.6/honkairail/src/tools/modalV1.py
--rw-r--r--   0        0        0     7083 2023-06-17 15:05:25.555223 honkairail-1.0.6/honkairail/src/tools/modalV2.py
--rw-r--r--   0        0        0     1127 2023-06-09 11:14:40.320720 honkairail-1.0.6/honkairail/src/tools/utilities.py
--rw-r--r--   0        0        0     1014 2023-06-17 14:55:45.750215 honkairail-1.0.6/honkairail/starrailapi.py
--rw-r--r--   0        0        0      489 2023-06-17 15:05:36.964040 honkairail-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3892 2023-06-10 09:41:05.266404 honkairail-1.0.6/README.md
--rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 honkairail-1.0.6/setup.py
--rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 honkairail-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 03:59:10.580471 honkairail-1.0.7/honkairail/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:03:31.753289 honkairail-1.0.7/honkairail/src/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-05 09:07:32.687441 honkairail-1.0.7/honkairail/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-06-05 03:58:24.588036 honkairail-1.0.7/honkairail/src/tools/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-05 09:07:32.690434 honkairail-1.0.7/honkairail/src/tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2869 2023-06-13 09:02:25.940990 honkairail-1.0.7/honkairail/src/tools/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0        0        0    12087 2023-06-09 11:33:55.802274 honkairail-1.0.7/honkairail/src/tools/__pycache__/modal.cpython-310.pyc
+-rw-r--r--   0        0        0     5919 2023-06-13 09:00:08.334290 honkairail-1.0.7/honkairail/src/tools/__pycache__/modalV1.cpython-310.pyc
+-rw-r--r--   0        0        0     7344 2023-06-13 09:03:44.338257 honkairail-1.0.7/honkairail/src/tools/__pycache__/modalV2.cpython-310.pyc
+-rw-r--r--   0        0        0     1310 2023-06-09 11:18:15.642417 honkairail-1.0.7/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc
+-rw-r--r--   0        0        0     2941 2023-06-17 12:58:36.838347 honkairail-1.0.7/honkairail/src/tools/api.py
+-rw-r--r--   0        0        0     4982 2023-06-13 08:54:13.093344 honkairail-1.0.7/honkairail/src/tools/modalV1.py
+-rw-r--r--   0        0        0     7125 2023-06-17 15:25:56.497661 honkairail-1.0.7/honkairail/src/tools/modalV2.py
+-rw-r--r--   0        0        0     1127 2023-06-09 11:14:40.320720 honkairail-1.0.7/honkairail/src/tools/utilities.py
+-rw-r--r--   0        0        0     1014 2023-06-17 14:55:45.750215 honkairail-1.0.7/honkairail/starrailapi.py
+-rw-r--r--   0        0        0      489 2023-06-17 15:26:40.636633 honkairail-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3892 2023-06-10 09:41:05.266404 honkairail-1.0.7/README.md
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 honkairail-1.0.7/setup.py
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 honkairail-1.0.7/PKG-INFO
```

### Comparing `honkairail-1.0.6/honkairail/src/tools/__pycache__/api.cpython-310.pyc` & `honkairail-1.0.7/honkairail/src/tools/__pycache__/api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/__pycache__/modal.cpython-310.pyc` & `honkairail-1.0.7/honkairail/src/tools/__pycache__/modal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/__pycache__/modalV1.cpython-310.pyc` & `honkairail-1.0.7/honkairail/src/tools/__pycache__/modalV1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/__pycache__/modalV2.cpython-310.pyc` & `honkairail-1.0.7/honkairail/src/tools/__pycache__/modalV2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc` & `honkairail-1.0.7/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/api.py` & `honkairail-1.0.7/honkairail/src/tools/api.py`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/modalV1.py` & `honkairail-1.0.7/honkairail/src/tools/modalV1.py`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/src/tools/modalV2.py` & `honkairail-1.0.7/honkairail/src/tools/modalV2.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         self.name = self.name.format(NICKNAME = "Trailblazer")
         self.icon = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.icon}"
         self.preview = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.preview}"
         self.portrait = f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{self.portrait}"
         new_rank_icons = []
         for key in self.rank_icons:
             new_rank_icons.append(f"https://raw.githubusercontent.com/Mar-7th/StarRailRes/master/{key}")
+        self.rank_icons = new_rank_icons
 
 
 class Avatar(BaseModel):
     id: Optional[str]
     name: Optional[str]
     icon: Optional[str]
```

### Comparing `honkairail-1.0.6/honkairail/src/tools/utilities.py` & `honkairail-1.0.7/honkairail/src/tools/utilities.py`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/honkairail/starrailapi.py` & `honkairail-1.0.7/honkairail/starrailapi.py`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/README.md` & `honkairail-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `honkairail-1.0.6/setup.py` & `honkairail-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['honkairail', 'honkairail.src', 'honkairail.src.tools']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkairail',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'A simple and convenient model for Mihoyo API which is complemented by other resources',
     'long_description': '# HonkaiRail\n A simple and convenient model for Mihoyo API which is complemented by other resources\n\n\n## Install:\n\n```\npip install honkairail\n```\n\n## Uses:\n``` py\nfrom honkairail import starrailapi\nimport asyncio\n\n#The sample code below matches version 1 (v = 1), but you can set it to 1 or 2. The second version is newer and contains a bit more data.\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang, v = 1)\n    data = await r.get_full_data(uid)\n    print(data)\n\nasyncio.run(main(700649319,"en"))\n```\n\n## Usage example:\n\n```py\nfrom honkairail import starrailapi\nimport asyncio\n\n\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang)\n    data = await r.get_full_data(uid)\n    print("====Player====")\n    print(f"Name: {data.player.name}")\n    print(f"UID: {data.player.uid}")\n    print(f"Level: {data.player.level}")\n    print(f"World Level: {data.player.worldlevel}")\n    \n    print(f"Friends: {data.player.friends}")\n\n    print(f"Pass Area Progress: {data.player.pass_area_progress}")\n    print(f"Achievement: {data.player.achievement}")\n\n    print(f"Characters: {data.player.characters}")\n    print(f"Light Cone: {data.player.light_cone}")\n\n    print(f"Icon: {data.player.icon}")\n    print(f"Signature: {data.player.signature}")\n    print(\'\\n\\n\')\n    print("====Characters====")\n    for character in data.characters:\n        print(f"Name: {character.name} | {character.id}")\n        print(f"Rarity: {\'★\'*character.rarity}")\n        print(f"LVL: {character.level}")\n        print(f"===={character.rank_text}====")\n        for rank in character.rank_icons:\n            print(f"Icon: {rank.icon}\\nUnlock: {rank.unlock}")\n        print("====Skill====")\n        for skill in character.skill:\n            print(f"Icon: {skill.icon}\\nLVL:{skill.level}")\n        print("=============")\n        if not character.light_cone is None:\n            print(f"Light Cone: {character.light_cone.name}")\n            print(f"Rarity: {\'★\'*character.light_cone.rarity}")\n            print(f"LVL: {character.light_cone.level} | R{character.light_cone.rank}")\n            print(f"Icon: {character.light_cone.icon}")\n            print(f"Portrait: {character.light_cone.portrait}")\n            light_cone = await r.get_light_cone_info(character.light_cone)\n            print(f"ATK: {light_cone.atk} | HP: {light_cone.hp} | DEF: {light_cone.defense}")\n            print(f"Path: {light_cone.patch.name}\\nImage: {light_cone.patch.url}")\n        print("====Stats====")\n        for property in character.property:\n            if property.addition is None:\n                print(f"{property.name}: {property.base}\\nIcon: {property.icon}")\n            else:\n                print(f"{property.name}: {property.base} ({property.addition})\\n==Icon: {property.icon}")\n        print(\'\\n\\n\')\n        print("====Relic====")\n        for i in character.relic:\n            print(f"{character.relic[i].name}: {character.relic[i].level} lvl | {\'★\'*character.relic[i].rarity}")\n            print(f"{character.relic[i].main_property.name}: {character.relic[i].main_property.value}")\n            for sub_property in character.relic[i].sub_property:\n                print(f"=={sub_property.name}: {sub_property.value}\\n====Icon: {sub_property.icon}")\n            print(\'\\n\')\n        print("\\n\\n")\n\nasyncio.run(main(700649319, "en"))\n```\n\n\n### Languages Supported\n| Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |\n|-------------|---------|-------------|---------|-------------|---------|\n|  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |\n|  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cn  |\n|  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |\n|  日本語      |     jp  | 中文        |     zh  | español    |     es  |\n|  中文        |     zh  | Indonesian |     id  | français   |     fr  |\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiRail',
```

### Comparing `honkairail-1.0.6/PKG-INFO` & `honkairail-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honkairail
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple and convenient model for Mihoyo API which is complemented by other resources
 Home-page: https://github.com/DEViantUA/HonkaiRail
 Author: None
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

