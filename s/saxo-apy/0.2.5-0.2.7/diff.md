# Comparing `tmp/saxo_apy-0.2.5.tar.gz` & `tmp/saxo_apy-0.2.7.tar.gz`

## Comparing `saxo_apy-0.2.5.tar` & `saxo_apy-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/.DS_Store
--rw-r--r--   0        0        0   211911 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/pdm.lock
--rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/01_getting_started.ipynb
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/02_advanced_login.ipynb
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/03_session_management.ipynb
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/04_debugging_and_logging.ipynb
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/05_price_alerts_crud.ipynb
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/06_instrument_search.ipynb
--rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/07_pricing_and_orders.ipynb
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/README.md
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/s01_async_requests.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/samples/s02_streaming_prices.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/__init__.py
--rw-r--r--   0        0        0    18398 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/client.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/models.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/redirect_server.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/utils.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/saxo_apy/version.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/test_client.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/test_models.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/test_utils.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/dummy_access_token.txt
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/dummy_app_config_live.json
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/dummy_app_config_sim.json
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/tests/fixtures/models.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/LICENSE
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/README.md
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 saxo_apy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/.DS_Store
+-rw-r--r--   0        0        0   211911 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/pdm.lock
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/01_getting_started.ipynb
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/02_advanced_login.ipynb
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/03_session_management.ipynb
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/04_debugging_and_logging.ipynb
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/05_price_alerts_crud.ipynb
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/06_instrument_search.ipynb
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/07_pricing_and_orders.ipynb
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/README.md
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/s01_async_requests.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/samples/s02_streaming_prices.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/saxo_apy/__init__.py
+-rw-r--r--   0        0        0    18457 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/saxo_apy/client.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/saxo_apy/models.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/saxo_apy/redirect_server.py
+-rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/saxo_apy/utils.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/saxo_apy/version.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/test_client.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/test_models.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/test_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/fixtures/dummy_access_token.txt
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/fixtures/dummy_app_config_live.json
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/fixtures/dummy_app_config_sim.json
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/tests/fixtures/models.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/LICENSE
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/README.md
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 saxo_apy-0.2.7/PKG-INFO
```

### Comparing `saxo_apy-0.2.5/.DS_Store` & `saxo_apy-0.2.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/pdm.lock` & `saxo_apy-0.2.7/pdm.lock`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/samples/01_getting_started.ipynb` & `saxo_apy-0.2.7/samples/01_getting_started.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951980311355312%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'text': {insert: [(2, '✅ authorization succeeded - connected to "*

 * *            'SIM environment with WRITE / TRADE permissions (session ID: '*

 * *            "aff96bc0ed7e482fb57e0c9d6428e605)\\n')], delete: [2]}}}, 'source': "*

 * *            "['client.login(start_async_refresh=True)']}, 6: {'outputs': {0: {'data': "*

 * *            '{\'text/plain\': ["\'2023-06-18T08:05:10+00:00\'"]}}}}, 7: {\'outputs\': {0: '*

 * *            '{\'data\': {\'text/plain\': ["\'vJnkGyXeBw\'"]}}}}, 8: {\'atta […]*

```diff
@@ -61,20 +61,20 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\ud83c\udf10 opening login page in browser - waiting for user to authenticate... \ud83d\udd11\n",
                         "\ud83d\udcde received callback from Saxo SSO\n",
-                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID: 4a3e4ae6939e456cadd88318ab23d70a)\n"
+                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID: aff96bc0ed7e482fb57e0c9d6428e605)\n"
                     ]
                 }
             ],
             "source": [
-                "client.login()"
+                "client.login(start_async_refresh=True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -106,15 +106,15 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'2023-01-22T09:57:48+00:00'"
+                            "'2023-06-18T08:05:10+00:00'"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -127,28 +127,29 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'DS227MQdeA'"
+                            "'vJnkGyXeBw'"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# show the last 10 characters of the current access token\n",
                 "client._token_data.access_token[-10:]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If the client is configured to refresh the tokens automatically, it will periodically call the SSO service for new tokens (30 seconds before expiry). It is also possible to explicitly refresh the session:"
             ]
         },
         {
@@ -164,15 +165,15 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'2023-01-22T09:57:56+00:00'"
+                            "'2023-06-18T08:05:15+00:00'"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -185,15 +186,15 @@
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'fgzrvU7F4Q'"
+                            "'GSZ2jy9uRg'"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -238,15 +239,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.1 (main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-1400.0.29.202)]"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "3f753197f020b6236bb06be37c192ff4bc0da2ccc1bf66f005a7556bcabdf016"
             }
         }
```

### Comparing `saxo_apy-0.2.5/samples/02_advanced_login.ipynb` & `saxo_apy-0.2.7/samples/02_advanced_login.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/samples/03_session_management.ipynb` & `saxo_apy-0.2.7/samples/03_session_management.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9934313482337379%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'At this point, a *OpenAPI session* has commenced, "*

 * *            "identified by a session id which typically looks something like this:\\n')], delete: "*

 * *            "[4]}}, 1: {'execution_count': 1, 'outputs': [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['🌐 opening login page in browser - waiting for "*

 * *            "user to authenticate... 🔑\\n', '📞 received callback from Saxo SSO\\n', '✅ "*

 * *            'authorization succeeded […]*

```diff
@@ -5,15 +5,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Managing the OpenAPI Session\n",
                 "\n",
                 "After login, the client will automatically retrieve a token pair (access and refresh token) from the endpoint specified in your app's application config. This is a default `/token` endpoint specific to the environment that your app is running in, which is what all applications use to generate tokens (standard OAuth implementation).\n",
                 "\n",
-                "At this point, a 'OpenAPI session' has commenced, identified by a session id which typically looks something like this:\n",
+                "At this point, a *OpenAPI session* has commenced, identified by a session id which typically looks something like this:\n",
                 "\n",
                 "```\n",
                 "95af38e86c1547fdafc4204a0684ded7\n",
                 "```\n",
                 "\n",
                 "By default, the access token is only valid for 20 minutes, after which it expires and the session is automatically disconnected. Requests to OpenAPI will error out with a 401 Unauthorized response if an expired token is used, which effectively means that the client is no longer logged in. Restricting token lifetimes is a fairly typical security measure to prevent tokens 'falling in the wrong hands' from being useful for extended periods (reducing the attack surface of a potential bad actor).\n",
                 "\n",
@@ -28,17 +28,27 @@
                 "Because of the ease-of-use and the prevalence of Jupyter Notebooks in the Python community, the client has a simple feature to keep the session authenticated as long as the notebook is 'running' (i.e. it is not closed/exited and the kernel is not restarted).\n",
                 "\n",
                 "When the `login()` method is called, set the following parameter to enable the refresh loop:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\ud83c\udf10 opening login page in browser - waiting for user to authenticate... \ud83d\udd11\n",
+                        "\ud83d\udcde received callback from Saxo SSO\n",
+                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID: a9689adda1614b629b6f5730ab1e129f)\n"
+                    ]
+                }
+            ],
             "source": [
                 "from saxo_apy import SaxoOpenAPIClient\n",
                 "\n",
                 "client = SaxoOpenAPIClient()\n",
                 "client.login(start_async_refresh=True)  # this will automatically hook to Jupyter's async loop to refresh the session"
             ]
         },
@@ -74,21 +84,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import asyncio\n",
+                "\n",
                 "client = SaxoOpenAPIClient()\n",
                 "client.login()\n",
                 "\n",
                 "\n",
                 "async def main() -> None:\n",
                 "    # do all kinds of application logic here\n",
-                "    # make sure nothing in here is looping/blocking otherwise the refresh call won't be reached\n",
+                "    # make sure nothing in here is blocking otherwise the refresh call won't be reached\n",
                 "\n",
                 "    # ensure that asyncio schedules the refresh loop\n",
                 "    asyncio.ensure_future(client.async_refresh())\n",
                 "\n",
                 "\n",
                 "# run the app\n",
                 "asyncio.run(main())"
@@ -100,15 +112,15 @@
             "metadata": {},
             "source": [
                 "## Confirming Refreshing is Correctly Scheduled\n",
                 "\n",
                 "If the refresh loop is correctly set up and the client has logging enabled (see next sample), the following DEBUG messages will come up in the logs confirming that the refresh flow is scheduled. The client waits until 30 seconds before the access token expires to refresh the session.\n",
                 "\n",
                 "```\n",
-                "DEBUG    client             237 async_refresh             async refresh will kick off refresh flow in 1169 seconds at: 2023-01-31 20:22:56+00:00\n",
+                "2023-03-23 15:35:32.631Z   DEBUG    client             244 async_refresh             async refresh will kick off refresh flow in 1170 seconds at: 2023-03-23 15:55:02+00:00\n",
                 "\n",
                 "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -122,15 +134,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.1 (main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-1400.0.29.202)]"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "3f753197f020b6236bb06be37c192ff4bc0da2ccc1bf66f005a7556bcabdf016"
             }
         }
```

### Comparing `saxo_apy-0.2.5/samples/05_price_alerts_crud.ipynb` & `saxo_apy-0.2.7/samples/05_price_alerts_crud.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984691472742944%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': {insert: [(2, '✅ authorization succeeded - connected to "*

 * *            'SIM environment with WRITE / TRADE permissions (session ID: '*

 * *            "2757e3a96e9c4687a498ae9bc86c2c86)\\n')], delete: [2]}}}}, 4: {'outputs': {0: {'text': "*

 * *            "['New price alert was configured with ID: 883953\\n']}}}, 6: {'outputs': {0: {'data': "*

 * *            '{\'text/plain\': {insert: [(2, "   \'AlertDefinitionId\': \'883953\',\\n"), (6, "   '*

 * *            '\'ExpiryDate\': \'2023- […]*

```diff
@@ -17,15 +17,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\ud83c\udf10 opening login page in browser - waiting for user to authenticate... \ud83d\udd11\n",
                         "\ud83d\udcde received callback from Saxo SSO\n",
-                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID 2c560ab41d0d4227b2becc7057cfe16c)\n"
+                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID: 2757e3a96e9c4687a498ae9bc86c2c86)\n"
                     ]
                 }
             ],
             "source": [
                 "from saxo_apy import SaxoOpenAPIClient\n",
                 "\n",
                 "client = SaxoOpenAPIClient()\n",
@@ -64,15 +64,15 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "New price alert was configured with ID: 878349\n"
+                        "New price alert was configured with ID: 883953\n"
                     ]
                 }
             ],
             "source": [
                 "# create new price alert: AAPL traded above 200 USD on default account, active for the next 10 days\n",
                 "from datetime import datetime, timedelta\n",
                 "\n",
@@ -110,19 +110,19 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'__count': 1,\n",
                             " 'Data': [{'AccountId': '16371609_USD',\n",
-                            "   'AlertDefinitionId': '878349',\n",
+                            "   'AlertDefinitionId': '883953',\n",
                             "   'AssetType': 'Stock',\n",
                             "   'ClientId': '16371609',\n",
                             "   'Comment': '',\n",
-                            "   'ExpiryDate': '2023-01-20T10:58:43.743000Z',\n",
+                            "   'ExpiryDate': '2023-06-28T09:52:48.090000Z',\n",
                             "   'IsExtendedHours': False,\n",
                             "   'IsRecurring': False,\n",
                             "   'Operator': 'GreaterOrEqual',\n",
                             "   'PriceVariable': 'Traded',\n",
                             "   'State': 'Enabled',\n",
                             "   'TargetValue': 200.0,\n",
                             "   'Uic': 211,\n",
@@ -176,15 +176,15 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Target value of price alert 878349 is now: 210.0\n"
+                        "Target value of price alert 883953 is now: 210.0\n"
                     ]
                 }
             ],
             "source": [
                 "# retrieve updated alert, price is indeed updated to 210\n",
                 "alert = client.get(f\"/vas/v1/pricealerts/definitions/{alert_id}\")\n",
                 "print(f\"Target value of price alert {alert_id} is now: {alert['TargetValue']}\")"
@@ -242,15 +242,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.1 (main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-1400.0.29.202)]"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "3f753197f020b6236bb06be37c192ff4bc0da2ccc1bf66f005a7556bcabdf016"
             }
         }
```

### Comparing `saxo_apy-0.2.5/samples/06_instrument_search.ipynb` & `saxo_apy-0.2.7/samples/06_instrument_search.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958403087797619%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': {insert: [(2, '✅ authorization succeeded - connected to "*

 * *            'SIM environment with WRITE / TRADE permissions (session ID: '*

 * *            "73e1f2013caf4d5c87442dc9241751a0)\\n')], delete: [2]}}}}, 3: {'outputs': {0: {'text': "*

 * *            "['Found 246 exchanges\\n']}}}, 4: {'outputs': {0: {'text': ['Found 118 "*

 * *            'instruments\\n\']}, 1: {\'data\': {\'text/plain\': {insert: [(2, " (\'Shell PLC\', '*

 * *            '\'SHELL:xams\', 27113371),\\n"), (4, "  […]*

```diff
@@ -14,15 +14,15 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\ud83c\udf10 opening login page in browser - waiting for user to authenticate... \ud83d\udd11\n",
                         "\ud83d\udcde received callback from Saxo SSO\n",
-                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID ea294e105e874ddfbbb6c95e1fd0e342)\n"
+                        "\u2705 authorization succeeded - connected to SIM environment with WRITE / TRADE permissions (session ID: 73e1f2013caf4d5c87442dc9241751a0)\n"
                     ]
                 }
             ],
             "source": [
                 "from saxo_apy import SaxoOpenAPIClient\n",
                 "\n",
                 "client = SaxoOpenAPIClient()\n",
@@ -81,15 +81,15 @@
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Found 243 exchanges\n"
+                        "Found 246 exchanges\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "[('New York Stock Exchange (ARCA)', 'NYSE_ARCA'),\n",
                             " ('Pacific Stock Exchange ( NYSE Arca )', 'PSE'),\n",
@@ -118,30 +118,30 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Found 123 instruments\n"
+                        "Found 118 instruments\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "[('ASML Holding NV', 'ASML:xams', 1636),\n",
-                            " ('Shell PLC', 'SHELL:xams', 27113371),\n",
                             " ('ING Groep ', 'ING:xams', 3066),\n",
+                            " ('Shell PLC', 'SHELL:xams', 27113371),\n",
                             " ('Just Eat Takeaway', 'TKWY:xams', 6900023),\n",
-                            " ('Philips (Royal)', 'PHIA:xams', 111721),\n",
-                            " ('ASM International', 'ASMI:xams', 13269),\n",
-                            " ('Prosus', 'PRX:xams', 14838059),\n",
+                            " ('Pharming Group', 'PHARM:xams', 23113),\n",
+                            " ('Aegon', 'AGN:xams', 111717),\n",
                             " ('BE Semiconductor Industries', 'BESI:xams', 43318),\n",
-                            " ('Adyen', 'ADYEN:xams', 9894784),\n",
-                            " ('Pharming Group', 'PHARM:xams', 23113)]"
+                            " ('ASM International', 'ASMI:xams', 13269),\n",
+                            " ('ABN AMRO Bank', 'ABN:xams', 2906958),\n",
+                            " ('NN Group', 'NN:xams', 984685)]"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -159,28 +159,28 @@
                 "\n",
                 "# show first 10 results:\n",
                 "[(result[\"Description\"], result[\"Symbol\"], result[\"Identifier\"]) for result in results][:10]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "['IBEX 35 Index',\n",
-                            " 'FTSE 250 Index',\n",
-                            " 'S&P 100 Index',\n",
-                            " 'Bats France 40 Price Return Index',\n",
-                            " 'Poland 20 Index']"
+                            "['S&P ASX 300 Index',\n",
+                            " 'CHINEXT Price Index',\n",
+                            " 'Morningstar US Large Cap Index',\n",
+                            " 'Morningstar US Small Cap Index',\n",
+                            " 'Morningstar Australia Index']"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# search for non-tradable instruments such as indices\n",
                 "\n",
@@ -209,15 +209,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.1 (main, Dec 23 2022, 09:28:24) [Clang 14.0.0 (clang-1400.0.29.202)]"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "3f753197f020b6236bb06be37c192ff4bc0da2ccc1bf66f005a7556bcabdf016"
             }
         }
```

### Comparing `saxo_apy-0.2.5/samples/07_pricing_and_orders.ipynb` & `saxo_apy-0.2.7/samples/07_pricing_and_orders.ipynb`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/samples/README.md` & `saxo_apy-0.2.7/samples/README.md`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/samples/s01_async_requests.py` & `saxo_apy-0.2.7/samples/s01_async_requests.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/samples/s02_streaming_prices.py` & `saxo_apy-0.2.7/samples/s02_streaming_prices.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/saxo_apy/client.py` & `saxo_apy-0.2.7/saxo_apy/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,18 @@
     TokenData,
     TokenExpiredError,
 )
 from .redirect_server import RedirectServer
 from .utils import (
     configure_logger,
     construct_auth_url,
-    handle_api_response,
+    log_request,
+    log_response,
     make_default_session_headers,
+    raise_api_error,
     unix_seconds_to_datetime,
     validate_redirect_url,
 )
 from .version import VERSION, version_info
 
 REQUEST_TIMEOUT = Timeout(timeout=60.0)
 ID_NUM_BYTES = 10
@@ -90,14 +92,15 @@
         logger.success(f"successfully parsed app config: {self._app_config}")
 
         # set instance members
         self._http_client: Client = Client(
             headers=make_default_session_headers(),
             base_url=self._app_config.api_base_url,
             timeout=REQUEST_TIMEOUT,
+            event_hooks={"request": [log_request], "response": [log_response, raise_api_error]},
         )
         self._token_data: Optional[TokenData] = None
         self.streaming_context_id: Optional[str] = None
         self.streaming_connection: Any = None
 
         try:
             self.async_loop = asyncio.get_running_loop()
@@ -131,26 +134,26 @@
             f"{start_async_refresh=} {redirect_port=}"
         )
         _redirect_url = validate_redirect_url(self._app_config, redirect_url)
         state = token_urlsafe(20)
         auth_url = construct_auth_url(self._app_config, _redirect_url, state)
         logger.debug(f"logging in with {str(_redirect_url)=} and {str(auth_url)=}")
 
-        if catch_redirect:
-            redirect_server = RedirectServer(_redirect_url, state=state, port=redirect_port)
-            redirect_server.start()
-
         if launch_browser:
             logger.debug("launching browser with login page")
             print("🌐 opening login page in browser - waiting for user to " "authenticate... 🔑")
             webbrowser.open_new(auth_url)
         else:
             print(f"🌐 navigate to the following web page to log in: {auth_url}")
 
+        _auth_code = None  # auth code returned by Saxo SSO
+
         if catch_redirect:
+            redirect_server = RedirectServer(_redirect_url, state=state, port=redirect_port)
+            redirect_server.start()
             try:
                 while not redirect_server.auth_code:
                     sleep(0.1)
                 print("📞 received callback from Saxo SSO")
                 _auth_code = parse_obj_as(AuthorizationCode, redirect_server.auth_code)
             except KeyboardInterrupt:
                 logger.warning("keyboard interrupt received - shutting down")
@@ -313,40 +316,46 @@
         self.streaming_context_id = token_urlsafe(ID_NUM_BYTES)
         url = f"{self._app_config.streaming_url}/connect?contextId={self.streaming_context_id}"
         headers = {"Authorization": f"Bearer {self._token_data.access_token}"}
         self.streaming_connection = ws_client.connect(url, extra_headers=headers)
 
     def get(self, path: str, params: Optional[Dict] = None) -> Dict:
         """Send GET request to OpenAPI and handle response."""
-        response = handle_api_response(self.openapi_request("GET", path, params))
+        response = self.openapi_request("GET", path, params)
         return response.json()
 
-    def post(self, path: str, data: Dict, params: Optional[Dict] = None) -> Dict:
+    def post(self, path: str, data: Dict, params: Optional[Dict] = None) -> Optional[Dict]:
         """Send POST request to OpenAPI and handle response."""
-        response = handle_api_response(self.openapi_request("POST", path, params, data))
-        return response.json()
+        response = self.openapi_request("POST", path, params, data)
+        if (
+            response.headers.get("content-type")
+            and "application/json" in response.headers.get("content-type").lower()  # response includes error body
+        ):
+            return response.json()
+        else:
+            return None
 
     def put(self, path: str, data: Optional[Dict], params: Optional[Dict] = None) -> None:
         """Send PUT request to OpenAPI and handle response."""
         # always returns 202 Accepted or 204 No Content
-        _ = handle_api_response(self.openapi_request("PUT", path, params, data))
+        _ = self.openapi_request("PUT", path, params, data)
 
     def patch(self, path: str, data: Dict, params: Optional[Dict] = None) -> Optional[Dict]:
         """Send PATCH request to OpenAPI and handle response."""
-        response = handle_api_response(self.openapi_request("PATCH", path, params, data))
+        response = self.openapi_request("PATCH", path, params, data)
         # may or may not return content based on endpoint
         if response.headers.get("Content-Length") and int(response.headers["Content-Length"]) > 0:
             return response.json()
         else:
             return None
 
     def delete(self, path: str, params: Optional[Dict] = None) -> None:
         """Send DELETE request to OpenAPI and handle response."""
         # always returns 204 No Content
-        _ = handle_api_response(self.openapi_request("DELETE", path, params))
+        _ = self.openapi_request("DELETE", path, params)
 
     async def aget(self, path: str, params: Optional[Dict] = None):  # type: ignore
         """Send GET request to OpenAPI asynchronously."""
         return await self.async_loop.run_in_executor(None, self.get, path, params)
 
     async def apost(self, path: str, data: Dict, params: Optional[Dict] = None):  # type: ignore
         """Send POST request to OpenAPI asynchronously."""
@@ -370,43 +379,37 @@
         path: str,
         params: Optional[Dict] = None,
         data: Optional[Dict] = None,
     ) -> Response:
         """Send a request to OpenAPI and provide direct access to the response object."""
         assert self.logged_in
 
-        if not path.startswith("/"):
-            logger.debug("prepended '/' to request path as it is not provided")
-            _path = "/" + path
-        else:
-            _path = path
-
         request_id = token_urlsafe(ID_NUM_BYTES)
 
         assert self._app_config.env  # assert for mypy
         assert self._token_data
         assert self._token_data.access_token
 
         headers = {
             "x-request-id": f"saxo-apy/{VERSION}/{self.client_session_id}/{request_id}",
             "x-openapi-env": self._app_config.env.value,
             "x-client-timestamp": datetime.utcnow().isoformat(),
             "authorization": f"Bearer {self._token_data.access_token}",
         }
 
-        logger.debug(f"performing request with id: {request_id} - {method} {_path}, {params=}, {data=}")
-
-        response = self._http_client.request(
+        request = self._http_client.build_request(
             method,
             path,
             params=params,
             json=data,
             headers=headers,
         )
 
+        response = self._http_client.send(request)
+
         return response
 
     @property
     def available_redirect_urls(self) -> List[AnyHttpUrl]:
         """Retrieve available redirect URLs for login from app config."""
         return self._app_config.redirect_urls
```

### Comparing `saxo_apy-0.2.5/saxo_apy/models.py` & `saxo_apy-0.2.7/saxo_apy/models.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/saxo_apy/redirect_server.py` & `saxo_apy-0.2.7/saxo_apy/redirect_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from loguru import logger
 from pydantic import AnyHttpUrl, parse_obj_as
 from werkzeug.serving import make_server
 
 response_html = """
 <head>
 <title>
-SAXO-APY Redirect Server
+SAXO-APY Client
 </title>
 <style>
 body {background-color: black;}
 h2 {color: white;}
 </style>
 </head>
 <body>
```

### Comparing `saxo_apy-0.2.5/saxo_apy/utils.py` & `saxo_apy-0.2.7/saxo_apy/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,26 @@
 """Utils used by SaxoOpenAPIClient."""
 
 import json
 from datetime import datetime, timezone
 from http import HTTPStatus
-from pprint import pformat
-from typing import Dict, Optional
+from typing import Callable, Dict, Optional, Union
 from urllib.parse import urlencode
 
-from httpx import Response
+from httpx import Request, Response
 from loguru import logger
 from pydantic import AnyHttpUrl, parse_obj_as
 
 from .models import APIResponseError, HttpsUrl, OpenAPIAppConfig, StreamingMessage
 from .version import VERSION
 
-KNOWN_ERRORS = {
-    HTTPStatus.BAD_REQUEST: "invalid request sent",
-    HTTPStatus.UNAUTHORIZED: "access token missing, incorrect, or expired",
-    HTTPStatus.FORBIDDEN: (
-        "you are not authorized to access this resource - check if you are logged in with write permissions and/or "
-        "market data has been enabled"
-    ),
-    HTTPStatus.NOT_FOUND: (
-        "requested resource or entity the request operates on could not be found "
-        "(or you don't have the required permissions for the requested entity)"
-    ),
-    HTTPStatus.METHOD_NOT_ALLOWED: "the requested method is not valid for this endpoint",
-    HTTPStatus.INTERNAL_SERVER_ERROR: (
-        "server error occurred, please ensure your request is valid and notify Saxo support if this error persists"
-    ),
-}
 
-
-def configure_logger(log_sink: str, log_level: str) -> None:
+def configure_logger(log_sink: Union[str, Callable], log_level: str) -> int:
     """Set defaults for log config."""
-    logger.add(
+    return logger.add(
         log_sink,
         format=(
             "{time:YYYY-MM-DD HH:mm:ss.SSS!UTC}Z {thread:12} {level:8} {module:16} {line:5} {function:25} {message}"
         ),
         level=log_level,
         enqueue=True,
     )
@@ -52,14 +34,74 @@
         "user-agent": f"saxo-apy/{VERSION}",
         "connection": "keep-alive",
         "cache-control": "no-cache",
     }
     return headers
 
 
+def log_request(request: Request) -> None:
+    """Log request details to INFO logs."""
+    request_id = request.headers.get("x-request-id").split("/")[3]
+    logger.info(f"{request_id:20} performing request: {request.method} {request.url}")
+    logger.debug(f"{request_id:20} request headers:    {request.headers}")
+    logger.debug(f"{request_id:20} request body:       {request.content.decode()}")
+
+
+def log_response(response: Response) -> None:
+    """Log response details to SUCCESS/ERROR logs."""
+    request_id = response.request.headers.get("x-request-id").split("/")[3]
+    status_code = HTTPStatus(response.status_code)
+    status_phrase = status_code.name.replace("_", " ")
+    server_trace_id = response.headers.get("x-correlation")
+    if response.is_success:
+        logger.success(
+            f"{request_id:20} request succeeded with status: {status_code} {status_phrase} - server trace id: "
+            f"{server_trace_id}"
+        )
+    elif response.is_error:
+        logger.error(
+            f"{request_id:20} request failed with status: {status_code} {status_phrase} - server trace id: "
+            f"{server_trace_id}"
+        )
+
+
+def raise_api_error(response: Response) -> None:
+    """Log response error to log and raise formatted exception."""
+    if response.is_error:
+        response.read()  # read error for possible error message
+
+        if (  # error content exist and is of type JSON
+            response.content
+            and response.headers.get("content-type")
+            and "application/json" in response.headers.get("content-type").lower()
+        ):
+            error_received = response.json()
+        else:
+            error_received = "No additional error details received from OpenAPI..."
+
+        # parse details from response
+        request_id = response.request.headers.get("x-request-id").split("/")[3]
+        env = response.request.headers.get("x-openapi-env")
+        client_ts = response.request.headers.get("x-client-timestamp")
+        status_code = HTTPStatus(response.status_code)
+        status_phrase = status_code.name.replace("_", " ")
+        server_trace_id = response.headers.get("x-correlation")
+
+        # construct human-friendly exception
+        exc = APIResponseError(
+            f"status: {status_code} - {status_phrase}\n"
+            f"client request id: {request_id}\n"
+            f"server trace id: {server_trace_id}\n"
+            f"timestamp (UTC): {client_ts} - elapsed: {response.elapsed} - env: {env}\n"
+            f"message: {error_received}"
+        )
+        logger.error(f"{request_id:20} error response received from API:\n{exc}")
+        raise exc
+
+
 def unix_seconds_to_datetime(timestamp: int) -> datetime:
     """Convert unix seconds to human-readable timestamp."""
     return datetime.fromtimestamp(timestamp, tz=timezone.utc)
 
 
 def validate_redirect_url(app_config: OpenAPIAppConfig, redirect_url: Optional[AnyHttpUrl]) -> AnyHttpUrl:
     """Check if provided redirect URL for login is valid - or default to config."""
@@ -85,61 +127,14 @@
 
     return parse_obj_as(
         HttpsUrl,
         app_config.auth_endpoint + "?" + urlencode(auth_request_query_params),
     )
 
 
-def handle_api_response(response: Response) -> Response:
-    """Handle response from OpenAPI."""
-    # parse response details
-    status_code = HTTPStatus(response.status_code)
-    status_phrase = status_code.name.replace("_", " ")
-    elapsed = response.elapsed
-
-    # headers set when request is sent
-    request_id = response.request.headers.get("x-request-id")
-    env = response.request.headers.get("x-openapi-env")
-    client_ts = response.request.headers.get("x-client-timestamp")
-
-    # header returned by OpenAPI
-    x_correlation = response.headers.get("x-correlation")
-    has_json_content = (
-        response.headers.get("content-type") and "application/json" in response.headers.get("content-type").lower()
-    )
-
-    # determine if response is known error to customize error message
-    error_msg = None
-    known_error = KNOWN_ERRORS.get(status_code)
-    if known_error:
-        error_msg = known_error
-    elif not response.is_success:
-        error_msg = "unknown error occurred - investigate response details for more information"
-
-    if error_msg:  # something has gone wrong
-        if has_json_content:
-            error_msg += f" - response content:\n{pformat(response.json(), width=120, indent=2)}"
-
-        exc = APIResponseError(
-            f"status: {status_code} - {status_phrase}\n"
-            f"error: {error_msg}\n"
-            f"client request id: {request_id}\n"
-            f"server trace id: {x_correlation}\n"
-            f"timestamp (UTC): {client_ts} - elapsed: {elapsed} - env: {env}"
-        )
-        logger.error(f"error response received from API:\n{exc}")
-        raise exc
-
-    logger.success(
-        f"success response received with status: {status_code} - {status_phrase}, time taken: {elapsed}, "
-        f"client request id: {request_id}, server trace id: {x_correlation}"
-    )
-    return response
-
-
 def decode_streaming_message(message: bytes) -> StreamingMessage:
     """Decode streaming message byte and convert to dict."""
     message_id = int.from_bytes(message[0:8], byteorder="little")
     ref_id_len = int(message[10])
     ref_id = message[11 : 11 + ref_id_len].decode()
     format = int(message[11 + ref_id_len])
     if format != 0:
```

### Comparing `saxo_apy-0.2.5/tests/test_client.py` & `saxo_apy-0.2.7/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/tests/test_utils.py` & `saxo_apy-0.2.7/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 )
 from saxo_apy.version import VERSION
 
 from .fixtures.models import DUMMY_LIVE_CONFIG, DUMMY_SIM_CONFIG
 
 
 def test_logger_setup() -> None:
-    configure_logger(log_sink="log.txt", log_level="DEBUG")
+    _ = []
+    handler_id = configure_logger(log_sink=_.append, log_level="DEBUG")
     logger_config = str(logger)
     assert "id=1" in logger_config
     assert "level=10" in logger_config
-    assert "sink='log.txt" in logger_config
+    assert "sink=append" in logger_config
+    logger.remove(handler_id)
 
 
 def test_make_default_session_headers() -> None:
     headers = make_default_session_headers()
 
     expected_headers = {
         "accept-encoding": "gzip",
```

### Comparing `saxo_apy-0.2.5/tests/fixtures/dummy_app_config_live.json` & `saxo_apy-0.2.7/tests/fixtures/dummy_app_config_live.json`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/tests/fixtures/dummy_app_config_sim.json` & `saxo_apy-0.2.7/tests/fixtures/dummy_app_config_sim.json`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/tests/fixtures/models.py` & `saxo_apy-0.2.7/tests/fixtures/models.py`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/LICENSE` & `saxo_apy-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/README.md` & `saxo_apy-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,295 +1,320 @@
-00000000: 6060 600a 2020 205f 5f5f 5f5f 2020 2020  ```.   _____    
-00000010: 2020 2020 205f 5f20 2020 5f5f 2020 5f5f       __   __  __
-00000020: 5f5f 2020 2020 2020 2020 2020 2020 2020  __              
-00000030: 2020 2020 205f 5f5f 5f5f 2020 5f5f 2020       _____  __  
-00000040: 2020 205f 5f0a 2020 2f20 5f5f 5f5f 7c20     __.  / ____| 
-00000050: 2020 2f5c 2020 205c 205c 202f 202f 202f    /\   \ \ / / /
-00000060: 205f 5f20 5c20 2020 2020 2020 2020 2020   __ \           
-00000070: 202f 5c20 2020 7c20 205f 5f20 5c20 5c20   /\   |  __ \ \ 
-00000080: 5c20 2020 2f20 2f0a 207c 2028 5f5f 5f20  \   / /. | (___ 
-00000090: 2020 202f 2020 5c20 2020 5c20 5620 2f20     /  \   \ V / 
-000000a0: 7c20 7c20 207c 207c 2020 5f5f 5f5f 2020  | |  | |  ____  
-000000b0: 2020 2f20 205c 2020 7c20 7c5f 5f29 207c    /  \  | |__) |
-000000c0: 205c 205c 5f2f 202f 200a 2020 5c5f 5f5f   \ \_/ / .  \___
-000000d0: 205c 2020 2f20 2f5c 205c 2020 2029 2028   \  / /\ \   ) (
-000000e0: 2020 7c20 7c20 207c 207c 207c 5f5f 5f5f    | |  | | |____
-000000f0: 7c20 202f 202f 5c20 5c20 7c20 205f 5f5f  |  / /\ \ |  ___
-00000100: 2f20 2020 5c20 2020 2f20 200a 2020 5f5f  /   \   /  .  __
-00000110: 5f5f 2920 7c2f 205f 5f5f 5f20 5c20 2f20  __) |/ ____ \ / 
-00000120: 5f20 5c20 7c20 7c5f 5f7c 207c 2020 2020  _ \ | |__| |    
-00000130: 2020 2020 2f20 5f5f 5f5f 205c 7c20 7c20      / ____ \| | 
-00000140: 2020 2020 2020 207c 207c 2020 200a 207c         | |   . |
-00000150: 5f5f 5f5f 5f2f 2f5f 2f20 2020 205c 2f2f  _____//_/    \//
-00000160: 5f2f 205c 5f5c 205c 5f5f 5f5f 2f20 2020  _/ \_\ \____/   
-00000170: 2020 2020 202f 5f2f 2020 2020 5c2f 7c5f       /_/    \/|_
-00000180: 7c20 2020 2020 2020 207c 5f7c 2020 0a20  |        |_|  . 
-00000190: 6060 600a 0a5b 215b 7079 7468 6f6e 5d28  ```..[![python](
-000001a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000001b0: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
-000001c0: 686f 6e2d 332e 3725 3242 2d62 6c75 6529  hon-3.7%2B-blue)
-000001d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000001e0: 2e63 6f6d 2f67 6964 7665 6e2f 7361 786f  .com/gidven/saxo
-000001f0: 2d6f 7065 6e61 7069 2d63 6c69 656e 742d  -openapi-client-
-00000200: 7079 7468 6f6e 290a 5b21 5b70 7970 695d  python).[![pypi]
-00000210: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000220: 656c 6473 2e69 6f2f 7079 7069 2f76 2f73  elds.io/pypi/v/s
-00000230: 6178 6f2d 6170 793f 7374 796c 653d 666c  axo-apy?style=fl
-00000240: 6174 2d73 7175 6172 6529 5d28 6874 7470  at-square)](http
-00000250: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000260: 6a65 6374 2f73 6178 6f2d 6170 7929 0a5b  ject/saxo-apy).[
-00000270: 215b 6c69 6365 6e73 655d 2868 7474 7073  ![license](https
-00000280: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000290: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-000002a0: 2f67 6964 7665 6e2f 7361 786f 2d6f 7065  /gidven/saxo-ope
-000002b0: 6e61 7069 2d63 6c69 656e 742d 7079 7468  napi-client-pyth
-000002c0: 6f6e 3f73 7479 6c65 3d66 6c61 742d 7371  on?style=flat-sq
-000002d0: 7561 7265 295d 2868 7474 7073 3a2f 2f67  uare)](https://g
-000002e0: 6974 6875 622e 636f 6d2f 6769 6476 656e  ithub.com/gidven
-000002f0: 2f73 6178 6f2d 6f70 656e 6170 692d 636c  /saxo-openapi-cl
-00000300: 6965 6e74 2d70 7974 686f 6e2f 626c 6f62  ient-python/blob
-00000310: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a0a  /main/LICENSE)..
-00000320: 2320 5361 786f 2d41 5059 3a20 5079 7468  # Saxo-APY: Pyth
-00000330: 6f6e 2043 6c69 656e 7420 666f 7220 5361  on Client for Sa
-00000340: 786f 2042 616e 6b20 4f70 656e 4150 490a  xo Bank OpenAPI.
-00000350: 0a2a 4120 6c69 6768 7477 6569 6768 7420  .*A lightweight 
-00000360: 5079 7468 6f6e 2063 6c69 656e 7420 666f  Python client fo
-00000370: 7220 6861 7373 6c65 2d66 7265 6520 7469  r hassle-free ti
-00000380: 6e6b 6572 696e 6720 7769 7468 2053 6178  nkering with Sax
-00000390: 6f20 4f70 656e 4150 492e 2a0a 0a3e 204e  o OpenAPI.*..> N
-000003a0: 4f54 453a 2054 6869 7320 5079 7468 6f6e  OTE: This Python
-000003b0: 2070 6163 6b61 6765 2077 6173 2063 7265   package was cre
-000003c0: 6174 6564 2062 7920 616e 2065 6e74 6875  ated by an enthu
-000003d0: 7369 6173 7420 6173 2061 206c 6561 726e  siast as a learn
-000003e0: 696e 6720 7072 6f6a 6563 742e 204e 6f6e  ing project. Non
-000003f0: 6520 6f66 2074 6865 2063 6f6e 7465 6e74  e of the content
-00000400: 7320 696e 2074 6869 7320 7265 706f 7369  s in this reposi
-00000410: 746f 7279 2061 7265 206d 6169 6e74 6169  tory are maintai
-00000420: 6e65 6420 6279 2053 6178 6f20 4261 6e6b  ned by Saxo Bank
-00000430: 2c20 616e 6420 5361 786f 2042 616e 6b20  , and Saxo Bank 
-00000440: 646f 6573 206e 6f74 2067 7561 7261 6e74  does not guarant
-00000450: 6565 2063 6f72 7265 6374 6e65 7373 206f  ee correctness o
-00000460: 6620 7468 6520 7072 6f76 6964 6564 2069  f the provided i
-00000470: 6d70 6c65 6d65 6e74 6174 696f 6e2e 0a0a  mplementation...
-00000480: 2323 2041 7420 4669 7273 7420 476c 616e  ## At First Glan
-00000490: 6365 0a0a 466f 7220 6d6f 7265 2069 6e73  ce..For more ins
-000004a0: 7069 7261 7469 6f6e 2073 6565 205b 7468  piration see [th
-000004b0: 6520 7361 6d70 6c65 735d 282e 2f73 616d  e samples](./sam
-000004c0: 706c 6573 2f29 210a 0a60 6060 7079 7468  ples/)!..```pyth
-000004d0: 6f6e 0a66 726f 6d20 7361 786f 5f61 7079  on.from saxo_apy
-000004e0: 2069 6d70 6f72 7420 5361 786f 4f70 656e   import SaxoOpen
-000004f0: 4150 4943 6c69 656e 740a 0a63 6c69 656e  APIClient..clien
-00000500: 7420 3d20 5361 786f 4f70 656e 4150 4943  t = SaxoOpenAPIC
-00000510: 6c69 656e 7428 2261 7070 5f63 6f6e 6669  lient("app_confi
-00000520: 672e 6a73 6f6e 2229 0a63 6c69 656e 742e  g.json").client.
-00000530: 6c6f 6769 6e28 290a 0a6d 6520 3d20 636c  login()..me = cl
-00000540: 6965 6e74 2e67 6574 2822 706f 7274 2f76  ient.get("port/v
-00000550: 312f 7573 6572 732f 6d65 2229 0a65 7572  1/users/me").eur
-00000560: 7573 645f 7072 6963 6520 3d20 636c 6965  usd_price = clie
-00000570: 6e74 2e67 6574 2822 2f74 7261 6465 2f76  nt.get("/trade/v
-00000580: 312f 696e 666f 7072 6963 6573 3f55 6963  1/infoprices?Uic
-00000590: 3d32 3126 4173 7365 7454 7970 653d 4678  =21&AssetType=Fx
-000005a0: 5370 6f74 2229 0a70 6f72 7466 6f6c 696f  Spot").portfolio
-000005b0: 5f6f 7264 6572 7320 3d20 636c 6965 6e74  _orders = client
-000005c0: 2e67 6574 2822 2f70 6f72 742f 7631 2f6f  .get("/port/v1/o
-000005d0: 7264 6572 732f 6d65 2229 0a0a 7072 696e  rders/me")..prin
-000005e0: 7428 6622 5765 6c63 6f6d 6520 7b6d 655b  t(f"Welcome {me[
-000005f0: 2755 7365 7249 6427 5d7d 2122 290a 7072  'UserId']}!").pr
-00000600: 696e 7428 6622 4555 5255 5344 2069 7320  int(f"EURUSD is 
-00000610: 7472 6164 696e 6720 6174 3a20 7b65 7572  trading at: {eur
-00000620: 7573 645f 7072 6963 655b 2751 756f 7465  usd_price['Quote
-00000630: 275d 5b27 4269 6427 5d7d 202f 207b 6575  ']['Bid']} / {eu
-00000640: 7275 7364 5f70 7269 6365 5b27 5175 6f74  rusd_price['Quot
-00000650: 6527 5d5b 2741 736b 275d 7d20 2842 6964  e']['Ask']} (Bid
-00000660: 2f41 736b 2922 290a 7072 696e 7428 6622  /Ask)").print(f"
-00000670: 596f 7520 6861 7665 3a20 7b70 6f72 7466  You have: {portf
-00000680: 6f6c 696f 5f6f 7264 6572 735b 275f 5f63  olio_orders['__c
-00000690: 6f75 6e74 275d 7d20 6f72 6465 7273 2069  ount']} orders i
-000006a0: 6e20 796f 7572 2070 6f72 7466 6f6c 696f  n your portfolio
-000006b0: 2229 0a60 6060 0a0a 2020 2020 f09f 8c90  ").```..    ....
-000006c0: 206f 7065 6e69 6e67 206c 6f67 696e 2070   opening login p
-000006d0: 6167 6520 696e 2062 726f 7773 6572 202d  age in browser -
-000006e0: 2077 6169 7469 6e67 2066 6f72 2075 7365   waiting for use
-000006f0: 7220 746f 2061 7574 6865 6e74 6963 6174  r to authenticat
-00000700: 652e 2e2e 20f0 9f94 910a 2020 2020 f09f  e... .....    ..
-00000710: 939e 2072 6563 6569 7665 6420 6361 6c6c  .. received call
-00000720: 6261 636b 2066 726f 6d20 5361 786f 2053  back from Saxo S
-00000730: 534f 0a20 2020 20e2 9c85 2061 7574 686f  SO.    ... autho
-00000740: 7269 7a61 7469 6f6e 2073 7563 6365 6564  rization succeed
-00000750: 6564 202d 2063 6f6e 6e65 6374 6564 2074  ed - connected t
-00000760: 6f20 5349 4d20 656e 7669 726f 6e6d 656e  o SIM environmen
-00000770: 7420 7769 7468 2057 5249 5445 202f 2054  t with WRITE / T
-00000780: 5241 4445 2070 6572 6d69 7373 696f 6e73  RADE permissions
-00000790: 2028 7365 7373 696f 6e20 4944 2063 6562   (session ID ceb
-000007a0: 3262 6539 3039 3566 3634 6561 6639 6535  2be9095f64eaf9e5
-000007b0: 6361 6562 3231 6436 6663 3739 3929 0a20  caeb21d6fc799). 
-000007c0: 2020 200a 2020 2020 5765 6c63 6f6d 6520     .    Welcome 
-000007d0: 3136 3337 3136 3039 210a 2020 2020 4555  16371609!.    EU
-000007e0: 5255 5344 2069 7320 7472 6164 696e 6720  RUSD is trading 
-000007f0: 6174 3a20 312e 3038 3232 3920 2f20 312e  at: 1.08229 / 1.
-00000800: 3038 3234 3920 2842 6964 2f41 736b 290a  08249 (Bid/Ask).
-00000810: 2020 2020 596f 7520 6861 7665 3a20 3135      You have: 15
-00000820: 206f 7264 6572 7320 696e 2079 6f75 7220   orders in your 
-00000830: 706f 7274 666f 6c69 6f0a 2020 2020 0a0a  portfolio.    ..
-00000840: 0a23 2320 4665 6174 7572 6573 0a0a 2d20  .## Features..- 
-00000850: 5b78 5d20 4175 7468 656e 7469 6361 7469  [x] Authenticati
-00000860: 6f6e 2061 6e64 2073 6573 7369 6f6e 206d  on and session m
-00000870: 616e 6167 656d 656e 7420 7769 7468 2053  anagement with S
-00000880: 6178 6f20 5353 4f0a 2020 2020 2d20 5375  axo SSO.    - Su
-00000890: 7070 6f72 7473 204f 4175 7468 2032 2e30  pports OAuth 2.0
-000008a0: 2060 436f 6465 6020 6772 616e 7420 7479   `Code` grant ty
-000008b0: 7065 0a20 2020 202d 2057 6f72 6b73 2073  pe.    - Works s
-000008c0: 6561 6d6c 6573 736c 7920 696e 2062 6f74  eamlessly in bot
-000008d0: 6820 6053 494d 6020 616e 6420 604c 4956  h `SIM` and `LIV
-000008e0: 4560 2065 6e76 6972 6f6e 6d65 6e74 730a  E` environments.
-000008f0: 2020 2020 2d20 4175 746f 6d61 7465 6420      - Automated 
-00000900: 6861 6e64 6c69 6e67 206f 6620 6361 6c6c  handling of call
-00000910: 6261 636b 2066 726f 6d20 5353 4f20 286f  back from SSO (o
-00000920: 7074 696f 6e61 6c29 0a20 2020 202d 2048  ptional).    - H
-00000930: 6561 646c 6573 7320 6175 7468 656e 7469  eadless authenti
-00000940: 6361 7469 6f6e 2066 6f72 2064 6570 6c6f  cation for deplo
-00000950: 7965 6420 6170 706c 6963 6174 696f 6e73  yed applications
-00000960: 2028 6f70 7469 6f6e 616c 290a 2020 2020   (optional).    
-00000970: 2d20 4b65 6570 2073 6573 7369 6f6e 7320  - Keep sessions 
-00000980: 616e 6420 6163 7469 7665 2077 6562 736f  and active webso
-00000990: 636b 6574 7320 636f 6e6e 6563 7469 6f6e  ckets connection
-000009a0: 7320 616c 6976 6520 6279 2072 6566 7265  s alive by refre
-000009b0: 7368 696e 6720 6163 6365 7373 2074 6f6b  shing access tok
-000009c0: 656e 7320 7669 6120 6173 796e 6369 6f0a  ens via asyncio.
-000009d0: 2d20 5b78 5d20 5265 6164 206f 7065 7261  - [x] Read opera
-000009e0: 7469 6f6e 7320 2860 4745 5460 2072 6571  tions (`GET` req
-000009f0: 7565 7374 7329 0a2d 205b 785d 2057 7269  uests).- [x] Wri
-00000a00: 7465 206f 7065 7261 7469 6f6e 7320 2860  te operations (`
-00000a10: 504f 5354 602c 2060 5055 5460 2c20 6050  POST`, `PUT`, `P
-00000a20: 4154 4348 602c 2060 4445 4c45 5445 6020  ATCH`, `DELETE` 
-00000a30: 7265 7175 6573 7473 290a 2d20 5b78 5d20  requests).- [x] 
-00000a40: 5375 7070 6f72 7473 2061 7379 6e63 2072  Supports async r
-00000a50: 6571 7565 7374 732c 2073 7472 6561 6d69  equests, streami
-00000a60: 6e67 2c20 616e 6420 6465 636f 6469 6e67  ng, and decoding
-00000a70: 206f 6620 7374 7265 616d 696e 6720 6d65   of streaming me
-00000a80: 7373 6167 6573 0a2d 205b 785d 2045 7272  ssages.- [x] Err
-00000a90: 6f72 2068 616e 646c 696e 6720 7769 7468  or handling with
-00000aa0: 2063 6f6d 7072 6568 656e 7369 7665 2065   comprehensive e
-00000ab0: 7863 6570 7469 6f6e 206d 6573 7361 6765  xception message
-00000ac0: 730a 0a23 2320 496e 7374 616c 6c61 7469  s..## Installati
-00000ad0: 6f6e 0a0a 5468 6973 2070 7974 686f 6e20  on..This python 
-00000ae0: 7061 636b 6167 6520 6973 2061 7661 696c  package is avail
-00000af0: 6162 6c65 206f 6e20 5079 5049 2e20 496e  able on PyPI. In
-00000b00: 7374 616c 6c20 7468 6520 636c 6965 6e74  stall the client
-00000b10: 2062 7920 7275 6e6e 696e 6720 7468 6520   by running the 
-00000b20: 6265 6c6f 7720 6070 6970 6020 636f 6d6d  below `pip` comm
-00000b30: 616e 6420 696e 2079 6f75 7220 7465 726d  and in your term
-00000b40: 696e 616c 3a0a 0a60 7069 7020 696e 7374  inal:..`pip inst
-00000b50: 616c 6c20 7361 786f 2d61 7079 600a 0a23  all saxo-apy`..#
-00000b60: 2320 5265 7175 6972 656d 656e 7473 0a0a  # Requirements..
-00000b70: 2d20 5079 7468 6f6e 2033 2e37 2b0a 2d20  - Python 3.7+.- 
-00000b80: 416e 204f 7065 6e41 5049 2061 7070 6c69  An OpenAPI appli
-00000b90: 6361 7469 6f6e 2072 6567 6973 7465 7265  cation registere
-00000ba0: 6420 5b6f 6e20 5361 786f 2042 616e 6b27  d [on Saxo Bank'
-00000bb0: 7320 4465 7665 6c6f 7065 7220 506f 7274  s Developer Port
-00000bc0: 616c 5d28 6874 7470 733a 2f2f 7777 772e  al](https://www.
-00000bd0: 6465 7665 6c6f 7065 722e 7361 786f 2f6f  developer.saxo/o
-00000be0: 7065 6e61 7069 2f61 7070 6d61 6e61 6765  penapi/appmanage
-00000bf0: 6d65 6e74 290a 2020 2020 2d20 5b43 7265  ment).    - [Cre
-00000c00: 6174 6520 6120 6672 6565 2064 6576 656c  ate a free devel
-00000c10: 6f70 6572 2061 6363 6f75 6e74 5d28 6874  oper account](ht
-00000c20: 7470 733a 2f2f 7777 772e 6465 7665 6c6f  tps://www.develo
-00000c30: 7065 722e 7361 786f 2f61 6363 6f75 6e74  per.saxo/account
-00000c40: 732f 7369 6d2f 7369 676e 7570 2920 6966  s/sim/signup) if
-00000c50: 2079 6f75 2064 6f6e 2774 2068 6176 6520   you don't have 
-00000c60: 6f6e 6520 616c 7265 6164 792e 0a20 2020  one already..   
-00000c70: 202d 2045 6e73 7572 6520 7468 6520 6170   - Ensure the ap
-00000c80: 706c 6963 6174 696f 6e20 6973 2073 6574  plication is set
-00000c90: 2075 7020 7769 7468 2060 4772 616e 7420   up with `Grant 
-00000ca0: 5479 7065 3a20 436f 6465 6020 6173 2061  Type: Code` as a
-00000cb0: 7574 6865 6e74 6963 6174 696f 6e20 666c  uthentication fl
-00000cc0: 6f77 2e0a 2020 2020 2d20 4174 206c 6561  ow..    - At lea
-00000cd0: 7374 2031 206c 6f63 616c 686f 7374 2072  st 1 localhost r
-00000ce0: 6564 6972 6563 7420 6e65 6564 7320 746f  edirect needs to
-00000cf0: 2062 6520 6465 6669 6e65 6420 7375 6368   be defined such
-00000d00: 2061 7320 6068 7474 703a 2f2f 6c6f 6361   as `http://loca
-00000d10: 6c68 6f73 743a 3132 3332 312f 7265 6469  lhost:12321/redi
-00000d20: 7265 6374 6020 2866 6f72 2064 6576 656c  rect` (for devel
-00000d30: 6f70 6d65 6e74 2f74 6573 7469 6e67 2070  opment/testing p
-00000d40: 7572 706f 7365 7329 0a20 2020 202d 2028  urposes).    - (
-00000d50: 4f70 7469 6f6e 616c 2920 656e 6162 6c65  Optional) enable
-00000d60: 2074 7261 6469 6e67 2070 6572 6d69 7373   trading permiss
-00000d70: 696f 6e73 2066 6f72 2074 6865 2061 7070  ions for the app
-00000d80: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
-00000d90: 2777 7269 7465 2720 746f 2079 6f75 7220  'write' to your 
-00000da0: 6163 636f 756e 7420 2861 6e64 2070 6c61  account (and pla
-00000db0: 6365 206f 7264 6572 7329 0a0a 2323 2044  ce orders)..## D
-00000dc0: 6570 656e 6465 6e63 6965 730a 0a54 6869  ependencies..Thi
-00000dd0: 7320 7061 636b 6167 6520 7265 7175 6972  s package requir
-00000de0: 6573 2035 2064 6570 656e 6465 6e63 6965  es 5 dependencie
-00000df0: 733a 0a0a 2d20 6070 7964 616e 7469 6360  s:..- `pydantic`
-00000e00: 2c20 666f 7220 7061 7273 696e 6720 636f  , for parsing co
-00000e10: 6e66 6967 2061 6e64 204a 534f 4e20 7265  nfig and JSON re
-00000e20: 7370 6f6e 7365 7320 0a2d 2060 466c 6173  sponses .- `Flas
-00000e30: 6b60 2c20 746f 2072 756e 2061 206c 6f63  k`, to run a loc
-00000e40: 616c 2073 6572 7665 7220 616e 6420 6361  al server and ca
-00000e50: 7463 6820 7468 6520 6361 6c6c 6261 636b  tch the callback
-00000e60: 2066 726f 6d20 5361 786f 2053 534f 0a2d   from Saxo SSO.-
-00000e70: 2060 6874 7470 7860 2c20 666f 7220 7365   `httpx`, for se
-00000e80: 6e64 696e 6720 7265 7175 6573 7473 2074  nding requests t
-00000e90: 6f20 4f70 656e 4150 4920 616e 6420 6d61  o OpenAPI and ma
-00000ea0: 6e61 6769 6e67 2074 6865 2063 6c69 656e  naging the clien
-00000eb0: 7420 7365 7373 696f 6e0a 2d20 6077 6562  t session.- `web
-00000ec0: 736f 636b 6574 7360 2c20 666f 7220 7365  sockets`, for se
-00000ed0: 7474 696e 6720 7570 2061 2077 6562 736f  tting up a webso
-00000ee0: 636b 6574 2063 6f6e 6e65 6374 696f 6e20  cket connection 
-00000ef0: 746f 2053 6178 6f27 7320 7374 7265 616d  to Saxo's stream
-00000f00: 696e 6720 7365 7276 6963 650a 2d20 606c  ing service.- `l
-00000f10: 6f67 7572 7560 2c20 746f 2068 616e 646c  oguru`, to handl
-00000f20: 6520 6c6f 6767 696e 670a 0a23 2320 4e6f  e logging..## No
-00000f30: 7465 730a 0a54 6865 2063 6c69 656e 7420  tes..The client 
-00000f40: 7375 7070 6f72 7473 204f 4175 7468 2043  supports OAuth C
-00000f50: 6f64 6520 666c 6f77 2061 6e64 2077 696c  ode flow and wil
-00000f60: 6c20 6175 746f 6d61 7469 6361 6c6c 7920  l automatically 
-00000f70: 7370 696e 2075 7020 6120 7365 7276 6572  spin up a server
-00000f80: 2074 6f20 6c69 7374 656e 2066 6f72 2074   to listen for t
-00000f90: 6865 2072 6564 6972 6563 7420 6672 6f6d  he redirect from
-00000fa0: 2053 6178 6f20 5353 4f2e 2041 7420 6c65   Saxo SSO. At le
-00000fb0: 6173 7420 3120 606c 6f63 616c 686f 7374  ast 1 `localhost
-00000fc0: 6020 7265 6469 7265 6374 206e 6565 6473  ` redirect needs
-00000fd0: 2074 6f20 6265 2064 6566 696e 6564 2069   to be defined i
-00000fe0: 6e20 6170 706c 6963 6174 696f 6e20 636f  n application co
-00000ff0: 6e66 6967 2066 6f72 2074 6869 7320 7075  nfig for this pu
-00001000: 7270 6f73 652e 0a0a 4279 2064 6566 6175  rpose...By defau
-00001010: 6c74 2c20 7468 6520 636c 6965 6e74 2077  lt, the client w
-00001020: 696c 6c20 7573 6520 7468 6520 5f66 6972  ill use the _fir
-00001030: 7374 2061 7661 696c 6162 6c65 206c 6f63  st available loc
-00001040: 616c 686f 7374 2072 6564 6972 6563 745f  alhost redirect_
-00001050: 2074 6f20 7275 6e20 7468 6520 7365 7276   to run the serv
-00001060: 6572 206f 6e20 2874 7970 6963 616c 6c79  er on (typically
-00001070: 206f 6e6c 7920 3120 6578 6973 7473 2069   only 1 exists i
-00001080: 6e20 7468 6520 636f 6e66 6967 292e 0a0a  n the config)...
-00001090: 5468 6520 636c 6965 6e74 2076 616c 6964  The client valid
-000010a0: 6174 6573 2072 6564 6972 6563 7420 7572  ates redirect ur
-000010b0: 6c73 2069 6e20 6170 706c 6963 6174 696f  ls in applicatio
-000010c0: 6e20 636f 6e66 6967 2061 7574 6f6d 6174  n config automat
-000010d0: 6963 616c 6c79 2e20 4f41 7574 6820 322e  ically. OAuth 2.
-000010e0: 3020 636f 6465 2066 6c6f 7720 7265 7175  0 code flow requ
-000010f0: 6972 6573 2061 2066 6978 6564 2070 6f72  ires a fixed por
-00001100: 7420 746f 2062 6520 7370 6563 6966 6965  t to be specifie
-00001110: 6420 6f6e 2074 6865 2072 6564 6972 6563  d on the redirec
-00001120: 7420 7572 6c2e 2049 6e20 6361 7365 2074  t url. In case t
-00001130: 6869 7320 6973 2069 6e63 6f72 7265 6374  his is incorrect
-00001140: 6c79 2063 6f6e 6669 6775 7265 642c 2061  ly configured, a
-00001150: 6e20 6572 726f 7220 6d65 7373 6167 6520  n error message 
-00001160: 7769 6c6c 2067 7569 6465 2079 6f75 2074  will guide you t
-00001170: 6f20 656e 7375 7265 2061 7070 2063 6f6e  o ensure app con
-00001180: 6669 6720 6973 2063 6f72 7265 6374 2077  fig is correct w
-00001190: 6974 6820 4f70 656e 4150 493a 0a0a 6060  ith OpenAPI:..``
-000011a0: 600a 6f6e 6520 6f72 206d 6f72 6520 7265  `.one or more re
-000011b0: 6469 7265 6374 2075 726c 7320 6861 7665  direct urls have
-000011c0: 206e 6f20 706f 7274 2063 6f6e 6669 6775   no port configu
-000011d0: 7265 642c 2077 6869 6368 2069 7320 7265  red, which is re
-000011e0: 7175 6972 6564 2066 6f72 2067 7261 6e74  quired for grant
-000011f0: 2074 7970 6520 2743 6f64 6527 202d 2065   type 'Code' - e
-00001200: 6e73 7572 6520 6120 706f 7274 2069 7320  nsure a port is 
-00001210: 636f 6e66 6967 7572 6564 2069 6e20 7468  configured in th
-00001220: 6520 6170 7020 636f 6e66 6967 206f 626a  e app config obj
-00001230: 6563 7420 666f 7220 6561 6368 2075 726c  ect for each url
-00001240: 2028 6578 616d 706c 653a 2068 7474 703a   (example: http:
-00001250: 2f2f 6c6f 6361 6c68 6f73 743a 3233 3433  //localhost:2343
-00001260: 322f 7265 6469 7265 6374 290a 6060 600a  2/redirect).```.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7361 786f  : 2.1.Name: saxo
+00000020: 2d61 7079 0a56 6572 7369 6f6e 3a20 302e  -apy.Version: 0.
+00000030: 322e 370a 5375 6d6d 6172 793a 2041 206c  2.7.Summary: A l
+00000040: 6967 6874 7765 6967 6874 2050 7974 686f  ightweight Pytho
+00000050: 6e20 636c 6965 6e74 2066 6f72 2068 6173  n client for has
+00000060: 736c 652d 6672 6565 2074 696e 6b65 7269  sle-free tinkeri
+00000070: 6e67 2077 6974 6820 5361 786f 204f 7065  ng with Saxo Ope
+00000080: 6e41 5049 2e0a 4175 7468 6f72 2d65 6d61  nAPI..Author-ema
+00000090: 696c 3a20 4769 6420 3c67 6964 6465 7661  il: Gid <giddeva
+000000a0: 6e64 6572 7665 6e40 676d 6169 6c2e 636f  nderven@gmail.co
+000000b0: 6d3e 0a4c 6963 656e 7365 3a20 4d49 540a  m>.License: MIT.
+000000c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+000000d0: 4345 4e53 450a 5265 7175 6972 6573 2d50  CENSE.Requires-P
+000000e0: 7974 686f 6e3a 203e 3d33 2e37 0a52 6571  ython: >=3.7.Req
+000000f0: 7569 7265 732d 4469 7374 3a20 666c 6173  uires-Dist: flas
+00000100: 6b3e 3d32 2e32 2e35 0a52 6571 7569 7265  k>=2.2.5.Require
+00000110: 732d 4469 7374 3a20 6874 7470 783e 3d30  s-Dist: httpx>=0
+00000120: 2e32 342e 310a 5265 7175 6972 6573 2d44  .24.1.Requires-D
+00000130: 6973 743a 206c 6f67 7572 753e 3d30 2e37  ist: loguru>=0.7
+00000140: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
+00000150: 3a20 7079 6461 6e74 6963 3e3d 312e 3130  : pydantic>=1.10
+00000160: 2e38 0a52 6571 7569 7265 732d 4469 7374  .8.Requires-Dist
+00000170: 3a20 7765 6273 6f63 6b65 7473 3e3d 3131  : websockets>=11
+00000180: 2e30 2e33 0a44 6573 6372 6970 7469 6f6e  .0.3.Description
+00000190: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000001a0: 6578 742f 6d61 726b 646f 776e 0a0a 6060  ext/markdown..``
+000001b0: 6074 6578 740a 2020 205f 5f5f 5f5f 2020  `text.   _____  
+000001c0: 2020 2020 2020 205f 5f20 2020 5f5f 2020         __   __  
+000001d0: 5f5f 5f5f 2020 2020 2020 2020 2020 2020  ____            
+000001e0: 2020 2020 2020 205f 5f5f 5f5f 2020 5f5f         _____  __
+000001f0: 2020 2020 205f 5f0a 2020 2f20 5f5f 5f5f       __.  / ____
+00000200: 7c20 2020 2f5c 2020 205c 205c 202f 202f  |   /\   \ \ / /
+00000210: 202f 205f 5f20 5c20 2020 2020 2020 2020   / __ \         
+00000220: 2020 202f 5c20 2020 7c20 205f 5f20 5c20     /\   |  __ \ 
+00000230: 5c20 5c20 2020 2f20 2f0a 207c 2028 5f5f  \ \   / /. | (__
+00000240: 5f20 2020 202f 2020 5c20 2020 5c20 5620  _    /  \   \ V 
+00000250: 2f20 7c20 7c20 207c 207c 2020 5f5f 5f5f  / | |  | |  ____
+00000260: 2020 2020 2f20 205c 2020 7c20 7c5f 5f29      /  \  | |__)
+00000270: 207c 205c 205c 5f2f 202f 200a 2020 5c5f   | \ \_/ / .  \_
+00000280: 5f5f 205c 2020 2f20 2f5c 205c 2020 2029  __ \  / /\ \   )
+00000290: 2028 2020 7c20 7c20 207c 207c 207c 5f5f   (  | |  | | |__
+000002a0: 5f5f 7c20 202f 202f 5c20 5c20 7c20 205f  __|  / /\ \ |  _
+000002b0: 5f5f 2f20 2020 5c20 2020 2f20 200a 2020  __/   \   /  .  
+000002c0: 5f5f 5f5f 2920 7c2f 205f 5f5f 5f20 5c20  ____) |/ ____ \ 
+000002d0: 2f20 5f20 5c20 7c20 7c5f 5f7c 207c 2020  / _ \ | |__| |  
+000002e0: 2020 2020 2020 2f20 5f5f 5f5f 205c 7c20        / ____ \| 
+000002f0: 7c20 2020 2020 2020 207c 207c 2020 200a  |        | |   .
+00000300: 207c 5f5f 5f5f 5f2f 2f5f 2f20 2020 205c   |_____//_/    \
+00000310: 2f2f 5f2f 205c 5f5c 205c 5f5f 5f5f 2f20  //_/ \_\ \____/ 
+00000320: 2020 2020 2020 202f 5f2f 2020 2020 5c2f         /_/    \/
+00000330: 7c5f 7c20 2020 2020 2020 207c 5f7c 2020  |_|        |_|  
+00000340: 0a20 6060 600a 0a5b 215b 7079 7468 6f6e  . ```..[![python
+00000350: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000360: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
+00000370: 7974 686f 6e2d 332e 3725 3242 2d62 6c75  ython-3.7%2B-blu
+00000380: 6529 5d28 6874 7470 733a 2f2f 6769 7468  e)](https://gith
+00000390: 7562 2e63 6f6d 2f67 6964 7665 6e2f 7361  ub.com/gidven/sa
+000003a0: 786f 2d6f 7065 6e61 7069 2d63 6c69 656e  xo-openapi-clien
+000003b0: 742d 7079 7468 6f6e 290a 5b21 5b70 7970  t-python).[![pyp
+000003c0: 695d 2868 7474 7073 3a2f 2f69 6d67 2e73  i](https://img.s
+000003d0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+000003e0: 2f73 6178 6f2d 6170 793f 7374 796c 653d  /saxo-apy?style=
+000003f0: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
+00000400: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000410: 726f 6a65 6374 2f73 6178 6f2d 6170 7929  roject/saxo-apy)
+00000420: 0a5b 215b 6c69 6365 6e73 655d 2868 7474  .[![license](htt
+00000430: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000440: 2e69 6f2f 6769 7468 7562 2f6c 6963 656e  .io/github/licen
+00000450: 7365 2f67 6964 7665 6e2f 7361 786f 2d6f  se/gidven/saxo-o
+00000460: 7065 6e61 7069 2d63 6c69 656e 742d 7079  penapi-client-py
+00000470: 7468 6f6e 3f73 7479 6c65 3d66 6c61 742d  thon?style=flat-
+00000480: 7371 7561 7265 295d 2868 7474 7073 3a2f  square)](https:/
+00000490: 2f67 6974 6875 622e 636f 6d2f 6769 6476  /github.com/gidv
+000004a0: 656e 2f73 6178 6f2d 6f70 656e 6170 692d  en/saxo-openapi-
+000004b0: 636c 6965 6e74 2d70 7974 686f 6e2f 626c  client-python/bl
+000004c0: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 4529  ob/main/LICENSE)
+000004d0: 0a0a 2320 5361 786f 2d41 5059 3a20 5079  ..# Saxo-APY: Py
+000004e0: 7468 6f6e 2043 6c69 656e 7420 666f 7220  thon Client for 
+000004f0: 5361 786f 2042 616e 6b20 4f70 656e 4150  Saxo Bank OpenAP
+00000500: 490a 0a2a 4120 6c69 6768 7477 6569 6768  I..*A lightweigh
+00000510: 7420 5079 7468 6f6e 2063 6c69 656e 7420  t Python client 
+00000520: 666f 7220 6861 7373 6c65 2d66 7265 6520  for hassle-free 
+00000530: 7469 6e6b 6572 696e 6720 7769 7468 2053  tinkering with S
+00000540: 6178 6f20 4f70 656e 4150 492e 2a0a 0a3e  axo OpenAPI.*..>
+00000550: 204e 4f54 453a 2054 6869 7320 5079 7468   NOTE: This Pyth
+00000560: 6f6e 2070 6163 6b61 6765 2077 6173 2063  on package was c
+00000570: 7265 6174 6564 2062 7920 616e 2065 6e74  reated by an ent
+00000580: 6875 7369 6173 7420 6173 2061 206c 6561  husiast as a lea
+00000590: 726e 696e 6720 7072 6f6a 6563 742e 204e  rning project. N
+000005a0: 6f6e 6520 6f66 2074 6865 2063 6f6e 7465  one of the conte
+000005b0: 6e74 7320 696e 2074 6869 7320 7265 706f  nts in this repo
+000005c0: 7369 746f 7279 2061 7265 206d 6169 6e74  sitory are maint
+000005d0: 6169 6e65 6420 6279 2053 6178 6f20 4261  ained by Saxo Ba
+000005e0: 6e6b 2c20 616e 6420 5361 786f 2042 616e  nk, and Saxo Ban
+000005f0: 6b20 646f 6573 206e 6f74 2067 7561 7261  k does not guara
+00000600: 6e74 6565 2063 6f72 7265 6374 6e65 7373  ntee correctness
+00000610: 206f 6620 7468 6520 7072 6f76 6964 6564   of the provided
+00000620: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2e   implementation.
+00000630: 0a0a 2323 2041 7420 4669 7273 7420 476c  ..## At First Gl
+00000640: 616e 6365 0a0a 3e20 466f 7220 6d6f 7265  ance..> For more
+00000650: 2069 6e73 7069 7261 7469 6f6e 2073 6565   inspiration see
+00000660: 205b 7468 6520 7361 6d70 6c65 735d 282e   [the samples](.
+00000670: 2f73 616d 706c 6573 2f29 210a 0a60 6060  /samples/)!..```
+00000680: 7079 7468 6f6e 0a66 726f 6d20 7361 786f  python.from saxo
+00000690: 5f61 7079 2069 6d70 6f72 7420 5361 786f  _apy import Saxo
+000006a0: 4f70 656e 4150 4943 6c69 656e 740a 0a63  OpenAPIClient..c
+000006b0: 6c69 656e 7420 3d20 5361 786f 4f70 656e  lient = SaxoOpen
+000006c0: 4150 4943 6c69 656e 7428 2261 7070 5f63  APIClient("app_c
+000006d0: 6f6e 6669 672e 6a73 6f6e 2229 0a63 6c69  onfig.json").cli
+000006e0: 656e 742e 6c6f 6769 6e28 290a 0a6d 6520  ent.login()..me 
+000006f0: 3d20 636c 6965 6e74 2e67 6574 2822 706f  = client.get("po
+00000700: 7274 2f76 312f 7573 6572 732f 6d65 2229  rt/v1/users/me")
+00000710: 0a65 7572 7573 645f 7072 6963 6520 3d20  .eurusd_price = 
+00000720: 636c 6965 6e74 2e67 6574 2822 2f74 7261  client.get("/tra
+00000730: 6465 2f76 312f 696e 666f 7072 6963 6573  de/v1/infoprices
+00000740: 3f55 6963 3d32 3126 4173 7365 7454 7970  ?Uic=21&AssetTyp
+00000750: 653d 4678 5370 6f74 2229 0a70 6f72 7466  e=FxSpot").portf
+00000760: 6f6c 696f 5f6f 7264 6572 7320 3d20 636c  olio_orders = cl
+00000770: 6965 6e74 2e67 6574 2822 2f70 6f72 742f  ient.get("/port/
+00000780: 7631 2f6f 7264 6572 732f 6d65 2229 0a0a  v1/orders/me")..
+00000790: 7072 696e 7428 6622 5765 6c63 6f6d 6520  print(f"Welcome 
+000007a0: 7b6d 655b 2755 7365 7249 6427 5d7d 2122  {me['UserId']}!"
+000007b0: 290a 7072 696e 7428 6622 4555 5255 5344  ).print(f"EURUSD
+000007c0: 2069 7320 7472 6164 696e 6720 6174 3a20   is trading at: 
+000007d0: 7b65 7572 7573 645f 7072 6963 655b 2751  {eurusd_price['Q
+000007e0: 756f 7465 275d 5b27 4269 6427 5d7d 202f  uote']['Bid']} /
+000007f0: 207b 6575 7275 7364 5f70 7269 6365 5b27   {eurusd_price['
+00000800: 5175 6f74 6527 5d5b 2741 736b 275d 7d22  Quote']['Ask']}"
+00000810: 290a 7072 696e 7428 6622 596f 7520 6861  ).print(f"You ha
+00000820: 7665 3a20 7b70 6f72 7466 6f6c 696f 5f6f  ve: {portfolio_o
+00000830: 7264 6572 735b 275f 5f63 6f75 6e74 275d  rders['__count']
+00000840: 7d20 6f72 6465 7273 2069 6e20 796f 7572  } orders in your
+00000850: 2070 6f72 7466 6f6c 696f 2229 0a60 6060   portfolio").```
+00000860: 0a0a 4f75 7470 7574 3a0a 0a60 6060 7465  ..Output:..```te
+00000870: 7874 0af0 9f8c 9020 6f70 656e 696e 6720  xt..... opening 
+00000880: 6c6f 6769 6e20 7061 6765 2069 6e20 6272  login page in br
+00000890: 6f77 7365 7220 2d20 7761 6974 696e 6720  owser - waiting 
+000008a0: 666f 7220 7573 6572 2074 6f20 6175 7468  for user to auth
+000008b0: 656e 7469 6361 7465 2e2e 2e20 f09f 9491  enticate... ....
+000008c0: 0af0 9f93 9e20 7265 6365 6976 6564 2063  ..... received c
+000008d0: 616c 6c62 6163 6b20 6672 6f6d 2053 6178  allback from Sax
+000008e0: 6f20 5353 4f0a e29c 8520 6175 7468 6f72  o SSO.... author
+000008f0: 697a 6174 696f 6e20 7375 6363 6565 6465  ization succeede
+00000900: 6420 2d20 636f 6e6e 6563 7465 6420 746f  d - connected to
+00000910: 2053 494d 2065 6e76 6972 6f6e 6d65 6e74   SIM environment
+00000920: 2077 6974 6820 5752 4954 4520 2f20 5452   with WRITE / TR
+00000930: 4144 4520 7065 726d 6973 7369 6f6e 7320  ADE permissions 
+00000940: 2873 6573 7369 6f6e 2049 4420 6365 6232  (session ID ceb2
+00000950: 6265 3930 3935 6636 3465 6166 3965 3563  be9095f64eaf9e5c
+00000960: 6165 6232 3164 3666 6337 3939 290a 0a57  aeb21d6fc799)..W
+00000970: 656c 636f 6d65 2031 3633 3731 3630 3921  elcome 16371609!
+00000980: 0a45 5552 5553 4420 6973 2074 7261 6469  .EURUSD is tradi
+00000990: 6e67 2061 743a 2031 2e30 3832 3239 202f  ng at: 1.08229 /
+000009a0: 2031 2e30 3832 3439 2028 4269 642f 4173   1.08249 (Bid/As
+000009b0: 6b29 0a59 6f75 2068 6176 653a 2031 3520  k).You have: 15 
+000009c0: 6f72 6465 7273 2069 6e20 796f 7572 2070  orders in your p
+000009d0: 6f72 7466 6f6c 696f 0a60 6060 0a0a 2323  ortfolio.```..##
+000009e0: 2046 6561 7475 7265 730a 0a2d 205b 785d   Features..- [x]
+000009f0: 2041 7574 6865 6e74 6963 6174 696f 6e20   Authentication 
+00000a00: 616e 6420 7365 7373 696f 6e20 6d61 6e61  and session mana
+00000a10: 6765 6d65 6e74 2077 6974 6820 5361 786f  gement with Saxo
+00000a20: 2053 534f 0a20 202d 2053 7570 706f 7274   SSO.  - Support
+00000a30: 7320 4f41 7574 6820 322e 3020 6043 6f64  s OAuth 2.0 `Cod
+00000a40: 6560 2067 7261 6e74 2074 7970 650a 2020  e` grant type.  
+00000a50: 2d20 576f 726b 7320 7365 616d 6c65 7373  - Works seamless
+00000a60: 6c79 2069 6e20 626f 7468 2060 5349 4d60  ly in both `SIM`
+00000a70: 2061 6e64 2060 4c49 5645 6020 656e 7669   and `LIVE` envi
+00000a80: 726f 6e6d 656e 7473 0a20 202d 2041 7574  ronments.  - Aut
+00000a90: 6f6d 6174 6564 2068 616e 646c 696e 6720  omated handling 
+00000aa0: 6f66 2063 616c 6c62 6163 6b20 6672 6f6d  of callback from
+00000ab0: 2053 534f 2028 6f70 7469 6f6e 616c 290a   SSO (optional).
+00000ac0: 2020 2d20 4865 6164 6c65 7373 2061 7574    - Headless aut
+00000ad0: 6865 6e74 6963 6174 696f 6e20 666f 7220  hentication for 
+00000ae0: 6465 706c 6f79 6564 2061 7070 6c69 6361  deployed applica
+00000af0: 7469 6f6e 7320 286f 7074 696f 6e61 6c29  tions (optional)
+00000b00: 0a20 202d 204b 6565 7020 7365 7373 696f  .  - Keep sessio
+00000b10: 6e73 2061 6e64 2061 6374 6976 6520 7765  ns and active we
+00000b20: 6273 6f63 6b65 7473 2063 6f6e 6e65 6374  bsockets connect
+00000b30: 696f 6e73 2061 6c69 7665 2062 7920 7265  ions alive by re
+00000b40: 6672 6573 6869 6e67 2061 6363 6573 7320  freshing access 
+00000b50: 746f 6b65 6e73 2076 6961 2061 7379 6e63  tokens via async
+00000b60: 696f 0a2d 205b 785d 2052 6561 6420 6f70  io.- [x] Read op
+00000b70: 6572 6174 696f 6e73 2028 6047 4554 6020  erations (`GET` 
+00000b80: 7265 7175 6573 7473 290a 2d20 5b78 5d20  requests).- [x] 
+00000b90: 5772 6974 6520 6f70 6572 6174 696f 6e73  Write operations
+00000ba0: 2028 6050 4f53 5460 2c20 6050 5554 602c   (`POST`, `PUT`,
+00000bb0: 2060 5041 5443 4860 2c20 6044 454c 4554   `PATCH`, `DELET
+00000bc0: 4560 2072 6571 7565 7374 7329 0a2d 205b  E` requests).- [
+00000bd0: 785d 2053 7570 706f 7274 7320 6173 796e  x] Supports asyn
+00000be0: 6320 7265 7175 6573 7473 2c20 7374 7265  c requests, stre
+00000bf0: 616d 696e 672c 2061 6e64 2064 6563 6f64  aming, and decod
+00000c00: 696e 6720 6f66 2073 7472 6561 6d69 6e67  ing of streaming
+00000c10: 206d 6573 7361 6765 730a 2d20 5b78 5d20   messages.- [x] 
+00000c20: 4572 726f 7220 6861 6e64 6c69 6e67 2077  Error handling w
+00000c30: 6974 6820 636f 6d70 7265 6865 6e73 6976  ith comprehensiv
+00000c40: 6520 6578 6365 7074 696f 6e20 6d65 7373  e exception mess
+00000c50: 6167 6573 0a0a 2323 2049 6e73 7461 6c6c  ages..## Install
+00000c60: 6174 696f 6e0a 0a54 6869 7320 7079 7468  ation..This pyth
+00000c70: 6f6e 2070 6163 6b61 6765 2069 7320 6176  on package is av
+00000c80: 6169 6c61 626c 6520 6f6e 2050 7950 492e  ailable on PyPI.
+00000c90: 2049 6e73 7461 6c6c 2074 6865 2063 6c69   Install the cli
+00000ca0: 656e 7420 6279 2072 756e 6e69 6e67 2074  ent by running t
+00000cb0: 6865 2062 656c 6f77 2060 7069 7060 2063  he below `pip` c
+00000cc0: 6f6d 6d61 6e64 2069 6e20 796f 7572 2074  ommand in your t
+00000cd0: 6572 6d69 6e61 6c3a 0a0a 6070 6970 2069  erminal:..`pip i
+00000ce0: 6e73 7461 6c6c 2073 6178 6f2d 6170 7960  nstall saxo-apy`
+00000cf0: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00000d00: 730a 0a2d 2050 7974 686f 6e20 332e 372b  s..- Python 3.7+
+00000d10: 0a2d 2041 6e20 4f70 656e 4150 4920 6170  .- An OpenAPI ap
+00000d20: 706c 6963 6174 696f 6e20 7265 6769 7374  plication regist
+00000d30: 6572 6564 205b 6f6e 2053 6178 6f20 4261  ered [on Saxo Ba
+00000d40: 6e6b 2773 2044 6576 656c 6f70 6572 2050  nk's Developer P
+00000d50: 6f72 7461 6c5d 2868 7474 7073 3a2f 2f77  ortal](https://w
+00000d60: 7777 2e64 6576 656c 6f70 6572 2e73 6178  ww.developer.sax
+00000d70: 6f2f 6f70 656e 6170 692f 6170 706d 616e  o/openapi/appman
+00000d80: 6167 656d 656e 7429 0a20 202d 205b 4372  agement).  - [Cr
+00000d90: 6561 7465 2061 2066 7265 6520 6465 7665  eate a free deve
+00000da0: 6c6f 7065 7220 6163 636f 756e 745d 2868  loper account](h
+00000db0: 7474 7073 3a2f 2f77 7777 2e64 6576 656c  ttps://www.devel
+00000dc0: 6f70 6572 2e73 6178 6f2f 6163 636f 756e  oper.saxo/accoun
+00000dd0: 7473 2f73 696d 2f73 6967 6e75 7029 2069  ts/sim/signup) i
+00000de0: 6620 796f 7520 646f 6e27 7420 6861 7665  f you don't have
+00000df0: 206f 6e65 2061 6c72 6561 6479 2e0a 2020   one already..  
+00000e00: 2d20 456e 7375 7265 2074 6865 2061 7070  - Ensure the app
+00000e10: 6c69 6361 7469 6f6e 2069 7320 7365 7420  lication is set 
+00000e20: 7570 2077 6974 6820 6047 7261 6e74 2054  up with `Grant T
+00000e30: 7970 653a 2043 6f64 6560 2061 7320 6175  ype: Code` as au
+00000e40: 7468 656e 7469 6361 7469 6f6e 2066 6c6f  thentication flo
+00000e50: 772e 0a20 202d 2041 7420 6c65 6173 7420  w..  - At least 
+00000e60: 3120 6c6f 6361 6c68 6f73 7420 7265 6469  1 localhost redi
+00000e70: 7265 6374 206e 6565 6473 2074 6f20 6265  rect needs to be
+00000e80: 2064 6566 696e 6564 2073 7563 6820 6173   defined such as
+00000e90: 2060 6874 7470 3a2f 2f6c 6f63 616c 686f   `http://localho
+00000ea0: 7374 3a31 3233 3231 2f72 6564 6972 6563  st:12321/redirec
+00000eb0: 7460 2028 666f 7220 6465 7665 6c6f 706d  t` (for developm
+00000ec0: 656e 742f 7465 7374 696e 6720 7075 7270  ent/testing purp
+00000ed0: 6f73 6573 290a 2020 2d20 284f 7074 696f  oses).  - (Optio
+00000ee0: 6e61 6c29 2065 6e61 626c 6520 7472 6164  nal) enable trad
+00000ef0: 696e 6720 7065 726d 6973 7369 6f6e 7320  ing permissions 
+00000f00: 666f 7220 7468 6520 6170 7020 6966 2079  for the app if y
+00000f10: 6f75 2077 616e 7420 746f 2027 7772 6974  ou want to 'writ
+00000f20: 6527 2074 6f20 796f 7572 2061 6363 6f75  e' to your accou
+00000f30: 6e74 2028 616e 6420 706c 6163 6520 6f72  nt (and place or
+00000f40: 6465 7273 290a 0a23 2320 4465 7065 6e64  ders)..## Depend
+00000f50: 656e 6369 6573 0a0a 5468 6973 2070 6163  encies..This pac
+00000f60: 6b61 6765 2072 6571 7569 7265 7320 3520  kage requires 5 
+00000f70: 6465 7065 6e64 656e 6369 6573 3a0a 0a2d  dependencies:..-
+00000f80: 2060 7079 6461 6e74 6963 602c 2066 6f72   `pydantic`, for
+00000f90: 2070 6172 7369 6e67 2063 6f6e 6669 6720   parsing config 
+00000fa0: 616e 6420 4a53 4f4e 2072 6573 706f 6e73  and JSON respons
+00000fb0: 6573 200a 2d20 6046 6c61 736b 602c 2074  es .- `Flask`, t
+00000fc0: 6f20 7275 6e20 6120 6c6f 6361 6c20 7365  o run a local se
+00000fd0: 7276 6572 2061 6e64 2063 6174 6368 2074  rver and catch t
+00000fe0: 6865 2063 616c 6c62 6163 6b20 6672 6f6d  he callback from
+00000ff0: 2053 6178 6f20 5353 4f0a 2d20 6068 7474   Saxo SSO.- `htt
+00001000: 7078 602c 2066 6f72 2073 656e 6469 6e67  px`, for sending
+00001010: 2072 6571 7565 7374 7320 746f 204f 7065   requests to Ope
+00001020: 6e41 5049 2061 6e64 206d 616e 6167 696e  nAPI and managin
+00001030: 6720 7468 6520 636c 6965 6e74 2073 6573  g the client ses
+00001040: 7369 6f6e 0a2d 2060 7765 6273 6f63 6b65  sion.- `websocke
+00001050: 7473 602c 2066 6f72 2073 6574 7469 6e67  ts`, for setting
+00001060: 2075 7020 6120 7765 6273 6f63 6b65 7420   up a websocket 
+00001070: 636f 6e6e 6563 7469 6f6e 2074 6f20 5361  connection to Sa
+00001080: 786f 2773 2073 7472 6561 6d69 6e67 2073  xo's streaming s
+00001090: 6572 7669 6365 0a2d 2060 6c6f 6775 7275  ervice.- `loguru
+000010a0: 602c 2074 6f20 6861 6e64 6c65 206c 6f67  `, to handle log
+000010b0: 6769 6e67 0a0a 2323 204e 6f74 6573 0a0a  ging..## Notes..
+000010c0: 5468 6520 636c 6965 6e74 2073 7570 706f  The client suppo
+000010d0: 7274 7320 4f41 7574 6820 436f 6465 2066  rts OAuth Code f
+000010e0: 6c6f 7720 616e 6420 7769 6c6c 2061 7574  low and will aut
+000010f0: 6f6d 6174 6963 616c 6c79 2073 7069 6e20  omatically spin 
+00001100: 7570 2061 2073 6572 7665 7220 746f 206c  up a server to l
+00001110: 6973 7465 6e20 666f 7220 7468 6520 7265  isten for the re
+00001120: 6469 7265 6374 2066 726f 6d20 5361 786f  direct from Saxo
+00001130: 2053 534f 2e20 4174 206c 6561 7374 2031   SSO. At least 1
+00001140: 2060 6c6f 6361 6c68 6f73 7460 2072 6564   `localhost` red
+00001150: 6972 6563 7420 6e65 6564 7320 746f 2062  irect needs to b
+00001160: 6520 6465 6669 6e65 6420 696e 2061 7070  e defined in app
+00001170: 6c69 6361 7469 6f6e 2063 6f6e 6669 6720  lication config 
+00001180: 666f 7220 7468 6973 2070 7572 706f 7365  for this purpose
+00001190: 2e0a 0a42 7920 6465 6661 756c 742c 2074  ...By default, t
+000011a0: 6865 2063 6c69 656e 7420 7769 6c6c 2075  he client will u
+000011b0: 7365 2074 6865 202a 6669 7273 7420 6176  se the *first av
+000011c0: 6169 6c61 626c 6520 6c6f 6361 6c68 6f73  ailable localhos
+000011d0: 7420 7265 6469 7265 6374 2a20 746f 2072  t redirect* to r
+000011e0: 756e 2074 6865 2073 6572 7665 7220 6f6e  un the server on
+000011f0: 2028 7479 7069 6361 6c6c 7920 6f6e 6c79   (typically only
+00001200: 2031 2065 7869 7374 7320 696e 2074 6865   1 exists in the
+00001210: 2063 6f6e 6669 6729 2e0a 0a54 6865 2063   config)...The c
+00001220: 6c69 656e 7420 7661 6c69 6461 7465 7320  lient validates 
+00001230: 7265 6469 7265 6374 2075 726c 7320 696e  redirect urls in
+00001240: 2061 7070 6c69 6361 7469 6f6e 2063 6f6e   application con
+00001250: 6669 6720 6175 746f 6d61 7469 6361 6c6c  fig automaticall
+00001260: 792e 204f 4175 7468 2032 2e30 2063 6f64  y. OAuth 2.0 cod
+00001270: 6520 666c 6f77 2072 6571 7569 7265 7320  e flow requires 
+00001280: 6120 6669 7865 6420 706f 7274 2074 6f20  a fixed port to 
+00001290: 6265 2073 7065 6369 6669 6564 206f 6e20  be specified on 
+000012a0: 7468 6520 7265 6469 7265 6374 2075 726c  the redirect url
+000012b0: 2e20 496e 2063 6173 6520 7468 6973 2069  . In case this i
+000012c0: 7320 696e 636f 7272 6563 746c 7920 636f  s incorrectly co
+000012d0: 6e66 6967 7572 6564 2c20 616e 2065 7272  nfigured, an err
+000012e0: 6f72 206d 6573 7361 6765 2077 696c 6c20  or message will 
+000012f0: 6775 6964 6520 796f 7520 746f 2065 6e73  guide you to ens
+00001300: 7572 6520 6170 7020 636f 6e66 6967 2069  ure app config i
+00001310: 7320 636f 7272 6563 7420 7769 7468 204f  s correct with O
+00001320: 7065 6e41 5049 3a0a 0a60 6060 7465 7874  penAPI:..```text
+00001330: 0a6f 6e65 206f 7220 6d6f 7265 2072 6564  .one or more red
+00001340: 6972 6563 7420 7572 6c73 2068 6176 6520  irect urls have 
+00001350: 6e6f 2070 6f72 7420 636f 6e66 6967 7572  no port configur
+00001360: 6564 2c20 7768 6963 6820 6973 2072 6571  ed, which is req
+00001370: 7569 7265 6420 666f 7220 6772 616e 7420  uired for grant 
+00001380: 7479 7065 2027 436f 6465 2720 2d20 656e  type 'Code' - en
+00001390: 7375 7265 2061 2070 6f72 7420 6973 2063  sure a port is c
+000013a0: 6f6e 6669 6775 7265 6420 696e 2074 6865  onfigured in the
+000013b0: 2061 7070 2063 6f6e 6669 6720 6f62 6a65   app config obje
+000013c0: 6374 2066 6f72 2065 6163 6820 7572 6c20  ct for each url 
+000013d0: 2865 7861 6d70 6c65 3a20 6874 7470 3a2f  (example: http:/
+000013e0: 2f6c 6f63 616c 686f 7374 3a32 3334 3332  /localhost:23432
+000013f0: 2f72 6564 6972 6563 7429 0a60 6060 0a    /redirect).```.
```

### Comparing `saxo_apy-0.2.5/pyproject.toml` & `saxo_apy-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `saxo_apy-0.2.5/PKG-INFO` & `saxo_apy-0.2.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,322 +1,294 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7361 786f  : 2.1.Name: saxo
-00000020: 2d61 7079 0a56 6572 7369 6f6e 3a20 302e  -apy.Version: 0.
-00000030: 322e 350a 5375 6d6d 6172 793a 2041 206c  2.5.Summary: A l
-00000040: 6967 6874 7765 6967 6874 2050 7974 686f  ightweight Pytho
-00000050: 6e20 636c 6965 6e74 2066 6f72 2068 6173  n client for has
-00000060: 736c 652d 6672 6565 2074 696e 6b65 7269  sle-free tinkeri
-00000070: 6e67 2077 6974 6820 5361 786f 204f 7065  ng with Saxo Ope
-00000080: 6e41 5049 2e0a 4175 7468 6f72 2d65 6d61  nAPI..Author-ema
-00000090: 696c 3a20 4769 6420 3c67 6964 6465 7661  il: Gid <giddeva
-000000a0: 6e64 6572 7665 6e40 676d 6169 6c2e 636f  nderven@gmail.co
-000000b0: 6d3e 0a4c 6963 656e 7365 3a20 4d49 540a  m>.License: MIT.
-000000c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000000d0: 4345 4e53 450a 5265 7175 6972 6573 2d50  CENSE.Requires-P
-000000e0: 7974 686f 6e3a 203e 3d33 2e37 0a52 6571  ython: >=3.7.Req
-000000f0: 7569 7265 732d 4469 7374 3a20 666c 6173  uires-Dist: flas
-00000100: 6b3e 3d32 2e32 2e35 0a52 6571 7569 7265  k>=2.2.5.Require
-00000110: 732d 4469 7374 3a20 6874 7470 783e 3d30  s-Dist: httpx>=0
-00000120: 2e32 342e 310a 5265 7175 6972 6573 2d44  .24.1.Requires-D
-00000130: 6973 743a 206c 6f67 7572 753e 3d30 2e37  ist: loguru>=0.7
-00000140: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
-00000150: 3a20 7079 6461 6e74 6963 3e3d 312e 3130  : pydantic>=1.10
-00000160: 2e38 0a52 6571 7569 7265 732d 4469 7374  .8.Requires-Dist
-00000170: 3a20 7765 6273 6f63 6b65 7473 3e3d 3131  : websockets>=11
-00000180: 2e30 2e33 0a44 6573 6372 6970 7469 6f6e  .0.3.Description
-00000190: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000001a0: 6578 742f 6d61 726b 646f 776e 0a0a 6060  ext/markdown..``
-000001b0: 600a 2020 205f 5f5f 5f5f 2020 2020 2020  `.   _____      
-000001c0: 2020 205f 5f20 2020 5f5f 2020 5f5f 5f5f     __   __  ____
-000001d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001e0: 2020 205f 5f5f 5f5f 2020 5f5f 2020 2020     _____  __    
-000001f0: 205f 5f0a 2020 2f20 5f5f 5f5f 7c20 2020   __.  / ____|   
-00000200: 2f5c 2020 205c 205c 202f 202f 202f 205f  /\   \ \ / / / _
-00000210: 5f20 5c20 2020 2020 2020 2020 2020 202f  _ \            /
-00000220: 5c20 2020 7c20 205f 5f20 5c20 5c20 5c20  \   |  __ \ \ \ 
-00000230: 2020 2f20 2f0a 207c 2028 5f5f 5f20 2020    / /. | (___   
-00000240: 202f 2020 5c20 2020 5c20 5620 2f20 7c20   /  \   \ V / | 
-00000250: 7c20 207c 207c 2020 5f5f 5f5f 2020 2020  |  | |  ____    
-00000260: 2f20 205c 2020 7c20 7c5f 5f29 207c 205c  /  \  | |__) | \
-00000270: 205c 5f2f 202f 200a 2020 5c5f 5f5f 205c   \_/ / .  \___ \
-00000280: 2020 2f20 2f5c 205c 2020 2029 2028 2020    / /\ \   ) (  
-00000290: 7c20 7c20 207c 207c 207c 5f5f 5f5f 7c20  | |  | | |____| 
-000002a0: 202f 202f 5c20 5c20 7c20 205f 5f5f 2f20   / /\ \ |  ___/ 
-000002b0: 2020 5c20 2020 2f20 200a 2020 5f5f 5f5f    \   /  .  ____
-000002c0: 2920 7c2f 205f 5f5f 5f20 5c20 2f20 5f20  ) |/ ____ \ / _ 
-000002d0: 5c20 7c20 7c5f 5f7c 207c 2020 2020 2020  \ | |__| |      
-000002e0: 2020 2f20 5f5f 5f5f 205c 7c20 7c20 2020    / ____ \| |   
-000002f0: 2020 2020 207c 207c 2020 200a 207c 5f5f       | |   . |__
-00000300: 5f5f 5f2f 2f5f 2f20 2020 205c 2f2f 5f2f  ___//_/    \//_/
-00000310: 205c 5f5c 205c 5f5f 5f5f 2f20 2020 2020   \_\ \____/     
-00000320: 2020 202f 5f2f 2020 2020 5c2f 7c5f 7c20     /_/    \/|_| 
-00000330: 2020 2020 2020 207c 5f7c 2020 0a20 6060         |_|  . ``
-00000340: 600a 0a5b 215b 7079 7468 6f6e 5d28 6874  `..[![python](ht
-00000350: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000360: 732e 696f 2f62 6164 6765 2f70 7974 686f  s.io/badge/pytho
-00000370: 6e2d 332e 3725 3242 2d62 6c75 6529 5d28  n-3.7%2B-blue)](
-00000380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000390: 6f6d 2f67 6964 7665 6e2f 7361 786f 2d6f  om/gidven/saxo-o
-000003a0: 7065 6e61 7069 2d63 6c69 656e 742d 7079  penapi-client-py
-000003b0: 7468 6f6e 290a 5b21 5b70 7970 695d 2868  thon).[![pypi](h
-000003c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000003d0: 6473 2e69 6f2f 7079 7069 2f76 2f73 6178  ds.io/pypi/v/sax
-000003e0: 6f2d 6170 793f 7374 796c 653d 666c 6174  o-apy?style=flat
-000003f0: 2d73 7175 6172 6529 5d28 6874 7470 733a  -square)](https:
-00000400: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000410: 6374 2f73 6178 6f2d 6170 7929 0a5b 215b  ct/saxo-apy).[![
-00000420: 6c69 6365 6e73 655d 2868 7474 7073 3a2f  license](https:/
-00000430: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000440: 6769 7468 7562 2f6c 6963 656e 7365 2f67  github/license/g
-00000450: 6964 7665 6e2f 7361 786f 2d6f 7065 6e61  idven/saxo-opena
-00000460: 7069 2d63 6c69 656e 742d 7079 7468 6f6e  pi-client-python
-00000470: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-00000480: 7265 295d 2868 7474 7073 3a2f 2f67 6974  re)](https://git
-00000490: 6875 622e 636f 6d2f 6769 6476 656e 2f73  hub.com/gidven/s
-000004a0: 6178 6f2d 6f70 656e 6170 692d 636c 6965  axo-openapi-clie
-000004b0: 6e74 2d70 7974 686f 6e2f 626c 6f62 2f6d  nt-python/blob/m
-000004c0: 6169 6e2f 4c49 4345 4e53 4529 0a0a 2320  ain/LICENSE)..# 
-000004d0: 5361 786f 2d41 5059 3a20 5079 7468 6f6e  Saxo-APY: Python
-000004e0: 2043 6c69 656e 7420 666f 7220 5361 786f   Client for Saxo
-000004f0: 2042 616e 6b20 4f70 656e 4150 490a 0a2a   Bank OpenAPI..*
-00000500: 4120 6c69 6768 7477 6569 6768 7420 5079  A lightweight Py
-00000510: 7468 6f6e 2063 6c69 656e 7420 666f 7220  thon client for 
-00000520: 6861 7373 6c65 2d66 7265 6520 7469 6e6b  hassle-free tink
-00000530: 6572 696e 6720 7769 7468 2053 6178 6f20  ering with Saxo 
-00000540: 4f70 656e 4150 492e 2a0a 0a3e 204e 4f54  OpenAPI.*..> NOT
-00000550: 453a 2054 6869 7320 5079 7468 6f6e 2070  E: This Python p
-00000560: 6163 6b61 6765 2077 6173 2063 7265 6174  ackage was creat
-00000570: 6564 2062 7920 616e 2065 6e74 6875 7369  ed by an enthusi
-00000580: 6173 7420 6173 2061 206c 6561 726e 696e  ast as a learnin
-00000590: 6720 7072 6f6a 6563 742e 204e 6f6e 6520  g project. None 
-000005a0: 6f66 2074 6865 2063 6f6e 7465 6e74 7320  of the contents 
-000005b0: 696e 2074 6869 7320 7265 706f 7369 746f  in this reposito
-000005c0: 7279 2061 7265 206d 6169 6e74 6169 6e65  ry are maintaine
-000005d0: 6420 6279 2053 6178 6f20 4261 6e6b 2c20  d by Saxo Bank, 
-000005e0: 616e 6420 5361 786f 2042 616e 6b20 646f  and Saxo Bank do
-000005f0: 6573 206e 6f74 2067 7561 7261 6e74 6565  es not guarantee
-00000600: 2063 6f72 7265 6374 6e65 7373 206f 6620   correctness of 
-00000610: 7468 6520 7072 6f76 6964 6564 2069 6d70  the provided imp
-00000620: 6c65 6d65 6e74 6174 696f 6e2e 0a0a 2323  lementation...##
-00000630: 2041 7420 4669 7273 7420 476c 616e 6365   At First Glance
-00000640: 0a0a 466f 7220 6d6f 7265 2069 6e73 7069  ..For more inspi
-00000650: 7261 7469 6f6e 2073 6565 205b 7468 6520  ration see [the 
-00000660: 7361 6d70 6c65 735d 282e 2f73 616d 706c  samples](./sampl
-00000670: 6573 2f29 210a 0a60 6060 7079 7468 6f6e  es/)!..```python
-00000680: 0a66 726f 6d20 7361 786f 5f61 7079 2069  .from saxo_apy i
-00000690: 6d70 6f72 7420 5361 786f 4f70 656e 4150  mport SaxoOpenAP
-000006a0: 4943 6c69 656e 740a 0a63 6c69 656e 7420  IClient..client 
-000006b0: 3d20 5361 786f 4f70 656e 4150 4943 6c69  = SaxoOpenAPICli
-000006c0: 656e 7428 2261 7070 5f63 6f6e 6669 672e  ent("app_config.
-000006d0: 6a73 6f6e 2229 0a63 6c69 656e 742e 6c6f  json").client.lo
-000006e0: 6769 6e28 290a 0a6d 6520 3d20 636c 6965  gin()..me = clie
-000006f0: 6e74 2e67 6574 2822 706f 7274 2f76 312f  nt.get("port/v1/
-00000700: 7573 6572 732f 6d65 2229 0a65 7572 7573  users/me").eurus
-00000710: 645f 7072 6963 6520 3d20 636c 6965 6e74  d_price = client
-00000720: 2e67 6574 2822 2f74 7261 6465 2f76 312f  .get("/trade/v1/
-00000730: 696e 666f 7072 6963 6573 3f55 6963 3d32  infoprices?Uic=2
-00000740: 3126 4173 7365 7454 7970 653d 4678 5370  1&AssetType=FxSp
-00000750: 6f74 2229 0a70 6f72 7466 6f6c 696f 5f6f  ot").portfolio_o
-00000760: 7264 6572 7320 3d20 636c 6965 6e74 2e67  rders = client.g
-00000770: 6574 2822 2f70 6f72 742f 7631 2f6f 7264  et("/port/v1/ord
-00000780: 6572 732f 6d65 2229 0a0a 7072 696e 7428  ers/me")..print(
-00000790: 6622 5765 6c63 6f6d 6520 7b6d 655b 2755  f"Welcome {me['U
-000007a0: 7365 7249 6427 5d7d 2122 290a 7072 696e  serId']}!").prin
-000007b0: 7428 6622 4555 5255 5344 2069 7320 7472  t(f"EURUSD is tr
-000007c0: 6164 696e 6720 6174 3a20 7b65 7572 7573  ading at: {eurus
-000007d0: 645f 7072 6963 655b 2751 756f 7465 275d  d_price['Quote']
-000007e0: 5b27 4269 6427 5d7d 202f 207b 6575 7275  ['Bid']} / {euru
-000007f0: 7364 5f70 7269 6365 5b27 5175 6f74 6527  sd_price['Quote'
-00000800: 5d5b 2741 736b 275d 7d20 2842 6964 2f41  ]['Ask']} (Bid/A
-00000810: 736b 2922 290a 7072 696e 7428 6622 596f  sk)").print(f"Yo
-00000820: 7520 6861 7665 3a20 7b70 6f72 7466 6f6c  u have: {portfol
-00000830: 696f 5f6f 7264 6572 735b 275f 5f63 6f75  io_orders['__cou
-00000840: 6e74 275d 7d20 6f72 6465 7273 2069 6e20  nt']} orders in 
-00000850: 796f 7572 2070 6f72 7466 6f6c 696f 2229  your portfolio")
-00000860: 0a60 6060 0a0a 2020 2020 f09f 8c90 206f  .```..    .... o
-00000870: 7065 6e69 6e67 206c 6f67 696e 2070 6167  pening login pag
-00000880: 6520 696e 2062 726f 7773 6572 202d 2077  e in browser - w
-00000890: 6169 7469 6e67 2066 6f72 2075 7365 7220  aiting for user 
-000008a0: 746f 2061 7574 6865 6e74 6963 6174 652e  to authenticate.
-000008b0: 2e2e 20f0 9f94 910a 2020 2020 f09f 939e  .. .....    ....
-000008c0: 2072 6563 6569 7665 6420 6361 6c6c 6261   received callba
-000008d0: 636b 2066 726f 6d20 5361 786f 2053 534f  ck from Saxo SSO
-000008e0: 0a20 2020 20e2 9c85 2061 7574 686f 7269  .    ... authori
-000008f0: 7a61 7469 6f6e 2073 7563 6365 6564 6564  zation succeeded
-00000900: 202d 2063 6f6e 6e65 6374 6564 2074 6f20   - connected to 
-00000910: 5349 4d20 656e 7669 726f 6e6d 656e 7420  SIM environment 
-00000920: 7769 7468 2057 5249 5445 202f 2054 5241  with WRITE / TRA
-00000930: 4445 2070 6572 6d69 7373 696f 6e73 2028  DE permissions (
-00000940: 7365 7373 696f 6e20 4944 2063 6562 3262  session ID ceb2b
-00000950: 6539 3039 3566 3634 6561 6639 6535 6361  e9095f64eaf9e5ca
-00000960: 6562 3231 6436 6663 3739 3929 0a20 2020  eb21d6fc799).   
-00000970: 200a 2020 2020 5765 6c63 6f6d 6520 3136   .    Welcome 16
-00000980: 3337 3136 3039 210a 2020 2020 4555 5255  371609!.    EURU
-00000990: 5344 2069 7320 7472 6164 696e 6720 6174  SD is trading at
-000009a0: 3a20 312e 3038 3232 3920 2f20 312e 3038  : 1.08229 / 1.08
-000009b0: 3234 3920 2842 6964 2f41 736b 290a 2020  249 (Bid/Ask).  
-000009c0: 2020 596f 7520 6861 7665 3a20 3135 206f    You have: 15 o
-000009d0: 7264 6572 7320 696e 2079 6f75 7220 706f  rders in your po
-000009e0: 7274 666f 6c69 6f0a 2020 2020 0a0a 0a23  rtfolio.    ...#
-000009f0: 2320 4665 6174 7572 6573 0a0a 2d20 5b78  # Features..- [x
-00000a00: 5d20 4175 7468 656e 7469 6361 7469 6f6e  ] Authentication
-00000a10: 2061 6e64 2073 6573 7369 6f6e 206d 616e   and session man
-00000a20: 6167 656d 656e 7420 7769 7468 2053 6178  agement with Sax
-00000a30: 6f20 5353 4f0a 2020 2020 2d20 5375 7070  o SSO.    - Supp
-00000a40: 6f72 7473 204f 4175 7468 2032 2e30 2060  orts OAuth 2.0 `
-00000a50: 436f 6465 6020 6772 616e 7420 7479 7065  Code` grant type
-00000a60: 0a20 2020 202d 2057 6f72 6b73 2073 6561  .    - Works sea
-00000a70: 6d6c 6573 736c 7920 696e 2062 6f74 6820  mlessly in both 
-00000a80: 6053 494d 6020 616e 6420 604c 4956 4560  `SIM` and `LIVE`
-00000a90: 2065 6e76 6972 6f6e 6d65 6e74 730a 2020   environments.  
-00000aa0: 2020 2d20 4175 746f 6d61 7465 6420 6861    - Automated ha
-00000ab0: 6e64 6c69 6e67 206f 6620 6361 6c6c 6261  ndling of callba
-00000ac0: 636b 2066 726f 6d20 5353 4f20 286f 7074  ck from SSO (opt
-00000ad0: 696f 6e61 6c29 0a20 2020 202d 2048 6561  ional).    - Hea
-00000ae0: 646c 6573 7320 6175 7468 656e 7469 6361  dless authentica
-00000af0: 7469 6f6e 2066 6f72 2064 6570 6c6f 7965  tion for deploye
-00000b00: 6420 6170 706c 6963 6174 696f 6e73 2028  d applications (
-00000b10: 6f70 7469 6f6e 616c 290a 2020 2020 2d20  optional).    - 
-00000b20: 4b65 6570 2073 6573 7369 6f6e 7320 616e  Keep sessions an
-00000b30: 6420 6163 7469 7665 2077 6562 736f 636b  d active websock
-00000b40: 6574 7320 636f 6e6e 6563 7469 6f6e 7320  ets connections 
-00000b50: 616c 6976 6520 6279 2072 6566 7265 7368  alive by refresh
-00000b60: 696e 6720 6163 6365 7373 2074 6f6b 656e  ing access token
-00000b70: 7320 7669 6120 6173 796e 6369 6f0a 2d20  s via asyncio.- 
-00000b80: 5b78 5d20 5265 6164 206f 7065 7261 7469  [x] Read operati
-00000b90: 6f6e 7320 2860 4745 5460 2072 6571 7565  ons (`GET` reque
-00000ba0: 7374 7329 0a2d 205b 785d 2057 7269 7465  sts).- [x] Write
-00000bb0: 206f 7065 7261 7469 6f6e 7320 2860 504f   operations (`PO
-00000bc0: 5354 602c 2060 5055 5460 2c20 6050 4154  ST`, `PUT`, `PAT
-00000bd0: 4348 602c 2060 4445 4c45 5445 6020 7265  CH`, `DELETE` re
-00000be0: 7175 6573 7473 290a 2d20 5b78 5d20 5375  quests).- [x] Su
-00000bf0: 7070 6f72 7473 2061 7379 6e63 2072 6571  pports async req
-00000c00: 7565 7374 732c 2073 7472 6561 6d69 6e67  uests, streaming
-00000c10: 2c20 616e 6420 6465 636f 6469 6e67 206f  , and decoding o
-00000c20: 6620 7374 7265 616d 696e 6720 6d65 7373  f streaming mess
-00000c30: 6167 6573 0a2d 205b 785d 2045 7272 6f72  ages.- [x] Error
-00000c40: 2068 616e 646c 696e 6720 7769 7468 2063   handling with c
-00000c50: 6f6d 7072 6568 656e 7369 7665 2065 7863  omprehensive exc
-00000c60: 6570 7469 6f6e 206d 6573 7361 6765 730a  eption messages.
-00000c70: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000c80: 0a0a 5468 6973 2070 7974 686f 6e20 7061  ..This python pa
-00000c90: 636b 6167 6520 6973 2061 7661 696c 6162  ckage is availab
-00000ca0: 6c65 206f 6e20 5079 5049 2e20 496e 7374  le on PyPI. Inst
-00000cb0: 616c 6c20 7468 6520 636c 6965 6e74 2062  all the client b
-00000cc0: 7920 7275 6e6e 696e 6720 7468 6520 6265  y running the be
-00000cd0: 6c6f 7720 6070 6970 6020 636f 6d6d 616e  low `pip` comman
-00000ce0: 6420 696e 2079 6f75 7220 7465 726d 696e  d in your termin
-00000cf0: 616c 3a0a 0a60 7069 7020 696e 7374 616c  al:..`pip instal
-00000d00: 6c20 7361 786f 2d61 7079 600a 0a23 2320  l saxo-apy`..## 
-00000d10: 5265 7175 6972 656d 656e 7473 0a0a 2d20  Requirements..- 
-00000d20: 5079 7468 6f6e 2033 2e37 2b0a 2d20 416e  Python 3.7+.- An
-00000d30: 204f 7065 6e41 5049 2061 7070 6c69 6361   OpenAPI applica
-00000d40: 7469 6f6e 2072 6567 6973 7465 7265 6420  tion registered 
-00000d50: 5b6f 6e20 5361 786f 2042 616e 6b27 7320  [on Saxo Bank's 
-00000d60: 4465 7665 6c6f 7065 7220 506f 7274 616c  Developer Portal
-00000d70: 5d28 6874 7470 733a 2f2f 7777 772e 6465  ](https://www.de
-00000d80: 7665 6c6f 7065 722e 7361 786f 2f6f 7065  veloper.saxo/ope
-00000d90: 6e61 7069 2f61 7070 6d61 6e61 6765 6d65  napi/appmanageme
-00000da0: 6e74 290a 2020 2020 2d20 5b43 7265 6174  nt).    - [Creat
-00000db0: 6520 6120 6672 6565 2064 6576 656c 6f70  e a free develop
-00000dc0: 6572 2061 6363 6f75 6e74 5d28 6874 7470  er account](http
-00000dd0: 733a 2f2f 7777 772e 6465 7665 6c6f 7065  s://www.develope
-00000de0: 722e 7361 786f 2f61 6363 6f75 6e74 732f  r.saxo/accounts/
-00000df0: 7369 6d2f 7369 676e 7570 2920 6966 2079  sim/signup) if y
-00000e00: 6f75 2064 6f6e 2774 2068 6176 6520 6f6e  ou don't have on
-00000e10: 6520 616c 7265 6164 792e 0a20 2020 202d  e already..    -
-00000e20: 2045 6e73 7572 6520 7468 6520 6170 706c   Ensure the appl
-00000e30: 6963 6174 696f 6e20 6973 2073 6574 2075  ication is set u
-00000e40: 7020 7769 7468 2060 4772 616e 7420 5479  p with `Grant Ty
-00000e50: 7065 3a20 436f 6465 6020 6173 2061 7574  pe: Code` as aut
-00000e60: 6865 6e74 6963 6174 696f 6e20 666c 6f77  hentication flow
-00000e70: 2e0a 2020 2020 2d20 4174 206c 6561 7374  ..    - At least
-00000e80: 2031 206c 6f63 616c 686f 7374 2072 6564   1 localhost red
-00000e90: 6972 6563 7420 6e65 6564 7320 746f 2062  irect needs to b
-00000ea0: 6520 6465 6669 6e65 6420 7375 6368 2061  e defined such a
-00000eb0: 7320 6068 7474 703a 2f2f 6c6f 6361 6c68  s `http://localh
-00000ec0: 6f73 743a 3132 3332 312f 7265 6469 7265  ost:12321/redire
-00000ed0: 6374 6020 2866 6f72 2064 6576 656c 6f70  ct` (for develop
-00000ee0: 6d65 6e74 2f74 6573 7469 6e67 2070 7572  ment/testing pur
-00000ef0: 706f 7365 7329 0a20 2020 202d 2028 4f70  poses).    - (Op
-00000f00: 7469 6f6e 616c 2920 656e 6162 6c65 2074  tional) enable t
-00000f10: 7261 6469 6e67 2070 6572 6d69 7373 696f  rading permissio
-00000f20: 6e73 2066 6f72 2074 6865 2061 7070 2069  ns for the app i
-00000f30: 6620 796f 7520 7761 6e74 2074 6f20 2777  f you want to 'w
-00000f40: 7269 7465 2720 746f 2079 6f75 7220 6163  rite' to your ac
-00000f50: 636f 756e 7420 2861 6e64 2070 6c61 6365  count (and place
-00000f60: 206f 7264 6572 7329 0a0a 2323 2044 6570   orders)..## Dep
-00000f70: 656e 6465 6e63 6965 730a 0a54 6869 7320  endencies..This 
-00000f80: 7061 636b 6167 6520 7265 7175 6972 6573  package requires
-00000f90: 2035 2064 6570 656e 6465 6e63 6965 733a   5 dependencies:
-00000fa0: 0a0a 2d20 6070 7964 616e 7469 6360 2c20  ..- `pydantic`, 
-00000fb0: 666f 7220 7061 7273 696e 6720 636f 6e66  for parsing conf
-00000fc0: 6967 2061 6e64 204a 534f 4e20 7265 7370  ig and JSON resp
-00000fd0: 6f6e 7365 7320 0a2d 2060 466c 6173 6b60  onses .- `Flask`
-00000fe0: 2c20 746f 2072 756e 2061 206c 6f63 616c  , to run a local
-00000ff0: 2073 6572 7665 7220 616e 6420 6361 7463   server and catc
-00001000: 6820 7468 6520 6361 6c6c 6261 636b 2066  h the callback f
-00001010: 726f 6d20 5361 786f 2053 534f 0a2d 2060  rom Saxo SSO.- `
-00001020: 6874 7470 7860 2c20 666f 7220 7365 6e64  httpx`, for send
-00001030: 696e 6720 7265 7175 6573 7473 2074 6f20  ing requests to 
-00001040: 4f70 656e 4150 4920 616e 6420 6d61 6e61  OpenAPI and mana
-00001050: 6769 6e67 2074 6865 2063 6c69 656e 7420  ging the client 
-00001060: 7365 7373 696f 6e0a 2d20 6077 6562 736f  session.- `webso
-00001070: 636b 6574 7360 2c20 666f 7220 7365 7474  ckets`, for sett
-00001080: 696e 6720 7570 2061 2077 6562 736f 636b  ing up a websock
-00001090: 6574 2063 6f6e 6e65 6374 696f 6e20 746f  et connection to
-000010a0: 2053 6178 6f27 7320 7374 7265 616d 696e   Saxo's streamin
-000010b0: 6720 7365 7276 6963 650a 2d20 606c 6f67  g service.- `log
-000010c0: 7572 7560 2c20 746f 2068 616e 646c 6520  uru`, to handle 
-000010d0: 6c6f 6767 696e 670a 0a23 2320 4e6f 7465  logging..## Note
-000010e0: 730a 0a54 6865 2063 6c69 656e 7420 7375  s..The client su
-000010f0: 7070 6f72 7473 204f 4175 7468 2043 6f64  pports OAuth Cod
-00001100: 6520 666c 6f77 2061 6e64 2077 696c 6c20  e flow and will 
-00001110: 6175 746f 6d61 7469 6361 6c6c 7920 7370  automatically sp
-00001120: 696e 2075 7020 6120 7365 7276 6572 2074  in up a server t
-00001130: 6f20 6c69 7374 656e 2066 6f72 2074 6865  o listen for the
-00001140: 2072 6564 6972 6563 7420 6672 6f6d 2053   redirect from S
-00001150: 6178 6f20 5353 4f2e 2041 7420 6c65 6173  axo SSO. At leas
-00001160: 7420 3120 606c 6f63 616c 686f 7374 6020  t 1 `localhost` 
-00001170: 7265 6469 7265 6374 206e 6565 6473 2074  redirect needs t
-00001180: 6f20 6265 2064 6566 696e 6564 2069 6e20  o be defined in 
-00001190: 6170 706c 6963 6174 696f 6e20 636f 6e66  application conf
-000011a0: 6967 2066 6f72 2074 6869 7320 7075 7270  ig for this purp
-000011b0: 6f73 652e 0a0a 4279 2064 6566 6175 6c74  ose...By default
-000011c0: 2c20 7468 6520 636c 6965 6e74 2077 696c  , the client wil
-000011d0: 6c20 7573 6520 7468 6520 5f66 6972 7374  l use the _first
-000011e0: 2061 7661 696c 6162 6c65 206c 6f63 616c   available local
-000011f0: 686f 7374 2072 6564 6972 6563 745f 2074  host redirect_ t
-00001200: 6f20 7275 6e20 7468 6520 7365 7276 6572  o run the server
-00001210: 206f 6e20 2874 7970 6963 616c 6c79 206f   on (typically o
-00001220: 6e6c 7920 3120 6578 6973 7473 2069 6e20  nly 1 exists in 
-00001230: 7468 6520 636f 6e66 6967 292e 0a0a 5468  the config)...Th
-00001240: 6520 636c 6965 6e74 2076 616c 6964 6174  e client validat
-00001250: 6573 2072 6564 6972 6563 7420 7572 6c73  es redirect urls
-00001260: 2069 6e20 6170 706c 6963 6174 696f 6e20   in application 
-00001270: 636f 6e66 6967 2061 7574 6f6d 6174 6963  config automatic
-00001280: 616c 6c79 2e20 4f41 7574 6820 322e 3020  ally. OAuth 2.0 
-00001290: 636f 6465 2066 6c6f 7720 7265 7175 6972  code flow requir
-000012a0: 6573 2061 2066 6978 6564 2070 6f72 7420  es a fixed port 
-000012b0: 746f 2062 6520 7370 6563 6966 6965 6420  to be specified 
-000012c0: 6f6e 2074 6865 2072 6564 6972 6563 7420  on the redirect 
-000012d0: 7572 6c2e 2049 6e20 6361 7365 2074 6869  url. In case thi
-000012e0: 7320 6973 2069 6e63 6f72 7265 6374 6c79  s is incorrectly
-000012f0: 2063 6f6e 6669 6775 7265 642c 2061 6e20   configured, an 
-00001300: 6572 726f 7220 6d65 7373 6167 6520 7769  error message wi
-00001310: 6c6c 2067 7569 6465 2079 6f75 2074 6f20  ll guide you to 
-00001320: 656e 7375 7265 2061 7070 2063 6f6e 6669  ensure app confi
-00001330: 6720 6973 2063 6f72 7265 6374 2077 6974  g is correct wit
-00001340: 6820 4f70 656e 4150 493a 0a0a 6060 600a  h OpenAPI:..```.
-00001350: 6f6e 6520 6f72 206d 6f72 6520 7265 6469  one or more redi
-00001360: 7265 6374 2075 726c 7320 6861 7665 206e  rect urls have n
-00001370: 6f20 706f 7274 2063 6f6e 6669 6775 7265  o port configure
-00001380: 642c 2077 6869 6368 2069 7320 7265 7175  d, which is requ
-00001390: 6972 6564 2066 6f72 2067 7261 6e74 2074  ired for grant t
-000013a0: 7970 6520 2743 6f64 6527 202d 2065 6e73  ype 'Code' - ens
-000013b0: 7572 6520 6120 706f 7274 2069 7320 636f  ure a port is co
-000013c0: 6e66 6967 7572 6564 2069 6e20 7468 6520  nfigured in the 
-000013d0: 6170 7020 636f 6e66 6967 206f 626a 6563  app config objec
-000013e0: 7420 666f 7220 6561 6368 2075 726c 2028  t for each url (
-000013f0: 6578 616d 706c 653a 2068 7474 703a 2f2f  example: http://
-00001400: 6c6f 6361 6c68 6f73 743a 3233 3433 322f  localhost:23432/
-00001410: 7265 6469 7265 6374 290a 6060 600a       redirect).```.
+00000000: 6060 6074 6578 740a 2020 205f 5f5f 5f5f  ```text.   _____
+00000010: 2020 2020 2020 2020 205f 5f20 2020 5f5f           __   __
+00000020: 2020 5f5f 5f5f 2020 2020 2020 2020 2020    ____          
+00000030: 2020 2020 2020 2020 205f 5f5f 5f5f 2020           _____  
+00000040: 5f5f 2020 2020 205f 5f0a 2020 2f20 5f5f  __     __.  / __
+00000050: 5f5f 7c20 2020 2f5c 2020 205c 205c 202f  __|   /\   \ \ /
+00000060: 202f 202f 205f 5f20 5c20 2020 2020 2020   / / __ \       
+00000070: 2020 2020 202f 5c20 2020 7c20 205f 5f20       /\   |  __ 
+00000080: 5c20 5c20 5c20 2020 2f20 2f0a 207c 2028  \ \ \   / /. | (
+00000090: 5f5f 5f20 2020 202f 2020 5c20 2020 5c20  ___    /  \   \ 
+000000a0: 5620 2f20 7c20 7c20 207c 207c 2020 5f5f  V / | |  | |  __
+000000b0: 5f5f 2020 2020 2f20 205c 2020 7c20 7c5f  __    /  \  | |_
+000000c0: 5f29 207c 205c 205c 5f2f 202f 200a 2020  _) | \ \_/ / .  
+000000d0: 5c5f 5f5f 205c 2020 2f20 2f5c 205c 2020  \___ \  / /\ \  
+000000e0: 2029 2028 2020 7c20 7c20 207c 207c 207c   ) (  | |  | | |
+000000f0: 5f5f 5f5f 7c20 202f 202f 5c20 5c20 7c20  ____|  / /\ \ | 
+00000100: 205f 5f5f 2f20 2020 5c20 2020 2f20 200a   ___/   \   /  .
+00000110: 2020 5f5f 5f5f 2920 7c2f 205f 5f5f 5f20    ____) |/ ____ 
+00000120: 5c20 2f20 5f20 5c20 7c20 7c5f 5f7c 207c  \ / _ \ | |__| |
+00000130: 2020 2020 2020 2020 2f20 5f5f 5f5f 205c          / ____ \
+00000140: 7c20 7c20 2020 2020 2020 207c 207c 2020  | |        | |  
+00000150: 200a 207c 5f5f 5f5f 5f2f 2f5f 2f20 2020   . |_____//_/   
+00000160: 205c 2f2f 5f2f 205c 5f5c 205c 5f5f 5f5f   \//_/ \_\ \____
+00000170: 2f20 2020 2020 2020 202f 5f2f 2020 2020  /        /_/    
+00000180: 5c2f 7c5f 7c20 2020 2020 2020 207c 5f7c  \/|_|        |_|
+00000190: 2020 0a20 6060 600a 0a5b 215b 7079 7468    . ```..[![pyth
+000001a0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+000001b0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000001c0: 2f70 7974 686f 6e2d 332e 3725 3242 2d62  /python-3.7%2B-b
+000001d0: 6c75 6529 5d28 6874 7470 733a 2f2f 6769  lue)](https://gi
+000001e0: 7468 7562 2e63 6f6d 2f67 6964 7665 6e2f  thub.com/gidven/
+000001f0: 7361 786f 2d6f 7065 6e61 7069 2d63 6c69  saxo-openapi-cli
+00000200: 656e 742d 7079 7468 6f6e 290a 5b21 5b70  ent-python).[![p
+00000210: 7970 695d 2868 7474 7073 3a2f 2f69 6d67  ypi](https://img
+00000220: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000230: 2f76 2f73 6178 6f2d 6170 793f 7374 796c  /v/saxo-apy?styl
+00000240: 653d 666c 6174 2d73 7175 6172 6529 5d28  e=flat-square)](
+00000250: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000260: 2f70 726f 6a65 6374 2f73 6178 6f2d 6170  /project/saxo-ap
+00000270: 7929 0a5b 215b 6c69 6365 6e73 655d 2868  y).[![license](h
+00000280: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000290: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
+000002a0: 656e 7365 2f67 6964 7665 6e2f 7361 786f  ense/gidven/saxo
+000002b0: 2d6f 7065 6e61 7069 2d63 6c69 656e 742d  -openapi-client-
+000002c0: 7079 7468 6f6e 3f73 7479 6c65 3d66 6c61  python?style=fla
+000002d0: 742d 7371 7561 7265 295d 2868 7474 7073  t-square)](https
+000002e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6769  ://github.com/gi
+000002f0: 6476 656e 2f73 6178 6f2d 6f70 656e 6170  dven/saxo-openap
+00000300: 692d 636c 6965 6e74 2d70 7974 686f 6e2f  i-client-python/
+00000310: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00000320: 4529 0a0a 2320 5361 786f 2d41 5059 3a20  E)..# Saxo-APY: 
+00000330: 5079 7468 6f6e 2043 6c69 656e 7420 666f  Python Client fo
+00000340: 7220 5361 786f 2042 616e 6b20 4f70 656e  r Saxo Bank Open
+00000350: 4150 490a 0a2a 4120 6c69 6768 7477 6569  API..*A lightwei
+00000360: 6768 7420 5079 7468 6f6e 2063 6c69 656e  ght Python clien
+00000370: 7420 666f 7220 6861 7373 6c65 2d66 7265  t for hassle-fre
+00000380: 6520 7469 6e6b 6572 696e 6720 7769 7468  e tinkering with
+00000390: 2053 6178 6f20 4f70 656e 4150 492e 2a0a   Saxo OpenAPI.*.
+000003a0: 0a3e 204e 4f54 453a 2054 6869 7320 5079  .> NOTE: This Py
+000003b0: 7468 6f6e 2070 6163 6b61 6765 2077 6173  thon package was
+000003c0: 2063 7265 6174 6564 2062 7920 616e 2065   created by an e
+000003d0: 6e74 6875 7369 6173 7420 6173 2061 206c  nthusiast as a l
+000003e0: 6561 726e 696e 6720 7072 6f6a 6563 742e  earning project.
+000003f0: 204e 6f6e 6520 6f66 2074 6865 2063 6f6e   None of the con
+00000400: 7465 6e74 7320 696e 2074 6869 7320 7265  tents in this re
+00000410: 706f 7369 746f 7279 2061 7265 206d 6169  pository are mai
+00000420: 6e74 6169 6e65 6420 6279 2053 6178 6f20  ntained by Saxo 
+00000430: 4261 6e6b 2c20 616e 6420 5361 786f 2042  Bank, and Saxo B
+00000440: 616e 6b20 646f 6573 206e 6f74 2067 7561  ank does not gua
+00000450: 7261 6e74 6565 2063 6f72 7265 6374 6e65  rantee correctne
+00000460: 7373 206f 6620 7468 6520 7072 6f76 6964  ss of the provid
+00000470: 6564 2069 6d70 6c65 6d65 6e74 6174 696f  ed implementatio
+00000480: 6e2e 0a0a 2323 2041 7420 4669 7273 7420  n...## At First 
+00000490: 476c 616e 6365 0a0a 3e20 466f 7220 6d6f  Glance..> For mo
+000004a0: 7265 2069 6e73 7069 7261 7469 6f6e 2073  re inspiration s
+000004b0: 6565 205b 7468 6520 7361 6d70 6c65 735d  ee [the samples]
+000004c0: 282e 2f73 616d 706c 6573 2f29 210a 0a60  (./samples/)!..`
+000004d0: 6060 7079 7468 6f6e 0a66 726f 6d20 7361  ``python.from sa
+000004e0: 786f 5f61 7079 2069 6d70 6f72 7420 5361  xo_apy import Sa
+000004f0: 786f 4f70 656e 4150 4943 6c69 656e 740a  xoOpenAPIClient.
+00000500: 0a63 6c69 656e 7420 3d20 5361 786f 4f70  .client = SaxoOp
+00000510: 656e 4150 4943 6c69 656e 7428 2261 7070  enAPIClient("app
+00000520: 5f63 6f6e 6669 672e 6a73 6f6e 2229 0a63  _config.json").c
+00000530: 6c69 656e 742e 6c6f 6769 6e28 290a 0a6d  lient.login()..m
+00000540: 6520 3d20 636c 6965 6e74 2e67 6574 2822  e = client.get("
+00000550: 706f 7274 2f76 312f 7573 6572 732f 6d65  port/v1/users/me
+00000560: 2229 0a65 7572 7573 645f 7072 6963 6520  ").eurusd_price 
+00000570: 3d20 636c 6965 6e74 2e67 6574 2822 2f74  = client.get("/t
+00000580: 7261 6465 2f76 312f 696e 666f 7072 6963  rade/v1/infopric
+00000590: 6573 3f55 6963 3d32 3126 4173 7365 7454  es?Uic=21&AssetT
+000005a0: 7970 653d 4678 5370 6f74 2229 0a70 6f72  ype=FxSpot").por
+000005b0: 7466 6f6c 696f 5f6f 7264 6572 7320 3d20  tfolio_orders = 
+000005c0: 636c 6965 6e74 2e67 6574 2822 2f70 6f72  client.get("/por
+000005d0: 742f 7631 2f6f 7264 6572 732f 6d65 2229  t/v1/orders/me")
+000005e0: 0a0a 7072 696e 7428 6622 5765 6c63 6f6d  ..print(f"Welcom
+000005f0: 6520 7b6d 655b 2755 7365 7249 6427 5d7d  e {me['UserId']}
+00000600: 2122 290a 7072 696e 7428 6622 4555 5255  !").print(f"EURU
+00000610: 5344 2069 7320 7472 6164 696e 6720 6174  SD is trading at
+00000620: 3a20 7b65 7572 7573 645f 7072 6963 655b  : {eurusd_price[
+00000630: 2751 756f 7465 275d 5b27 4269 6427 5d7d  'Quote']['Bid']}
+00000640: 202f 207b 6575 7275 7364 5f70 7269 6365   / {eurusd_price
+00000650: 5b27 5175 6f74 6527 5d5b 2741 736b 275d  ['Quote']['Ask']
+00000660: 7d22 290a 7072 696e 7428 6622 596f 7520  }").print(f"You 
+00000670: 6861 7665 3a20 7b70 6f72 7466 6f6c 696f  have: {portfolio
+00000680: 5f6f 7264 6572 735b 275f 5f63 6f75 6e74  _orders['__count
+00000690: 275d 7d20 6f72 6465 7273 2069 6e20 796f  ']} orders in yo
+000006a0: 7572 2070 6f72 7466 6f6c 696f 2229 0a60  ur portfolio").`
+000006b0: 6060 0a0a 4f75 7470 7574 3a0a 0a60 6060  ``..Output:..```
+000006c0: 7465 7874 0af0 9f8c 9020 6f70 656e 696e  text..... openin
+000006d0: 6720 6c6f 6769 6e20 7061 6765 2069 6e20  g login page in 
+000006e0: 6272 6f77 7365 7220 2d20 7761 6974 696e  browser - waitin
+000006f0: 6720 666f 7220 7573 6572 2074 6f20 6175  g for user to au
+00000700: 7468 656e 7469 6361 7465 2e2e 2e20 f09f  thenticate... ..
+00000710: 9491 0af0 9f93 9e20 7265 6365 6976 6564  ....... received
+00000720: 2063 616c 6c62 6163 6b20 6672 6f6d 2053   callback from S
+00000730: 6178 6f20 5353 4f0a e29c 8520 6175 7468  axo SSO.... auth
+00000740: 6f72 697a 6174 696f 6e20 7375 6363 6565  orization succee
+00000750: 6465 6420 2d20 636f 6e6e 6563 7465 6420  ded - connected 
+00000760: 746f 2053 494d 2065 6e76 6972 6f6e 6d65  to SIM environme
+00000770: 6e74 2077 6974 6820 5752 4954 4520 2f20  nt with WRITE / 
+00000780: 5452 4144 4520 7065 726d 6973 7369 6f6e  TRADE permission
+00000790: 7320 2873 6573 7369 6f6e 2049 4420 6365  s (session ID ce
+000007a0: 6232 6265 3930 3935 6636 3465 6166 3965  b2be9095f64eaf9e
+000007b0: 3563 6165 6232 3164 3666 6337 3939 290a  5caeb21d6fc799).
+000007c0: 0a57 656c 636f 6d65 2031 3633 3731 3630  .Welcome 1637160
+000007d0: 3921 0a45 5552 5553 4420 6973 2074 7261  9!.EURUSD is tra
+000007e0: 6469 6e67 2061 743a 2031 2e30 3832 3239  ding at: 1.08229
+000007f0: 202f 2031 2e30 3832 3439 2028 4269 642f   / 1.08249 (Bid/
+00000800: 4173 6b29 0a59 6f75 2068 6176 653a 2031  Ask).You have: 1
+00000810: 3520 6f72 6465 7273 2069 6e20 796f 7572  5 orders in your
+00000820: 2070 6f72 7466 6f6c 696f 0a60 6060 0a0a   portfolio.```..
+00000830: 2323 2046 6561 7475 7265 730a 0a2d 205b  ## Features..- [
+00000840: 785d 2041 7574 6865 6e74 6963 6174 696f  x] Authenticatio
+00000850: 6e20 616e 6420 7365 7373 696f 6e20 6d61  n and session ma
+00000860: 6e61 6765 6d65 6e74 2077 6974 6820 5361  nagement with Sa
+00000870: 786f 2053 534f 0a20 202d 2053 7570 706f  xo SSO.  - Suppo
+00000880: 7274 7320 4f41 7574 6820 322e 3020 6043  rts OAuth 2.0 `C
+00000890: 6f64 6560 2067 7261 6e74 2074 7970 650a  ode` grant type.
+000008a0: 2020 2d20 576f 726b 7320 7365 616d 6c65    - Works seamle
+000008b0: 7373 6c79 2069 6e20 626f 7468 2060 5349  ssly in both `SI
+000008c0: 4d60 2061 6e64 2060 4c49 5645 6020 656e  M` and `LIVE` en
+000008d0: 7669 726f 6e6d 656e 7473 0a20 202d 2041  vironments.  - A
+000008e0: 7574 6f6d 6174 6564 2068 616e 646c 696e  utomated handlin
+000008f0: 6720 6f66 2063 616c 6c62 6163 6b20 6672  g of callback fr
+00000900: 6f6d 2053 534f 2028 6f70 7469 6f6e 616c  om SSO (optional
+00000910: 290a 2020 2d20 4865 6164 6c65 7373 2061  ).  - Headless a
+00000920: 7574 6865 6e74 6963 6174 696f 6e20 666f  uthentication fo
+00000930: 7220 6465 706c 6f79 6564 2061 7070 6c69  r deployed appli
+00000940: 6361 7469 6f6e 7320 286f 7074 696f 6e61  cations (optiona
+00000950: 6c29 0a20 202d 204b 6565 7020 7365 7373  l).  - Keep sess
+00000960: 696f 6e73 2061 6e64 2061 6374 6976 6520  ions and active 
+00000970: 7765 6273 6f63 6b65 7473 2063 6f6e 6e65  websockets conne
+00000980: 6374 696f 6e73 2061 6c69 7665 2062 7920  ctions alive by 
+00000990: 7265 6672 6573 6869 6e67 2061 6363 6573  refreshing acces
+000009a0: 7320 746f 6b65 6e73 2076 6961 2061 7379  s tokens via asy
+000009b0: 6e63 696f 0a2d 205b 785d 2052 6561 6420  ncio.- [x] Read 
+000009c0: 6f70 6572 6174 696f 6e73 2028 6047 4554  operations (`GET
+000009d0: 6020 7265 7175 6573 7473 290a 2d20 5b78  ` requests).- [x
+000009e0: 5d20 5772 6974 6520 6f70 6572 6174 696f  ] Write operatio
+000009f0: 6e73 2028 6050 4f53 5460 2c20 6050 5554  ns (`POST`, `PUT
+00000a00: 602c 2060 5041 5443 4860 2c20 6044 454c  `, `PATCH`, `DEL
+00000a10: 4554 4560 2072 6571 7565 7374 7329 0a2d  ETE` requests).-
+00000a20: 205b 785d 2053 7570 706f 7274 7320 6173   [x] Supports as
+00000a30: 796e 6320 7265 7175 6573 7473 2c20 7374  ync requests, st
+00000a40: 7265 616d 696e 672c 2061 6e64 2064 6563  reaming, and dec
+00000a50: 6f64 696e 6720 6f66 2073 7472 6561 6d69  oding of streami
+00000a60: 6e67 206d 6573 7361 6765 730a 2d20 5b78  ng messages.- [x
+00000a70: 5d20 4572 726f 7220 6861 6e64 6c69 6e67  ] Error handling
+00000a80: 2077 6974 6820 636f 6d70 7265 6865 6e73   with comprehens
+00000a90: 6976 6520 6578 6365 7074 696f 6e20 6d65  ive exception me
+00000aa0: 7373 6167 6573 0a0a 2323 2049 6e73 7461  ssages..## Insta
+00000ab0: 6c6c 6174 696f 6e0a 0a54 6869 7320 7079  llation..This py
+00000ac0: 7468 6f6e 2070 6163 6b61 6765 2069 7320  thon package is 
+00000ad0: 6176 6169 6c61 626c 6520 6f6e 2050 7950  available on PyP
+00000ae0: 492e 2049 6e73 7461 6c6c 2074 6865 2063  I. Install the c
+00000af0: 6c69 656e 7420 6279 2072 756e 6e69 6e67  lient by running
+00000b00: 2074 6865 2062 656c 6f77 2060 7069 7060   the below `pip`
+00000b10: 2063 6f6d 6d61 6e64 2069 6e20 796f 7572   command in your
+00000b20: 2074 6572 6d69 6e61 6c3a 0a0a 6070 6970   terminal:..`pip
+00000b30: 2069 6e73 7461 6c6c 2073 6178 6f2d 6170   install saxo-ap
+00000b40: 7960 0a0a 2323 2052 6571 7569 7265 6d65  y`..## Requireme
+00000b50: 6e74 730a 0a2d 2050 7974 686f 6e20 332e  nts..- Python 3.
+00000b60: 372b 0a2d 2041 6e20 4f70 656e 4150 4920  7+.- An OpenAPI 
+00000b70: 6170 706c 6963 6174 696f 6e20 7265 6769  application regi
+00000b80: 7374 6572 6564 205b 6f6e 2053 6178 6f20  stered [on Saxo 
+00000b90: 4261 6e6b 2773 2044 6576 656c 6f70 6572  Bank's Developer
+00000ba0: 2050 6f72 7461 6c5d 2868 7474 7073 3a2f   Portal](https:/
+00000bb0: 2f77 7777 2e64 6576 656c 6f70 6572 2e73  /www.developer.s
+00000bc0: 6178 6f2f 6f70 656e 6170 692f 6170 706d  axo/openapi/appm
+00000bd0: 616e 6167 656d 656e 7429 0a20 202d 205b  anagement).  - [
+00000be0: 4372 6561 7465 2061 2066 7265 6520 6465  Create a free de
+00000bf0: 7665 6c6f 7065 7220 6163 636f 756e 745d  veloper account]
+00000c00: 2868 7474 7073 3a2f 2f77 7777 2e64 6576  (https://www.dev
+00000c10: 656c 6f70 6572 2e73 6178 6f2f 6163 636f  eloper.saxo/acco
+00000c20: 756e 7473 2f73 696d 2f73 6967 6e75 7029  unts/sim/signup)
+00000c30: 2069 6620 796f 7520 646f 6e27 7420 6861   if you don't ha
+00000c40: 7665 206f 6e65 2061 6c72 6561 6479 2e0a  ve one already..
+00000c50: 2020 2d20 456e 7375 7265 2074 6865 2061    - Ensure the a
+00000c60: 7070 6c69 6361 7469 6f6e 2069 7320 7365  pplication is se
+00000c70: 7420 7570 2077 6974 6820 6047 7261 6e74  t up with `Grant
+00000c80: 2054 7970 653a 2043 6f64 6560 2061 7320   Type: Code` as 
+00000c90: 6175 7468 656e 7469 6361 7469 6f6e 2066  authentication f
+00000ca0: 6c6f 772e 0a20 202d 2041 7420 6c65 6173  low..  - At leas
+00000cb0: 7420 3120 6c6f 6361 6c68 6f73 7420 7265  t 1 localhost re
+00000cc0: 6469 7265 6374 206e 6565 6473 2074 6f20  direct needs to 
+00000cd0: 6265 2064 6566 696e 6564 2073 7563 6820  be defined such 
+00000ce0: 6173 2060 6874 7470 3a2f 2f6c 6f63 616c  as `http://local
+00000cf0: 686f 7374 3a31 3233 3231 2f72 6564 6972  host:12321/redir
+00000d00: 6563 7460 2028 666f 7220 6465 7665 6c6f  ect` (for develo
+00000d10: 706d 656e 742f 7465 7374 696e 6720 7075  pment/testing pu
+00000d20: 7270 6f73 6573 290a 2020 2d20 284f 7074  rposes).  - (Opt
+00000d30: 696f 6e61 6c29 2065 6e61 626c 6520 7472  ional) enable tr
+00000d40: 6164 696e 6720 7065 726d 6973 7369 6f6e  ading permission
+00000d50: 7320 666f 7220 7468 6520 6170 7020 6966  s for the app if
+00000d60: 2079 6f75 2077 616e 7420 746f 2027 7772   you want to 'wr
+00000d70: 6974 6527 2074 6f20 796f 7572 2061 6363  ite' to your acc
+00000d80: 6f75 6e74 2028 616e 6420 706c 6163 6520  ount (and place 
+00000d90: 6f72 6465 7273 290a 0a23 2320 4465 7065  orders)..## Depe
+00000da0: 6e64 656e 6369 6573 0a0a 5468 6973 2070  ndencies..This p
+00000db0: 6163 6b61 6765 2072 6571 7569 7265 7320  ackage requires 
+00000dc0: 3520 6465 7065 6e64 656e 6369 6573 3a0a  5 dependencies:.
+00000dd0: 0a2d 2060 7079 6461 6e74 6963 602c 2066  .- `pydantic`, f
+00000de0: 6f72 2070 6172 7369 6e67 2063 6f6e 6669  or parsing confi
+00000df0: 6720 616e 6420 4a53 4f4e 2072 6573 706f  g and JSON respo
+00000e00: 6e73 6573 200a 2d20 6046 6c61 736b 602c  nses .- `Flask`,
+00000e10: 2074 6f20 7275 6e20 6120 6c6f 6361 6c20   to run a local 
+00000e20: 7365 7276 6572 2061 6e64 2063 6174 6368  server and catch
+00000e30: 2074 6865 2063 616c 6c62 6163 6b20 6672   the callback fr
+00000e40: 6f6d 2053 6178 6f20 5353 4f0a 2d20 6068  om Saxo SSO.- `h
+00000e50: 7474 7078 602c 2066 6f72 2073 656e 6469  ttpx`, for sendi
+00000e60: 6e67 2072 6571 7565 7374 7320 746f 204f  ng requests to O
+00000e70: 7065 6e41 5049 2061 6e64 206d 616e 6167  penAPI and manag
+00000e80: 696e 6720 7468 6520 636c 6965 6e74 2073  ing the client s
+00000e90: 6573 7369 6f6e 0a2d 2060 7765 6273 6f63  ession.- `websoc
+00000ea0: 6b65 7473 602c 2066 6f72 2073 6574 7469  kets`, for setti
+00000eb0: 6e67 2075 7020 6120 7765 6273 6f63 6b65  ng up a websocke
+00000ec0: 7420 636f 6e6e 6563 7469 6f6e 2074 6f20  t connection to 
+00000ed0: 5361 786f 2773 2073 7472 6561 6d69 6e67  Saxo's streaming
+00000ee0: 2073 6572 7669 6365 0a2d 2060 6c6f 6775   service.- `logu
+00000ef0: 7275 602c 2074 6f20 6861 6e64 6c65 206c  ru`, to handle l
+00000f00: 6f67 6769 6e67 0a0a 2323 204e 6f74 6573  ogging..## Notes
+00000f10: 0a0a 5468 6520 636c 6965 6e74 2073 7570  ..The client sup
+00000f20: 706f 7274 7320 4f41 7574 6820 436f 6465  ports OAuth Code
+00000f30: 2066 6c6f 7720 616e 6420 7769 6c6c 2061   flow and will a
+00000f40: 7574 6f6d 6174 6963 616c 6c79 2073 7069  utomatically spi
+00000f50: 6e20 7570 2061 2073 6572 7665 7220 746f  n up a server to
+00000f60: 206c 6973 7465 6e20 666f 7220 7468 6520   listen for the 
+00000f70: 7265 6469 7265 6374 2066 726f 6d20 5361  redirect from Sa
+00000f80: 786f 2053 534f 2e20 4174 206c 6561 7374  xo SSO. At least
+00000f90: 2031 2060 6c6f 6361 6c68 6f73 7460 2072   1 `localhost` r
+00000fa0: 6564 6972 6563 7420 6e65 6564 7320 746f  edirect needs to
+00000fb0: 2062 6520 6465 6669 6e65 6420 696e 2061   be defined in a
+00000fc0: 7070 6c69 6361 7469 6f6e 2063 6f6e 6669  pplication confi
+00000fd0: 6720 666f 7220 7468 6973 2070 7572 706f  g for this purpo
+00000fe0: 7365 2e0a 0a42 7920 6465 6661 756c 742c  se...By default,
+00000ff0: 2074 6865 2063 6c69 656e 7420 7769 6c6c   the client will
+00001000: 2075 7365 2074 6865 202a 6669 7273 7420   use the *first 
+00001010: 6176 6169 6c61 626c 6520 6c6f 6361 6c68  available localh
+00001020: 6f73 7420 7265 6469 7265 6374 2a20 746f  ost redirect* to
+00001030: 2072 756e 2074 6865 2073 6572 7665 7220   run the server 
+00001040: 6f6e 2028 7479 7069 6361 6c6c 7920 6f6e  on (typically on
+00001050: 6c79 2031 2065 7869 7374 7320 696e 2074  ly 1 exists in t
+00001060: 6865 2063 6f6e 6669 6729 2e0a 0a54 6865  he config)...The
+00001070: 2063 6c69 656e 7420 7661 6c69 6461 7465   client validate
+00001080: 7320 7265 6469 7265 6374 2075 726c 7320  s redirect urls 
+00001090: 696e 2061 7070 6c69 6361 7469 6f6e 2063  in application c
+000010a0: 6f6e 6669 6720 6175 746f 6d61 7469 6361  onfig automatica
+000010b0: 6c6c 792e 204f 4175 7468 2032 2e30 2063  lly. OAuth 2.0 c
+000010c0: 6f64 6520 666c 6f77 2072 6571 7569 7265  ode flow require
+000010d0: 7320 6120 6669 7865 6420 706f 7274 2074  s a fixed port t
+000010e0: 6f20 6265 2073 7065 6369 6669 6564 206f  o be specified o
+000010f0: 6e20 7468 6520 7265 6469 7265 6374 2075  n the redirect u
+00001100: 726c 2e20 496e 2063 6173 6520 7468 6973  rl. In case this
+00001110: 2069 7320 696e 636f 7272 6563 746c 7920   is incorrectly 
+00001120: 636f 6e66 6967 7572 6564 2c20 616e 2065  configured, an e
+00001130: 7272 6f72 206d 6573 7361 6765 2077 696c  rror message wil
+00001140: 6c20 6775 6964 6520 796f 7520 746f 2065  l guide you to e
+00001150: 6e73 7572 6520 6170 7020 636f 6e66 6967  nsure app config
+00001160: 2069 7320 636f 7272 6563 7420 7769 7468   is correct with
+00001170: 204f 7065 6e41 5049 3a0a 0a60 6060 7465   OpenAPI:..```te
+00001180: 7874 0a6f 6e65 206f 7220 6d6f 7265 2072  xt.one or more r
+00001190: 6564 6972 6563 7420 7572 6c73 2068 6176  edirect urls hav
+000011a0: 6520 6e6f 2070 6f72 7420 636f 6e66 6967  e no port config
+000011b0: 7572 6564 2c20 7768 6963 6820 6973 2072  ured, which is r
+000011c0: 6571 7569 7265 6420 666f 7220 6772 616e  equired for gran
+000011d0: 7420 7479 7065 2027 436f 6465 2720 2d20  t type 'Code' - 
+000011e0: 656e 7375 7265 2061 2070 6f72 7420 6973  ensure a port is
+000011f0: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
+00001200: 6865 2061 7070 2063 6f6e 6669 6720 6f62  he app config ob
+00001210: 6a65 6374 2066 6f72 2065 6163 6820 7572  ject for each ur
+00001220: 6c20 2865 7861 6d70 6c65 3a20 6874 7470  l (example: http
+00001230: 3a2f 2f6c 6f63 616c 686f 7374 3a32 3334  ://localhost:234
+00001240: 3332 2f72 6564 6972 6563 7429 0a60 6060  32/redirect).```
+00001250: 0a                                       .
```

