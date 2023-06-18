# Comparing `tmp/gcocf-0.9.98.tar.gz` & `tmp/gcocf-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcocf-0.9.98.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gcocf-0.9.99.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gcocf-0.9.98.tar` & `gcocf-0.9.99.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      124 2023-06-17 11:26:51.690818 gcocf-0.9.98/.example.envrc
--rw-r--r--   0        0        0      669 2023-06-17 11:26:51.690818 gcocf-0.9.98/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      644 2023-06-17 11:26:51.690818 gcocf-0.9.98/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      501 2023-06-17 11:26:51.690818 gcocf-0.9.98/.github/dependabot.yml
--rw-r--r--   0        0        0     1076 2023-06-17 11:26:51.690818 gcocf-0.9.98/.github/pull_request_template.md
--rw-r--r--   0        0        0     2489 2023-06-17 11:26:51.690818 gcocf-0.9.98/.github/workflows/Testing.yml
--rw-r--r--   0        0        0      118 2023-06-17 11:26:51.690818 gcocf-0.9.98/.gitignore
--rw-r--r--   0        0        0     5224 2023-06-17 11:26:51.690818 gcocf-0.9.98/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      203 2023-06-17 11:26:51.690818 gcocf-0.9.98/CONTRIBUTING.md
--rw-r--r--   0        0        0      252 2023-06-17 11:26:51.690818 gcocf-0.9.98/Dockerfile
--rw-r--r--   0        0        0      145 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/__init__.py
--rwxr-xr-x   0        0        0    10649 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/__main__.py
--rw-r--r--   0        0        0     2224 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/api.py
--rw-r--r--   0        0        0    10419 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/formatters.py
--rw-r--r--   0        0        0     2369 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/locales/messages.pot
--rw-r--r--   0        0        0    12638 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/models.py
--rw-r--r--   0        0        0     1009 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/notifiers.py
--rw-r--r--   0        0        0     1378 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF/utils.py
--rw-r--r--   0        0        0     1603 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF_Bot/database.py
--rw-r--r--   0        0        0     2551 2023-06-17 11:26:51.690818 gcocf-0.9.98/GCoCF_Bot/service_bot.py
--rw-r--r--   0        0        0     1070 2023-06-17 11:26:51.690818 gcocf-0.9.98/LICENSE.txt
--rw-r--r--   0        0        0     1317 2023-06-17 11:26:51.690818 gcocf-0.9.98/README.md
--rw-r--r--   0        0        0     2495 2023-06-17 11:26:51.690818 gcocf-0.9.98/SECURITY.md
--rw-r--r--   0        0        0    41692 2023-06-17 11:26:51.690818 gcocf-0.9.98/data/full_destruction.json
--rw-r--r--   0        0        0    77643 2023-06-17 11:26:51.690818 gcocf-0.9.98/data/inWar_40.json
--rw-r--r--   0        0        0     1059 2023-06-17 11:26:51.690818 gcocf-0.9.98/data/notInWar.json
--rw-r--r--   0        0        0    24207 2023-06-17 11:26:51.690818 gcocf-0.9.98/data/op_full_destruction.json
--rw-r--r--   0        0        0    98300 2023-06-17 11:26:51.690818 gcocf-0.9.98/data/warEnded_50.json
--rw-r--r--   0        0        0      832 2023-06-17 11:26:51.690818 gcocf-0.9.98/pyproject.toml
--rw-r--r--   0        0        0       54 2023-06-17 11:26:51.690818 gcocf-0.9.98/requirements.txt
--rw-r--r--   0        0        0    13950 2023-06-17 11:26:51.690818 gcocf-0.9.98/test_everything.py
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 gcocf-0.9.98/PKG-INFO
+-rw-r--r--   0        0        0      174 2023-06-17 15:58:34.665051 gcocf-0.9.99/.example.envrc
+-rw-r--r--   0        0        0      669 2023-06-17 15:58:34.665051 gcocf-0.9.99/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      644 2023-06-17 15:58:34.665051 gcocf-0.9.99/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      501 2023-06-17 15:58:34.665051 gcocf-0.9.99/.github/dependabot.yml
+-rw-r--r--   0        0        0     1076 2023-06-17 15:58:34.665051 gcocf-0.9.99/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2582 2023-06-17 15:58:34.665051 gcocf-0.9.99/.github/workflows/Testing.yml
+-rw-r--r--   0        0        0      118 2023-06-17 15:58:34.665051 gcocf-0.9.99/.gitignore
+-rw-r--r--   0        0        0     5224 2023-06-17 15:58:34.665051 gcocf-0.9.99/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      203 2023-06-17 15:58:34.665051 gcocf-0.9.99/CONTRIBUTING.md
+-rw-r--r--   0        0        0      252 2023-06-17 15:58:34.665051 gcocf-0.9.99/Dockerfile
+-rw-r--r--   0        0        0      145 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/__init__.py
+-rwxr-xr-x   0        0        0    10649 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/__main__.py
+-rw-r--r--   0        0        0     2224 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/api.py
+-rw-r--r--   0        0        0    10419 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/formatters.py
+-rw-r--r--   0        0        0     2369 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/locales/messages.pot
+-rw-r--r--   0        0        0    12638 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/models.py
+-rw-r--r--   0        0        0     1009 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/notifiers.py
+-rw-r--r--   0        0        0     1378 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF/utils.py
+-rw-r--r--   0        0        0     2215 2023-06-17 15:58:34.665051 gcocf-0.9.99/GCoCF_Bot/database.py
+-rw-r--r--   0        0        0     5034 2023-06-17 15:58:34.669051 gcocf-0.9.99/GCoCF_Bot/service_bot.py
+-rw-r--r--   0        0        0     1070 2023-06-17 15:58:34.669051 gcocf-0.9.99/LICENSE.txt
+-rw-r--r--   0        0        0     1317 2023-06-17 15:58:34.669051 gcocf-0.9.99/README.md
+-rw-r--r--   0        0        0     2495 2023-06-17 15:58:34.669051 gcocf-0.9.99/SECURITY.md
+-rw-r--r--   0        0        0    41692 2023-06-17 15:58:34.669051 gcocf-0.9.99/data/full_destruction.json
+-rw-r--r--   0        0        0    77643 2023-06-17 15:58:34.669051 gcocf-0.9.99/data/inWar_40.json
+-rw-r--r--   0        0        0     1059 2023-06-17 15:58:34.669051 gcocf-0.9.99/data/notInWar.json
+-rw-r--r--   0        0        0    24207 2023-06-17 15:58:34.669051 gcocf-0.9.99/data/op_full_destruction.json
+-rw-r--r--   0        0        0    98300 2023-06-17 15:58:34.669051 gcocf-0.9.99/data/warEnded_50.json
+-rw-r--r--   0        0        0      832 2023-06-17 15:58:34.669051 gcocf-0.9.99/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-17 15:58:34.669051 gcocf-0.9.99/requirements.txt
+-rw-r--r--   0        0        0    13950 2023-06-17 15:58:34.669051 gcocf-0.9.99/test_everything.py
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 gcocf-0.9.99/PKG-INFO
```

### Comparing `gcocf-0.9.98/.github/ISSUE_TEMPLATE/bug_report.md` & `gcocf-0.9.99/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/.github/ISSUE_TEMPLATE/feature_request.md` & `gcocf-0.9.99/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/.github/pull_request_template.md` & `gcocf-0.9.99/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/.github/workflows/Testing.yml` & `gcocf-0.9.99/.github/workflows/Testing.yml`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,25 @@
           pip install pytest
           pytest test_everything.py
 
   build-and-publish:
     needs: [build-and-test]
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && github.ref == 'refs/heads/master'
+    strategy:
+      matrix:
+        python-version: [3.11]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v3.1.4
         with:
-          python-version: '3.11'
+          python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flit
         #  pip install pyarmor
 
@@ -70,22 +73,22 @@
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && github.ref == 'refs/heads/master'
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Log in to GitHub Container Registry
-        uses: docker/login-action@v1
+        uses: docker/login-action@v2.2.0
         with:
           registry: ghcr.io
           username: ${{ github.actor }}
           password: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Build and push Docker image
-        uses: docker/build-push-action@v2
+        uses: docker/build-push-action@v4.1.1
         with:
           context: .
           push: true
           tags: ghcr.io/gillesmaster/gcocf/gcocf:latest
           
   send-summary:
     runs-on: ubuntu-latest
@@ -93,11 +96,11 @@
     needs:
       - build-and-test
       - build-and-publish
       - build-and-contain
 
     steps:
       - name: Send Test Summary
-        uses: CalmDownVal/webhook-summary@v1
+        uses: CalmDownVal/webhook-summary@v1.0.2
         with:
           token: ${{ secrets.TOKEN }}
           url: ${{ secrets.WEBHOOK_URL }}
```

### Comparing `gcocf-0.9.98/CODE_OF_CONDUCT.md` & `gcocf-0.9.99/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/__main__.py` & `gcocf-0.9.99/GCoCF/__main__.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/api.py` & `gcocf-0.9.99/GCoCF/api.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/formatters.py` & `gcocf-0.9.99/GCoCF/formatters.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/locales/messages.pot` & `gcocf-0.9.99/GCoCF/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/models.py` & `gcocf-0.9.99/GCoCF/models.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/notifiers.py` & `gcocf-0.9.99/GCoCF/notifiers.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF/utils.py` & `gcocf-0.9.99/GCoCF/utils.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/GCoCF_Bot/database.py` & `gcocf-0.9.99/GCoCF_Bot/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,75 @@
 import sqlite3
 from typing import Optional, Tuple
 
 
+DB_NAME = "service_bot.db"
+
 def setup_database():
-    conn = sqlite3.connect("service_bot.db")
+    conn = sqlite3.connect(DB_NAME)
     c = conn.cursor()
+
     c.execute("""
         CREATE TABLE IF NOT EXISTS users (
             user_id INTEGER PRIMARY KEY,
             api_key TEXT NOT NULL,
             webhook_url TEXT NOT NULL,
             clan_tag TEXT NOT NULL,
             instance_count INTEGER NOT NULL
         )
     """)
+
+    c.execute("""
+        CREATE TABLE IF NOT EXISTS whitelist (
+            user_id INTEGER PRIMARY KEY
+        )
+    """)
+
     conn.commit()
     conn.close()
 
+async def is_user_whitelisted(user_id: int) -> bool:
+    with sqlite3.connect(DB_NAME) as conn:
+        cursor = conn.cursor()
+        cursor.execute("SELECT * FROM whitelist WHERE user_id=?", (user_id,))
+        return cursor.fetchone() is not None
+    
+async def add_user_to_whitelist(target_id: int):
+    with sqlite3.connect(DB_NAME) as conn:
+        cursor = conn.cursor()
+        cursor.execute("INSERT OR IGNORE INTO whitelist (user_id) VALUES (?)", (target_id,))
+        conn.commit()
 
 async def store_user_data(user_id: int, api_key: str, webhook_url: str, clan_tag: str):
-    conn = sqlite3.connect("service_bot.db")
+    conn = sqlite3.connect(DB_NAME)
     c = conn.cursor()
 
     c.execute("SELECT * FROM users WHERE user_id=?", (user_id,))
     user_data = c.fetchone()
     if user_data is None:
         c.execute("INSERT INTO users VALUES (?, ?, ?, ?, 0)", (user_id, api_key, webhook_url, clan_tag))
     else:
         c.execute("UPDATE users SET api_key=?, webhook_url=?, clan_tag=? WHERE user_id=?", (api_key, webhook_url, clan_tag, user_id))
 
     conn.commit()
     conn.close()
 
 async def get_user_data(user_id: int) -> Optional[Tuple[int, str, str, str, int]]:
-    conn = sqlite3.connect("service_bot.db")
+    conn = sqlite3.connect(DB_NAME)
     c = conn.cursor()
 
     c.execute("SELECT user_id, api_key, webhook_url, clan_tag, instance_count FROM users WHERE user_id=?", (user_id,))
     user_data = c.fetchone()
 
     conn.close()
 
     return user_data
 
 
 async def update_instance_count(user_id: int, count: int):
-    conn = sqlite3.connect("service_bot.db")
+    conn = sqlite3.connect(DB_NAME)
     c = conn.cursor()
 
     c.execute("UPDATE users SET instance_count=? WHERE user_id=?", (count, user_id))
 
     conn.commit()
     conn.close()
```

### Comparing `gcocf-0.9.98/LICENSE.txt` & `gcocf-0.9.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/README.md` & `gcocf-0.9.99/README.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/SECURITY.md` & `gcocf-0.9.99/SECURITY.md`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/data/full_destruction.json` & `gcocf-0.9.99/data/full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/data/inWar_40.json` & `gcocf-0.9.99/data/inWar_40.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/data/notInWar.json` & `gcocf-0.9.99/data/notInWar.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/data/op_full_destruction.json` & `gcocf-0.9.99/data/op_full_destruction.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/data/warEnded_50.json` & `gcocf-0.9.99/data/warEnded_50.json`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/pyproject.toml` & `gcocf-0.9.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/test_everything.py` & `gcocf-0.9.99/test_everything.py`

 * *Files identical despite different names*

### Comparing `gcocf-0.9.98/PKG-INFO` & `gcocf-0.9.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCoCF
-Version: 0.9.98
+Version: 0.9.99
 Summary: Clash of Clans war moniting for Discord.
 Home-page: https://github.com/GILLESMaster/GCoCF
 Keywords: coc clashofclans discord
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

