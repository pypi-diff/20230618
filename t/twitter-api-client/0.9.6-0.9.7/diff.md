# Comparing `tmp/twitter-api-client-0.9.6.tar.gz` & `tmp/twitter-api-client-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.6.tar", last modified: Thu Jun 15 18:23:06 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.7.tar", last modified: Sun Jun 18 18:59:42 2023, max compression
```

## Comparing `twitter-api-client-0.9.6.tar` & `twitter-api-client-0.9.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-15 18:23:06.605269 twitter-api-client-0.9.6/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.9.6/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    11479 2023-06-15 18:23:06.605269 twitter-api-client-0.9.6/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-15 18:23:06.605269 twitter-api-client-0.9.6/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    13412 2023-06-15 18:22:46.000000 twitter-api-client-0.9.6/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-15 18:23:06.604269 twitter-api-client-0.9.6/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.9.6/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    26861 2023-06-15 17:57:39.000000 twitter-api-client-0.9.6/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    30104 2023-06-15 18:20:32.000000 twitter-api-client-0.9.6/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-15 17:28:10.000000 twitter-api-client-0.9.6/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-15 17:57:39.000000 twitter-api-client-0.9.6/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-15 17:57:39.000000 twitter-api-client-0.9.6/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-15 17:31:50.000000 twitter-api-client-0.9.6/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-15 18:23:06.604269 twitter-api-client-0.9.6/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    11479 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-15 18:23:06.000000 twitter-api-client-0.9.6/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-18 18:59:42.179033 twitter-api-client-0.9.7/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    11750 2023-06-18 18:59:42.179033 twitter-api-client-0.9.7/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-18 18:59:42.179033 twitter-api-client-0.9.7/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    13719 2023-06-18 18:58:01.000000 twitter-api-client-0.9.7/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-18 18:59:42.175700 twitter-api-client-0.9.7/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    28656 2023-06-18 18:48:03.000000 twitter-api-client-0.9.7/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    30178 2023-06-18 18:29:35.000000 twitter-api-client-0.9.7/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9855 2023-06-16 21:34:23.000000 twitter-api-client-0.9.7/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-18 18:59:42.175700 twitter-api-client-0.9.7/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    11750 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-18 18:59:42.000000 twitter-api-client-0.9.7/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.6/LICENSE` & `twitter-api-client-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.6/PKG-INFO` & `twitter-api-client-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.6
+Version: 0.9.7
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -127,22 +127,31 @@
 # get timelines
 timeline = account.home_timeline()
 latest_timeline = account.home_latest_timeline(limit=500)
 
 # get bookmarks
 bookmarks = account.bookmarks()
 
-# get all dms
-dms = account.dm_history(['12345-67890'])
+# get DM inbox metadata    
+inbox = account.dm_inbox()
 
-# search dms
-dms = account.dm_search('test')
+# get DMs from all conversations    
+dms = account.dm_history()
 
-# delete conversation
-account.dm_delete('12345-67890')
+# get DMs from specific conversations
+dms = account.dm_history(['123456-789012', '345678-901234'])
+
+# search DMs by keyword
+dms = account.dm_search('test123')
+
+# delete entire conversation
+account.dm_delete(conversation_id='123456-789012')
+
+# delete (hide) specific DM
+account.dm_delete(message_id='123456')
 
 # example configuration
 account.update_settings({
     "address_book_live_sync_enabled": False,
     "allow_ads_personalization": False,
     "allow_authenticated_periscope_requests": True,
     "allow_dm_groups_from": "following",
```

### Comparing `twitter-api-client-0.9.6/setup.py` & `twitter-api-client-0.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.6",
+    version="0.9.7",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
     
@@ -134,22 +134,31 @@
     # get timelines
     timeline = account.home_timeline()
     latest_timeline = account.home_latest_timeline(limit=500)
     
     # get bookmarks
     bookmarks = account.bookmarks()
     
-    # get all dms
-    dms = account.dm_history(['12345-67890'])
+    # get DM inbox metadata    
+    inbox = account.dm_inbox()
     
-    # search dms
-    dms = account.dm_search('test')
+    # get DMs from all conversations    
+    dms = account.dm_history()
     
-    # delete conversation
-    account.dm_delete('12345-67890')
+    # get DMs from specific conversations
+    dms = account.dm_history(['123456-789012', '345678-901234'])
+    
+    # search DMs by keyword
+    dms = account.dm_search('test123')
+    
+    # delete entire conversation
+    account.dm_delete(conversation_id='123456-789012')
+    
+    # delete (hide) specific DM
+    account.dm_delete(message_id='123456')
     
     # example configuration
     account.update_settings({
         "address_book_live_sync_enabled": False,
         "allow_ads_personalization": False,
         "allow_authenticated_periscope_requests": True,
         "allow_dm_groups_from": "following",
```

### Comparing `twitter-api-client-0.9.6/twitter/account.py` & `twitter-api-client-0.9.7/twitter/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -602,62 +602,119 @@
             _session = Client(cookies=orjson.loads(Path(cookies).read_bytes()), follow_redirects=True)
             _session.headers.update(get_headers(_session))
             return _session
 
         raise Exception('Session not authenticated. '
                         'Please use an authenticated session or remove the `session` argument and try again.')
 
-    def dm_history(self, conversation_ids: list[str]) -> list[dict]:
+    def dm_inbox(self) -> dict:
+        """
+        Get DM inbox metadata.
+
+        @return: inbox as dict
+        """
+        r = self.session.get(
+            f'{self.v1_api}/dm/inbox_initial_state.json',
+            headers=get_headers(self.session),
+            params=dm_params
+        )
+        return r.json()
+
+    def dm_history(self, conversation_ids: list[str] = None) -> list[dict]:
+        """
+        Get DM history.
+
+        Call without arguments to get all DMS from all conversations.
+
+        @param conversation_ids: optional list of conversation ids
+        @return: list of messages as dicts
+        """
+
         async def get(session: AsyncClient, conversation_id: str):
-            params = deepcopy(dm_history_params)
+            params = deepcopy(dm_params)
             r = await session.get(
                 f'{self.v1_api}/dm/conversation/{conversation_id}.json',
                 params=params,
             )
             res = r.json().get('conversation_timeline', {})
-            data = [x['message'] for x in res.get('entries', [])]
+            data = [x.get('message') for x in res.get('entries', [])]
             entry_id = res.get('min_entry_id')
             while entry_id:
                 params['max_id'] = entry_id
                 r = await session.get(
                     f'{self.v1_api}/dm/conversation/{conversation_id}.json',
                     params=params,
                 )
                 res = r.json().get('conversation_timeline', {})
                 data.extend(x['message'] for x in res.get('entries', []))
                 entry_id = res.get('min_entry_id')
             return data
 
-        async def process():
+        async def process(ids):
             limits = Limits(max_connections=100)
             headers, cookies = get_headers(self.session), self.session.cookies
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
-                return await tqdm_asyncio.gather(*(get(c, _id) for _id in conversation_ids), desc="Getting DMs")
-
-        return asyncio.run(process())
+                return await tqdm_asyncio.gather(*(get(c, _id) for _id in ids), desc="Getting DMs")
 
-    def dm_delete(self, conversation_id: str):
-        return self.session.post(
-            f'{self.v1_api}/dm/conversation/{conversation_id}/delete.json',
-            headers=get_headers(self.session),
-        )
+        if conversation_ids:
+            ids = conversation_ids
+        else:
+            # get all conversations
+            inbox = self.dm_inbox()
+            ids = list(inbox['inbox_initial_state']['conversations'])
+
+        return asyncio.run(process(ids))
+
+    def dm_delete(self, *, conversation_id: str = None, message_id: str = None) -> dict:
+        """
+        Delete operations
+
+        - delete (hide) a single DM
+        - delete an entire conversation
+
+        @param conversation_id: the conversation id
+        @param message_id: the message id
+        @return: result metadata
+        """
+        self.session.headers.update(headers=get_headers(self.session))
+        results = {'conversation': None, 'message': None}
+        if conversation_id:
+            results['conversation'] = self.session.post(
+                f'{self.v1_api}/dm/conversation/{conversation_id}/delete.json',
+            ).text  # not json response
+        if message_id:
+            # delete single message
+            _id, op = Operation.DMMessageDeleteMutation
+            results['message'] = self.session.post(
+                f'https://twitter.com/i/api/graphql/{_id}/{op}',
+                json={'queryId': _id, 'variables': {'messageId': message_id}},
+            ).json()
+        return results
+
+    def dm_search(self, query: str) -> dict:
+        """
+        Search DMs by keyword
+
+        @param query: search term
+        @return: search results as dict
+        """
 
-    def dm_search(self, query: str):
         def get(cursor=None):
             if cursor:
                 params['variables']['cursor'] = cursor.pop()
             _id, op = Operation.DmAllSearchSlice
             r = self.session.get(
                 f'https://twitter.com/i/api/graphql/{_id}/{op}',
-                params=build_params(params)
+                params=build_params(params),
             )
             res = r.json()
             cursor = find_key(res, 'next_cursor')
             return res, cursor
 
+        self.session.headers.update(headers=get_headers(self.session))
         variables = deepcopy(Operation.default_variables)
         variables['count'] = 50  # strict limit, errors thrown if exceeded
         variables['query'] = query
         params = {'variables': variables, 'features': Operation.default_features}
         res, cursor = get()
         data = [res]
         while cursor:
```

### Comparing `twitter-api-client-0.9.6/twitter/constants.py` & `twitter-api-client-0.9.7/twitter/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,15 @@
     DeleteTweetReaction = 'GKwK0Rj4EdkfwdHQMZTpuw', 'DeleteTweetReaction'
     DisableUserAccountLabel = '_ckHEj05gan2VfNHG6thBA', 'DisableUserAccountLabel'
     DisableVerifiedPhoneLabel = 'g2m0pAOamawNtVIfjXNMJg', 'DisableVerifiedPhoneLabel'
     DismissRitoSuggestedAction = 'jYvwa61cv3NwNP24iUru6g', 'DismissRitoSuggestedAction'
     DmAllSearchSlice = 'U-QXVRZ6iddb1QuZweh5DQ', 'DmAllSearchSlice'
     DmGroupSearchSlice = '5zpY1dCR-8NyxQJS_CFJoQ', 'DmGroupSearchSlice'
     DmMutedTimeline = 'lrcWa13oyrQc7L33wRdLAQ', 'DmMutedTimeline'
+    DMMessageDeleteMutation = 'BJ6DtxA2llfjnRoRjaiIiw', 'DMMessageDeleteMutation'
     DmNsfwMediaFilterUpdate = 'of_N6O33zfyD4qsFJMYFxA', 'DmNsfwMediaFilterUpdate'
     DmPeopleSearchSlice = 'xYSm8m5kJnzm_gFCn5GH-w', 'DmPeopleSearchSlice'
     EditBookmarkFolder = 'a6kPp1cS1Dgbsjhapz1PNw', 'EditBookmarkFolder'
     EditDraftTweet = 'JIeXE-I6BZXHfxsgOkyHYQ', 'EditDraftTweet'
     EditScheduledTweet = '_mHkQ5LHpRRjSXKOcG6eZw', 'EditScheduledTweet'
     EnableLoggedOutWebNotifications = 'BqIHKmwZKtiUBPi07jKctg', 'EnableLoggedOutWebNotifications'
     EnableVerifiedPhoneLabel = 'C3RJFfMsb_KcEytpKmRRkw', 'EnableVerifiedPhoneLabel'
@@ -557,15 +558,15 @@
     'requestContext': 'launch',
     'pc': 1,
     'spelling_corrections': 1,
     'include_ext_edit_control': 'true',
     'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,collab_control,vibe'
 }
 
-dm_history_params = {
+dm_params = {
     'context': 'FETCH_DM_CONVERSATION',
     'include_profile_interstitial_type': '1',
     'include_blocking': '1',
     'include_blocked_by': '1',
     'include_followed_by': '1',
     'include_want_retweets': '1',
     'include_mute_edge': '1',
```

### Comparing `twitter-api-client-0.9.6/twitter/login.py` & `twitter-api-client-0.9.7/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.6/twitter/scraper.py` & `twitter-api-client-0.9.7/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.6/twitter/search.py` & `twitter-api-client-0.9.7/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.6/twitter/util.py` & `twitter-api-client-0.9.7/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.6/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.7/twitter_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.6
+Version: 0.9.7
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -127,22 +127,31 @@
 # get timelines
 timeline = account.home_timeline()
 latest_timeline = account.home_latest_timeline(limit=500)
 
 # get bookmarks
 bookmarks = account.bookmarks()
 
-# get all dms
-dms = account.dm_history(['12345-67890'])
+# get DM inbox metadata    
+inbox = account.dm_inbox()
 
-# search dms
-dms = account.dm_search('test')
+# get DMs from all conversations    
+dms = account.dm_history()
 
-# delete conversation
-account.dm_delete('12345-67890')
+# get DMs from specific conversations
+dms = account.dm_history(['123456-789012', '345678-901234'])
+
+# search DMs by keyword
+dms = account.dm_search('test123')
+
+# delete entire conversation
+account.dm_delete(conversation_id='123456-789012')
+
+# delete (hide) specific DM
+account.dm_delete(message_id='123456')
 
 # example configuration
 account.update_settings({
     "address_book_live_sync_enabled": False,
     "allow_ads_personalization": False,
     "allow_authenticated_periscope_requests": True,
     "allow_dm_groups_from": "following",
```

