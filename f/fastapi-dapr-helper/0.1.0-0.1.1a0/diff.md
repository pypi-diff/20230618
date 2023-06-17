# Comparing `tmp/fastapi-dapr-helper-0.1.0.tar.gz` & `tmp/fastapi-dapr-helper-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-dapr-helper-0.1.0.tar", max compression
+gzip compressed data, was "fastapi-dapr-helper-0.1.1a0.tar", max compression
```

## Comparing `fastapi-dapr-helper-0.1.0.tar` & `fastapi-dapr-helper-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-19 19:32:38.318982 fastapi-dapr-helper-0.1.0/fastapi_dapr_helper/__init__.py
--rw-r--r--   0        0        0     4344 2023-05-20 21:15:49.326755 fastapi-dapr-helper-0.1.0/fastapi_dapr_helper/pubsub.py
--rw-r--r--   0        0        0     1081 2023-05-19 19:08:45.571236 fastapi-dapr-helper-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      913 2023-05-20 20:39:34.380183 fastapi-dapr-helper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4710 2023-05-21 00:53:42.399530 fastapi-dapr-helper-0.1.0/README.md
--rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 fastapi-dapr-helper-0.1.0/setup.py
--rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 fastapi-dapr-helper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-06-17 22:10:38.336512 fastapi-dapr-helper-0.1.1a0/fastapi_dapr_helper/__init__.py
+-rw-r--r--   0        0        0     4611 2023-06-17 21:52:30.278025 fastapi-dapr-helper-0.1.1a0/fastapi_dapr_helper/pubsub.py
+-rw-r--r--   0        0        0     1081 2023-05-19 19:08:45.571236 fastapi-dapr-helper-0.1.1a0/LICENSE.md
+-rw-r--r--   0        0        0      920 2023-06-17 22:11:00.992116 fastapi-dapr-helper-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0     5389 2023-05-22 20:09:04.451094 fastapi-dapr-helper-0.1.1a0/README.md
+-rw-r--r--   0        0        0     6026 1970-01-01 00:00:00.000000 fastapi-dapr-helper-0.1.1a0/setup.py
+-rw-r--r--   0        0        0     5595 1970-01-01 00:00:00.000000 fastapi-dapr-helper-0.1.1a0/PKG-INFO
```

### Comparing `fastapi-dapr-helper-0.1.0/fastapi_dapr_helper/pubsub.py` & `fastapi-dapr-helper-0.1.1a0/fastapi_dapr_helper/pubsub.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,16 @@
             methods=["POST"],
             tags=tags,
             openapi_extra=openapi_extra,
             *args,
             **kwargs,
         )
 
+        return func
+
     return decorator
 
 
 # pylint: disable=R0903
 class DaprFastAPI:
     """
     Class to handle Dapr subscriptions and the FastAPI application.
@@ -97,18 +99,24 @@
         route_info = []
 
         for route in app.routes:
             if hasattr(route, "openapi_extra") is False:
                 logging.info(f"Skipping route {route.path} as it has no openapi_extra")
                 continue
 
+            if route.openapi_extra is None:
+                logging.info(f"Skipping route {route.path} as it has no openapi_extra")
+                continue
+
             if "dapr" not in route.openapi_extra:
                 logging.info(f"Skipping route {route.path} as it has no dapr info")
                 continue
 
+            logging.info(f"Extracting route {route.path} as it has dapr info")
+
             dapr_info = route.openapi_extra["dapr"]
             info = {
                 "pubsubname": dapr_info["pubsubname"],
                 "topic": dapr_info["topic"],
                 "route": route.path,
                 "metadata": dapr_info["metadata"],
             }
```

### Comparing `fastapi-dapr-helper-0.1.0/LICENSE.md` & `fastapi-dapr-helper-0.1.1a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi-dapr-helper-0.1.0/pyproject.toml` & `fastapi-dapr-helper-0.1.1a0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-dapr-helper"
-version = "0.1.0"
+version = "v0.1.1-alpha"
 description = ""
 authors = ["Clayton Black <CBlack@fanatics.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_dapr_helper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
```

### Comparing `fastapi-dapr-helper-0.1.0/README.md` & `fastapi-dapr-helper-0.1.1a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,151 +1,190 @@
-FastAPI Dapr Helper
-===================
-
-FastAPI Dapr Helper is a Python library that facilitates creating subscriptions to Dapr pubsub topics with FastAPI.
-
-This library introduces a decorator named `subscribe` which, in conjunction with a route generator, allows you to easily setup Dapr pubsub topic subscriptions within your FastAPI application. The package also provides a `DaprFastAPI` class to manage the subscriptions and generate a subscription route in your FastAPI application.
-
-## Installation
-
-### pip
-
-```bash
-pip install fastapi-dapr-helper
-```
-
-### Poetry
-
-```bash
-poetry add fastapi-dapr-helper
-```
-
-
-## Subscribe Decorator
-
-The `subscribe` decorator is designed to be used in combination with a route generator. It creates subscriptions to Dapr pubsub topics with FastAPI.
-
-```python
-from fastapi_dapr_helper.pubsub import subscribe
-
-@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")
-def test_endpoint():
-    return {"message": "test"}
-```
-
-In the above example, the `subscribe` decorator is used to define a pubsub subscription on the `test_endpoint` route.
-
-## DaprFastAPI Class
-
-The `DaprFastAPI` class is used to handle Dapr subscriptions and the FastAPI application.
-
-```python
-from fastapi_dapr_helper.pubsub import DaprFastAPI
-
-app = FastAPI()
-dapr = DaprFastAPI()
-
-dapr.generate_subscribe_route(app)
-```
-
-In this example, the `DaprFastAPI` class is used to handle subscriptions and to generate a `/dapr/subscribe` route in the FastAPI app.
-
-# Working Examples
-
-Here are some working examples of how to use FastAPI Dapr Helper in your project.
-
-## Working Example with FastAPI
-
-```python
-import uvicorn
-from fastapi import FastAPI
-from fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI
-
-app = FastAPI()
-dapr = DaprFastAPI()
-
-@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")
-def test_endpoint():
-    return {"message": "test"}
-
-dapr.generate_subscribe_route(app)
-
-uvicorn.run(app, host="0.0.0.0", port=8000)
-```
-
-## Working Example with APIRouter
-
-```python
-import uvicorn
-from fastapi import FastAPI, APIRouter
-from fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI
-
-app = FastAPI()
-router = APIRouter()
-dapr = DaprFastAPI()
-
-@subscribe(app=router, path="/test", pubsub="test_pubsub", topic="test_topic")
-def test_endpoint():
-    return {"message": "test"}
-
-app.include_router(router, prefix="/api")
-dapr.generate_subscribe_route(app)
-
-uvicorn.run(app, host="0.0.0.0", port=8000)
-```
-
-## Functionality Overview
-
-The main function of FastAPI Dapr Helper is to make it easier to create subscriptions to Dapr pubsub topics within FastAPI applications.
-It achieves this by using the decorator `subscribe` to embed subscription information into the OpenAPI schema for the route. 
-Then the `DaprFastAPI` class uses this information to generate a `/dapr/subscribe` route in the FastAPI app.
-
-The Dapr sidecar will call the `/dapr/subscribe` route to register the subscriptions.
-
-# Contributing
-
-I welcome contributions from the community!
-Follow the basic Githubflow PR process:
-
-1. Fork the repo on GitHub.
-2. Clone the project to your own machine.
-3. Commit changes to your own branch.
-4. Push your work back up to your fork.
-5. Submit a Pull Request so that your changes can be reviewed.
-
-## Style Guidelines
-
-### TLDR
-```bash
-black .
-```
-
-We follow stringent style guidelines to ensure the readability and maintainability of our code. 
-The primary tools used for enforcing these guidelines are `flake8` and `pylint`.
-
-Please see the pyproject.toml file for the specific configuration of these tools.
-
-## Testing
-
-Testing is a vital part of our development process.
-Not only must all tests pass before a change can be merged,
-but any new sections of code must also include corresponding tests.
-This allows us to ensure the stability and reliability of our codebase.
-
-If you are adding a new feature or fixing a bug,
-please include detailed tests to demonstrate the correctness of your changes.
-These tests will be automatically run when you submit your pull request.
-Any pull request that causes existing tests to fail cannot be merged.
-
-To facilitate the testing process, we use `pytest` as our primary testing framework.
-Please familiarize yourself with `pytest` to write effective tests for your contributions.
-
-Remember, good tests are as important as the code itself.
-They ensure the functionality of the code and prevent regressions.
-Thank you for helping maintain the quality of the codebase.
-
-# Conclusion
-Please ensure that your code conforms to our style guidelines before submitting a PR. 
-If you have any questions, feel free to open an issue for clarification.
-
-Thank you for your contribution!
-Happy coding!
+FastAPI Dapr Helper
+===================
+
+FastAPI Dapr Helper is a Python library that facilitates creating subscriptions to Dapr pubsub topics with FastAPI.
+
+This library introduces a decorator named `subscribe` which, in conjunction with a route generator, allows you to easily setup Dapr pubsub topic subscriptions within your FastAPI application. The package also provides a `DaprFastAPI` class to manage the subscriptions and generate a subscription route in your FastAPI application.
+
+## Installation
+
+### pip
+
+```bash
+pip install fastapi-dapr-helper
+```
+
+### Poetry
+
+```bash
+poetry add fastapi-dapr-helper
+```
+
+
+## Subscribe Decorator
+
+The `subscribe` decorator is designed to be used in combination with a route generator. It creates subscriptions to Dapr pubsub topics with FastAPI.
+
+```python
+from fastapi_dapr_helper.pubsub import subscribe
+
+@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")
+def test_endpoint():
+    return {"message": "test"}
+```
+
+In the above example, the `subscribe` decorator is used to define a pubsub subscription on the `test_endpoint` route.
+
+## DaprFastAPI Class
+
+The `DaprFastAPI` class is used to handle Dapr subscriptions and the FastAPI application.
+
+```python
+from fastapi_dapr_helper.pubsub import DaprFastAPI
+
+app = FastAPI()
+dapr = DaprFastAPI()
+
+dapr.generate_subscribe_route(app)
+```
+
+In this example, the `DaprFastAPI` class is used to handle subscriptions and to generate a `/dapr/subscribe` route in the FastAPI app.
+
+# Working Examples
+
+Here are some working examples of how to use FastAPI Dapr Helper in your project.
+
+## Working Example with FastAPI
+
+```python
+import uvicorn
+from fastapi import FastAPI
+from fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI
+
+app = FastAPI()
+dapr = DaprFastAPI()
+
+@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")
+def test_endpoint():
+    return {"message": "test"}
+
+dapr.generate_subscribe_route(app)
+
+uvicorn.run(app, host="0.0.0.0", port=8000)
+```
+
+### Output
+
+```bash
+curl -X 'GET' \
+  'http://localhost:8000/dapr/subscribe' \
+  -H 'accept: application/json'
+```
+
+```json
+[
+  {
+    "pubsubname": "test_pubsub",
+    "topic": "test_topic",
+    "route": "/test",
+    "metadata": {}
+  }
+]
+```
+
+## Working Example with APIRouter
+
+```python
+import uvicorn
+from fastapi import FastAPI, APIRouter
+from fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI
+
+app = FastAPI()
+router = APIRouter()
+dapr = DaprFastAPI()
+
+@subscribe(app=router, path="/test", pubsub="test_pubsub", topic="test_topic")
+def test_endpoint():
+    return {"message": "test"}
+
+app.include_router(router, prefix="/api")
+dapr.generate_subscribe_route(app)
+
+uvicorn.run(app, host="0.0.0.0", port=8000)
+```
+
+### Output
+
+```bash
+curl -X 'GET' \
+  'http://localhost:8000/dapr/subscribe' \
+  -H 'accept: application/json'
+```
+
+```json
+[
+  {
+    "pubsubname": "test_pubsub",
+    "topic": "test_topic",
+    "route": "/api/test",
+    "metadata": {}
+  }
+]
+```
+
+
+## Functionality Overview
+
+The main function of FastAPI Dapr Helper is to make it easier to create subscriptions to Dapr pubsub topics within FastAPI applications.
+It achieves this by using the decorator `subscribe` to embed subscription information into the OpenAPI schema for the route. 
+Then the `DaprFastAPI` class uses this information to generate a `/dapr/subscribe` route in the FastAPI app.
+
+The Dapr sidecar will call the `/dapr/subscribe` route to register the subscriptions.
+
+# Contributing
+
+I welcome contributions from the community!
+Follow the basic Githubflow PR process:
+
+1. Fork the repo on GitHub.
+2. Clone the project to your own machine.
+3. Commit changes to your own branch.
+4. Push your work back up to your fork.
+5. Submit a Pull Request so that your changes can be reviewed.
+
+## Style Guidelines
+
+### TLDR
+```bash
+black .
+```
+
+We follow stringent style guidelines to ensure the readability and maintainability of our code. 
+The primary tools used for enforcing these guidelines are `flake8` and `pylint`.
+
+Please see the pyproject.toml file for the specific configuration of these tools.
+
+## Testing
+
+Testing is a vital part of our development process.
+Not only must all tests pass before a change can be merged,
+but any new sections of code must also include corresponding tests.
+This allows us to ensure the stability and reliability of our codebase.
+
+If you are adding a new feature or fixing a bug,
+please include detailed tests to demonstrate the correctness of your changes.
+These tests will be automatically run when you submit your pull request.
+Any pull request that causes existing tests to fail cannot be merged.
+
+To facilitate the testing process, we use `pytest` as our primary testing framework.
+Please familiarize yourself with `pytest` to write effective tests for your contributions.
+
+Remember, good tests are as important as the code itself.
+They ensure the functionality of the code and prevent regressions.
+Thank you for helping maintain the quality of the codebase.
+
+# Conclusion
+Please ensure that your code conforms to our style guidelines before submitting a PR. 
+If you have any questions, feel free to open an issue for clarification.
+
+Thank you for your contribution!
+Happy coding!
```

### Comparing `fastapi-dapr-helper-0.1.0/setup.py` & `fastapi-dapr-helper-0.1.1a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.95.2,<0.96.0']
 
 setup_kwargs = {
     'name': 'fastapi-dapr-helper',
-    'version': '0.1.0',
+    'version': '0.1.1a0',
     'description': '',
-    'long_description': 'FastAPI Dapr Helper\n===================\n\nFastAPI Dapr Helper is a Python library that facilitates creating subscriptions to Dapr pubsub topics with FastAPI.\n\nThis library introduces a decorator named `subscribe` which, in conjunction with a route generator, allows you to easily setup Dapr pubsub topic subscriptions within your FastAPI application. The package also provides a `DaprFastAPI` class to manage the subscriptions and generate a subscription route in your FastAPI application.\n\n## Installation\n\n### pip\n\n```bash\npip install fastapi-dapr-helper\n```\n\n### Poetry\n\n```bash\npoetry add fastapi-dapr-helper\n```\n\n\n## Subscribe Decorator\n\nThe `subscribe` decorator is designed to be used in combination with a route generator. It creates subscriptions to Dapr pubsub topics with FastAPI.\n\n```python\nfrom fastapi_dapr_helper.pubsub import subscribe\n\n@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")\ndef test_endpoint():\n    return {"message": "test"}\n```\n\nIn the above example, the `subscribe` decorator is used to define a pubsub subscription on the `test_endpoint` route.\n\n## DaprFastAPI Class\n\nThe `DaprFastAPI` class is used to handle Dapr subscriptions and the FastAPI application.\n\n```python\nfrom fastapi_dapr_helper.pubsub import DaprFastAPI\n\napp = FastAPI()\ndapr = DaprFastAPI()\n\ndapr.generate_subscribe_route(app)\n```\n\nIn this example, the `DaprFastAPI` class is used to handle subscriptions and to generate a `/dapr/subscribe` route in the FastAPI app.\n\n# Working Examples\n\nHere are some working examples of how to use FastAPI Dapr Helper in your project.\n\n## Working Example with FastAPI\n\n```python\nimport uvicorn\nfrom fastapi import FastAPI\nfrom fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI\n\napp = FastAPI()\ndapr = DaprFastAPI()\n\n@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")\ndef test_endpoint():\n    return {"message": "test"}\n\ndapr.generate_subscribe_route(app)\n\nuvicorn.run(app, host="0.0.0.0", port=8000)\n```\n\n## Working Example with APIRouter\n\n```python\nimport uvicorn\nfrom fastapi import FastAPI, APIRouter\nfrom fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI\n\napp = FastAPI()\nrouter = APIRouter()\ndapr = DaprFastAPI()\n\n@subscribe(app=router, path="/test", pubsub="test_pubsub", topic="test_topic")\ndef test_endpoint():\n    return {"message": "test"}\n\napp.include_router(router, prefix="/api")\ndapr.generate_subscribe_route(app)\n\nuvicorn.run(app, host="0.0.0.0", port=8000)\n```\n\n## Functionality Overview\n\nThe main function of FastAPI Dapr Helper is to make it easier to create subscriptions to Dapr pubsub topics within FastAPI applications.\nIt achieves this by using the decorator `subscribe` to embed subscription information into the OpenAPI schema for the route. \nThen the `DaprFastAPI` class uses this information to generate a `/dapr/subscribe` route in the FastAPI app.\n\nThe Dapr sidecar will call the `/dapr/subscribe` route to register the subscriptions.\n\n# Contributing\n\nI welcome contributions from the community!\nFollow the basic Githubflow PR process:\n\n1. Fork the repo on GitHub.\n2. Clone the project to your own machine.\n3. Commit changes to your own branch.\n4. Push your work back up to your fork.\n5. Submit a Pull Request so that your changes can be reviewed.\n\n## Style Guidelines\n\n### TLDR\n```bash\nblack .\n```\n\nWe follow stringent style guidelines to ensure the readability and maintainability of our code. \nThe primary tools used for enforcing these guidelines are `flake8` and `pylint`.\n\nPlease see the pyproject.toml file for the specific configuration of these tools.\n\n## Testing\n\nTesting is a vital part of our development process.\nNot only must all tests pass before a change can be merged,\nbut any new sections of code must also include corresponding tests.\nThis allows us to ensure the stability and reliability of our codebase.\n\nIf you are adding a new feature or fixing a bug,\nplease include detailed tests to demonstrate the correctness of your changes.\nThese tests will be automatically run when you submit your pull request.\nAny pull request that causes existing tests to fail cannot be merged.\n\nTo facilitate the testing process, we use `pytest` as our primary testing framework.\nPlease familiarize yourself with `pytest` to write effective tests for your contributions.\n\nRemember, good tests are as important as the code itself.\nThey ensure the functionality of the code and prevent regressions.\nThank you for helping maintain the quality of the codebase.\n\n# Conclusion\nPlease ensure that your code conforms to our style guidelines before submitting a PR. \nIf you have any questions, feel free to open an issue for clarification.\n\nThank you for your contribution!\nHappy coding!\n',
+    'long_description': 'FastAPI Dapr Helper\n===================\n\nFastAPI Dapr Helper is a Python library that facilitates creating subscriptions to Dapr pubsub topics with FastAPI.\n\nThis library introduces a decorator named `subscribe` which, in conjunction with a route generator, allows you to easily setup Dapr pubsub topic subscriptions within your FastAPI application. The package also provides a `DaprFastAPI` class to manage the subscriptions and generate a subscription route in your FastAPI application.\n\n## Installation\n\n### pip\n\n```bash\npip install fastapi-dapr-helper\n```\n\n### Poetry\n\n```bash\npoetry add fastapi-dapr-helper\n```\n\n\n## Subscribe Decorator\n\nThe `subscribe` decorator is designed to be used in combination with a route generator. It creates subscriptions to Dapr pubsub topics with FastAPI.\n\n```python\nfrom fastapi_dapr_helper.pubsub import subscribe\n\n@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")\ndef test_endpoint():\n    return {"message": "test"}\n```\n\nIn the above example, the `subscribe` decorator is used to define a pubsub subscription on the `test_endpoint` route.\n\n## DaprFastAPI Class\n\nThe `DaprFastAPI` class is used to handle Dapr subscriptions and the FastAPI application.\n\n```python\nfrom fastapi_dapr_helper.pubsub import DaprFastAPI\n\napp = FastAPI()\ndapr = DaprFastAPI()\n\ndapr.generate_subscribe_route(app)\n```\n\nIn this example, the `DaprFastAPI` class is used to handle subscriptions and to generate a `/dapr/subscribe` route in the FastAPI app.\n\n# Working Examples\n\nHere are some working examples of how to use FastAPI Dapr Helper in your project.\n\n## Working Example with FastAPI\n\n```python\nimport uvicorn\nfrom fastapi import FastAPI\nfrom fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI\n\napp = FastAPI()\ndapr = DaprFastAPI()\n\n@subscribe(app=app, path="/test", pubsub="test_pubsub", topic="test_topic")\ndef test_endpoint():\n    return {"message": "test"}\n\ndapr.generate_subscribe_route(app)\n\nuvicorn.run(app, host="0.0.0.0", port=8000)\n```\n\n### Output\n\n```bash\ncurl -X \'GET\' \\\n  \'http://localhost:8000/dapr/subscribe\' \\\n  -H \'accept: application/json\'\n```\n\n```json\n[\n  {\n    "pubsubname": "test_pubsub",\n    "topic": "test_topic",\n    "route": "/test",\n    "metadata": {}\n  }\n]\n```\n\n## Working Example with APIRouter\n\n```python\nimport uvicorn\nfrom fastapi import FastAPI, APIRouter\nfrom fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI\n\napp = FastAPI()\nrouter = APIRouter()\ndapr = DaprFastAPI()\n\n@subscribe(app=router, path="/test", pubsub="test_pubsub", topic="test_topic")\ndef test_endpoint():\n    return {"message": "test"}\n\napp.include_router(router, prefix="/api")\ndapr.generate_subscribe_route(app)\n\nuvicorn.run(app, host="0.0.0.0", port=8000)\n```\n\n### Output\n\n```bash\ncurl -X \'GET\' \\\n  \'http://localhost:8000/dapr/subscribe\' \\\n  -H \'accept: application/json\'\n```\n\n```json\n[\n  {\n    "pubsubname": "test_pubsub",\n    "topic": "test_topic",\n    "route": "/api/test",\n    "metadata": {}\n  }\n]\n```\n\n\n## Functionality Overview\n\nThe main function of FastAPI Dapr Helper is to make it easier to create subscriptions to Dapr pubsub topics within FastAPI applications.\nIt achieves this by using the decorator `subscribe` to embed subscription information into the OpenAPI schema for the route. \nThen the `DaprFastAPI` class uses this information to generate a `/dapr/subscribe` route in the FastAPI app.\n\nThe Dapr sidecar will call the `/dapr/subscribe` route to register the subscriptions.\n\n# Contributing\n\nI welcome contributions from the community!\nFollow the basic Githubflow PR process:\n\n1. Fork the repo on GitHub.\n2. Clone the project to your own machine.\n3. Commit changes to your own branch.\n4. Push your work back up to your fork.\n5. Submit a Pull Request so that your changes can be reviewed.\n\n## Style Guidelines\n\n### TLDR\n```bash\nblack .\n```\n\nWe follow stringent style guidelines to ensure the readability and maintainability of our code. \nThe primary tools used for enforcing these guidelines are `flake8` and `pylint`.\n\nPlease see the pyproject.toml file for the specific configuration of these tools.\n\n## Testing\n\nTesting is a vital part of our development process.\nNot only must all tests pass before a change can be merged,\nbut any new sections of code must also include corresponding tests.\nThis allows us to ensure the stability and reliability of our codebase.\n\nIf you are adding a new feature or fixing a bug,\nplease include detailed tests to demonstrate the correctness of your changes.\nThese tests will be automatically run when you submit your pull request.\nAny pull request that causes existing tests to fail cannot be merged.\n\nTo facilitate the testing process, we use `pytest` as our primary testing framework.\nPlease familiarize yourself with `pytest` to write effective tests for your contributions.\n\nRemember, good tests are as important as the code itself.\nThey ensure the functionality of the code and prevent regressions.\nThank you for helping maintain the quality of the codebase.\n\n# Conclusion\nPlease ensure that your code conforms to our style guidelines before submitting a PR. \nIf you have any questions, feel free to open an issue for clarification.\n\nThank you for your contribution!\nHappy coding!\n',
     'author': 'Clayton Black',
     'author_email': 'CBlack@fanatics.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi-dapr-helper-0.1.0/PKG-INFO` & `fastapi-dapr-helper-0.1.1a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-dapr-helper
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: 
 Author: Clayton Black
 Author-email: CBlack@fanatics.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -81,14 +81,33 @@
     return {"message": "test"}
 
 dapr.generate_subscribe_route(app)
 
 uvicorn.run(app, host="0.0.0.0", port=8000)
 ```
 
+### Output
+
+```bash
+curl -X 'GET' \
+  'http://localhost:8000/dapr/subscribe' \
+  -H 'accept: application/json'
+```
+
+```json
+[
+  {
+    "pubsubname": "test_pubsub",
+    "topic": "test_topic",
+    "route": "/test",
+    "metadata": {}
+  }
+]
+```
+
 ## Working Example with APIRouter
 
 ```python
 import uvicorn
 from fastapi import FastAPI, APIRouter
 from fastapi_dapr_helper.pubsub import subscribe, DaprFastAPI
 
@@ -102,14 +121,34 @@
 
 app.include_router(router, prefix="/api")
 dapr.generate_subscribe_route(app)
 
 uvicorn.run(app, host="0.0.0.0", port=8000)
 ```
 
+### Output
+
+```bash
+curl -X 'GET' \
+  'http://localhost:8000/dapr/subscribe' \
+  -H 'accept: application/json'
+```
+
+```json
+[
+  {
+    "pubsubname": "test_pubsub",
+    "topic": "test_topic",
+    "route": "/api/test",
+    "metadata": {}
+  }
+]
+```
+
+
 ## Functionality Overview
 
 The main function of FastAPI Dapr Helper is to make it easier to create subscriptions to Dapr pubsub topics within FastAPI applications.
 It achieves this by using the decorator `subscribe` to embed subscription information into the OpenAPI schema for the route. 
 Then the `DaprFastAPI` class uses this information to generate a `/dapr/subscribe` route in the FastAPI app.
 
 The Dapr sidecar will call the `/dapr/subscribe` route to register the subscriptions.
```

