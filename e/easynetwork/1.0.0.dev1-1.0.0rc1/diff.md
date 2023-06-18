# Comparing `tmp/easynetwork-1.0.0.dev1.tar.gz` & `tmp/easynetwork-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Mar 19 21:02:58 2023, max compression
+gzip compressed data, last modified: Sun Jun 18 16:42:45 2023, max compression
```

## Comparing `easynetwork-1.0.0.dev1.tar` & `easynetwork-1.0.0rc1.tar`

### file list

```diff
@@ -1,92 +1,178 @@
--rw-r--r--   0        0        0      847 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/.flake8
--rw-r--r--   0        0        0     2067 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    95174 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/pdm.lock
--rw-r--r--   0        0        0     1891 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tox.ini
--rw-r--r--   0        0        0     1260 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/.vscode/settings.example.json
--rw-r--r--   0        0        0      639 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/__init__.py
--rw-r--r--   0        0        0     1865 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/converter.py
--rw-r--r--   0        0        0     1995 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/exceptions.py
--rw-r--r--   0        0        0     5116 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/protocol.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/py.typed
--rw-r--r--   0        0        0      335 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/client/__init__.py
--rw-r--r--   0        0        0     2063 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/client/abc.py
--rw-r--r--   0        0        0     8922 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/client/tcp.py
--rw-r--r--   0        0        0    12528 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/client/udp.py
--rw-r--r--   0        0        0     1008 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/__init__.py
--rw-r--r--   0        0        0     2316 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/abc.py
--rw-r--r--   0        0        0     7408 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/base_stream.py
--rw-r--r--   0        0        0     2897 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/cbor.py
--rw-r--r--   0        0        0     7615 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/json.py
--rw-r--r--   0        0        0     3047 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/pickle.py
--rw-r--r--   0        0        0     4927 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/struct.py
--rw-r--r--   0        0        0      422 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/wrapper/__init__.py
--rw-r--r--   0        0        0     2419 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/wrapper/base64.py
--rw-r--r--   0        0        0     5930 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/wrapper/compressor.py
--rw-r--r--   0        0        0     2207 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/serializers/wrapper/encryptor.py
--rw-r--r--   0        0        0      348 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/server/__init__.py
--rw-r--r--   0        0        0     1602 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/server/abc.py
--rw-r--r--   0        0        0    31183 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/server/tcp.py
--rw-r--r--   0        0        0    16766 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/server/udp.py
--rw-r--r--   0        0        0      195 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/tools/__init__.py
--rw-r--r--   0        0        0     1362 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/tools/_utils.py
--rw-r--r--   0        0        0     5309 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/tools/socket.py
--rw-r--r--   0        0        0     5379 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/src/easynetwork/tools/stream.py
--rw-r--r--   0        0        0      131 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/__init__.py
--rw-r--r--   0        0        0      581 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/conftest.py
--rw-r--r--   0        0        0     1113 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/tools.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/__init__.py
--rw-r--r--   0        0        0      355 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/conftest.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/__init__.py
--rw-r--r--   0        0        0     2858 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/conftest.py
--rw-r--r--   0        0        0     1781 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/serializer.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_client/__init__.py
--rw-r--r--   0        0        0     9014 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_client/test_tcp.py
--rw-r--r--   0        0        0    15985 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_server/__init__.py
--rw-r--r--   0        0        0    12669 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_server/test_tcp.py
--rw-r--r--   0        0        0     8416 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_server/test_udp.py
--rw-r--r--   0        0        0      130 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/__init__.py
--rw-r--r--   0        0        0     9234 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/base.py
--rw-r--r--   0        0        0      424 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/conftest.py
--rw-r--r--   0        0        0     5964 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_base64.py
--rw-r--r--   0        0        0     2171 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_cbor.py
--rw-r--r--   0        0        0     4033 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_compressors.py
--rw-r--r--   0        0        0     3504 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_encryptor.py
--rw-r--r--   0        0        0     2277 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_json.py
--rw-r--r--   0        0        0     2711 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_namedtuple.py
--rw-r--r--   0        0        0     4024 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_pickle.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/samples/__init__.py
--rw-r--r--   0        0        0    10664 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/samples/json.py
--rw-r--r--   0        0        0     2356 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/samples/pickle.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/other_test/__init__.py
--rw-r--r--   0        0        0     4820 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/other_test/test_import.py
--rw-r--r--   0        0        0     2856 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/scripts/server_test.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/__init__.py
--rw-r--r--   0        0        0      606 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/_utils.py
--rw-r--r--   0        0        0     4499 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/conftest.py
--rw-r--r--   0        0        0     2060 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_converter.py
--rw-r--r--   0        0        0    15746 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_protocol.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_client/__init__.py
--rw-r--r--   0        0        0     1346 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_client/base.py
--rw-r--r--   0        0        0     3014 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_client/test_abc.py
--rw-r--r--   0        0        0    41322 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_client/test_tcp.py
--rw-r--r--   0        0        0    43524 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_client/test_udp.py
--rw-r--r--   0        0        0      130 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/__init__.py
--rw-r--r--   0        0        0      612 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/base.py
--rw-r--r--   0        0        0      355 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/conftest.py
--rw-r--r--   0        0        0    31004 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_abc.py
--rw-r--r--   0        0        0     3514 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_base64.py
--rw-r--r--   0        0        0     5909 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_cbor.py
--rw-r--r--   0        0        0    19718 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_compressor.py
--rw-r--r--   0        0        0     4264 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_encryptor.py
--rw-r--r--   0        0        0    14534 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_json.py
--rw-r--r--   0        0        0     8374 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_pickle.py
--rw-r--r--   0        0        0    14061 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_struct.py
--rw-r--r--   0        0        0        0 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_tools/__init__.py
--rw-r--r--   0        0        0     5823 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_tools/test_socket.py
--rw-r--r--   0        0        0    14620 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/tests/unit_test/test_tools/test_stream.py
--rw-r--r--   0        0        0     1913 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/.gitignore
--rw-r--r--   0        0        0     1097 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/LICENSE
--rw-r--r--   0        0        0       55 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/README.md
--rw-r--r--   0        0        0     4437 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      953 2023-03-19 21:02:58.000000 easynetwork-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      847 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.flake8
+-rw-r--r--   0        0        0     1939 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   123771 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/pdm.lock
+-rw-r--r--   0        0        0     3673 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tox.ini
+-rw-r--r--   0        0        0     1260 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.vscode/settings.example.json
+-rw-r--r--   0        0        0      637 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/converter.py
+-rw-r--r--   0        0        0     2120 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/exceptions.py
+-rw-r--r--   0        0        0     5291 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/protocol.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/py.typed
+-rw-r--r--   0        0        0      206 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/__init__.py
+-rw-r--r--   0        0        0    11364 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/abc.py
+-rw-r--r--   0        0        0     6289 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/factory.py
+-rw-r--r--   0        0        0     2002 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/futures.py
+-rw-r--r--   0        0        0      708 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/sniffio.py
+-rw-r--r--   0        0        0     1918 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/backend/tasks.py
+-rw-r--r--   0        0        0      368 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/__init__.py
+-rw-r--r--   0        0        0     2407 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/abc.py
+-rw-r--r--   0        0        0    13391 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/tcp.py
+-rw-r--r--   0        0        0    13060 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/client/udp.py
+-rw-r--r--   0        0        0      585 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/__init__.py
+-rw-r--r--   0        0        0     1428 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/abc.py
+-rw-r--r--   0        0        0     2798 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/handler.py
+-rw-r--r--   0        0        0     8043 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/standalone.py
+-rw-r--r--   0        0        0    22757 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/tcp.py
+-rw-r--r--   0        0        0    18880 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_async/server/udp.py
+-rw-r--r--   0        0        0      205 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/__init__.py
+-rw-r--r--   0        0        0     2146 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/abc.py
+-rw-r--r--   0        0        0    14942 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/tcp.py
+-rw-r--r--   0        0        0    12195 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/udp.py
+-rw-r--r--   0        0        0     1164 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/__init__.py
+-rw-r--r--   0        0        0     2264 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/abc.py
+-rw-r--r--   0        0        0     7602 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/base_stream.py
+-rw-r--r--   0        0        0     2897 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/cbor.py
+-rw-r--r--   0        0        0     8165 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/json.py
+-rw-r--r--   0        0        0     2313 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/line.py
+-rw-r--r--   0        0        0     3794 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/msgpack.py
+-rw-r--r--   0        0        0     3297 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/pickle.py
+-rw-r--r--   0        0        0     5084 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/struct.py
+-rw-r--r--   0        0        0      422 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/__init__.py
+-rw-r--r--   0        0        0     2881 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/base64.py
+-rw-r--r--   0        0        0     6344 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/compressor.py
+-rw-r--r--   0        0        0     2246 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/encryptor.py
+-rw-r--r--   0        0        0      195 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/__init__.py
+-rw-r--r--   0        0        0    10880 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/_utils.py
+-rw-r--r--   0        0        0     1196 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/lock.py
+-rw-r--r--   0        0        0     7948 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/socket.py
+-rw-r--r--   0        0        0     5533 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork/tools/stream.py
+-rw-r--r--   0        0        0      288 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/__init__.py
+-rw-r--r--   0        0        0     6217 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/_utils.py
+-rw-r--r--   0        0        0    17671 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/backend.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/py.typed
+-rw-r--r--   0        0        0     5395 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/socket.py
+-rw-r--r--   0        0        0     4696 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/tasks.py
+-rw-r--r--   0        0        0     4186 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/threads.py
+-rw-r--r--   0        0        0      208 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/__init__.py
+-rw-r--r--   0        0        0     8604 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/endpoint.py
+-rw-r--r--   0        0        0     3694 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/datagram/socket.py
+-rw-r--r--   0        0        0      208 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/__init__.py
+-rw-r--r--   0        0        0     5423 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/listener.py
+-rw-r--r--   0        0        0     4113 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/src/easynetwork_asyncio/stream/socket.py
+-rw-r--r--   0        0        0      131 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     1113 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/tools.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/__init__.py
+-rw-r--r--   0        0        0    19654 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_asyncio_backend.py
+-rw-r--r--   0        0        0     1288 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_backend_factory.py
+-rw-r--r--   0        0        0     3201 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_futures.py
+-rw-r--r--   0        0        0     2424 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_async/test_backend/test_tasks.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/__init__.py
+-rw-r--r--   0        0        0     4173 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/conftest.py
+-rw-r--r--   0        0        0     1781 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/serializer.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/_utils.py
+-rw-r--r--   0        0        0      527 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/__init__.py
+-rw-r--r--   0        0        0    19354 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/test_tcp.py
+-rw-r--r--   0        0        0    31112 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/base.py
+-rw-r--r--   0        0        0     4666 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_standalone.py
+-rw-r--r--   0        0        0    31268 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_tcp.py
+-rw-r--r--   0        0        0    18286 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_async/test_server/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/__init__.py
+-rw-r--r--   0        0        0     1279 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/__init__.py
+-rw-r--r--   0        0        0    12790 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py
+-rw-r--r--   0        0        0    16039 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_udp.py
+-rw-r--r--   0        0        0      130 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/__init__.py
+-rw-r--r--   0        0        0     9118 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/base.py
+-rw-r--r--   0        0        0      424 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/conftest.py
+-rw-r--r--   0        0        0     6240 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_base64.py
+-rw-r--r--   0        0        0     2233 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_cbor.py
+-rw-r--r--   0        0        0     4069 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_compressors.py
+-rw-r--r--   0        0        0     3572 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_encryptor.py
+-rw-r--r--   0        0        0     2639 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_json.py
+-rw-r--r--   0        0        0     3440 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_line.py
+-rw-r--r--   0        0        0     1926 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_msgpack.py
+-rw-r--r--   0        0        0     2747 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_namedtuple.py
+-rw-r--r--   0        0        0     3609 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_pickle.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/__init__.py
+-rw-r--r--   0        0        0    10664 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/json.py
+-rw-r--r--   0        0        0     2356 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/pickle.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/other_test/__init__.py
+-rw-r--r--   0        0        0     4925 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/other_test/test_import.py
+-rw-r--r--   0        0        0      578 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/other_test/test_project_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/asyncio_event_loop.py
+-rw-r--r--   0        0        0     1792 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/extra_features.py
+-rw-r--r--   0        0        0      620 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/pytest_plugins/session_exit_code.py
+-rw-r--r--   0        0        0     2671 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/scripts/async_server_test.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/__init__.py
+-rw-r--r--   0        0        0     1795 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/_utils.py
+-rw-r--r--   0        0        0     1808 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/base.py
+-rw-r--r--   0        0        0     5555 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/conftest.py
+-rw-r--r--   0        0        0     5098 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_converter.py
+-rw-r--r--   0        0        0    15717 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_protocol.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/__init__.py
+-rw-r--r--   0        0        0     1114 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/base.py
+-rw-r--r--   0        0        0     2340 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py
+-rw-r--r--   0        0        0    17863 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/test_backend.py
+-rw-r--r--   0        0        0     5327 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_backend/test_futures.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/base.py
+-rw-r--r--   0        0        0     2682 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_abc.py
+-rw-r--r--   0        0        0    51599 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_tcp.py
+-rw-r--r--   0        0        0    41442 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_server/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_server/test_handler.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/__init__.py
+-rw-r--r--   0        0        0     1679 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/conftest.py
+-rw-r--r--   0        0        0    46304 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_backend.py
+-rw-r--r--   0        0        0    32981 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py
+-rw-r--r--   0        0        0    14186 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_socket.py
+-rw-r--r--   0        0        0    27018 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_stream.py
+-rw-r--r--   0        0        0     9534 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py
+-rw-r--r--   0        0        0     4898 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_threads.py
+-rw-r--r--   0        0        0    30962 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_async/test_asyncio_backend/test_utils.py
+-rw-r--r--   0        0        0      130 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/__init__.py
+-rw-r--r--   0        0        0      612 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/base.py
+-rw-r--r--   0        0        0      355 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/conftest.py
+-rw-r--r--   0        0        0    30904 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_abc.py
+-rw-r--r--   0        0        0     3514 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_base64.py
+-rw-r--r--   0        0        0     5880 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_cbor.py
+-rw-r--r--   0        0        0    20502 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_compressor.py
+-rw-r--r--   0        0        0     4351 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_encryptor.py
+-rw-r--r--   0        0        0    15194 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_json.py
+-rw-r--r--   0        0        0     7216 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_line.py
+-rw-r--r--   0        0        0     7146 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_msgpack.py
+-rw-r--r--   0        0        0     9953 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_pickle.py
+-rw-r--r--   0        0        0    16647 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_struct.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/__init__.py
+-rw-r--r--   0        0        0      526 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/base.py
+-rw-r--r--   0        0        0     1019 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/conftest.py
+-rw-r--r--   0        0        0     3294 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_abc.py
+-rw-r--r--   0        0        0    67599 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_tcp.py
+-rw-r--r--   0        0        0    44378 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/__init__.py
+-rw-r--r--   0        0        0     2153 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_lock.py
+-rw-r--r--   0        0        0     7763 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_socket.py
+-rw-r--r--   0        0        0    14621 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_stream.py
+-rw-r--r--   0        0        0    22406 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_utils.py
+-rw-r--r--   0        0        0     1915 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/.gitignore
+-rw-r--r--   0        0        0     1097 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0       55 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     5202 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1429 2023-06-18 16:42:45.000000 easynetwork-1.0.0rc1/PKG-INFO
```

### Comparing `easynetwork-1.0.0.dev1/.flake8` & `easynetwork-1.0.0rc1/.flake8`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/.pre-commit-config.yaml` & `easynetwork-1.0.0rc1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 default_language_version:
-  python: python3.10
+  python: python3.11
 minimum_pre_commit_version: '2.20.0'
 
 ci:
   skip: [mypy]
 
 repos:
   - repo: local
     hooks:
       - id: mypy
         name: mypy (project)
-        entry: tox run -q -e mypy-lite,mypy-full
+        entry: tox run -q -e mypy-full
         language: system
         files: ^(src/)
         types_or: [python, pyi]
         require_serial: true
         pass_filenames: false
       - id: mypy
         name: mypy (tests)
@@ -24,43 +24,39 @@
         types_or: [python, pyi]
         require_serial: true
         pass_filenames: false
   - repo: https://github.com/PyCQA/isort
     rev: '5.12.0'
     hooks:
       - id: isort
-        exclude: ^(\.github)/
         args: ['--filter-files', '--settings-file', 'pyproject.toml']
   - repo: https://github.com/psf/black
-    rev: '23.1.0'
+    rev: '23.3.0'
     hooks:
       - id: black
-        exclude: ^(\.github)/
         args: ['--config', 'pyproject.toml']
   - repo: https://github.com/PyCQA/flake8
     rev: '6.0.0'
     hooks:
       - id: flake8
-        exclude: ^(\.github)/
         args: ['--config', '.flake8']
         types: []  # Overwrite with empty in order to fallback to types_or
         types_or: [python, pyi]
         additional_dependencies: [
           'flake8-pyi>=22.11.0',
-          'flake8-dunder-all @ git+https://github.com/francis-clairicia/flake8-dunder-all.git@main'
+          'flake8-dunder-all @ git+https://github.com/francis-clairicia/flake8-dunder-all.git@v0.1.0'
         ]
   - repo: https://github.com/aio-libs/sort-all
     rev: 'v1.2.0'
     hooks:
       - id: sort-all
-        exclude: ^(\.github)/
         types: []  # Overwrite with empty in order to fallback to types_or
         types_or: [python, pyi]
   - repo: https://github.com/pdm-project/pdm
-    rev: '2.4.9'
+    rev: '2.6.1'
     hooks:
       - id: pdm-lock-check
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: 'v4.4.0'
     hooks:
       - id: mixed-line-ending
         args: [--fix=lf]
```

### Comparing `easynetwork-1.0.0.dev1/pdm.lock` & `easynetwork-1.0.0rc1/pdm.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [[package]]
-name = "attrs"
-version = "22.2.0"
-requires_python = ">=3.6"
-summary = "Classes Without Boilerplate"
-
-[[package]]
 name = "black"
-version = "23.1.0"
+version = "23.3.0"
 requires_python = ">=3.7"
 summary = "The uncompromising code formatter."
 dependencies = [
     "click>=8.0.0",
     "mypy-extensions>=0.4.3",
     "packaging>=22.0",
     "pathspec>=0.9.0",
     "platformdirs>=2",
-    "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 
 [[package]]
 name = "bump2version"
 version = "1.0.1"
 requires_python = ">=3.5"
 summary = "Version-bump your software with a single command!"
 
 [[package]]
 name = "cachetools"
-version = "5.3.0"
-requires_python = "~=3.7"
+version = "5.3.1"
+requires_python = ">=3.7"
 summary = "Extensible memoizing collections and decorators"
 
 [[package]]
 name = "cbor2"
 version = "5.4.6"
 requires_python = ">=3.7"
 summary = "CBOR (de)serializer with extensive tag support"
@@ -72,52 +65,51 @@
 name = "colorama"
 version = "0.4.6"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 summary = "Cross-platform colored terminal text."
 
 [[package]]
 name = "coverage"
-version = "7.2.2"
+version = "7.2.7"
 requires_python = ">=3.7"
 summary = "Code coverage measurement for Python"
 
 [[package]]
 name = "coverage"
-version = "7.2.2"
+version = "7.2.7"
 extras = ["toml"]
 requires_python = ">=3.7"
 summary = "Code coverage measurement for Python"
 dependencies = [
-    "coverage==7.2.2",
-    "tomli; python_full_version <= \"3.11.0a6\"",
+    "coverage==7.2.7",
 ]
 
 [[package]]
 name = "cryptography"
-version = "39.0.2"
-requires_python = ">=3.6"
+version = "41.0.1"
+requires_python = ">=3.7"
 summary = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
 dependencies = [
     "cffi>=1.12",
 ]
 
 [[package]]
 name = "distlib"
 version = "0.3.6"
 summary = "Distribution utilities"
 
 [[package]]
-name = "exceptiongroup"
-version = "1.1.1"
-requires_python = ">=3.7"
-summary = "Backport of PEP 654 (exception groups)"
+name = "execnet"
+version = "1.9.0"
+requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
+summary = "execnet: rapid multi-Python deployment"
 
 [[package]]
 name = "filelock"
-version = "3.10.0"
+version = "3.12.2"
 requires_python = ">=3.7"
 summary = "A platform independent file lock."
 
 [[package]]
 name = "flake8"
 version = "6.0.0"
 requires_python = ">=3.8.1"
@@ -129,38 +121,44 @@
 ]
 
 [[package]]
 name = "flake8-dunder-all"
 version = "0.1.0"
 requires_python = ">=3.10"
 git = "https://github.com/francis-clairicia/flake8-dunder-all.git"
-ref = "main"
+ref = "v0.1.0"
 revision = "df321969b1a332fe4ecb8958f9994abcbb8d06bc"
 summary = "flake8 plugin dealing with modules' __all__"
 dependencies = [
     "flake8>=6.0.0",
 ]
 
 [[package]]
 name = "flake8-pyi"
-version = "23.3.0"
+version = "23.5.0"
 requires_python = ">=3.7"
 summary = "A plugin for flake8 to enable linting .pyi stub files."
 dependencies = [
-    "flake8<7.0.0,>=3.2.1",
+    "flake8<7.0.0,>=5.0.4",
     "pyflakes>=2.1.1",
 ]
 
 [[package]]
 name = "identify"
-version = "2.5.21"
+version = "2.5.24"
 requires_python = ">=3.7"
 summary = "File identification library for Python"
 
 [[package]]
+name = "idna"
+version = "3.4"
+requires_python = ">=3.5"
+summary = "Internationalized Domain Names in Applications (IDNA)"
+
+[[package]]
 name = "iniconfig"
 version = "2.0.0"
 requires_python = ">=3.7"
 summary = "brain-dead simple config-ini parsing"
 
 [[package]]
 name = "isort"
@@ -171,66 +169,76 @@
 [[package]]
 name = "mccabe"
 version = "0.7.0"
 requires_python = ">=3.6"
 summary = "McCabe checker, plugin for flake8"
 
 [[package]]
+name = "msgpack"
+version = "1.0.5"
+summary = "MessagePack serializer"
+
+[[package]]
+name = "msgpack-types"
+version = "0.2.0"
+requires_python = ">=3.7,<4.0"
+summary = "Type stubs for msgpack"
+
+[[package]]
 name = "mypy"
-version = "0.991"
+version = "1.3.0"
 requires_python = ">=3.7"
 summary = "Optional static typing for Python"
 dependencies = [
-    "mypy-extensions>=0.4.3",
-    "tomli>=1.1.0; python_version < \"3.11\"",
+    "mypy-extensions>=1.0.0",
     "typing-extensions>=3.10",
 ]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 requires_python = ">=3.5"
 summary = "Type system extensions for programs checked with the mypy type checker."
 
 [[package]]
 name = "nodeenv"
-version = "1.7.0"
+version = "1.8.0"
 requires_python = ">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*"
 summary = "Node.js virtual environment builder"
 dependencies = [
     "setuptools",
 ]
 
 [[package]]
 name = "packaging"
-version = "23.0"
+version = "23.1"
 requires_python = ">=3.7"
 summary = "Core utilities for Python packages"
 
 [[package]]
 name = "pathspec"
 version = "0.11.1"
 requires_python = ">=3.7"
 summary = "Utility library for gitignore style pattern matching of file paths."
 
 [[package]]
 name = "platformdirs"
-version = "3.1.1"
+version = "3.6.0"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
 summary = "plugin and hook calling mechanisms for python"
 
 [[package]]
 name = "pre-commit"
-version = "3.2.0"
+version = "3.3.3"
 requires_python = ">=3.8"
 summary = "A framework for managing and maintaining multi-language pre-commit hooks."
 dependencies = [
     "cfgv>=2.0.0",
     "identify>=1.0.0",
     "nodeenv>=0.11.1",
     "pyyaml>=5.1",
@@ -253,41 +261,46 @@
 name = "pyflakes"
 version = "3.0.1"
 requires_python = ">=3.6"
 summary = "passive checker of Python programs"
 
 [[package]]
 name = "pyproject-api"
-version = "1.5.1"
+version = "1.5.2"
 requires_python = ">=3.7"
 summary = "API to interact with the python pyproject.toml based projects"
 dependencies = [
-    "packaging>=23",
-    "tomli>=2.0.1; python_version < \"3.11\"",
+    "packaging>=23.1",
 ]
 
 [[package]]
 name = "pytest"
-version = "7.2.2"
+version = "7.3.2"
 requires_python = ">=3.7"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
-    "attrs>=19.2.0",
     "colorama; sys_platform == \"win32\"",
-    "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
     "pluggy<2.0,>=0.12",
-    "tomli>=1.0.0; python_version < \"3.11\"",
+]
+
+[[package]]
+name = "pytest-asyncio"
+version = "0.21.0"
+requires_python = ">=3.7"
+summary = "Pytest support for asyncio"
+dependencies = [
+    "pytest>=7.0.0",
 ]
 
 [[package]]
 name = "pytest-cov"
-version = "4.0.0"
-requires_python = ">=3.6"
+version = "4.1.0"
+requires_python = ">=3.7"
 summary = "Pytest plugin for measuring coverage."
 dependencies = [
     "coverage[toml]>=5.2.1",
     "pytest>=4.6",
 ]
 
 [[package]]
@@ -296,109 +309,142 @@
 requires_python = ">=3.7"
 summary = "Thin-wrapper around the mock package for easier use with pytest"
 dependencies = [
     "pytest>=5.0",
 ]
 
 [[package]]
+name = "pytest-xdist"
+version = "3.3.1"
+requires_python = ">=3.7"
+summary = "pytest xdist plugin for distributed testing, most importantly across multiple CPUs"
+dependencies = [
+    "execnet>=1.1",
+    "pytest>=6.2.0",
+]
+
+[[package]]
 name = "pyyaml"
 version = "6.0"
 requires_python = ">=3.6"
 summary = "YAML parser and emitter for Python"
 
 [[package]]
 name = "setuptools"
-version = "67.6.0"
+version = "67.8.0"
 requires_python = ">=3.7"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
 
 [[package]]
-name = "tomli"
-version = "2.0.1"
+name = "sniffio"
+version = "1.3.0"
 requires_python = ">=3.7"
-summary = "A lil' TOML parser"
+summary = "Sniff out which async library your code is running under"
 
 [[package]]
 name = "tox"
-version = "4.4.7"
+version = "4.6.2"
 requires_python = ">=3.7"
 summary = "tox is a generic virtualenv management and test command line tool"
 dependencies = [
-    "cachetools>=5.3",
+    "cachetools>=5.3.1",
     "chardet>=5.1",
     "colorama>=0.4.6",
-    "filelock>=3.9",
-    "packaging>=23",
-    "platformdirs>=2.6.2",
+    "filelock>=3.12.2",
+    "packaging>=23.1",
+    "platformdirs>=3.5.3",
     "pluggy>=1",
-    "pyproject-api>=1.5",
-    "tomli>=2.0.1; python_version < \"3.11\"",
-    "virtualenv>=20.17.1",
+    "pyproject-api>=1.5.2",
+    "virtualenv>=20.23.1",
+]
+
+[[package]]
+name = "trove-classifiers"
+version = "2023.5.2"
+summary = "Canonical source for classifiers on PyPI (pypi.org)."
+
+[[package]]
+name = "trustme"
+version = "1.0.0"
+requires_python = ">=3.7"
+summary = "#1 quality TLS certs while you wait, for the discerning tester"
+dependencies = [
+    "cryptography>=3.1",
+    "idna>=2.0",
 ]
 
 [[package]]
+name = "types-cryptography"
+version = "3.3.23.2"
+summary = "Typing stubs for cryptography"
+
+[[package]]
 name = "typing-extensions"
-version = "4.5.0"
+version = "4.6.3"
 requires_python = ">=3.7"
 summary = "Backported and Experimental Type Hints for Python 3.7+"
 
 [[package]]
+name = "uvloop"
+version = "0.17.0"
+requires_python = ">=3.7"
+summary = "Fast implementation of asyncio event loop on top of libuv"
+
+[[package]]
 name = "virtualenv"
-version = "20.21.0"
+version = "20.23.1"
 requires_python = ">=3.7"
 summary = "Virtual Python Environment builder"
 dependencies = [
     "distlib<1,>=0.3.6",
-    "filelock<4,>=3.4.1",
-    "platformdirs<4,>=2.4",
+    "filelock<4,>=3.12",
+    "platformdirs<4,>=3.5.1",
 ]
 
 [metadata]
-lock_version = "4.1"
-content_hash = "sha256:4c1ab48a7f88fb2a5e497790871d09c6aa92bca7d0cfb7b2169dc67d56b4fdad"
+lock_version = "4.2"
+cross_platform = true
+groups = ["default", "cbor", "dev", "encryption", "flake8", "format", "msgpack", "mypy", "sniffio", "test", "tox", "uvloop"]
+content_hash = "sha256:4b69c46e0bcb6711f4305bda72e844b575a954b45c3e5e4246ea82ccdd5ad6a8"
 
 [metadata.files]
-"attrs 22.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/21/31/3f468da74c7de4fcf9b25591e682856389b3400b4b62f201e65f15ea3e07/attrs-22.2.0.tar.gz", hash = "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"},
-    {url = "https://files.pythonhosted.org/packages/fb/6e/6f83bf616d2becdf333a1640f1d463fef3150e2e926b7010cb0f81c95e88/attrs-22.2.0-py3-none-any.whl", hash = "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836"},
-]
-"black 23.1.0" = [
-    {url = "https://files.pythonhosted.org/packages/01/8a/065d0a59c1ebe13186b12a2fa3965a41fc1588828709995e2630004d216e/black-23.1.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8"},
-    {url = "https://files.pythonhosted.org/packages/15/11/533355217b1cc4a6df3263048060c1527f733d4720e158de2085293112bb/black-23.1.0.tar.gz", hash = "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac"},
-    {url = "https://files.pythonhosted.org/packages/18/99/bb1be0ff3a7e912679ad234a3c4884fa7689dfcc4eae85bddb6c04feaa62/black-23.1.0-py3-none-any.whl", hash = "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32"},
-    {url = "https://files.pythonhosted.org/packages/20/de/eff8e3ccc22b5c2be1265a9e61f1006d03e194519a3ca2e83dd8483dbbb5/black-23.1.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580"},
-    {url = "https://files.pythonhosted.org/packages/2d/9a/a81bf384a08d8a5e13d97223a60a74ac3c16c0aecdbd85edbc662d158bde/black-23.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074"},
-    {url = "https://files.pythonhosted.org/packages/32/a7/1d207427b87780c505a41c9430d26362e729954503b8ffba27c4f53a6810/black-23.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a"},
-    {url = "https://files.pythonhosted.org/packages/3d/dc/12dc29bb38b8db68c79b8339de1590fe1ae796858bfa6cf7494eb672be21/black-23.1.0-cp38-cp38-win_amd64.whl", hash = "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753"},
-    {url = "https://files.pythonhosted.org/packages/3e/c0/abc7031d670d211e4e2a063910d587dfcb62ce469631e779b23b66653442/black-23.1.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26"},
-    {url = "https://files.pythonhosted.org/packages/43/bc/5232fd6b0fd6d6177140cfb7d8f0f0e06638e2a750122767e265beb91161/black-23.1.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651"},
-    {url = "https://files.pythonhosted.org/packages/6b/d1/4394e4b0a24ad0f556aca3ab11e27f2e199f03b43f147c31a4befbf62b48/black-23.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481"},
-    {url = "https://files.pythonhosted.org/packages/77/11/db2ae5bf93af5185086d9b1baf4ce369ca34c3a01835230873aa9163d52d/black-23.1.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06"},
-    {url = "https://files.pythonhosted.org/packages/7e/fe/6c05c3f9255b7b498cfb88faa85b45329f1b7b0ecb444ebdc6b74ffa1457/black-23.1.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648"},
-    {url = "https://files.pythonhosted.org/packages/96/af/3361b34907efbfd9d55af453488be2282f831d98b7d201248b38d4c44346/black-23.1.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad"},
-    {url = "https://files.pythonhosted.org/packages/9a/ee/549e8be7f635cabcc3c7c3f2c3b27971dc32735155631b9ef2dcb1bd861f/black-23.1.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27"},
-    {url = "https://files.pythonhosted.org/packages/a4/ec/934e89820289e6952922fa5965aec0e046ed65da168ffb0515af1e3364e1/black-23.1.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6"},
-    {url = "https://files.pythonhosted.org/packages/ae/93/1e62fe94ab531bdc3f6cbbbd5b518727277bf40f695777b4097db5da2a38/black-23.1.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739"},
-    {url = "https://files.pythonhosted.org/packages/b1/7e/c368e9c795387a01bc181d8acbfd178278cc9960c5e7ef1059222a4419f9/black-23.1.0-cp37-cp37m-win_amd64.whl", hash = "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24"},
-    {url = "https://files.pythonhosted.org/packages/b7/33/8e074fd8b86a1c8668f5493ed28929d87bdccb6aa68c2975b47a02f92287/black-23.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9"},
-    {url = "https://files.pythonhosted.org/packages/be/f9/11e401323cd5b4e53d138fc880564765466a86acd2d4b50d7c8cdd048c18/black-23.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"},
-    {url = "https://files.pythonhosted.org/packages/c0/1d/8dac412cf5cc4120a438969a4fafefdc3de8fa13d411f317a9f9f1e268a4/black-23.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555"},
-    {url = "https://files.pythonhosted.org/packages/cf/fe/dda4b7eedb9d4dc46e306b814f7838cd9026907fdc889f75eb9f6d47d414/black-23.1.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b"},
-    {url = "https://files.pythonhosted.org/packages/d0/cb/0a38ffdafbb4b3f337adaf1b79aeaf4b8a21ed18835acad6349e46c78c80/black-23.1.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221"},
-    {url = "https://files.pythonhosted.org/packages/dd/19/875b5006e40ea69a4120671f50317100b24732f2b877203722c91bc4eef3/black-23.1.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468"},
-    {url = "https://files.pythonhosted.org/packages/e6/0a/9a5fca4a2ca07d4dbc3b00445c9353f05ea182b000f68c9ad6ba1da87a47/black-23.1.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd"},
-    {url = "https://files.pythonhosted.org/packages/f1/89/ccc28cb74a66c094b609295b009b5e0350c10b75661d2450eeed2f60ce37/black-23.1.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958"},
+"black 23.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/06/1e/273d610249f0335afb1ddb03664a03223f4826e3d1a95170a0142cb19fb4/black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
+    {url = "https://files.pythonhosted.org/packages/12/4b/99c71d1cf1353edd5aff2700b8960f92e9b805c9dab72639b67dbb449d3a/black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
+    {url = "https://files.pythonhosted.org/packages/13/0a/ed8b66c299e896780e4528eed4018f5b084da3b9ba4ee48328550567d866/black-23.3.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5"},
+    {url = "https://files.pythonhosted.org/packages/13/25/cfa06788d0a936f2445af88f13604b5bcd5c9d050db618c718e6ebe66f74/black-23.3.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30"},
+    {url = "https://files.pythonhosted.org/packages/21/14/d5a2bec5fb15f9118baab7123d344646fac0b1c6939d51c2b05259cd2d9c/black-23.3.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331"},
+    {url = "https://files.pythonhosted.org/packages/24/eb/2d2d2c27cb64cfd073896f62a952a802cd83cf943a692a2f278525b57ca9/black-23.3.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b"},
+    {url = "https://files.pythonhosted.org/packages/27/70/07aab2623cfd3789786f17e051487a41d5657258c7b1ef8f780512ffea9c/black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
+    {url = "https://files.pythonhosted.org/packages/29/b1/b584fc863c155653963039664a592b3327b002405043b7e761b9b0212337/black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
+    {url = "https://files.pythonhosted.org/packages/3c/d7/85f3d79f9e543402de2244c4d117793f262149e404ea0168841613c33e07/black-23.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab"},
+    {url = "https://files.pythonhosted.org/packages/3f/0d/81dd4194ce7057c199d4f28e4c2a885082d9d929e7a55c514b23784f7787/black-23.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326"},
+    {url = "https://files.pythonhosted.org/packages/49/36/15d2122f90ff1cd70f06892ebda777b650218cf84b56b5916a993dc1359a/black-23.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2"},
+    {url = "https://files.pythonhosted.org/packages/49/d7/f3b7da6c772800f5375aeb050a3dcf682f0bbeb41d313c9c2820d0156e4e/black-23.3.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266"},
+    {url = "https://files.pythonhosted.org/packages/69/49/7e1f0cf585b0d607aad3f971f95982cc4208fc77f92363d632d23021ee57/black-23.3.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d"},
+    {url = "https://files.pythonhosted.org/packages/6d/b4/0f13ab7f5e364795ff82b76b0f9a4c9c50afda6f1e2feeb8b03fdd7ec57d/black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
+    {url = "https://files.pythonhosted.org/packages/ad/e7/4642b7f462381799393fbad894ba4b32db00870a797f0616c197b07129a9/black-23.3.0-py3-none-any.whl", hash = "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4"},
+    {url = "https://files.pythonhosted.org/packages/c0/53/42e312c17cfda5c8fc4b6b396a508218807a3fcbb963b318e49d3ddd11d5/black-23.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70"},
+    {url = "https://files.pythonhosted.org/packages/ca/44/eb41edd3f558a6139f09eee052dead4a7a464e563b822ddf236f5a8ee286/black-23.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925"},
+    {url = "https://files.pythonhosted.org/packages/ce/f4/2b0c6ac9e1f8584296747f66dd511898b4ebd51d6510dba118279bff53b6/black-23.3.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27"},
+    {url = "https://files.pythonhosted.org/packages/d1/6e/5810b6992ed70403124c67e8b3f62858a32b35405177553f1a78ed6b6e31/black-23.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8"},
+    {url = "https://files.pythonhosted.org/packages/d6/36/66370f5017b100225ec4950a60caeef60201a10080da57ddb24124453fba/black-23.3.0.tar.gz", hash = "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940"},
+    {url = "https://files.pythonhosted.org/packages/d7/6f/d3832960a3b646b333b7f0d80d336a3c123012e9d9d5dba4a622b2b6181d/black-23.3.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6"},
+    {url = "https://files.pythonhosted.org/packages/db/f4/7908f71cc71da08df1317a3619f002cbf91927fb5d3ffc7723905a2113f7/black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
+    {url = "https://files.pythonhosted.org/packages/de/b4/76f152c5eb0be5471c22cd18380d31d188930377a1a57969073b89d6615d/black-23.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c"},
+    {url = "https://files.pythonhosted.org/packages/eb/a5/17b40bfd9b607b69fa726b0b3a473d14b093dcd5191ea1a1dd664eccfee3/black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
+    {url = "https://files.pythonhosted.org/packages/fd/5b/fc2d7922c1a6bb49458d424b5be71d251f2d0dc97be9534e35d171bdc653/black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
 ]
 "bump2version 1.0.1" = [
     {url = "https://files.pythonhosted.org/packages/1d/e3/fa60c47d7c344533142eb3af0b73234ef8ea3fb2da742ab976b947e717df/bump2version-1.0.1-py2.py3-none-any.whl", hash = "sha256:37f927ea17cde7ae2d7baf832f8e80ce3777624554a653006c9144f8017fe410"},
     {url = "https://files.pythonhosted.org/packages/29/2a/688aca6eeebfe8941235be53f4da780c6edee05dbbea5d7abaa3aab6fad2/bump2version-1.0.1.tar.gz", hash = "sha256:762cb2bfad61f4ec8e2bdf452c7c267416f8c70dd9ecb1653fd0bbb01fa936e6"},
 ]
-"cachetools 5.3.0" = [
-    {url = "https://files.pythonhosted.org/packages/4d/91/5837e9f9e77342bb4f3ffac19ba216eef2cd9b77d67456af420e7bafe51d/cachetools-5.3.0.tar.gz", hash = "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14"},
-    {url = "https://files.pythonhosted.org/packages/db/14/2b48a834d349eee94677e8702ea2ef98b7c674b090153ea8d3f6a788584e/cachetools-5.3.0-py3-none-any.whl", hash = "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"},
+"cachetools 5.3.1" = [
+    {url = "https://files.pythonhosted.org/packages/9d/8b/8e2ebf5ee26c21504de5ea2fb29cc6ae612b35fd05f959cdb641feb94ec4/cachetools-5.3.1.tar.gz", hash = "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"},
+    {url = "https://files.pythonhosted.org/packages/a9/c9/c8a7710f2cedcb1db9224fdd4d8307c9e48cbddc46c18b515fefc0f1abbe/cachetools-5.3.1-py3-none-any.whl", hash = "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590"},
 ]
 "cbor2 5.4.6" = [
     {url = "https://files.pythonhosted.org/packages/05/c6/8ea5ce170f43958b0ea8e788d0f3ec08fbf57bb18c49c301a0a09f294b92/cbor2-5.4.6-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:309fffbb7f561d67f02095d4b9657b73c9220558701c997e9bfcfbca2696e927"},
     {url = "https://files.pythonhosted.org/packages/05/cc/6d0b722065ba5a58a7be126b0a503ba13031887a4569498a5c86a10b924a/cbor2-5.4.6-cp310-cp310-win_amd64.whl", hash = "sha256:0b956f19e93ba3180c336282cd1b6665631f2d3a196a9c19b29a833bf979e7a4"},
     {url = "https://files.pythonhosted.org/packages/08/b6/d08e93922ffc39fea4cb91bab7f90db07adfeda4602a0e2baa770223fe89/cbor2-5.4.6-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:78304df140b9e13b93bcbb2aecee64c9aaa9f1cadbd45f043b5e7b93cc2f21a2"},
     {url = "https://files.pythonhosted.org/packages/1c/92/895e5c31b3dd1cff4cde8e1dcabe93f83f444fbf9bafaf932ad2a4eb32ed/cbor2-5.4.6-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:4ce1a2c272ba8523a55ea2f1d66e3464e89fa0e37c9a3d786a919fe64e68dbd7"},
     {url = "https://files.pythonhosted.org/packages/1d/30/9d8d4a392b50313c9fe6b808a130c14a40bac2032dd7365e891a97de3df1/cbor2-5.4.6-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3950be57a1698086cf26d8710b4e5a637b65133c5b1f9eec23967d4089d8cfed"},
@@ -512,216 +558,298 @@
     {url = "https://files.pythonhosted.org/packages/59/87/84326af34517fca8c58418d148f2403df25303e02736832403587318e9e8/click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
     {url = "https://files.pythonhosted.org/packages/c2/f1/df59e28c642d583f7dacffb1e0965d0e00b218e0186d7858ac5233dce840/click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
 ]
 "colorama 0.4.6" = [
     {url = "https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {url = "https://files.pythonhosted.org/packages/d8/53/6f443c9a4a8358a93a6792e2acffb9d9d5cb0a5cfd8802644b7b1c9a02e4/colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
-"coverage 7.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/06/ab/1dd1a592ca3dff0c0d1da895c609f6b8b6b3092a2cc06f5494826b7689c8/coverage-7.2.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005"},
-    {url = "https://files.pythonhosted.org/packages/0d/49/ef6f4681a90ad12b734e8fd85913dc310eb58bfc33eb95534bdfef073476/coverage-7.2.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4"},
-    {url = "https://files.pythonhosted.org/packages/0d/d3/7c6d91fc5dd15496954e9a941a765fce70913314181289e441db0e5c6568/coverage-7.2.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e"},
-    {url = "https://files.pythonhosted.org/packages/11/da/b52e1f1492d6431ce0ebdd9da8744faf9f9fb75c3077165aca44c178f6e7/coverage-7.2.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90"},
-    {url = "https://files.pythonhosted.org/packages/13/31/8a4be0305f60f9a856965e076388cf3b93bac36a1324897854accecc4e94/coverage-7.2.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5"},
-    {url = "https://files.pythonhosted.org/packages/15/35/5a6ac4b81c41fe067af22a5e9ac440609a122c1ece220b8c565dfb27f205/coverage-7.2.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88"},
-    {url = "https://files.pythonhosted.org/packages/18/a9/98d8eddba099f79548527af0aa546c31c3d8a2cc9e5d1c59a10a584ffc6d/coverage-7.2.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540"},
-    {url = "https://files.pythonhosted.org/packages/1b/21/e757c7147ff8ef4be811d5fb3731ec0936ba6689444fc20dff953536a243/coverage-7.2.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd"},
-    {url = "https://files.pythonhosted.org/packages/1c/02/46d5dc331c9419d01e66c497f3974af895aaccf6a2a2695cfd6f83f1935f/coverage-7.2.2-cp39-cp39-win32.whl", hash = "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc"},
-    {url = "https://files.pythonhosted.org/packages/29/3f/e2cef2978bfd787da8e02892448098ecb4a5909970c08b6220d0867460c3/coverage-7.2.2-cp310-cp310-win32.whl", hash = "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292"},
-    {url = "https://files.pythonhosted.org/packages/30/0c/6e0a65466f8008b2001c0354782753a880617b15dba857eb7e97928313fc/coverage-7.2.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149"},
-    {url = "https://files.pythonhosted.org/packages/34/7d/380f87502e91d1da48eb5d0dead8cee4911eb19e2d4b60e3f1ee9c975c85/coverage-7.2.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2"},
-    {url = "https://files.pythonhosted.org/packages/38/0f/2e384888c47e111a7a4c025812d33f197aa39a59338cfd5e08874c940f6c/coverage-7.2.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5"},
-    {url = "https://files.pythonhosted.org/packages/3c/12/51c5bdce0ad62a29bff429e99a9b2f23a0220cca89e768fc22694d4aeb4f/coverage-7.2.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988"},
-    {url = "https://files.pythonhosted.org/packages/42/1b/340c1d2d3bdfe33664a63307ae1143bf3e7929290715d8034e40aff6bcef/coverage-7.2.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f"},
-    {url = "https://files.pythonhosted.org/packages/44/50/b752e846395b17d3789b070b82ac54e88cc2e4f4d906b9f864074caf04b9/coverage-7.2.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84"},
-    {url = "https://files.pythonhosted.org/packages/47/21/632047c45edb08f0eb51f9e8e49591d23c15ff078b32e0a88ddf99f4e8c2/coverage-7.2.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8"},
-    {url = "https://files.pythonhosted.org/packages/4a/73/031f7380e2912f78801d28120091ba2dcf5bc0ad689e958d6b970ce67cb7/coverage-7.2.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be"},
-    {url = "https://files.pythonhosted.org/packages/4f/ec/acf6816f7fd5e628746db61725f7a3f5eb16b3b55c919c885072c60d17fa/coverage-7.2.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57"},
-    {url = "https://files.pythonhosted.org/packages/50/32/82dea3a1e928f8f7d2cdf6f0c6498fd42c5e9d661de0191f8c47d3966306/coverage-7.2.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137"},
-    {url = "https://files.pythonhosted.org/packages/54/8a/db9d9cd24f96bb872eea151bb0d5c8cb6a96825b70a0cfaf07bceab2884d/coverage-7.2.2.tar.gz", hash = "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2"},
-    {url = "https://files.pythonhosted.org/packages/56/65/fedba1cb8d954823eded8e7b943749531f81060f8e4214fe9ee8dd1da5bc/coverage-7.2.2-cp38-cp38-win_amd64.whl", hash = "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8"},
-    {url = "https://files.pythonhosted.org/packages/59/4b/8a1077b2cf0c21e2f39105f3c94fac4e1bb18ff341d386ba60374487ae49/coverage-7.2.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67"},
-    {url = "https://files.pythonhosted.org/packages/5e/92/cffba484a7a34ca08097f7991b72cbd85da4adc717c69c067bab2e1f612c/coverage-7.2.2-pp37.pp38.pp39-none-any.whl", hash = "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968"},
-    {url = "https://files.pythonhosted.org/packages/5e/f1/cf01ea71b3c525f5cb4aa9956b5bf2d4e0ac59cdc1e2aead8e73374ab420/coverage-7.2.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"},
-    {url = "https://files.pythonhosted.org/packages/6f/e4/9576c24b37c941e70a4815cbbd44ff2779c83b821ab3a38022b6f530d61c/coverage-7.2.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d"},
-    {url = "https://files.pythonhosted.org/packages/70/74/7ceb96c38dac56e5894c3b0af6c4adfd0dd7f96521e8b829544d1dcec8fe/coverage-7.2.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140"},
-    {url = "https://files.pythonhosted.org/packages/74/bf/ae3344872e1a33e58481afaa1587e39a4e626fdaa69bd11c1454fd34e0d3/coverage-7.2.2-cp37-cp37m-win32.whl", hash = "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8"},
-    {url = "https://files.pythonhosted.org/packages/75/93/1821ffa10c91b0c4220f1b525f82b408ca49a605481d76687078cd251504/coverage-7.2.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69"},
-    {url = "https://files.pythonhosted.org/packages/76/6b/30aa019a24ba3ba3487b6d61e468c898dcba77a153012f2032d72695ec13/coverage-7.2.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd"},
-    {url = "https://files.pythonhosted.org/packages/83/db/85c50845c1ca6c83082decfed61a8d928903ef6d72f8a2c20a615118fc8a/coverage-7.2.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9"},
-    {url = "https://files.pythonhosted.org/packages/85/e3/377befb686b7ebe288ef084c2822db81722681fab3774e389d026ea2d7ca/coverage-7.2.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0"},
-    {url = "https://files.pythonhosted.org/packages/8c/c8/efee5b6e98f1009ca92333884d17eb205acb7aad800dc9b2d91475aef2a4/coverage-7.2.2-cp311-cp311-win32.whl", hash = "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d"},
-    {url = "https://files.pythonhosted.org/packages/8d/a6/6b3aae5b60e1e2ad8feb807cc33c5d313511980c3ee5de4662384165cec9/coverage-7.2.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d"},
-    {url = "https://files.pythonhosted.org/packages/8e/7f/b5709cc511c226c01ee8da008b9737726d8c62bd88cb20ef93eb5c9d80c8/coverage-7.2.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54"},
-    {url = "https://files.pythonhosted.org/packages/91/57/629e70906739102dbd742bcd7484f5446dfaacbd6dc3f46f42a88a0677c5/coverage-7.2.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2"},
-    {url = "https://files.pythonhosted.org/packages/95/06/b0541156f46970339776c42dafe5d227710127025cb96e4bd3176422016f/coverage-7.2.2-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6"},
-    {url = "https://files.pythonhosted.org/packages/9f/f0/ca6217975c4d756cbf136abfab805b470424279b322f8c9f191c21898ee9/coverage-7.2.2-cp38-cp38-win32.whl", hash = "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3"},
-    {url = "https://files.pythonhosted.org/packages/a6/8c/8a5f4fb03c4e23c69192ac8452f3448d2a408d204e39605614d7956dafa0/coverage-7.2.2-cp37-cp37m-win_amd64.whl", hash = "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25"},
-    {url = "https://files.pythonhosted.org/packages/af/dc/3fe8388df88c8dfa3d5771b1f746ef5bc92f0c718a10fcef3600199d00f7/coverage-7.2.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7"},
-    {url = "https://files.pythonhosted.org/packages/c1/dc/ef3f63275d1046b910a474eedf8eb9fa3265c30b5fab1c1391ed6351e9d9/coverage-7.2.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b"},
-    {url = "https://files.pythonhosted.org/packages/c7/de/80032c5d6340a3a3b29920ade4e09e3f240cee8410b88173babb9e7012be/coverage-7.2.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212"},
-    {url = "https://files.pythonhosted.org/packages/ca/45/687fb10526b66642a479b8703cd5ea53030fc582e76e7236e7a6318fd660/coverage-7.2.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9"},
-    {url = "https://files.pythonhosted.org/packages/cb/03/76ca85381dd6aea8b190ae0fa9e7e7c3964f72f65fc32ef0454e68df4611/coverage-7.2.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6"},
-    {url = "https://files.pythonhosted.org/packages/d0/94/fa6095cce802c11a53685c5267330caed7ef02e2fb99b9f9f1c892859259/coverage-7.2.2-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d"},
-    {url = "https://files.pythonhosted.org/packages/d4/cd/ef9d489e9c943636193de07e5089d84252c611572865e50e475495528070/coverage-7.2.2-cp39-cp39-win_amd64.whl", hash = "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef"},
-    {url = "https://files.pythonhosted.org/packages/d8/3f/9df4f173d6f43ff80a11720cc3a9f4fa12d14ab36a2fb1a1d83ce026dd37/coverage-7.2.2-cp310-cp310-win_amd64.whl", hash = "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab"},
-    {url = "https://files.pythonhosted.org/packages/d8/de/effbd360724a67b8e8f7f297c4cffdd5510161aeb4de08b08e1fc6fbbd49/coverage-7.2.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5"},
-    {url = "https://files.pythonhosted.org/packages/d9/55/f45a1d08ad1299c5199f3cf1baaa02fcffe347fdec8ddacc484858700ef6/coverage-7.2.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016"},
-    {url = "https://files.pythonhosted.org/packages/e5/d4/d8ee18c995b806b3d0d38dc17ab5888de148244da5be8d3dfbd7cea6cd7e/coverage-7.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731"},
-    {url = "https://files.pythonhosted.org/packages/f5/6f/7811ed60d4088b6a54bb48d57b48f647e55c876ee9088e3fa123eb879673/coverage-7.2.2-cp311-cp311-win_amd64.whl", hash = "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512"},
-]
-"cryptography 39.0.2" = [
-    {url = "https://files.pythonhosted.org/packages/06/ea/d998c35ac871396749f14a4b4e82f080422182e1830f02959e893abd3016/cryptography-39.0.2-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:e944fe07b6f229f4c1a06a7ef906a19652bdd9fd54c761b0ff87e83ae7a30354"},
-    {url = "https://files.pythonhosted.org/packages/0b/20/f406c0d2edb7b3974c39099816795d629bbd8716cd41cda8c3c4703de095/cryptography-39.0.2-cp36-abi3-win32.whl", hash = "sha256:c43ac224aabcbf83a947eeb8b17eaf1547bce3767ee2d70093b461f31729a480"},
-    {url = "https://files.pythonhosted.org/packages/13/40/acfea5abe60f483bfba44a24419fa89d584e1e93dca750b800805ef272b9/cryptography-39.0.2-pp39-pypy39_pp73-manylinux_2_24_x86_64.whl", hash = "sha256:30b1d1bfd00f6fc80d11300a29f1d8ab2b8d9febb6ed4a38a76880ec564fae84"},
-    {url = "https://files.pythonhosted.org/packages/1e/85/d5b768b45e564a66fc5ba6344145334208f01d64939adcb8c4032545d164/cryptography-39.0.2-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:103e8f7155f3ce2ffa0049fe60169878d47a4364b277906386f8de21c9234aa1"},
-    {url = "https://files.pythonhosted.org/packages/26/d2/85480f4e754375c6d8e4a18cc8d2f28ef1984cf2843395c4d1ea396331d3/cryptography-39.0.2-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ffd394c7896ed7821a6d13b24657c6a34b6e2650bd84ae063cf11ccffa4f1a97"},
-    {url = "https://files.pythonhosted.org/packages/3c/0c/ac188ca210fbc02102d34ad8dba6956fe16fc566e5c5110a7f7bdbd30138/cryptography-39.0.2-cp36-abi3-macosx_10_12_x86_64.whl", hash = "sha256:23df8ca3f24699167daf3e23e51f7ba7334d504af63a94af468f468b975b7dd7"},
-    {url = "https://files.pythonhosted.org/packages/3c/5a/6c180b745336f989e9b298e1790af0ef5b37640edb861fc536b5663726e3/cryptography-39.0.2-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:eb40fe69cfc6f5cdab9a5ebd022131ba21453cf7b8a7fd3631f45bbf52bed612"},
-    {url = "https://files.pythonhosted.org/packages/4f/0e/55b8cff87b572da828e9c6b7e7c5ecb9dc955b551ab863c28464a15f6451/cryptography-39.0.2-cp36-abi3-win_amd64.whl", hash = "sha256:788b3921d763ee35dfdb04248d0e3de11e3ca8eb22e2e48fef880c42e1f3c8f9"},
-    {url = "https://files.pythonhosted.org/packages/6d/5b/516dc11fa0a638cb707293ad44cc1cb93924bb4b5ba03881dfdb819e23b0/cryptography-39.0.2-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:d15809e0dbdad486f4ad0979753518f47980020b7a34e9fc56e8be4f60702fac"},
-    {url = "https://files.pythonhosted.org/packages/77/19/47d55b3f609fc03b6f80c63820996671dfccb28e1d07427dd81319d514d5/cryptography-39.0.2-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:50cadb9b2f961757e712a9737ef33d89b8190c3ea34d0fb6675e00edbe35d074"},
-    {url = "https://files.pythonhosted.org/packages/7b/49/05debd3f2dfc43987063575cffb58116daf80b3db278555ecb1af765a2bd/cryptography-39.0.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:8bc0008ef798231fac03fe7d26e82d601d15bd16f3afaad1c6113771566570f3"},
-    {url = "https://files.pythonhosted.org/packages/9c/30/e787edf59f35192799d340a0a36976870ce487ba32948f086c29dc5d54ab/cryptography-39.0.2-cp36-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:8f35c17bd4faed2bc7797d2a66cbb4f986242ce2e30340ab832e5d99ae60e011"},
-    {url = "https://files.pythonhosted.org/packages/9e/a0/4c0c8b827f430246b48a0f2415a432427d365c77b04a911c5139ae9c79b1/cryptography-39.0.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:6236a9610c912b129610eb1a274bdc1350b5df834d124fa84729ebeaf7da42c3"},
-    {url = "https://files.pythonhosted.org/packages/b2/54/2b2a610b6eced5a7be96c0d2e214be9cee6824b9494756e6043470ca594f/cryptography-39.0.2-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:fa507318e427169ade4e9eccef39e9011cdc19534f55ca2f36ec3f388c1f70f3"},
-    {url = "https://files.pythonhosted.org/packages/c5/8a/6dcd53c995506d4ff0de3a7da2202715654493fd12d7875f2a43b3a44150/cryptography-39.0.2-cp36-abi3-macosx_10_12_universal2.whl", hash = "sha256:2725672bb53bb92dc7b4150d233cd4b8c59615cd8288d495eaa86db00d4e5c06"},
-    {url = "https://files.pythonhosted.org/packages/c6/c4/354c78bade0270f951a14db9f8248ab975ca7df050476dc3759831e52a7f/cryptography-39.0.2-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:35d658536b0a4117c885728d1a7032bdc9a5974722ae298d6c533755a6ee3915"},
-    {url = "https://files.pythonhosted.org/packages/cb/76/c9fa9cda16ac5b47b5bb29b3e3b8536ca3584458e889a6df82bbee18e693/cryptography-39.0.2-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:e029b844c21116564b8b61216befabca4b500e6816fa9f0ba49527653cae2108"},
-    {url = "https://files.pythonhosted.org/packages/d3/26/da69282ae3b350ee869536994e6816ac77057a7b5970068fabe56c644624/cryptography-39.0.2-cp36-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:5f8c682e736513db7d04349b4f6693690170f95aac449c56f97415c6980edef5"},
-    {url = "https://files.pythonhosted.org/packages/d6/99/12d3b9c8df83b52799f9994da17bb67bb4565c418b3a8284ed1f79b692e1/cryptography-39.0.2-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bc0521cce2c1d541634b19f3ac661d7a64f9555135e9d8af3980965be717fd4a"},
-    {url = "https://files.pythonhosted.org/packages/e8/5c/9e47aac90fb5923d09c413909af6bf6ad4af2bfeeff707a2485c3f2af8be/cryptography-39.0.2-cp36-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:d7d84a512a59f4412ca8549b01f94be4161c94efc598bf09d027d67826beddc0"},
-    {url = "https://files.pythonhosted.org/packages/f4/6d/1afb19efbe093f0b1af7a788bb8a693e495dc6c1d2139316b05b40f5e1dd/cryptography-39.0.2-cp36-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:b49a88ff802e1993b7f749b1eeb31134f03c8d5c956e3c125c75558955cda536"},
-    {url = "https://files.pythonhosted.org/packages/f7/c0/daaeedc40e3385f01bb1af8c001ac214dcea6716b61efebabf9066b6f619/cryptography-39.0.2-cp36-abi3-manylinux_2_24_x86_64.whl", hash = "sha256:e8a0772016feeb106efd28d4a328e77dc2edae84dfbac06061319fdb669ff828"},
-    {url = "https://files.pythonhosted.org/packages/fa/f3/f4b8c175ea9a1de650b0085858059050b7953a93d66c97ed89b93b232996/cryptography-39.0.2.tar.gz", hash = "sha256:bc5b871e977c8ee5a1bbc42fa8d19bcc08baf0c51cbf1586b0e87a2694dde42f"},
+"coverage 7.2.7" = [
+    {url = "https://files.pythonhosted.org/packages/01/24/be01e62a7bce89bcffe04729c540382caa5a06bee45ae42136c93e2499f5/coverage-7.2.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8"},
+    {url = "https://files.pythonhosted.org/packages/03/ec/6f30b4e0c96ce03b0e64aec46b4af2a8c49b70d1b5d0d69577add757b946/coverage-7.2.7-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a"},
+    {url = "https://files.pythonhosted.org/packages/04/d6/8cba3bf346e8b1a4fb3f084df7d8cea25a6b6c56aaca1f2e53829be17e9e/coverage-7.2.7-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d"},
+    {url = "https://files.pythonhosted.org/packages/04/fa/43b55101f75a5e9115259e8be70ff9279921cb6b17f04c34a5702ff9b1f7/coverage-7.2.7-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97"},
+    {url = "https://files.pythonhosted.org/packages/0d/31/340428c238eb506feb96d4fb5c9ea614db1149517f22cc7ab8c6035ef6d9/coverage-7.2.7-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050"},
+    {url = "https://files.pythonhosted.org/packages/0e/bc/7e3a31534fabb043269f14fb64e2bb2733f85d4cf39e5bbc71357c57553a/coverage-7.2.7-cp37-cp37m-win_amd64.whl", hash = "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0"},
+    {url = "https://files.pythonhosted.org/packages/15/81/b108a60bc758b448c151e5abceed027ed77a9523ecbc6b8a390938301841/coverage-7.2.7-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01"},
+    {url = "https://files.pythonhosted.org/packages/1f/e9/d6730247d8dec2a3dddc520ebe11e2e860f0f98cee3639e23de6cf920255/coverage-7.2.7-cp310-cp310-win_amd64.whl", hash = "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850"},
+    {url = "https://files.pythonhosted.org/packages/22/c1/2f6c1b6f01a0996c9e067a9c780e1824351dbe17faae54388a4477e6d86f/coverage-7.2.7-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959"},
+    {url = "https://files.pythonhosted.org/packages/24/df/6765898d54ea20e3197a26d26bb65b084deefadd77ce7de946b9c96dfdc5/coverage-7.2.7-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4"},
+    {url = "https://files.pythonhosted.org/packages/28/d7/9a8de57d87f4bbc6f9a6a5ded1eaac88a89bf71369bb935dac3c0cf2893e/coverage-7.2.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5"},
+    {url = "https://files.pythonhosted.org/packages/29/8f/4fad1c2ba98104425009efd7eaa19af9a7c797e92d40cd2ec026fa1f58cb/coverage-7.2.7-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495"},
+    {url = "https://files.pythonhosted.org/packages/2b/86/3dbf9be43f8bf6a5ca28790a713e18902b2d884bc5fa9512823a81dff601/coverage-7.2.7-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1"},
+    {url = "https://files.pythonhosted.org/packages/3d/80/7060a445e1d2c9744b683dc935248613355657809d6c6b2716cdf4ca4766/coverage-7.2.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb"},
+    {url = "https://files.pythonhosted.org/packages/44/55/49f65ccdd4dfd6d5528e966b28c37caec64170c725af32ab312889d2f857/coverage-7.2.7-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e"},
+    {url = "https://files.pythonhosted.org/packages/45/8b/421f30467e69ac0e414214856798d4bc32da1336df745e49e49ae5c1e2a8/coverage-7.2.7.tar.gz", hash = "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59"},
+    {url = "https://files.pythonhosted.org/packages/4a/fb/78986d3022e5ccf2d4370bc43a5fef8374f092b3c21d32499dee8e30b7b6/coverage-7.2.7-cp38-cp38-win32.whl", hash = "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e"},
+    {url = "https://files.pythonhosted.org/packages/61/90/c76b9462f39897ebd8714faf21bc985b65c4e1ea6dff428ea9dc711ed0dd/coverage-7.2.7-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6"},
+    {url = "https://files.pythonhosted.org/packages/61/af/5964b8d7d9a5c767785644d9a5a63cacba9a9c45cc42ba06d25895ec87be/coverage-7.2.7-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7"},
+    {url = "https://files.pythonhosted.org/packages/66/2e/c99fe1f6396d93551aa352c75410686e726cd4ea104479b9af1af22367ce/coverage-7.2.7-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250"},
+    {url = "https://files.pythonhosted.org/packages/67/a2/6fa66a50e6e894286d79a3564f42bd54a9bd27049dc0a63b26d9924f0aa3/coverage-7.2.7-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9"},
+    {url = "https://files.pythonhosted.org/packages/67/d7/cd8fe689b5743fffac516597a1222834c42b80686b99f5b44ef43ccc2a43/coverage-7.2.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe"},
+    {url = "https://files.pythonhosted.org/packages/67/fb/b3b1d7887e1ea25a9608b0776e480e4bbc303ca95a31fd585555ec4fff5a/coverage-7.2.7-pp37.pp38.pp39-none-any.whl", hash = "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d"},
+    {url = "https://files.pythonhosted.org/packages/68/5f/d2bd0f02aa3c3e0311986e625ccf97fdc511b52f4f1a063e4f37b624772f/coverage-7.2.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a"},
+    {url = "https://files.pythonhosted.org/packages/69/8c/26a95b08059db1cbb01e4b0e6d40f2e9debb628c6ca86b78f625ceaf9bab/coverage-7.2.7-cp312-cp312-win32.whl", hash = "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511"},
+    {url = "https://files.pythonhosted.org/packages/6e/ea/4a252dc77ca0605b23d477729d139915e753ee89e4c9507630e12ad64a80/coverage-7.2.7-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de"},
+    {url = "https://files.pythonhosted.org/packages/7a/05/084864fa4bbf8106f44fb72a56e67e0cd372d3bf9d893be818338c81af5d/coverage-7.2.7-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb"},
+    {url = "https://files.pythonhosted.org/packages/7b/e3/f552d5871943f747165b92a924055c5d6daa164ae659a13f9018e22f3990/coverage-7.2.7-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6"},
+    {url = "https://files.pythonhosted.org/packages/80/d7/67937c80b8fd4c909fdac29292bc8b35d9505312cff6bcab41c53c5b1df6/coverage-7.2.7-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f"},
+    {url = "https://files.pythonhosted.org/packages/88/8b/b0d9fe727acae907fa7f1c8194ccb6fe9d02e1c3e9001ecf74c741f86110/coverage-7.2.7-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9"},
+    {url = "https://files.pythonhosted.org/packages/88/da/495944ebf0ad246235a6bd523810d9f81981f9b81c6059ba1f56e943abe0/coverage-7.2.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9"},
+    {url = "https://files.pythonhosted.org/packages/8c/95/16eed713202406ca0a37f8ac259bbf144c9d24f9b8097a8e6ead61da2dbb/coverage-7.2.7-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"},
+    {url = "https://files.pythonhosted.org/packages/8d/d6/53e999ec1bf7498ca4bc5f3b8227eb61db39068d2de5dcc359dec5601b5a/coverage-7.2.7-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02"},
+    {url = "https://files.pythonhosted.org/packages/8f/a8/12cc7b261f3082cc299ab61f677f7e48d93e35ca5c3c2f7241ed5525ccea/coverage-7.2.7-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833"},
+    {url = "https://files.pythonhosted.org/packages/91/e8/469ed808a782b9e8305a08bad8c6fa5f8e73e093bda6546c5aec68275bff/coverage-7.2.7-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353"},
+    {url = "https://files.pythonhosted.org/packages/94/4e/d4e46a214ae857be3d7dc5de248ba43765f60daeb1ab077cb6c1536c7fba/coverage-7.2.7-cp310-cp310-win32.whl", hash = "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818"},
+    {url = "https://files.pythonhosted.org/packages/9f/5c/d9760ac497c41f9c4841f5972d0edf05d50cad7814e86ee7d133ec4a0ac8/coverage-7.2.7-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d"},
+    {url = "https://files.pythonhosted.org/packages/a7/cd/3ce94ad9d407a052dc2a74fbeb1c7947f442155b28264eb467ee78dea812/coverage-7.2.7-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb"},
+    {url = "https://files.pythonhosted.org/packages/a9/0c/4a848ae663b47f1195abcb09a951751dd61f80b503303b9b9d768e0fd321/coverage-7.2.7-cp39-cp39-win_amd64.whl", hash = "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27"},
+    {url = "https://files.pythonhosted.org/packages/b1/96/c12ed0dfd4ec587f3739f53eb677b9007853fd486ccb0e7d5512a27bab2e/coverage-7.2.7-cp311-cp311-win_amd64.whl", hash = "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562"},
+    {url = "https://files.pythonhosted.org/packages/b1/d5/a8e276bc005e42114468d4fe03e0a9555786bc51cbfe0d20827a46c1565a/coverage-7.2.7-cp39-cp39-win32.whl", hash = "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb"},
+    {url = "https://files.pythonhosted.org/packages/b4/bd/1b2331e3a04f4cc9b7b332b1dd0f3a1261dfc4114f8479bebfcc2afee9e8/coverage-7.2.7-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063"},
+    {url = "https://files.pythonhosted.org/packages/b7/00/14b00a0748e9eda26e97be07a63cc911108844004687321ddcc213be956c/coverage-7.2.7-cp312-cp312-win_amd64.whl", hash = "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3"},
+    {url = "https://files.pythonhosted.org/packages/b8/9d/926fce7e03dbfc653104c2d981c0fa71f0572a9ebd344d24c573bd6f7c4f/coverage-7.2.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6"},
+    {url = "https://files.pythonhosted.org/packages/ba/92/69c0722882643df4257ecc5437b83f4c17ba9e67f15dc6b77bad89b6982e/coverage-7.2.7-cp311-cp311-win32.whl", hash = "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a"},
+    {url = "https://files.pythonhosted.org/packages/bb/e9/88747b40c8fb4a783b40222510ce6d66170217eb05d7f46462c36b4fa8cc/coverage-7.2.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2"},
+    {url = "https://files.pythonhosted.org/packages/c1/49/4d487e2ad5d54ed82ac1101e467e8994c09d6123c91b2a962145f3d262c2/coverage-7.2.7-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f"},
+    {url = "https://files.pythonhosted.org/packages/c3/1c/6b3c9c363fb1433c79128e0d692863deb761b1b78162494abb9e5c328bc0/coverage-7.2.7-cp38-cp38-win_amd64.whl", hash = "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c"},
+    {url = "https://files.pythonhosted.org/packages/c6/fa/529f55c9a1029c840bcc9109d5a15ff00478b7ff550a1ae361f8745f8ad5/coverage-7.2.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f"},
+    {url = "https://files.pythonhosted.org/packages/c6/fc/be19131010930a6cf271da48202c8cc1d3f971f68c02fb2d3a78247f43dc/coverage-7.2.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5"},
+    {url = "https://files.pythonhosted.org/packages/c8/e4/e6182e4697665fb594a7f4e4f27cb3a4dd00c2e3d35c5c706765de8c7866/coverage-7.2.7-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9"},
+    {url = "https://files.pythonhosted.org/packages/ca/0c/3dfeeb1006c44b911ee0ed915350db30325d01808525ae7cc8d57643a2ce/coverage-7.2.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2"},
+    {url = "https://files.pythonhosted.org/packages/d1/3a/67f5d18f911abf96857f6f7e4df37ca840e38179e2cc9ab6c0b9c3380f19/coverage-7.2.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2"},
+    {url = "https://files.pythonhosted.org/packages/d9/1d/cd467fceb62c371f9adb1d739c92a05d4e550246daa90412e711226bd320/coverage-7.2.7-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e"},
+    {url = "https://files.pythonhosted.org/packages/dd/ce/97c1dd6592c908425622fe7f31c017d11cf0421729b09101d4de75bcadc8/coverage-7.2.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5"},
+    {url = "https://files.pythonhosted.org/packages/de/a3/5a98dc9e239d0dc5f243ef5053d5b1bdcaa1dee27a691dfc12befeccf878/coverage-7.2.7-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f"},
+    {url = "https://files.pythonhosted.org/packages/e2/c0/73f139794c742840b9ab88e2e17fe14a3d4668a166ff95d812ac66c0829d/coverage-7.2.7-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd"},
+    {url = "https://files.pythonhosted.org/packages/e9/40/383305500d24122dbed73e505a4d6828f8f3356d1f68ab6d32c781754b81/coverage-7.2.7-cp37-cp37m-win32.whl", hash = "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f"},
+    {url = "https://files.pythonhosted.org/packages/fe/57/e4f8ad64d84ca9e759d783a052795f62a9f9111585e46068845b1cb52c2b/coverage-7.2.7-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1"},
+    {url = "https://files.pythonhosted.org/packages/ff/d5/52fa1891d1802ab2e1b346d37d349cb41cdd4fd03f724ebbf94e80577687/coverage-7.2.7-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4"},
+]
+"cryptography 41.0.1" = [
+    {url = "https://files.pythonhosted.org/packages/00/5e/39850ff94df530b24c5600f56769d56da44ede9f2c6ef5f2a204dd6c0881/cryptography-41.0.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5"},
+    {url = "https://files.pythonhosted.org/packages/06/04/71b679d76336fc5fd82041e492e4c372c6b605dba15047e3184654aa5fc7/cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c"},
+    {url = "https://files.pythonhosted.org/packages/12/82/8d41bda1fc6e5a51ae4f47abc910e40c0207233bf44f2bcd794272db2c69/cryptography-41.0.1-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca"},
+    {url = "https://files.pythonhosted.org/packages/19/8c/47f061de65d1571210dc46436c14a0a4c260fd0f3eaf61ce9b9d445ce12f/cryptography-41.0.1.tar.gz", hash = "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006"},
+    {url = "https://files.pythonhosted.org/packages/2c/74/5ccc293b24678010611eb43185663064a9c195cdebfbcef8fc323f71eb41/cryptography-41.0.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485"},
+    {url = "https://files.pythonhosted.org/packages/2d/18/1c1098a3faeb21e73d83acccaa01f25bcfe6218f59b8dfc59bc31505cbe0/cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3"},
+    {url = "https://files.pythonhosted.org/packages/32/86/2037a52402f8d03f7a2be172ffb4bbac0250c54e51d50136c0c6c4e0cf70/cryptography-41.0.1-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43"},
+    {url = "https://files.pythonhosted.org/packages/49/35/80c346e1a9509210defa857a05e9b7931093719aab25665d4d54f9b3ba83/cryptography-41.0.1-cp37-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3"},
+    {url = "https://files.pythonhosted.org/packages/52/4c/a5b0cabca7033510d490b5a9fddce62f87a0420ddc4d96b1ab4435f10f75/cryptography-41.0.1-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31"},
+    {url = "https://files.pythonhosted.org/packages/6a/35/7d7ac1ecd59c88f760584d3b9606ebfd48c5442377d67a8d3081226be424/cryptography-41.0.1-cp37-abi3-win_amd64.whl", hash = "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c"},
+    {url = "https://files.pythonhosted.org/packages/92/12/f33c6911b70c59b92af870b2e4a8c11f8293a12a4d1318be96082e09318f/cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a"},
+    {url = "https://files.pythonhosted.org/packages/a6/09/ac646c5f3ae56a2a895014ede63148a6e2be2689d7bfbdbaab02ed9fe684/cryptography-41.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc"},
+    {url = "https://files.pythonhosted.org/packages/b7/88/3e6c5eda9ab474fa9b0cf84e6119385aaefbe5c9700a5eacd6e0a9f415bb/cryptography-41.0.1-cp37-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b"},
+    {url = "https://files.pythonhosted.org/packages/c9/f1/94c71c6fd96ae2ec799c8e5d7a953944a7c7b2ddd8ba941ddc89443645c3/cryptography-41.0.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb"},
+    {url = "https://files.pythonhosted.org/packages/d8/80/e32f30266381f6ca05ee4aa92ce5f305aa1acbef4117a9a8d94d9b60bb67/cryptography-41.0.1-cp37-abi3-macosx_10_12_universal2.whl", hash = "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"},
+    {url = "https://files.pythonhosted.org/packages/e5/1d/184779dc4c1e9686bc87628c0bf1b1c846885c6c9ff79c954fda0a4b2498/cryptography-41.0.1-cp37-abi3-win32.whl", hash = "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5"},
+    {url = "https://files.pythonhosted.org/packages/eb/09/6b2c7f6dcf756f318cc232576c2198c114758510317ddade9490e568362a/cryptography-41.0.1-cp37-abi3-macosx_10_12_x86_64.whl", hash = "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a"},
+    {url = "https://files.pythonhosted.org/packages/ef/78/d391ec7a08d4adf8a93d0fd9fa9fd468493ef50b6213c28deadf5322379d/cryptography-41.0.1-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db"},
+    {url = "https://files.pythonhosted.org/packages/fc/db/bccda95237c4a823164d2f243aac25036f8d81c1083a49e85457d185dd31/cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039"},
 ]
 "distlib 0.3.6" = [
     {url = "https://files.pythonhosted.org/packages/58/07/815476ae605bcc5f95c87a62b95e74a1bce0878bc7a3119bc2bf4178f175/distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
     {url = "https://files.pythonhosted.org/packages/76/cb/6bbd2b10170ed991cf64e8c8b85e01f2fb38f95d1bc77617569e0b0b26ac/distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
 ]
-"exceptiongroup 1.1.1" = [
-    {url = "https://files.pythonhosted.org/packages/61/97/17ed81b7a8d24d8f69b62c0db37abbd8c0042d4b3fc429c73dab986e7483/exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
-    {url = "https://files.pythonhosted.org/packages/cc/38/57f14ddc8e8baeddd8993a36fe57ce7b4ba174c35048b9a6d270bb01e833/exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
-]
-"filelock 3.10.0" = [
-    {url = "https://files.pythonhosted.org/packages/4f/1f/6e1b740698069650b245744957a25957d599b953550a959ab2a584a8825b/filelock-3.10.0.tar.gz", hash = "sha256:3199fd0d3faea8b911be52b663dfccceb84c95949dd13179aa21436d1a79c4ce"},
-    {url = "https://files.pythonhosted.org/packages/9a/eb/95844b279593fd79c0a4d5eadad029203528509bccb0efe117543e1a1704/filelock-3.10.0-py3-none-any.whl", hash = "sha256:e90b34656470756edf8b19656785c5fea73afa1953f3e1b0d645cef11cab3182"},
+"execnet 1.9.0" = [
+    {url = "https://files.pythonhosted.org/packages/7a/3c/b5ac9fc61e1e559ced3e40bf5b518a4142536b34eb274aa50dff29cb89f5/execnet-1.9.0.tar.gz", hash = "sha256:8f694f3ba9cc92cab508b152dcfe322153975c29bda272e2fd7f3f00f36e47c5"},
+    {url = "https://files.pythonhosted.org/packages/81/c0/3072ecc23f4c5e0a1af35e3a222855cfd9c80a1a105ca67be3b6172637dd/execnet-1.9.0-py2.py3-none-any.whl", hash = "sha256:a295f7cc774947aac58dde7fdc85f4aa00c42adf5d8f5468fc630c1acf30a142"},
+]
+"filelock 3.12.2" = [
+    {url = "https://files.pythonhosted.org/packages/00/0b/c506e9e44e4c4b6c89fcecda23dc115bf8e7ff7eb127e0cb9c114cbc9a15/filelock-3.12.2.tar.gz", hash = "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81"},
+    {url = "https://files.pythonhosted.org/packages/00/45/ec3407adf6f6b5bf867a4462b2b0af27597a26bd3cd6e2534cb6ab029938/filelock-3.12.2-py3-none-any.whl", hash = "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"},
 ]
 "flake8 6.0.0" = [
     {url = "https://files.pythonhosted.org/packages/66/53/3ad4a3b74d609b3b9008a10075c40e7c8909eae60af53623c3888f7a529a/flake8-6.0.0.tar.gz", hash = "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"},
     {url = "https://files.pythonhosted.org/packages/d9/6a/bb0122ebe280476c924470779d2595f1403878cafe3c8a343ac56a5a9c0e/flake8-6.0.0-py2.py3-none-any.whl", hash = "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7"},
 ]
-"flake8-pyi 23.3.0" = [
-    {url = "https://files.pythonhosted.org/packages/76/a7/330f055c0015211b363f43666ed20d1095f64a96f4e4f6102f64381a003f/flake8_pyi-23.3.0-py3-none-any.whl", hash = "sha256:30789ae75b95537e51de9cb091d91f7a15dcc431531b9da453a7c95477251009"},
-    {url = "https://files.pythonhosted.org/packages/a7/ab/389188998129818cf2e69d35ee14b171650e443b66399a4e99cf41c8d427/flake8_pyi-23.3.0.tar.gz", hash = "sha256:59e030e4412e78a8a16cc5bbb9e17d4f41e640fc8e230f09144b362a07b7c41d"},
-]
-"identify 2.5.21" = [
-    {url = "https://files.pythonhosted.org/packages/85/0d/5d875ec52e1a0b8290d5cf1995f1afc9f6830146b8c6565d800b47522e46/identify-2.5.21.tar.gz", hash = "sha256:7671a05ef9cfaf8ff63b15d45a91a1147a03aaccb2976d4e9bd047cbbc508471"},
-    {url = "https://files.pythonhosted.org/packages/bc/d3/717d212dafbf2c5cd837f0b4f5eb10202a2a1f20b171c4bfdd09d5603229/identify-2.5.21-py2.py3-none-any.whl", hash = "sha256:69edcaffa8e91ae0f77d397af60f148b6b45a8044b2cc6d99cafa5b04793ff00"},
+"flake8-pyi 23.5.0" = [
+    {url = "https://files.pythonhosted.org/packages/58/ac/625d0b7dafef5752c1910cbc13d8bcc38d597ff3f44208c0d5c9176ee227/flake8_pyi-23.5.0-py3-none-any.whl", hash = "sha256:6806822a7eea0343b2583c088d73983b7c0c022b3810f403fd1b6edda053b7e1"},
+    {url = "https://files.pythonhosted.org/packages/b0/4f/ca2fd3f9bd77be3485154952b38030d586bc1ae3e292bda21234af1f3f53/flake8_pyi-23.5.0.tar.gz", hash = "sha256:a1038d5a4bb679fb0c142c5ed14da308c6ef99b0138ff5f5e6c65e47d2a7d23e"},
+]
+"identify 2.5.24" = [
+    {url = "https://files.pythonhosted.org/packages/4f/fd/2c46fba2bc032ba4c970bb8de59d25187087d7138a0ebf7c1dcc91d94f01/identify-2.5.24-py2.py3-none-any.whl", hash = "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"},
+    {url = "https://files.pythonhosted.org/packages/c4/f8/498e13e408d25ee6ff04aa0acbf91ad8e9caae74be91720fc0e811e649b7/identify-2.5.24.tar.gz", hash = "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4"},
+]
+"idna 3.4" = [
+    {url = "https://files.pythonhosted.org/packages/8b/e1/43beb3d38dba6cb420cefa297822eac205a277ab43e5ba5d5c46faf96438/idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
+    {url = "https://files.pythonhosted.org/packages/fc/34/3030de6f1370931b9dbb4dad48f6ab1015ab1d32447850b9fc94e60097be/idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
 ]
 "iniconfig 2.0.0" = [
     {url = "https://files.pythonhosted.org/packages/d7/4b/cbd8e699e64a6f16ca3a8220661b5f83792b3017d0f79807cb8708d33913/iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
     {url = "https://files.pythonhosted.org/packages/ef/a6/62565a6e1cf69e10f5727360368e451d4b7f58beeac6173dc9db836a5b46/iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
 ]
 "isort 5.12.0" = [
     {url = "https://files.pythonhosted.org/packages/0a/63/4036ae70eea279c63e2304b91ee0ac182f467f24f86394ecfe726092340b/isort-5.12.0-py3-none-any.whl", hash = "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"},
     {url = "https://files.pythonhosted.org/packages/a9/c4/dc00e42c158fc4dda2afebe57d2e948805c06d5169007f1724f0683010a9/isort-5.12.0.tar.gz", hash = "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504"},
 ]
 "mccabe 0.7.0" = [
     {url = "https://files.pythonhosted.org/packages/27/1a/1f68f9ba0c207934b35b86a8ca3aad8395a3d6dd7921c0686e23853ff5a9/mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {url = "https://files.pythonhosted.org/packages/e7/ff/0ffefdcac38932a54d2b5eed4e0ba8a408f215002cd178ad1df0f2806ff8/mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
-"mypy 0.991" = [
-    {url = "https://files.pythonhosted.org/packages/0e/5c/fbe112ca73d4c6a9e65336f48099c60800514d8949b4129c093a84a28dc8/mypy-0.991.tar.gz", hash = "sha256:3c0165ba8f354a6d9881809ef29f1a9318a236a6d81c690094c5df32107bde06"},
-    {url = "https://files.pythonhosted.org/packages/14/05/5a4206e269268f4aecb1096bf2375a231c959987ccf3e31313221b8bc153/mypy-0.991-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:37bd02ebf9d10e05b00d71302d2c2e6ca333e6c2a8584a98c00e038db8121f05"},
-    {url = "https://files.pythonhosted.org/packages/28/9c/e1805f2fea93a92671f33b00dd577119f37e4a8b859d6f6ea62d3e9129fa/mypy-0.991-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:1c8cd4fb70e8584ca1ed5805cbc7c017a3d1a29fb450621089ffed3e99d1857f"},
-    {url = "https://files.pythonhosted.org/packages/33/20/c4c15c9e9b7929ef44e35e83c0bcc254c8bf5998bbef0954ae658288e8c6/mypy-0.991-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:b86ce2c1866a748c0f6faca5232059f881cda6dda2a893b9a8373353cfe3715a"},
-    {url = "https://files.pythonhosted.org/packages/39/05/7a7d58afc7d00e819e553ad2485a29141e14575e3b0c43b9da6f869ede4c/mypy-0.991-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bc9ec663ed6c8f15f4ae9d3c04c989b744436c16d26580eaa760ae9dd5d662eb"},
-    {url = "https://files.pythonhosted.org/packages/44/d0/81d47bffc80d0cff84174aab266adc3401e735e13c5613418e825c146986/mypy-0.991-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:7d17e0a9707d0772f4a7b878f04b4fd11f6f5bcb9b3813975a9b13c9332153ab"},
-    {url = "https://files.pythonhosted.org/packages/49/83/34d682a10604845d77a0e7dbde1d0e70f3784d0f67b0df11d2eaf7bb8360/mypy-0.991-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a12c56bf73cdab116df96e4ff39610b92a348cc99a1307e1da3c3768bbb5b135"},
-    {url = "https://files.pythonhosted.org/packages/4b/98/125e5d14222de8e92f44314f8df21a9c351b531b37c551526acd67486a7d/mypy-0.991-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:26efb2fcc6b67e4d5a55561f39176821d2adf88f2745ddc72751b7890f3194ad"},
-    {url = "https://files.pythonhosted.org/packages/5d/c8/fc9b7cd600330e8c9dbd52b499a76eeaf4b48969a605fb50415a9d361d5b/mypy-0.991-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:652b651d42f155033a1967739788c436491b577b6a44e4c39fb340d0ee7f0d70"},
-    {url = "https://files.pythonhosted.org/packages/6b/22/5e19d1a6f8e029296e7b2fa462d8753fb4365126684c2f840dcb1447e6e8/mypy-0.991-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6d7464bac72a85cb3491c7e92b5b62f3dcccb8af26826257760a552a5e244aa5"},
-    {url = "https://files.pythonhosted.org/packages/80/23/76e56e004acca691b4da4086a8c38bd67b7ae73536848dcab76cfed5c188/mypy-0.991-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:4307270436fd7694b41f913eb09210faff27ea4979ecbcd849e57d2da2f65305"},
-    {url = "https://files.pythonhosted.org/packages/87/ec/62fd00fa5d8ead3ecafed3eb99ee805911f41b11536c5940df1bcb2c845d/mypy-0.991-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0c8f3be99e8a8bd403caa8c03be619544bc2c77a7093685dcf308c6b109426c6"},
-    {url = "https://files.pythonhosted.org/packages/89/76/7159258fdbf26a5ceef100b80a82d2f79b9066725a5daeb6383a8f773910/mypy-0.991-cp311-cp311-win_amd64.whl", hash = "sha256:3a700330b567114b673cf8ee7388e949f843b356a73b5ab22dd7cff4742a5297"},
-    {url = "https://files.pythonhosted.org/packages/90/a5/3a2c0c02e99a845318cc25556097d96eb8eb85fe53619ac8ff37b44acc46/mypy-0.991-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3d80e36b7d7a9259b740be6d8d906221789b0d836201af4234093cae89ced0cd"},
-    {url = "https://files.pythonhosted.org/packages/91/27/716b1cfce990cb58dc92f6601852141bc25e1524c06b3f3a39b0de6d9210/mypy-0.991-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:c9166b3f81a10cdf9b49f2d594b21b31adadb3d5e9db9b834866c3258b695be3"},
-    {url = "https://files.pythonhosted.org/packages/97/e3/1da0f08c60f555c04b93eff4016611fa1858ea53111dbdc757a37c234042/mypy-0.991-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:641411733b127c3e0dab94c45af15fea99e4468f99ac88b39efb1ad677da5711"},
-    {url = "https://files.pythonhosted.org/packages/9b/b1/0d5f1549c2894fd9af744e886156870d98ea0b1784952989f10e51eb0030/mypy-0.991-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:1f7d1a520373e2272b10796c3ff721ea1a0712288cafaa95931e66aa15798813"},
-    {url = "https://files.pythonhosted.org/packages/ac/a6/e4d6dca539c637735d0d93f1eee3ac35cedfd9c047da7386b3a59e93f35b/mypy-0.991-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5e80e758243b97b618cdf22004beb09e8a2de1af481382e4d84bc52152d1c476"},
-    {url = "https://files.pythonhosted.org/packages/af/9a/ee3b76f36e90ecb5e44dd2827bf5992d02c127192366a4c7864cfeab95b6/mypy-0.991-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:0cca5adf694af539aeaa6ac633a7afe9bbd760df9d31be55ab780b77ab5ae8bf"},
-    {url = "https://files.pythonhosted.org/packages/b1/30/24a92552a7c3df25db5a2e56ae359b4aa9bba6aebc8f0e25523a94e5c1e7/mypy-0.991-cp37-cp37m-win_amd64.whl", hash = "sha256:e62ebaad93be3ad1a828a11e90f0e76f15449371ffeecca4a0a0b9adc99abcef"},
-    {url = "https://files.pythonhosted.org/packages/b8/ab/aa2e02fce8ee8885fe98ee2a0549290e9de5caa28febc0cf243bfab020e7/mypy-0.991-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:d13674f3fb73805ba0c45eb6c0c3053d218aa1f7abead6e446d474529aafc372"},
-    {url = "https://files.pythonhosted.org/packages/bc/b2/6e71e47b259992dcd99d257ce452c0de3f711be713d048fe8f0fda9a9996/mypy-0.991-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:98e781cd35c0acf33eb0295e8b9c55cdbef64fcb35f6d3aa2186f289bed6e80d"},
-    {url = "https://files.pythonhosted.org/packages/ca/0d/da98f81e7c13a60111dc10a16cbf1b48dc8500df90a1fc959878a5981f49/mypy-0.991-cp39-cp39-win_amd64.whl", hash = "sha256:74e259b5c19f70d35fcc1ad3d56499065c601dfe94ff67ae48b85596b9ec1461"},
-    {url = "https://files.pythonhosted.org/packages/d7/f4/dcab9f3c5ed410caca1b9374dbb2b2caa778d225e32f174e266e20291edf/mypy-0.991-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:0714258640194d75677e86c786e80ccf294972cc76885d3ebbb560f11db0003d"},
-    {url = "https://files.pythonhosted.org/packages/df/bb/3cf400e05e30939a0fc58b34e0662d8abe8e206464665065b56cf2ca9a62/mypy-0.991-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:209ee89fbb0deed518605edddd234af80506aec932ad28d73c08f1400ef80a33"},
-    {url = "https://files.pythonhosted.org/packages/e3/84/188ddeaebfc8b5bbdcc3c7f05c09b61758540b2df84aad0146263d66960a/mypy-0.991-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:ac6e503823143464538efda0e8e356d871557ef60ccd38f8824a4257acc18d93"},
-    {url = "https://files.pythonhosted.org/packages/e7/a1/c503a15ad69ff133a76c159b8287f0eadc1f521d9796bf81f935886c98f6/mypy-0.991-py3-none-any.whl", hash = "sha256:de32edc9b0a7e67c2775e574cb061a537660e51210fbf6006b0b36ea695ae9bb"},
-    {url = "https://files.pythonhosted.org/packages/e9/7e/cc2de45afb46fee694bf285f91df3e227a3b0c671f775524814549c26556/mypy-0.991-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b8472f736a5bfb159a5e36740847808f6f5b659960115ff29c7cecec1741c648"},
-    {url = "https://files.pythonhosted.org/packages/f3/1d/cc67a674f1cd7f1c10619487a4245185f6f8f14cbd685b60709318e9ac27/mypy-0.991-cp310-cp310-win_amd64.whl", hash = "sha256:901c2c269c616e6cb0998b33d4adbb4a6af0ac4ce5cd078afd7bc95830e62c1c"},
-    {url = "https://files.pythonhosted.org/packages/f7/3a/19c01d59d24f1f36fabdeb61a286b4fc5e0456bf6211f5159ad5ebb5f735/mypy-0.991-cp38-cp38-win_amd64.whl", hash = "sha256:4175593dc25d9da12f7de8de873a33f9b2b8bdb4e827a7cae952e5b1a342e243"},
+"msgpack 1.0.5" = [
+    {url = "https://files.pythonhosted.org/packages/0a/04/bc319ba061f6dc9077745988be288705b3f9f18c5a209772a3e8fcd419fd/msgpack-1.0.5-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9985b214f33311df47e274eb788a5893a761d025e2b92c723ba4c63936b69b1"},
+    {url = "https://files.pythonhosted.org/packages/0d/90/44edef4a8c6f035b054c4b017c5adcb22a35ec377e17e50dd5dced279a6b/msgpack-1.0.5-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:916723458c25dfb77ff07f4c66aed34e47503b2eb3188b3adbec8d8aa6e00f48"},
+    {url = "https://files.pythonhosted.org/packages/0e/69/3d10e741dd2bbb806af5cdc76551735baab5f5f9773701eb05502c913a6e/msgpack-1.0.5-cp311-cp311-win32.whl", hash = "sha256:c396e2cc213d12ce017b686e0f53497f94f8ba2b24799c25d913d46c08ec422c"},
+    {url = "https://files.pythonhosted.org/packages/10/ca/50c3a5e92d459a942169747315afd8c226d05427eccff903ddf33135c574/msgpack-1.0.5-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:20a97bf595a232c3ee6d57ddaadd5453d174a52594bf9c21d10407e2a2d9b3bd"},
+    {url = "https://files.pythonhosted.org/packages/10/fe/9e004c4deb457f1ef1ad88c1188da5691ff1855e0d03a5ac3635ae1f6530/msgpack-1.0.5-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:55b56a24893105dc52c1253649b60f475f36b3aa0fc66115bffafb624d7cb30b"},
+    {url = "https://files.pythonhosted.org/packages/12/6e/0cfd1dc07f61a6ac606587a393f489c3ca463469d285a73c8e5e2f61b021/msgpack-1.0.5-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:20c784e66b613c7f16f632e7b5e8a1651aa5702463d61394671ba07b2fc9e025"},
+    {url = "https://files.pythonhosted.org/packages/17/10/be97811782473d709d07b65a3955a5a76d47686aff3d62bb41d48aea7c92/msgpack-1.0.5-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:362d9655cd369b08fda06b6657a303eb7172d5279997abe094512e919cf74b11"},
+    {url = "https://files.pythonhosted.org/packages/18/3f/3860151fbdf50e369bbe4ffd307a588417669c725025e383f3ce5893690f/msgpack-1.0.5-cp39-cp39-win32.whl", hash = "sha256:ac9dd47af78cae935901a9a500104e2dea2e253207c924cc95de149606dc43cc"},
+    {url = "https://files.pythonhosted.org/packages/19/0c/2c3b443df88f5d400f2e19a3d867564d004b26e137f18c2f2663913987bc/msgpack-1.0.5-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:476a8fe8fae289fdf273d6d2a6cb6e35b5a58541693e8f9f019bfe990a51e4ba"},
+    {url = "https://files.pythonhosted.org/packages/1a/f7/df5814697c25bdebb14ea97d27ddca04f5d4c6e249f096d086fea521c139/msgpack-1.0.5-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:b72d0698f86e8d9ddf9442bdedec15b71df3598199ba33322d9711a19f08145c"},
+    {url = "https://files.pythonhosted.org/packages/27/ad/4edfe383ec3185611441179ffee8cbc8155d7575fbad73f6d31015e35451/msgpack-1.0.5-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:9f5ae84c5c8a857ec44dc180a8b0cc08238e021f57abdf51a8182e915e6299f0"},
+    {url = "https://files.pythonhosted.org/packages/28/8f/c58c53c884217cc572c19349c7e1129b5a6eae36df0a017aae3a8f3d7aa8/msgpack-1.0.5-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:addab7e2e1fcc04bd08e4eb631c2a90960c340e40dfc4a5e24d2ff0d5a3b3edb"},
+    {url = "https://files.pythonhosted.org/packages/29/56/1fb6b96aab759ab3bc05b03ba6d936b350db72aac203cde56ea6bd001237/msgpack-1.0.5-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d25dd59bbbbb996eacf7be6b4ad082ed7eacc4e8f3d2df1ba43822da9bfa122a"},
+    {url = "https://files.pythonhosted.org/packages/2b/c4/f2c8695ae69d1425eddc5e2f849c525b562dc8409bc2979e525f3dd4fecd/msgpack-1.0.5-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:56a62ec00b636583e5cb6ad313bbed36bb7ead5fa3a3e38938503142c72cba4f"},
+    {url = "https://files.pythonhosted.org/packages/2b/d4/9165cf113f9b86ce55e36f36bc6cd9e0c5601b0ade02741b2ead8b5dc254/msgpack-1.0.5-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:a2b031c2e9b9af485d5e3c4520f4220d74f4d222a5b8dc8c1a3ab9448ca79c57"},
+    {url = "https://files.pythonhosted.org/packages/2c/e9/c79ecc36cfa34d850a01773565e0fccafd69efff07172028c3a5f758b83f/msgpack-1.0.5-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:b2de4c1c0538dcb7010902a2b97f4e00fc4ddf2c8cda9749af0e594d3b7fa3d7"},
+    {url = "https://files.pythonhosted.org/packages/2f/21/e488871f8e498efe14821b0c870eb95af52cfafb9b8dd41d83fad85b383b/msgpack-1.0.5-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:48296af57cdb1d885843afd73c4656be5c76c0c6328db3440c9601a98f303d87"},
+    {url = "https://files.pythonhosted.org/packages/33/0a/aa7b53ae17cf1dc1c352d705ab3162fc572c55048cc3177c1a88009c47fd/msgpack-1.0.5-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1ab2f3331cb1b54165976a9d976cb251a83183631c88076613c6c780f0d6e45a"},
+    {url = "https://files.pythonhosted.org/packages/33/52/099f0dde1283bac7bf267ab941dfa3b7c89ee701e4252973f8d3c10e68d6/msgpack-1.0.5-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:379026812e49258016dd84ad79ac8446922234d498058ae1d415f04b522d5b2d"},
+    {url = "https://files.pythonhosted.org/packages/34/3c/34e94b091b3fdf941dbce5bc619e2fa5488d49fdf00944b50f5a1d6e1871/msgpack-1.0.5-cp36-cp36m-win32.whl", hash = "sha256:b5ef2f015b95f912c2fcab19c36814963b5463f1fb9049846994b007962743e9"},
+    {url = "https://files.pythonhosted.org/packages/3c/e5/3d436bed11849ba05d777ed3fd1a0440170bad460335ea541dd6946047ed/msgpack-1.0.5-cp310-cp310-win_amd64.whl", hash = "sha256:4867aa2df9e2a5fa5f76d7d5565d25ec76e84c106b55509e78c1ede0f152659a"},
+    {url = "https://files.pythonhosted.org/packages/3e/80/bc7fdb75a35bf32c7c529c247dcadfd0502aac2309e207a89b0be6fe42ea/msgpack-1.0.5-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5cb47c21a8a65b165ce29f2bec852790cbc04936f502966768e4aae9fa763cb7"},
+    {url = "https://files.pythonhosted.org/packages/43/87/6507d56f62b958d822ae4ffe1c4507ed7d3cf37ad61114665816adcf4adc/msgpack-1.0.5-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a740fa0e4087a734455f0fc3abf5e746004c9da72fbd541e9b113013c8dc3282"},
+    {url = "https://files.pythonhosted.org/packages/45/85/6b55b0cabad846d3e730226a897f878f8f63ee505668bb6c55a697b0bfb0/msgpack-1.0.5-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:bf22a83f973b50f9d38e55c6aade04c41ddda19b00c4ebc558930d78eecc64ed"},
+    {url = "https://files.pythonhosted.org/packages/45/e1/6408389bd2cf0c339ea317926beb64d100f60bc8d236ac59f1c1162be2e4/msgpack-1.0.5-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b1d46dfe3832660f53b13b925d4e0fa1432b00f5f7210eb3ad3bb9a13c6204a6"},
+    {url = "https://files.pythonhosted.org/packages/49/57/a28120d82f8e77622a1e1efc652389c71145f6b89b47b39814a7c6038373/msgpack-1.0.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:57e1f3528bd95cc44684beda696f74d3aaa8a5e58c816214b9046512240ef437"},
+    {url = "https://files.pythonhosted.org/packages/4b/3d/cc5eb6d69e0ecde80a78cc42f48579971ec333e509d56a4a6de1a2c40ba2/msgpack-1.0.5-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:266fa4202c0eb94d26822d9bfd7af25d1e2c088927fe8de9033d929dd5ba24c5"},
+    {url = "https://files.pythonhosted.org/packages/56/50/bfcc0fad07067b6f1b09d940272ec749d5fe82570d938c2348c3ad0babf7/msgpack-1.0.5-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:821c7e677cc6acf0fd3f7ac664c98803827ae6de594a9f99563e48c5a2f27eb0"},
+    {url = "https://files.pythonhosted.org/packages/59/67/f992ada3b42889f1b984e5651d63ea21ca3a92049cff6d75fe0a4a63e422/msgpack-1.0.5-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e42b9594cc3bf4d838d67d6ed62b9e59e201862a25e9a157019e171fbe672dd3"},
+    {url = "https://files.pythonhosted.org/packages/60/bc/af94acdebc26b8d92d5673d20529438aa225698dc23338fb43c875c8968e/msgpack-1.0.5-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:f933bbda5a3ee63b8834179096923b094b76f0c7a73c1cfe8f07ad608c58844b"},
+    {url = "https://files.pythonhosted.org/packages/62/57/170af6c6fccd2d950ea01e1faa58cae9643226fa8705baded11eca3aa8b5/msgpack-1.0.5-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0c05a4a96585525916b109bb85f8cb6511db1c6f5b9d9cbcbc940dc6b4be944b"},
+    {url = "https://files.pythonhosted.org/packages/62/5c/9c7fed4ca0235a2d7b8d15b4047c328976b97d2b227719e54cad1e47c244/msgpack-1.0.5-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ef8108f8dedf204bb7b42994abf93882da1159728a2d4c5e82012edd92c9da9f"},
+    {url = "https://files.pythonhosted.org/packages/67/f8/e3ab674f4a945308362e9342297fe6b35a89dd0f648aa325aabffa5dc210/msgpack-1.0.5-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:3055b0455e45810820db1f29d900bf39466df96ddca11dfa6d074fa47054376d"},
+    {url = "https://files.pythonhosted.org/packages/6b/6d/de239d77d347f1990c41b4800075a15e06f748186dd120166270dd071734/msgpack-1.0.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28592e20bbb1620848256ebc105fc420436af59515793ed27d5c77a217477705"},
+    {url = "https://files.pythonhosted.org/packages/6b/79/0dec8f035160464ca88b221cc79691a71cf88dc25207c17f1d918b2c7bb0/msgpack-1.0.5-cp311-cp311-win_amd64.whl", hash = "sha256:6c4c68d87497f66f96d50142a2b73b97972130d93677ce930718f68828b382e2"},
+    {url = "https://files.pythonhosted.org/packages/6c/fa/3ca00fb1e53bcacf8c186fa6aff2d2086862b12e289bcf38227d9d40bd86/msgpack-1.0.5-cp39-cp39-win_amd64.whl", hash = "sha256:06f5174b5f8ed0ed919da0e62cbd4ffde676a374aba4020034da05fab67b9164"},
+    {url = "https://files.pythonhosted.org/packages/6c/fe/8a7747ca57074307a2e8f1de58441952a9dbdf9e8a8e5873d53a5ce0835c/msgpack-1.0.5-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5494ea30d517a3576749cad32fa27f7585c65f5f38309c88c6d137877fa28a5a"},
+    {url = "https://files.pythonhosted.org/packages/72/ac/2eda5af7cd1450c52d031e48c76b280eac5bb2e588678876612f95be34ab/msgpack-1.0.5-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:e57916ef1bd0fee4f21c4600e9d1da352d8816b52a599c46460e93a6e9f17086"},
+    {url = "https://files.pythonhosted.org/packages/73/99/f338ce8b69e934c04e5d9187f85de1ae395882cd56e7deb48e78a1749af8/msgpack-1.0.5-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:cdc793c50be3f01106245a61b739328f7dccc2c648b501e237f0699fe1395b81"},
+    {url = "https://files.pythonhosted.org/packages/7b/e9/b47f9e93fc381885624c40cbbbd0480b18ae11ca588162fe724d43495372/msgpack-1.0.5-cp310-cp310-win32.whl", hash = "sha256:382b2c77589331f2cb80b67cc058c00f225e19827dbc818d700f61513ab47bea"},
+    {url = "https://files.pythonhosted.org/packages/7e/1c/9d0fd241a4e88e1cd2f5babea4a27ac25b1b86dbbc05fa10741e82079a93/msgpack-1.0.5-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fe5c63197c55bce6385d9aee16c4d0641684628f63ace85f73571e65ad1c1e8d"},
+    {url = "https://files.pythonhosted.org/packages/80/f0/c1fadb4e4a38fda19e35b1b6f887d72cc9c57778af43b53f64a8cd62e922/msgpack-1.0.5-cp38-cp38-win32.whl", hash = "sha256:1c0f7c47f0087ffda62961d425e4407961a7ffd2aa004c81b9c07d9269512f6e"},
+    {url = "https://files.pythonhosted.org/packages/95/c9/560c3203c4327881c9f2de26c42dacdd9567bfe7fa43458e2a680c4bdcaf/msgpack-1.0.5-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:1967f6129fc50a43bfe0951c35acbb729be89a55d849fab7686004da85103f1c"},
+    {url = "https://files.pythonhosted.org/packages/9a/0b/ea8a49d24654f9e8604ea78b80a4d7b0cc31817d8fb6987001223ae7feaf/msgpack-1.0.5-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:36961b0568c36027c76e2ae3ca1132e35123dcec0706c4b7992683cc26c1320c"},
+    {url = "https://files.pythonhosted.org/packages/9f/4a/36d936e54cf71e23ad276564465f6a54fb129e3d61520b76e13e0bb29167/msgpack-1.0.5-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:525228efd79bb831cf6830a732e2e80bc1b05436b086d4264814b4b2955b2fa9"},
+    {url = "https://files.pythonhosted.org/packages/a2/e0/f3d5dd7809cf5728bb1bae683032ce50547d009be6551054815a8bf2a2da/msgpack-1.0.5-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:4c075728a1095efd0634a7dccb06204919a2f67d1893b6aa8e00497258bf926c"},
+    {url = "https://files.pythonhosted.org/packages/ab/ff/ca74e519c47139b6c08fb21db5ead2bd2eed6cb1225f9be69390cdb48182/msgpack-1.0.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:586d0d636f9a628ddc6a17bfd45aa5b5efaf1606d2b60fa5d87b8986326e933f"},
+    {url = "https://files.pythonhosted.org/packages/b8/bc/1d5fe4732dc78ff86aaf677596da08f0ae736e60ca8ab49c1f1c7366cb1a/msgpack-1.0.5-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ed40e926fa2f297e8a653c954b732f125ef97bdd4c889f243182299de27e2aa9"},
+    {url = "https://files.pythonhosted.org/packages/bf/68/032e62ad44f92ba6a4ae7c45054843cdec7f0c405ecdfd166f25123b0c47/msgpack-1.0.5-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:18334484eafc2b1aa47a6d42427da7fa8f2ab3d60b674120bce7a895a0a85bdd"},
+    {url = "https://files.pythonhosted.org/packages/c1/57/01f2d8805160f559ec21d095fc7576a26fbaed2475af24ce4a135c380c14/msgpack-1.0.5-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:9e6ca5d5699bcd89ae605c150aee83b5321f2115695e741b99618f4856c50898"},
+    {url = "https://files.pythonhosted.org/packages/c2/3b/70d1eaaafb451679663a72164c46fadfb93f59c90f584dcd77289f90e4c5/msgpack-1.0.5-cp36-cp36m-win_amd64.whl", hash = "sha256:288e32b47e67f7b171f86b030e527e302c91bd3f40fd9033483f2cacc37f327a"},
+    {url = "https://files.pythonhosted.org/packages/c5/c1/1b591574ba71481fbf38359a8fca5108e4ad130a6dbb9b2acb3e9277d0fe/msgpack-1.0.5-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:137850656634abddfb88236008339fdaba3178f4751b28f270d2ebe77a563b6c"},
+    {url = "https://files.pythonhosted.org/packages/ce/b8/89cb1809b076a4651169851aa1f98128b75cbfe14034b914c9040b13c4cf/msgpack-1.0.5-cp37-cp37m-win32.whl", hash = "sha256:cb5aaa8c17760909ec6cb15e744c3ebc2ca8918e727216e79607b7bbce9c8f77"},
+    {url = "https://files.pythonhosted.org/packages/d3/32/9b7a2dba9485dd7d201e4e00638fbf86e0d535a91653889c5b4dc813efdf/msgpack-1.0.5-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:366c9a7b9057e1547f4ad51d8facad8b406bab69c7d72c0eb6f529cf76d4b85f"},
+    {url = "https://files.pythonhosted.org/packages/da/46/855bdcbf004fd87b6a4451e8dcd61329439dcd9039887f71ca5085769216/msgpack-1.0.5-cp38-cp38-win_amd64.whl", hash = "sha256:bae7de2026cbfe3782c8b78b0db9cbfc5455e079f1937cb0ab8d133496ac55e1"},
+    {url = "https://files.pythonhosted.org/packages/dc/a1/eba11a0d4b764bc62966a565b470f8c6f38242723ba3057e9b5098678c30/msgpack-1.0.5.tar.gz", hash = "sha256:c075544284eadc5cddc70f4757331d99dcbc16b2bbd4849d15f8aae4cf36d31c"},
+    {url = "https://files.pythonhosted.org/packages/e8/1f/be19c9c9cfdcc2ae8ee8c65dbe5f281cc1f3331f9b9523735f39b090b448/msgpack-1.0.5-cp37-cp37m-win_amd64.whl", hash = "sha256:ab31e908d8424d55601ad7075e471b7d0140d4d3dd3272daf39c5c19d936bd82"},
+    {url = "https://files.pythonhosted.org/packages/e8/60/78906f564804aae23eb1102eca8b8830f1e08a649c179774c05fa7dc0aad/msgpack-1.0.5-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:17358523b85973e5f242ad74aa4712b7ee560715562554aa2134d96e7aa4cbbf"},
+    {url = "https://files.pythonhosted.org/packages/e9/f1/45b73a9e97f702bcb5f51569b93990e456bc969363e55122374c22ed7d24/msgpack-1.0.5-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:a61215eac016f391129a013c9e46f3ab308db5f5ec9f25811e811f96962599a8"},
+    {url = "https://files.pythonhosted.org/packages/ef/13/c110d89d5079169354394dc226e6f84d818722939bc1fe3f9c25f982e903/msgpack-1.0.5-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:1835c84d65f46900920b3708f5ba829fb19b1096c1800ad60bae8418652a951d"},
+    {url = "https://files.pythonhosted.org/packages/f1/1f/cc3e8274934c8323f6106dae22cba8bad413166f4efb3819573de58c215c/msgpack-1.0.5-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:332360ff25469c346a1c5e47cbe2a725517919892eda5cfaffe6046656f0b7bb"},
+    {url = "https://files.pythonhosted.org/packages/f2/da/770118f8d48e11cc9a2c7cb60d7d3c8016266526bd42c6ff5bd21013d099/msgpack-1.0.5-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:4f8d8b3bf1ff2672567d6b5c725a1b347fe838b912772aa8ae2bf70338d5a198"},
+    {url = "https://files.pythonhosted.org/packages/f5/80/ef9c31210ac580163c0de2db4fb3179c6a3f1228c18fd366280e01d9e5d2/msgpack-1.0.5-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4f837b93669ce4336e24d08286c38761132bc7ab29782727f8557e1eb21b2080"},
+]
+"msgpack-types 0.2.0" = [
+    {url = "https://files.pythonhosted.org/packages/36/28/c48d188f61f429ce8fa4fbeea0ec9319b37b6c9cd01f0949f2c88b9915c0/msgpack_types-0.2.0-py3-none-any.whl", hash = "sha256:7e5bce9e3bba9fe08ed14005ad107aa44ea8d4b779ec28b8db880826d4c67303"},
+    {url = "https://files.pythonhosted.org/packages/e8/65/ce10db8bf2f8f84734b58bb6883e9a6d7e698fe872c34454296239d1ab4c/msgpack-types-0.2.0.tar.gz", hash = "sha256:b6b7ce9f52599f9dc3497006be8cf6bed7bd2c83fa48c4df43ac6958b97b0720"},
+]
+"mypy 1.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/09/7b/8eb0d648352c61b08cb364d278b5c12c3f1c5841724fdd2929d7172b7eaf/mypy-1.3.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e"},
+    {url = "https://files.pythonhosted.org/packages/11/41/d24f93eefc89c650782bf1f9acfdb02a32f327b841058a5b0ce5857b60af/mypy-1.3.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85"},
+    {url = "https://files.pythonhosted.org/packages/25/c7/4735f81858a727e170279144600881fe3299aa7589ed585af6b788ea4556/mypy-1.3.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd"},
+    {url = "https://files.pythonhosted.org/packages/2b/27/4a26f91301804969194ee0dc9393843f10566d7fdf192ce11fc0218a989d/mypy-1.3.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d"},
+    {url = "https://files.pythonhosted.org/packages/3c/5d/b87339c1fdfec7d13899cd7ad2ee992801695114c1cf9e1645da264cd437/mypy-1.3.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305"},
+    {url = "https://files.pythonhosted.org/packages/47/f6/25c154bb1c479f2047093f0580c2c35ffc1ff007d52b7e50020cca60c010/mypy-1.3.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409"},
+    {url = "https://files.pythonhosted.org/packages/4c/10/530d2df4d57f46f77b8211cf9bbe090baacff02e7076f21f1bf08148d541/mypy-1.3.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8"},
+    {url = "https://files.pythonhosted.org/packages/55/e1/90487a3ea5a88b8f5c9d7fbf6f5fa7fcc8633d0132ce8364810a1da901c9/mypy-1.3.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152"},
+    {url = "https://files.pythonhosted.org/packages/5b/fb/0b1c90c635319b98dd65c6d6d6347413e42397e94057993011eeedeffbd9/mypy-1.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee"},
+    {url = "https://files.pythonhosted.org/packages/6a/d0/4681d84878cecfd911752016ab30566366f6de7296fdc977b746eb68bf45/mypy-1.3.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c"},
+    {url = "https://files.pythonhosted.org/packages/6a/d9/48de5203f4b6287a98fadcc47072b1bc69e3faaa39cba59a3a600b05a42c/mypy-1.3.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca"},
+    {url = "https://files.pythonhosted.org/packages/7e/75/021af7f0683ea19b9ad6a436e1b5c7cb39899c0f7b31040fa69b2395421e/mypy-1.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228"},
+    {url = "https://files.pythonhosted.org/packages/86/56/08c5ff6b2139f301d9aa56cb8e7b2a24d4faa6fc3e94234dfe7eeecc9c44/mypy-1.3.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"},
+    {url = "https://files.pythonhosted.org/packages/88/0e/646696eb8fe7658b752009a495054a0214ae8e659e9cbcde8181f16ae999/mypy-1.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae"},
+    {url = "https://files.pythonhosted.org/packages/8d/c8/681f4a19c62aa71bdc9ad3a4bc9a0fb8846bd0b5a8bc1b29d261c8025f80/mypy-1.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd"},
+    {url = "https://files.pythonhosted.org/packages/90/b6/a2d2ba604982af6034e3fcad17a464a66127be47f07b4587beec76e8f80b/mypy-1.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf"},
+    {url = "https://files.pythonhosted.org/packages/b1/ce/8d87f684bb7e2a520cfa9cd17b8dc686a83143bb12a3e1ac4ad6d8d4825c/mypy-1.3.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f"},
+    {url = "https://files.pythonhosted.org/packages/b1/e1/399e3dfeb2842e4a2634866e4ef8b69151d465b7a5ceb648d7f1296f17d0/mypy-1.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a"},
+    {url = "https://files.pythonhosted.org/packages/b8/36/6628916f94bb0816e1719117e1962750413ab408f83673ce7d571caf3960/mypy-1.3.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703"},
+    {url = "https://files.pythonhosted.org/packages/ba/ac/1c280246fc0c5239409f31e1a321f178ba11a9c6e5eaaf6d56f9ff627cdf/mypy-1.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017"},
+    {url = "https://files.pythonhosted.org/packages/c9/c5/f3e4ed59e08e3a728a15da198317edfcd13b7dc2215d52b5d85fce716285/mypy-1.3.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb"},
+    {url = "https://files.pythonhosted.org/packages/cd/b9/6abe1cd8ac8e70f12f43eebe6427814f9d36142d331eae5cc5bba77585a2/mypy-1.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf"},
+    {url = "https://files.pythonhosted.org/packages/d8/c6/de2e214a42b63d7ea0abef9f02a6da69cad6d532165bb7a8cc8291099a0c/mypy-1.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4"},
+    {url = "https://files.pythonhosted.org/packages/d9/79/82d452b409d7610944ba3a1a6079987d3ed6062cb8fe5c8850f26dafb6e0/mypy-1.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929"},
+    {url = "https://files.pythonhosted.org/packages/e3/f7/1fed3b24abb75f244fa6bc60ea03cd9d3d8ad225a4cfda7533042fe6d831/mypy-1.3.0-py3-none-any.whl", hash = "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897"},
+    {url = "https://files.pythonhosted.org/packages/f9/88/3bfe07521fb9e74b449cbc4367434067ec70bfd8a24c652fa3e0f9597389/mypy-1.3.0.tar.gz", hash = "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11"},
 ]
 "mypy-extensions 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/2a/e2/5d3f6ada4297caebe1a2add3b126fe800c96f56dbe5d1988a2cbe0b267aa/mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {url = "https://files.pythonhosted.org/packages/98/a4/1ab47638b92648243faf97a5aeb6ea83059cc3624972ab6b8d2316078d3f/mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
-"nodeenv 1.7.0" = [
-    {url = "https://files.pythonhosted.org/packages/96/a8/d3b5baead78adadacb99e7281b3e842126da825cf53df61688cfc8b8ff91/nodeenv-1.7.0-py2.py3-none-any.whl", hash = "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e"},
-    {url = "https://files.pythonhosted.org/packages/f3/9d/a28ecbd1721cd6c0ea65da6bfb2771d31c5d7e32d916a8f643b062530af3/nodeenv-1.7.0.tar.gz", hash = "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"},
-]
-"packaging 23.0" = [
-    {url = "https://files.pythonhosted.org/packages/47/d5/aca8ff6f49aa5565df1c826e7bf5e85a6df852ee063600c1efa5b932968c/packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
-    {url = "https://files.pythonhosted.org/packages/ed/35/a31aed2993e398f6b09a790a181a7927eb14610ee8bbf02dc14d31677f1c/packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
+"nodeenv 1.8.0" = [
+    {url = "https://files.pythonhosted.org/packages/1a/e6/6d2ead760a9ddb35e65740fd5a57e46aadd7b0c49861ab24f94812797a1c/nodeenv-1.8.0-py2.py3-none-any.whl", hash = "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"},
+    {url = "https://files.pythonhosted.org/packages/48/92/8e83a37d3f4e73c157f9fcf9fb98ca39bd94701a469dc093b34dca31df65/nodeenv-1.8.0.tar.gz", hash = "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2"},
+]
+"packaging 23.1" = [
+    {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pathspec 0.11.1" = [
     {url = "https://files.pythonhosted.org/packages/95/60/d93628975242cc515ab2b8f5b2fc831d8be2eff32f5a1be4776d49305d13/pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
     {url = "https://files.pythonhosted.org/packages/be/c8/551a803a6ebb174ec1c124e68b449b98a0961f0b737def601e3c1fbb4cfd/pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
 ]
-"platformdirs 3.1.1" = [
-    {url = "https://files.pythonhosted.org/packages/79/c4/f98a05535344f79699bbd494e56ac9efc986b7a253fe9f4dba7414a7f505/platformdirs-3.1.1.tar.gz", hash = "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa"},
-    {url = "https://files.pythonhosted.org/packages/7b/e1/593f693096c50411a2bf9571f66bc3be9d0f79a4a50e95aab581458b0e3c/platformdirs-3.1.1-py3-none-any.whl", hash = "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"},
+"platformdirs 3.6.0" = [
+    {url = "https://files.pythonhosted.org/packages/05/31/793923615e85deef0c25abf5d044b3f99f1348b620122ab184b7d3f70f21/platformdirs-3.6.0.tar.gz", hash = "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640"},
+    {url = "https://files.pythonhosted.org/packages/a7/4d/00f9fe4bbb3459da0d6c790b1526e5edebaeff2a80166eabb0a42f9e0a05/platformdirs-3.6.0-py3-none-any.whl", hash = "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
-"pre-commit 3.2.0" = [
-    {url = "https://files.pythonhosted.org/packages/59/5d/157a051b2a402d7d27eb7c478fd7c1a231b94779054b3d7aef1719378e2d/pre_commit-3.2.0.tar.gz", hash = "sha256:818f0d998059934d0f81bb3667e3ccdc32da6ed7ccaac33e43dc231561ddaaa9"},
-    {url = "https://files.pythonhosted.org/packages/c6/99/f068bcb1fd31ec4de7852732c99e5fc18d8f22bf3c471646b9f077a83c01/pre_commit-3.2.0-py2.py3-none-any.whl", hash = "sha256:f712d3688102e13c8e66b7d7dbd8934a6dda157e58635d89f7d6fecdca39ce8a"},
+"pre-commit 3.3.3" = [
+    {url = "https://files.pythonhosted.org/packages/35/0e/564c71fe3cdf59a4acaaccaea354d066e5d9044eba564dac070bb2075432/pre_commit-3.3.3.tar.gz", hash = "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"},
+    {url = "https://files.pythonhosted.org/packages/e3/b7/1d145c985d8be9729672a45b8b8113030ad60dff45dec592efc4e5f5897a/pre_commit-3.3.3-py2.py3-none-any.whl", hash = "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb"},
 ]
 "pycodestyle 2.10.0" = [
     {url = "https://files.pythonhosted.org/packages/06/6b/5ca0d12ef7dcf7d20dfa35287d02297f3e0f9e515da5183654c03a9636ce/pycodestyle-2.10.0.tar.gz", hash = "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053"},
     {url = "https://files.pythonhosted.org/packages/a2/54/001fdc0d69e8d0bb86c3423a6fa6dfada8cc26317c2635ab543e9ac411bd/pycodestyle-2.10.0-py2.py3-none-any.whl", hash = "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"},
 ]
 "pycparser 2.21" = [
     {url = "https://files.pythonhosted.org/packages/5e/0b/95d387f5f4433cb0f53ff7ad859bd2c6051051cebbb564f139a999ab46de/pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
     {url = "https://files.pythonhosted.org/packages/62/d5/5f610ebe421e85889f2e55e33b7f9a6795bd982198517d912eb1c76e1a53/pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
 ]
 "pyflakes 3.0.1" = [
     {url = "https://files.pythonhosted.org/packages/af/4c/b1c7008aa7788b3e26c06c60aa18da7d3aa1f00e344aa3f18ac92768854b/pyflakes-3.0.1-py2.py3-none-any.whl", hash = "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf"},
     {url = "https://files.pythonhosted.org/packages/f2/51/506ddcfab10d708e8460554cc1cf37c727a6a2cccbad8dfe57766cfce33c/pyflakes-3.0.1.tar.gz", hash = "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"},
 ]
-"pyproject-api 1.5.1" = [
-    {url = "https://files.pythonhosted.org/packages/23/6f/d02d1cab4a30998806687036e03ffecbf66e35df6bfab5a29f22ec61a075/pyproject_api-1.5.1.tar.gz", hash = "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9"},
-    {url = "https://files.pythonhosted.org/packages/3e/39/5b1d0ac2c8fddd06b68edb38cf813e0659d940f7781ab38e8ade1e3387a1/pyproject_api-1.5.1-py3-none-any.whl", hash = "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"},
-]
-"pytest 7.2.2" = [
-    {url = "https://files.pythonhosted.org/packages/b2/68/5321b5793bd506961bd40bdbdd0674e7de4fb873ee7cab33dd27283ad513/pytest-7.2.2-py3-none-any.whl", hash = "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e"},
-    {url = "https://files.pythonhosted.org/packages/b9/29/311895d9cd3f003dd58e8fdea36dd895ba2da5c0c90601836f7de79f76fe/pytest-7.2.2.tar.gz", hash = "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"},
-]
-"pytest-cov 4.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/ea/70/da97fd5f6270c7d2ce07559a19e5bf36a76f0af21500256f005a69d9beba/pytest-cov-4.0.0.tar.gz", hash = "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"},
-    {url = "https://files.pythonhosted.org/packages/fe/1f/9ec0ddd33bd2b37d6ec50bb39155bca4fe7085fa78b3b434c05459a860e3/pytest_cov-4.0.0-py3-none-any.whl", hash = "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b"},
+"pyproject-api 1.5.2" = [
+    {url = "https://files.pythonhosted.org/packages/6f/26/82a2773463e1b739b62e432cff62d39daf21b3172e5ace6213b7f2bbfad7/pyproject_api-1.5.2.tar.gz", hash = "sha256:999f58fa3c92b23ebd31a6bad5d1f87d456744d75e05391be7f5c729015d3d91"},
+    {url = "https://files.pythonhosted.org/packages/ce/a7/0666a457fe35518d998448a6606b5f66c4bf092864bac6ef7fc380da582b/pyproject_api-1.5.2-py3-none-any.whl", hash = "sha256:9cffcbfb64190f207444d7579d315f3278f2c04ba46d685fad93197b5326d348"},
+]
+"pytest 7.3.2" = [
+    {url = "https://files.pythonhosted.org/packages/58/2a/07c65fdc40846ecb8a9dcda2c38fcb5a06a3e39d08d4a4960916431951cb/pytest-7.3.2.tar.gz", hash = "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"},
+    {url = "https://files.pythonhosted.org/packages/7a/d0/de969198293cdea22b3a6fb99a99aeeddb7b3827f0823b33c5dc0734bbe5/pytest-7.3.2-py3-none-any.whl", hash = "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295"},
+]
+"pytest-asyncio 0.21.0" = [
+    {url = "https://files.pythonhosted.org/packages/66/73/817ddb37c627338ecbb96486c03fe69a19bef72de1b6bd641aa06fed13f4/pytest_asyncio-0.21.0-py3-none-any.whl", hash = "sha256:f2b3366b7cd501a4056858bd39349d5af19742aed2d81660b7998b6341c7eb9c"},
+    {url = "https://files.pythonhosted.org/packages/85/c7/9db0c6215f12f26b590c24acc96d048e03989315f198454540dff95109cd/pytest-asyncio-0.21.0.tar.gz", hash = "sha256:2b38a496aef56f56b0e87557ec313e11e1ab9276fc3863f6a7be0f1d0e415e1b"},
+]
+"pytest-cov 4.1.0" = [
+    {url = "https://files.pythonhosted.org/packages/7a/15/da3df99fd551507694a9b01f512a2f6cf1254f33601605843c3775f39460/pytest-cov-4.1.0.tar.gz", hash = "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6"},
+    {url = "https://files.pythonhosted.org/packages/a7/4b/8b78d126e275efa2379b1c2e09dc52cf70df16fc3b90613ef82531499d73/pytest_cov-4.1.0-py3-none-any.whl", hash = "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"},
 ]
 "pytest-mock 3.10.0" = [
     {url = "https://files.pythonhosted.org/packages/91/84/c951790e199cd54ddbf1021965b62a5415b81193ebdb4f4af2659fd06a73/pytest_mock-3.10.0-py3-none-any.whl", hash = "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b"},
     {url = "https://files.pythonhosted.org/packages/f6/2b/137a7db414aeaf3d753d415a2bc3b90aba8c5f61dff7a7a736d84b2ec60d/pytest-mock-3.10.0.tar.gz", hash = "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"},
 ]
+"pytest-xdist 3.3.1" = [
+    {url = "https://files.pythonhosted.org/packages/db/d1/70a67f79b31cb5cba09c96bc4590c6ac22608558664901df03fdee24f6a6/pytest_xdist-3.3.1-py3-none-any.whl", hash = "sha256:ff9daa7793569e6a68544850fd3927cd257cc03a7ef76c95e86915355e82b5f2"},
+    {url = "https://files.pythonhosted.org/packages/e2/5c/eae1b20cbea054d4e11ca5cb4f9b163000e885a2ae62e433375e8cdf1097/pytest-xdist-3.3.1.tar.gz", hash = "sha256:d5ee0520eb1b7bcca50a60a518ab7a7707992812c578198f8b44fdfac78e8c93"},
+]
 "pyyaml 6.0" = [
     {url = "https://files.pythonhosted.org/packages/02/25/6ba9f6bb50a3d4fbe22c1a02554dc670682a07c8701d1716d19ddea2c940/PyYAML-6.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"},
     {url = "https://files.pythonhosted.org/packages/08/f4/ffa743f860f34a5e8c60abaaa686f82c9ac7a2b50e5a1c3b1eb564d59159/PyYAML-6.0-cp39-cp39-win_amd64.whl", hash = "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c"},
     {url = "https://files.pythonhosted.org/packages/0f/93/5f81d1925ce3b531f5ff215376445ec220887cd1c9a8bde23759554dbdfd/PyYAML-6.0-cp310-cp310-win32.whl", hash = "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513"},
     {url = "https://files.pythonhosted.org/packages/12/fc/a4d5a7554e0067677823f7265cb3ae22aed8a238560b5133b58cda252dad/PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0"},
     {url = "https://files.pythonhosted.org/packages/21/67/b42191239c5650c9e419c4a08a7a022bbf1abf55b0391c380a72c3af5462/PyYAML-6.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803"},
     {url = "https://files.pythonhosted.org/packages/2e/b3/13dfd4eeb5e4b2d686b6d1822b40702e991bf3a4194ca5cbcce8d43749db/PyYAML-6.0-cp39-cp39-win32.whl", hash = "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb"},
@@ -756,27 +884,71 @@
     {url = "https://files.pythonhosted.org/packages/df/75/ee0565bbf65133e5b6ffa154db43544af96ea4c42439e6b58c1e0eb44b4e/PyYAML-6.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0"},
     {url = "https://files.pythonhosted.org/packages/eb/5f/6e6fe6904e1a9c67bc2ca5629a69e7a5a0b17f079da838bab98a1e548b25/PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9"},
     {url = "https://files.pythonhosted.org/packages/ef/ad/b443cce94539e57e1a745a845f95c100ad7b97593d7e104051e43f730ecd/PyYAML-6.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b"},
     {url = "https://files.pythonhosted.org/packages/f5/6f/b8b4515346af7c33d3b07cd8ca8ea0700ca72e8d7a750b2b87ac0268ca4e/PyYAML-6.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b"},
     {url = "https://files.pythonhosted.org/packages/f8/54/799b059314b13e1063473f76e908f44106014d18f54b16c83a16edccd5ec/PyYAML-6.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358"},
     {url = "https://files.pythonhosted.org/packages/fc/48/531ecd926fe0a374346dd811bf1eda59a95583595bb80eadad511f3269b8/PyYAML-6.0-cp311-cp311-win32.whl", hash = "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7"},
 ]
-"setuptools 67.6.0" = [
-    {url = "https://files.pythonhosted.org/packages/25/f3/d68c20919bc774c6cb127f1762f2f2f999d700a58198556e883dd3700e58/setuptools-67.6.0.tar.gz", hash = "sha256:2ee892cd5f29f3373097f5a814697e397cf3ce313616df0af11231e2ad118077"},
-    {url = "https://files.pythonhosted.org/packages/c3/9e/8a7ba2c9984a060daa6c6f9fff4d576b7ace3936239d6b771541eab972ed/setuptools-67.6.0-py3-none-any.whl", hash = "sha256:b78aaa36f6b90a074c1fa651168723acbf45d14cb1196b6f02c0fd07f17623b2"},
-]
-"tomli 2.0.1" = [
-    {url = "https://files.pythonhosted.org/packages/97/75/10a9ebee3fd790d20926a90a2547f0bf78f371b2f13aa822c759680ca7b9/tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
-    {url = "https://files.pythonhosted.org/packages/c0/3f/d7af728f075fb08564c5949a9c95e44352e23dee646869fa104a3b2060a3/tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
-]
-"tox 4.4.7" = [
-    {url = "https://files.pythonhosted.org/packages/66/94/72db9d8b1ce82274e462e0a128b19a3a1618f99900adbb37edf69ab29f9c/tox-4.4.7-py3-none-any.whl", hash = "sha256:da10ca1d809b99fae80b706b9dc9656b1daf505a395ac427d130a8a85502d08f"},
-    {url = "https://files.pythonhosted.org/packages/ad/65/5afee4b3e6d3fd242340b3c3a1d787f987c0aabe2597f6c7c44b04be6c51/tox-4.4.7.tar.gz", hash = "sha256:52c92a96e2c3fd47c5301e9c26f5a871466133d5376958c1ed95ef4ff4629cbe"},
-]
-"typing-extensions 4.5.0" = [
-    {url = "https://files.pythonhosted.org/packages/31/25/5abcd82372d3d4a3932e1fa8c3dbf9efac10cc7c0d16e78467460571b404/typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
-    {url = "https://files.pythonhosted.org/packages/d3/20/06270dac7316220643c32ae61694e451c98f8caf4c8eab3aa80a2bedf0df/typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
-]
-"virtualenv 20.21.0" = [
-    {url = "https://files.pythonhosted.org/packages/86/2f/35a79942c38d4ca89b444085d67900f713f1967446fdcefc8351619d7c65/virtualenv-20.21.0-py3-none-any.whl", hash = "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc"},
-    {url = "https://files.pythonhosted.org/packages/87/14/ca9890d58cd33d9122eb87ffec2f3c6be0714785f992a0fd3b56a3b6c993/virtualenv-20.21.0.tar.gz", hash = "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"},
+"setuptools 67.8.0" = [
+    {url = "https://files.pythonhosted.org/packages/03/20/630783571e76e5fa5f3e9f29398ca3ace377207b8196b54e0ffdf09f12c1/setuptools-67.8.0.tar.gz", hash = "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"},
+    {url = "https://files.pythonhosted.org/packages/f5/2c/074ab1c5be9c7d523d8d6d69d1f46f450fe7f11713147dc9e779aa4ca4ea/setuptools-67.8.0-py3-none-any.whl", hash = "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f"},
+]
+"sniffio 1.3.0" = [
+    {url = "https://files.pythonhosted.org/packages/c3/a0/5dba8ed157b0136607c7f2151db695885606968d1fae123dc3391e0cfdbf/sniffio-1.3.0-py3-none-any.whl", hash = "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"},
+    {url = "https://files.pythonhosted.org/packages/cd/50/d49c388cae4ec10e8109b1b833fd265511840706808576df3ada99ecb0ac/sniffio-1.3.0.tar.gz", hash = "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101"},
+]
+"tox 4.6.2" = [
+    {url = "https://files.pythonhosted.org/packages/1d/c8/965a461a5bdce62275ed274bf2acabe64f56a43bb9acedf035827eba0d84/tox-4.6.2.tar.gz", hash = "sha256:58c7c2acce2f3d44cd1b359349557162336288ecf19ef53ccda89c9cee0ad9c4"},
+    {url = "https://files.pythonhosted.org/packages/3c/d7/092d1293f4bc30cd5c4532cdfb459c652b676f254750bb1fe04ec743c800/tox-4.6.2-py3-none-any.whl", hash = "sha256:52241851a7b0cd7de07d6ef067a13b092d2a4f82fe9048efb2444aed1708d713"},
+]
+"trove-classifiers 2023.5.2" = [
+    {url = "https://files.pythonhosted.org/packages/33/75/4e87c5021949ece4171eddebb11ef30d7e787a99c4d24c7dc383dd306a6c/trove-classifiers-2023.5.2.tar.gz", hash = "sha256:c46d6e40a9581599b16c712e0164fec3764872a4085c673c07559787caedb867"},
+    {url = "https://files.pythonhosted.org/packages/75/1b/5dc22279eee99da8c685606a699868853e11b6736b23e83d443636c67eda/trove_classifiers-2023.5.2-py3-none-any.whl", hash = "sha256:0f3eceb7d16186211bcd7edafc7b7934399f738ed985998e4e557e52fe136a71"},
+]
+"trustme 1.0.0" = [
+    {url = "https://files.pythonhosted.org/packages/34/42/9958ef9b4a8f804f142b262f029d121706646db98d8459a83a5104496264/trustme-1.0.0.tar.gz", hash = "sha256:1d4f0b0fe28091506edc29c19ad90cca387646add436c3ca66ba7bcc53807f55"},
+    {url = "https://files.pythonhosted.org/packages/cd/f9/a3553be95c658e64ef898156036a77bf2c8f6b36a63c844b1b74b6e05bdb/trustme-1.0.0-py3-none-any.whl", hash = "sha256:7a9f82ad494d661cd10c9eed38e0f708154eb59a2e415da6b02af3e5dac53134"},
+]
+"types-cryptography 3.3.23.2" = [
+    {url = "https://files.pythonhosted.org/packages/18/05/a57fe8bbed10fe4b739fac6e16c4e80c5199ce2f74ae67fa7d7f6e3750da/types-cryptography-3.3.23.2.tar.gz", hash = "sha256:09cc53f273dd4d8c29fa7ad11fefd9b734126d467960162397bc5e3e604dea75"},
+    {url = "https://files.pythonhosted.org/packages/b6/36/92dfe7e5056694e78caefd05b383140c74c7fcbfc63d26ee514c77f2d8a2/types_cryptography-3.3.23.2-py3-none-any.whl", hash = "sha256:b965d548f148f8e87f353ccf2b7bd92719fdf6c845ff7cedf2abb393a0643e4f"},
+]
+"typing-extensions 4.6.3" = [
+    {url = "https://files.pythonhosted.org/packages/42/56/cfaa7a5281734dadc842f3a22e50447c675a1c5a5b9f6ad8a07b467bffe7/typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+    {url = "https://files.pythonhosted.org/packages/5f/86/d9b1518d8e75b346a33eb59fa31bdbbee11459a7e2cc5be502fa779e96c5/typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
+]
+"uvloop 0.17.0" = [
+    {url = "https://files.pythonhosted.org/packages/04/e3/e8c6b6b2ece6b0ab6033c62344d3de1706ed773d10c1798ee8afb0007b8c/uvloop-0.17.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8efcadc5a0003d3a6e887ccc1fb44dec25594f117a94e3127954c05cf144d811"},
+    {url = "https://files.pythonhosted.org/packages/08/f2/99ea33be2a601d74b345605f4843f678b8fc19b6b348c0cf07883791f0b2/uvloop-0.17.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c092a2c1e736086d59ac8e41f9c98f26bbf9b9222a76f21af9dfe949b99b2eb9"},
+    {url = "https://files.pythonhosted.org/packages/0e/27/f4f8afa5f34626f5e4fdd6b96734546d293dfe3593a6d73a8785c3e79817/uvloop-0.17.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:cbbe908fda687e39afd6ea2a2f14c2c3e43f2ca88e3a11964b297822358d0e6c"},
+    {url = "https://files.pythonhosted.org/packages/13/12/58a06670863b147f2b5bcd35ec16e55c2e811a67e926f62b4c04e6f52755/uvloop-0.17.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6aafa5a78b9e62493539456f8b646f85abc7093dd997f4976bb105537cf2635e"},
+    {url = "https://files.pythonhosted.org/packages/14/58/333a56082bf25dee13cf9e8de5f408d107d75bf6145835ec6d6b2fd35980/uvloop-0.17.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:3378eb62c63bf336ae2070599e49089005771cc651c8769aaad72d1bd9385a7c"},
+    {url = "https://files.pythonhosted.org/packages/20/9b/920b4b52028a84cc6031b4ce4bef1077d3475e6ce87969a0f0d220807307/uvloop-0.17.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ff3d00b70ce95adce264462c930fbaecb29718ba6563db354608f37e49e09024"},
+    {url = "https://files.pythonhosted.org/packages/2b/6f/ec3a30f0de00b8d240ab2128d50e4bf20b263065bc51eb0b4bbfaae6c87d/uvloop-0.17.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c686a47d57ca910a2572fddfe9912819880b8765e2f01dc0dd12a9bf8573e539"},
+    {url = "https://files.pythonhosted.org/packages/2c/08/c76bc0325b1a372e6780a169c1da56117591335a08ee19c09e3e6839a195/uvloop-0.17.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:7d37dccc7ae63e61f7b96ee2e19c40f153ba6ce730d8ba4d3b4e9738c1dccc1b"},
+    {url = "https://files.pythonhosted.org/packages/2c/70/c4162951c8c3a4a8b19a62b2668517e16b4e74499e040c07c7d99dad5126/uvloop-0.17.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:8887d675a64cfc59f4ecd34382e5b4f0ef4ae1da37ed665adba0c2badf0d6578"},
+    {url = "https://files.pythonhosted.org/packages/33/f5/94d267b8286fd9390a3276843300461edaa65431b428634056994b24b16a/uvloop-0.17.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0949caf774b9fcefc7c5756bacbbbd3fc4c05a6b7eebc7c7ad6f825b23998d6d"},
+    {url = "https://files.pythonhosted.org/packages/5b/68/08d63f6e426fdb18d718251de786e784254985f633bbd16685e0befb5b04/uvloop-0.17.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:3db8de10ed684995a7f34a001f15b374c230f7655ae840964d51496e2f8a8474"},
+    {url = "https://files.pythonhosted.org/packages/5d/bc/c1ef0b1c8faa3960b22f5809ebfd1eaa009e441b28b697f8871c31fc51d7/uvloop-0.17.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:6708f30db9117f115eadc4f125c2a10c1a50d711461699a0cbfaa45b9a78e376"},
+    {url = "https://files.pythonhosted.org/packages/7f/17/e300f183e5cbcc197eaa62c0c020072b778039297b0df896b6274a73a7da/uvloop-0.17.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:45cea33b208971e87a31c17622e4b440cac231766ec11e5d22c76fab3bf9df62"},
+    {url = "https://files.pythonhosted.org/packages/83/c0/9ade5760e31bc67fc30e74cf896cc72f7f8f8121b0ac64113c684571a22b/uvloop-0.17.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:a5abddb3558d3f0a78949c750644a67be31e47936042d4f6c888dd6f3c95f4aa"},
+    {url = "https://files.pythonhosted.org/packages/88/0b/f795eeada85d2971b0718a45683e673ad2211ba8d68b166d1f917fc0b86f/uvloop-0.17.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:9b09e0f0ac29eee0451d71798878eae5a4e6a91aa275e114037b27f7db72702d"},
+    {url = "https://files.pythonhosted.org/packages/8a/ff/bb80345a3fc39b0ce1ad27e8906874337a29dfb77e6d1e26740439be4a93/uvloop-0.17.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3ebeeec6a6641d0adb2ea71dcfb76017602ee2bfd8213e3fcc18d8f699c5104f"},
+    {url = "https://files.pythonhosted.org/packages/8f/93/6e0ce46158943650c6f15c4acfb008d9314fe670a1376399cdea295bf71e/uvloop-0.17.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:a4aee22ece20958888eedbad20e4dbb03c37533e010fb824161b4f05e641f738"},
+    {url = "https://files.pythonhosted.org/packages/90/75/e856169afc8c4676402a2c45ecb409f25e3dca4e17a5291bf6804006deba/uvloop-0.17.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:68532f4349fd3900b839f588972b3392ee56042e440dd5873dfbbcd2cc67617c"},
+    {url = "https://files.pythonhosted.org/packages/93/f8/5ba5eb1e005e2419d455d8d677211bf58ba500f204236e0b089c1a6067be/uvloop-0.17.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:23609ca361a7fc587031429fa25ad2ed7242941adec948f9d10c045bfecab06b"},
+    {url = "https://files.pythonhosted.org/packages/97/ae/e60b67eca95e9bf8f3407996acc478a8df2a0cda4cce5c3d231a831d79ba/uvloop-0.17.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:30babd84706115626ea78ea5dbc7dd8d0d01a2e9f9b306d24ca4ed5796c66ded"},
+    {url = "https://files.pythonhosted.org/packages/a9/17/e0a10e6b5a1ace1861ba496981fed35dd806c81fa18260e6e631f2713c3c/uvloop-0.17.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:2a6149e1defac0faf505406259561bc14b034cdf1d4711a3ddcdfbaa8d825a05"},
+    {url = "https://files.pythonhosted.org/packages/ab/03/ed3a0d08c9d307e8babdbed7fc6c54b273602adb3fa41748b6c1785108b3/uvloop-0.17.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f1e507c9ee39c61bfddd79714e4f85900656db1aec4d40c6de55648e85c2799c"},
+    {url = "https://files.pythonhosted.org/packages/ad/14/f791682bc94a80b03431de5d753484ac1c8a5cc3b966fd21f053ad14d5c8/uvloop-0.17.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:ce9f61938d7155f79d3cb2ffa663147d4a76d16e08f65e2c66b77bd41b356718"},
+    {url = "https://files.pythonhosted.org/packages/b1/0c/f08c6863c9e0a6823b69fbbc6753a3e4f47c3a48628ce6e8370bd39b76e7/uvloop-0.17.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:864e1197139d651a76c81757db5eb199db8866e13acb0dfe96e6fc5d1cf45fc4"},
+    {url = "https://files.pythonhosted.org/packages/ba/86/6dda1760481abf244cbd3908b79a4520d757040ca9ec37a79fc0fd01e2a0/uvloop-0.17.0.tar.gz", hash = "sha256:0ddf6baf9cf11a1a22c71487f39f15b2cf78eb5bde7e5b45fbb99e8a9d91b9e1"},
+    {url = "https://files.pythonhosted.org/packages/c5/56/745a5e615edbec0e6062397782285fbb01c50bf659e2b22489bdd9f9318f/uvloop-0.17.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:307958f9fc5c8bb01fad752d1345168c0abc5d62c1b72a4a8c6c06f042b45b20"},
+    {url = "https://files.pythonhosted.org/packages/c6/b3/60fc0f21b58b86335e2435b2cd6a9d75cb79d99787f15663fae01406c8c5/uvloop-0.17.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2deae0b0fb00a6af41fe60a675cec079615b01d68beb4cc7b722424406b126a8"},
+    {url = "https://files.pythonhosted.org/packages/d3/85/2fea43f570b32027dbf11426ea88aea9e4525f40f6e0b7017a74ab7d57ad/uvloop-0.17.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3d97672dc709fa4447ab83276f344a165075fd9f366a97b712bdd3fee05efae8"},
+    {url = "https://files.pythonhosted.org/packages/fa/28/8a3c2f067014018ba6647c39af64e3b45e5391cf85ba882fa824bda9dba3/uvloop-0.17.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:dbbaf9da2ee98ee2531e0c780455f2841e4675ff580ecf93fe5c48fe733b5667"},
+    {url = "https://files.pythonhosted.org/packages/fb/11/fef3cf9f2aa23a7daf84c39dbd66dcd562479ffc2c064496d0525adc4b43/uvloop-0.17.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1436c8673c1563422213ac6907789ecb2b070f5939b9cbff9ef7113f2b531595"},
+]
+"virtualenv 20.23.1" = [
+    {url = "https://files.pythonhosted.org/packages/21/6b/0910aebe4d5c2a27d5a79ab8fae06d22f7e01dff46baf29ced8d080134c3/virtualenv-20.23.1.tar.gz", hash = "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"},
+    {url = "https://files.pythonhosted.org/packages/2a/5b/f5ba6ec56448dc85abb75b97dc918a621a52d119ade29c8c1b7e916b0cd3/virtualenv-20.23.1-py3-none-any.whl", hash = "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419"},
 ]
```

### Comparing `easynetwork-1.0.0.dev1/.vscode/settings.example.json` & `easynetwork-1.0.0rc1/.vscode/settings.example.json`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/__init__.py` & `easynetwork-1.0.0rc1/src/easynetwork/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 __copyright__ = "Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine"
 __credits__ = ["FrankySnow9"]
 __deprecated__ = False
 __email__ = "clairicia.rcj.francis@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "FrankySnow9"
 __status__ = "Development"
-__version__ = "1.0.0.dev1"
+__version__ = "1.0.0rc1"
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/exceptions.py` & `easynetwork-1.0.0rc1/src/easynetwork/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 #
 #
 """Exceptions definition module"""
 
 from __future__ import annotations
 
 __all__ = [
+    "BaseProtocolParseError",
     "ClientClosedError",
+    "DatagramProtocolParseError",
     "DeserializeError",
     "IncrementalDeserializeError",
+    "PacketConversionError",
+    "StreamProtocolParseError",
 ]
 
 from typing import Any, Literal, TypeAlias
 
 
 class ClientClosedError(ConnectionError):
     """Error raised when trying to do an operation on a closed client"""
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/protocol.py` & `easynetwork-1.0.0rc1/src/easynetwork/protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,22 @@
 __all__ = [
     "DatagramProtocol",
     "StreamProtocol",
 ]
 
 from typing import Any, Generator, Generic, TypeVar, overload
 
-from .converter import AbstractPacketConverter, PacketConversionError
-from .exceptions import DatagramProtocolParseError, DeserializeError, IncrementalDeserializeError, StreamProtocolParseError
+from .converter import AbstractPacketConverterComposite
+from .exceptions import (
+    DatagramProtocolParseError,
+    DeserializeError,
+    IncrementalDeserializeError,
+    PacketConversionError,
+    StreamProtocolParseError,
+)
 from .serializers.abc import AbstractIncrementalPacketSerializer, AbstractPacketSerializer
 
 _SentDTOPacketT = TypeVar("_SentDTOPacketT")
 _ReceivedDTOPacketT = TypeVar("_ReceivedDTOPacketT")
 
 _SentPacketT = TypeVar("_SentPacketT")
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
@@ -35,27 +41,27 @@
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         serializer: AbstractPacketSerializer[_SentDTOPacketT, _ReceivedDTOPacketT],
-        converter: AbstractPacketConverter[_SentPacketT, _SentDTOPacketT, _ReceivedPacketT, _ReceivedDTOPacketT],
+        converter: AbstractPacketConverterComposite[_SentPacketT, _SentDTOPacketT, _ReceivedPacketT, _ReceivedDTOPacketT],
     ) -> None:
         ...
 
     def __init__(
         self,
         serializer: AbstractPacketSerializer[Any, Any],
-        converter: AbstractPacketConverter[_SentPacketT, Any, _ReceivedPacketT, Any] | None = None,
+        converter: AbstractPacketConverterComposite[_SentPacketT, Any, _ReceivedPacketT, Any] | None = None,
     ) -> None:
         assert isinstance(serializer, AbstractPacketSerializer)
-        assert converter is None or isinstance(converter, AbstractPacketConverter)
+        assert converter is None or isinstance(converter, AbstractPacketConverterComposite)
         self.__serializer: AbstractPacketSerializer[Any, Any] = serializer
-        self.__converter: AbstractPacketConverter[_SentPacketT, Any, _ReceivedPacketT, Any] | None = converter
+        self.__converter: AbstractPacketConverterComposite[_SentPacketT, Any, _ReceivedPacketT, Any] | None = converter
 
     def make_datagram(self, packet: _SentPacketT) -> bytes:
         if (converter := self.__converter) is not None:
             packet = converter.convert_to_dto_packet(packet)
         return self.__serializer.serialize(packet)
 
     def build_packet_from_datagram(self, datagram: bytes) -> _ReceivedPacketT:
@@ -82,39 +88,40 @@
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         serializer: AbstractIncrementalPacketSerializer[_SentDTOPacketT, _ReceivedDTOPacketT],
-        converter: AbstractPacketConverter[_SentPacketT, _SentDTOPacketT, _ReceivedPacketT, _ReceivedDTOPacketT],
+        converter: AbstractPacketConverterComposite[_SentPacketT, _SentDTOPacketT, _ReceivedPacketT, _ReceivedDTOPacketT],
     ) -> None:
         ...
 
     def __init__(
         self,
         serializer: AbstractIncrementalPacketSerializer[Any, Any],
-        converter: AbstractPacketConverter[_SentPacketT, Any, _ReceivedPacketT, Any] | None = None,
+        converter: AbstractPacketConverterComposite[_SentPacketT, Any, _ReceivedPacketT, Any] | None = None,
     ) -> None:
         assert isinstance(serializer, AbstractIncrementalPacketSerializer)
-        assert converter is None or isinstance(converter, AbstractPacketConverter)
+        assert converter is None or isinstance(converter, AbstractPacketConverterComposite)
         self.__serializer: AbstractIncrementalPacketSerializer[Any, Any] = serializer
-        self.__converter: AbstractPacketConverter[_SentPacketT, Any, _ReceivedPacketT, Any] | None = converter
+        self.__converter: AbstractPacketConverterComposite[_SentPacketT, Any, _ReceivedPacketT, Any] | None = converter
 
     def generate_chunks(self, packet: _SentPacketT) -> Generator[bytes, None, None]:
         if (converter := self.__converter) is not None:
             packet = converter.convert_to_dto_packet(packet)
         return (yield from self.__serializer.incremental_serialize(packet))
 
     def build_packet_from_chunks(self) -> Generator[None, bytes, tuple[_ReceivedPacketT, bytes]]:
         packet: _ReceivedPacketT
         try:
             packet, remaining_data = yield from self.__serializer.incremental_deserialize()
         except IncrementalDeserializeError as exc:
-            raise StreamProtocolParseError(exc.remaining_data, "deserialization", str(exc), error_info=exc.error_info) from exc
+            remaining_data, exc.remaining_data = exc.remaining_data, b""
+            raise StreamProtocolParseError(remaining_data, "deserialization", str(exc), error_info=exc.error_info) from exc
         except DeserializeError as exc:
             raise RuntimeError("DeserializeError raised instead of IncrementalDeserializeError") from exc
 
         if (converter := self.__converter) is not None:
             try:
                 packet = converter.create_from_dto_packet(packet)
             except PacketConversionError as exc:
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/client/abc.py` & `easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/abc.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,32 +5,29 @@
 """Network client module"""
 
 from __future__ import annotations
 
 __all__ = ["AbstractNetworkClient"]
 
 from abc import ABCMeta, abstractmethod
-from typing import TYPE_CHECKING, Any, Generic, Iterator, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, Iterator, Self, TypeVar
 
-from ..tools.socket import SocketAddress
+from ...tools.socket import SocketAddress
 
 if TYPE_CHECKING:
     from types import TracebackType
 
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
 _SentPacketT = TypeVar("_SentPacketT")
 
 
 class AbstractNetworkClient(Generic[_SentPacketT, _ReceivedPacketT], metaclass=ABCMeta):
     __slots__ = ("__weakref__",)
 
-    if TYPE_CHECKING:
-        __Self = TypeVar("__Self", bound="AbstractNetworkClient[Any, Any]")
-
-    def __enter__(self: __Self) -> __Self:
+    def __enter__(self) -> Self:
         return self
 
     def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
         self.close()
 
     def __getstate__(self) -> Any:  # pragma: no cover
         raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
@@ -56,18 +53,24 @@
         raise NotImplementedError
 
     @abstractmethod
     def recv_packet(self, timeout: float | None = ...) -> _ReceivedPacketT:
         raise NotImplementedError
 
     def iter_received_packets(self, timeout: float | None = 0) -> Iterator[_ReceivedPacketT]:
+        from time import monotonic
+
         recv_packet = self.recv_packet
         while True:
             try:
+                _start = monotonic()
                 packet = recv_packet(timeout)
+                _end = monotonic()
             except OSError:
                 return
             yield packet
+            if timeout is not None:
+                timeout -= _end - _start
 
     @abstractmethod
     def fileno(self) -> int:
         raise NotImplementedError
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/client/tcp.py` & `easynetwork-1.0.0rc1/src/easynetwork/api_sync/client/udp.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,251 +2,358 @@
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
 """Network client module"""
 
 from __future__ import annotations
 
-__all__ = ["TCPNetworkClient"]
+__all__ = ["UDPNetworkClient", "UDPNetworkEndpoint"]
 
-import errno as _errno
 import socket as _socket
-from threading import Lock as _Lock
-from time import monotonic as _time_monotonic
-from typing import Any, Callable, Generic, Iterator, TypeVar, final, overload
-
-from ..exceptions import ClientClosedError, StreamProtocolParseError
-from ..protocol import StreamProtocol
-from ..tools._utils import (
+from operator import itemgetter as _itemgetter
+from typing import TYPE_CHECKING, Any, Generic, Iterator, Self, TypeVar, final, overload
+
+from ...exceptions import ClientClosedError, DatagramProtocolParseError
+from ...protocol import DatagramProtocol
+from ...tools._utils import (
     check_real_socket_state as _check_real_socket_state,
-    error_from_errno as _error_from_errno,
-    restore_timeout_at_end as _restore_timeout_at_end,
+    check_socket_family as _check_socket_family,
+    check_socket_no_ssl as _check_socket_no_ssl,
+    ensure_datagram_socket_bound as _ensure_datagram_socket_bound,
+    retry_socket_method as _retry_socket_method,
 )
-from ..tools.socket import MAX_STREAM_BUFSIZE, SocketAddress, SocketProxy, new_socket_address
-from ..tools.stream import StreamDataConsumer
+from ...tools.lock import ForkSafeLock
+from ...tools.socket import MAX_DATAGRAM_BUFSIZE, SocketAddress, SocketProxy, new_socket_address
 from .abc import AbstractNetworkClient
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
 _SentPacketT = TypeVar("_SentPacketT")
 
 
-class TCPNetworkClient(AbstractNetworkClient[_SentPacketT, _ReceivedPacketT], Generic[_SentPacketT, _ReceivedPacketT]):
+class UDPNetworkEndpoint(Generic[_SentPacketT, _ReceivedPacketT]):
     __slots__ = (
         "__socket",
         "__socket_proxy",
-        "__owner",
-        "__lock",
-        "__producer",
-        "__consumer",
         "__addr",
         "__peer",
-        "__eof_reached",
-        "__max_recv_bufsize",
+        "__protocol",
+        "__send_lock",
+        "__receive_lock",
+        "__socket_lock",
+        "__weakref__",
     )
 
     @overload
     def __init__(
         self,
-        address: tuple[str, int],
         /,
-        protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
+        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
         *,
-        timeout: float | None = ...,
-        source_address: tuple[str, int] | None = ...,
-        max_recv_size: int | None = ...,
+        family: int = ...,
+        remote_address: tuple[str, int] | None = ...,
+        local_address: tuple[str, int] | None = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
-        socket: _socket.socket,
         /,
-        protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
+        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
         *,
-        give: bool,
-        max_recv_size: int | None = ...,
+        socket: _socket.socket,
     ) -> None:
         ...
 
     def __init__(
         self,
-        __arg: _socket.socket | tuple[str, int],
         /,
-        protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
-        *,
-        max_recv_size: int | None = None,
+        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
         **kwargs: Any,
     ) -> None:
         self.__socket: _socket.socket | None = None  # If any exception occurs, the client will already be in a closed state
         super().__init__()
-        self.__lock = _Lock()
+
+        from threading import Lock
+
+        self.__send_lock = ForkSafeLock(Lock)
+        self.__receive_lock = ForkSafeLock(Lock)
+        self.__socket_lock = ForkSafeLock(Lock)
+
+        assert isinstance(protocol, DatagramProtocol)
+
+        self.__protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT] = protocol
 
         socket: _socket.socket
-        self.__owner: bool
-        if isinstance(__arg, _socket.socket):
-            try:
-                give: bool = kwargs.pop("give")
-            except KeyError:
-                raise TypeError("Missing keyword argument 'give'") from None
-            if kwargs:  # pragma: no cover
+        peername: SocketAddress | None = None
+        external_socket: bool
+        match kwargs:
+            case {"socket": _socket.socket() as socket, **remainder} if not remainder:
+                external_socket = True
+            case _ if "socket" not in kwargs:
+                external_socket = False
+                socket, peername = _create_udp_socket(**kwargs)
+            case _:  # pragma: no cover
                 raise TypeError("Invalid arguments")
-            socket = __arg
-            self.__owner = bool(give)
-        elif isinstance(__arg, tuple):
-            address: tuple[str, int] = __arg
-            socket = _socket.create_connection(address, **kwargs)
-            self.__owner = True
-        else:  # pragma: no cover
-            raise TypeError("Invalid arguments")
 
         try:
-            if socket.type != _socket.SOCK_STREAM:
+            if socket.type != _socket.SOCK_DGRAM:
                 raise ValueError("Invalid socket type")
 
-            if max_recv_size is None:
-                max_recv_size = MAX_STREAM_BUFSIZE
-            if not isinstance(max_recv_size, int) or max_recv_size <= 0:
-                raise ValueError("max_size must be a strict positive integer")
+            _check_socket_no_ssl(socket)
+            if external_socket:
+                _check_socket_family(socket.family)
+                _ensure_datagram_socket_bound(socket)
+                try:
+                    peername = new_socket_address(socket.getpeername(), socket.family)
+                except OSError:
+                    peername = None
+
+            # Do not use global default timeout here
+            socket.settimeout(0)
 
             self.__addr: SocketAddress = new_socket_address(socket.getsockname(), socket.family)
-            self.__peer: SocketAddress = new_socket_address(socket.getpeername(), socket.family)
-            self.__producer: Callable[[_SentPacketT], Iterator[bytes]] = protocol.generate_chunks
-            self.__consumer: StreamDataConsumer[_ReceivedPacketT] = StreamDataConsumer(protocol)
-            self.__socket_proxy = SocketProxy(socket, lock=self.__lock)
-            self.__eof_reached: bool = False
-            self.__max_recv_bufsize: int = max_recv_size
+            self.__peer: SocketAddress | None = peername
+            self.__socket_proxy = SocketProxy(socket, lock=self.__socket_lock.get)
         except BaseException:
-            if self.__owner:
-                socket.close()
+            socket.close()
             raise
-
-        self.__socket = socket  # There was no errors
+        self.__socket = socket
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             socket: _socket.socket | None = self.__socket
-            owner: bool = self.__owner
         except AttributeError:
             return
-        if owner and socket is not None:
+        if socket is not None:
             socket.close()
 
     def __repr__(self) -> str:
-        socket = self.__socket
-        if socket is None:
+        try:
+            socket = self.__socket
+        except AttributeError:
             return f"<{type(self).__name__} closed>"
         return f"<{type(self).__name__} socket={socket!r}>"
 
+    def __enter__(self) -> Self:
+        return self
+
+    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+        self.close()
+
+    def __getstate__(self) -> Any:  # pragma: no cover
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
     @final
     def is_closed(self) -> bool:
-        with self.__lock:
+        with self.__socket_lock.get():
             return self.__socket is None
 
     def close(self) -> None:
-        with self.__lock:
+        with self.__send_lock.get(), self.__socket_lock.get():
             if (socket := self.__socket) is None:
                 return
             self.__socket = None
-            if not self.__owner:
-                return
             socket.close()
 
-    def shutdown(self, how: int) -> None:
-        with self.__lock:
+    def send_packet_to(
+        self,
+        packet: _SentPacketT,
+        address: tuple[str, int] | tuple[str, int, int, int] | None,
+    ) -> None:
+        with self.__send_lock.get():
             if (socket := self.__socket) is None:
                 raise ClientClosedError("Closed client")
-            socket.shutdown(how)
+            if (remote_addr := self.__peer) is not None:
+                if address is not None:
+                    if new_socket_address(address, socket.family) != remote_addr:
+                        raise ValueError(f"Invalid address: must be None or {remote_addr}")
+                    address = None
+            elif address is None:
+                raise ValueError("Invalid address: must not be None")
+            data: bytes = self.__protocol.make_datagram(packet)
+            try:
+                if address is None:
+                    _retry_socket_method(socket, None, "write", socket.send, data)
+                else:
+                    _retry_socket_method(socket, None, "write", socket.sendto, data, address)
+                _check_real_socket_state(socket)
+            finally:
+                del data
 
-    def send_packet(self, packet: _SentPacketT) -> None:
-        with self.__lock:
+    def recv_packet_from(self, timeout: float | None = None) -> tuple[_ReceivedPacketT, SocketAddress]:
+        with self.__receive_lock.get():
             if (socket := self.__socket) is None:
                 raise ClientClosedError("Closed client")
-            if self.__eof_reached:
-                raise _error_from_errno(_errno.ECONNABORTED)
+            try:
+                data, sender = _retry_socket_method(socket, timeout, "read", socket.recvfrom, MAX_DATAGRAM_BUFSIZE)
+            except TimeoutError as exc:
+                if timeout is None:  # pragma: no cover
+                    raise RuntimeError("socket.recvfrom() timed out with timeout=None ?") from exc
+                raise TimeoutError("recv_packet() timed out") from None
+            try:
+                return self.__protocol.build_packet_from_datagram(data), new_socket_address(sender, socket.family)
+            except DatagramProtocolParseError:
+                raise
+            except Exception as exc:  # pragma: no cover
+                raise RuntimeError(str(exc)) from exc
+            finally:
+                del data
 
-            # The list call should be roughly
-            # equivalent to the PySequence_Fast that ''.join() would do.
-            data: bytes = b"".join(list(self.__producer(packet)))
-
-            with _restore_timeout_at_end(socket):
-                socket.settimeout(None)
-                socket.sendall(data)
-                _check_real_socket_state(socket)
+    def iter_received_packets_from(self, timeout: float | None = 0) -> Iterator[tuple[_ReceivedPacketT, SocketAddress]]:
+        from time import monotonic
 
-    def recv_packet(self, timeout: float | None = None) -> _ReceivedPacketT:
-        with self.__lock:
-            consumer = self.__consumer
-            next_packet = self.__next_packet
-            try:
-                return next_packet(consumer)  # If there is enough data from last call to create a packet, return immediately
-            except StopIteration:
-                pass
-            if (socket := self.__socket) is None:
-                raise ClientClosedError("Closed client")
-            if self.__eof_reached:  # Do not need to call socket.recv()
-                raise _error_from_errno(_errno.ECONNABORTED)
-            bufsize: int = self.__max_recv_bufsize
-            monotonic = _time_monotonic  # pull function to local namespace
-
-            with _restore_timeout_at_end(socket):
-                socket.settimeout(timeout)
-                while True:
-                    try:
-                        _start = monotonic()
-                        chunk: bytes = socket.recv(bufsize)
-                        _end = monotonic()
-                    except (TimeoutError, BlockingIOError) as exc:
-                        if timeout is None:  # pragma: no cover
-                            raise RuntimeError("socket.recv() timed out with timeout=None ?") from exc
-                        break
-                    if not chunk:
-                        self.__eof_reached = True
-                        raise _error_from_errno(_errno.ECONNABORTED)
-                    consumer.feed(chunk)
-                    try:
-                        return next_packet(consumer)
-                    except StopIteration:
-                        if timeout is not None:
-                            if timeout > 0:
-                                timeout -= _end - _start
-                                if timeout < 0:  # pragma: no cover
-                                    timeout = 0
-                                socket.settimeout(timeout)
-                            elif len(chunk) < bufsize:
-                                break
-                        continue
-                    finally:
-                        del chunk
-                # Loop break
-                raise TimeoutError("recv_packet() timed out")
+        recv_packet_from = self.recv_packet_from
 
-    @staticmethod
-    def __next_packet(consumer: StreamDataConsumer[_ReceivedPacketT]) -> _ReceivedPacketT:
-        try:
-            return next(consumer)
-        except (StopIteration, StreamProtocolParseError):
-            raise
-        except Exception as exc:  # pragma: no cover
-            raise RuntimeError(str(exc)) from exc
+        while True:
+            try:
+                _start = monotonic()
+                packet_tuple = recv_packet_from(timeout=timeout)
+                _end = monotonic()
+            except OSError:
+                return
+            yield packet_tuple
+            if timeout is not None:
+                timeout -= _end - _start
 
     def get_local_address(self) -> SocketAddress:
         return self.__addr
 
-    def get_remote_address(self) -> SocketAddress:
+    def get_remote_address(self) -> SocketAddress | None:
         return self.__peer
 
     def fileno(self) -> int:
-        with self.__lock:
+        with self.__socket_lock.get():
             if (socket := self.__socket) is None:
                 return -1
             return socket.fileno()
 
     @property
     @final
     def socket(self) -> SocketProxy:
         return self.__socket_proxy
 
+
+class UDPNetworkClient(AbstractNetworkClient[_SentPacketT, _ReceivedPacketT], Generic[_SentPacketT, _ReceivedPacketT]):
+    __slots__ = ("__endpoint", "__peer")
+
+    @overload
+    def __init__(
+        self,
+        address: tuple[str, int],
+        /,
+        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        *,
+        family: int = ...,
+        local_address: tuple[str, int] | None = ...,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self,
+        socket: _socket.socket,
+        /,
+        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+    ) -> None:
+        ...
+
+    def __init__(
+        self,
+        __arg: _socket.socket | tuple[str, int],
+        /,
+        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        **kwargs: Any,
+    ) -> None:
+        super().__init__()
+
+        endpoint: UDPNetworkEndpoint[_SentPacketT, _ReceivedPacketT]
+        match __arg:
+            case _socket.socket() as socket:
+                endpoint = UDPNetworkEndpoint(protocol=protocol, socket=socket, **kwargs)
+            case tuple() as address:
+                endpoint = UDPNetworkEndpoint(protocol=protocol, remote_address=address, **kwargs)
+            case _:  # pragma: no cover
+                raise TypeError("Invalid arguments")
+
+        try:
+            self.__endpoint: UDPNetworkEndpoint[_SentPacketT, _ReceivedPacketT] = endpoint
+            remote_address = endpoint.get_remote_address()
+            if remote_address is None:
+                raise OSError("No remote address configured")
+            self.__peer: SocketAddress = remote_address
+        except BaseException:
+            endpoint.close()
+            raise
+
+    def __repr__(self) -> str:
+        try:
+            return f"<{type(self).__name__} endpoint={self.__endpoint!r}>"
+        except AttributeError:
+            return f"<{type(self).__name__} (partially initialized)>"
+
+    @final
+    def is_closed(self) -> bool:
+        try:
+            endpoint = self.__endpoint
+        except AttributeError:  # pragma: no cover
+            return True
+        return endpoint.is_closed()
+
+    def close(self) -> None:
+        try:
+            endpoint = self.__endpoint
+        except AttributeError:  # pragma: no cover
+            return
+        return endpoint.close()
+
+    def get_local_address(self) -> SocketAddress:
+        return self.__endpoint.get_local_address()
+
+    def get_remote_address(self) -> SocketAddress:
+        return self.__peer
+
+    def send_packet(self, packet: _SentPacketT) -> None:
+        return self.__endpoint.send_packet_to(packet, None)
+
+    def recv_packet(self, timeout: float | None = None) -> _ReceivedPacketT:
+        packet, _ = self.__endpoint.recv_packet_from(timeout=timeout)
+        return packet
+
+    def iter_received_packets(self, timeout: float | None = 0) -> Iterator[_ReceivedPacketT]:
+        return map(_itemgetter(0), self.__endpoint.iter_received_packets_from(timeout=timeout))
+
+    def fileno(self) -> int:
+        return self.__endpoint.fileno()
+
     @property
     @final
-    def max_recv_bufsize(self) -> int:
-        return self.__max_recv_bufsize
+    def socket(self) -> SocketProxy:
+        return self.__endpoint.socket
+
+
+def _create_udp_socket(
+    *,
+    family: int = _socket.AF_INET,
+    remote_address: tuple[str, int] | None = None,
+    local_address: tuple[str, int] | None = None,
+) -> tuple[_socket.socket, SocketAddress | None]:
+    _check_socket_family(family)
+    socket = _socket.socket(family, _socket.SOCK_DGRAM)
+    try:
+        peername: SocketAddress | None = None
+        if local_address is None:
+            socket.bind(("", 0))
+        else:
+            local_host, local_port = local_address
+            socket.bind((local_host, local_port))
+        if remote_address is not None:
+            remote_host, remote_port = remote_address
+            socket.connect((remote_host, remote_port))
+            peername = new_socket_address(socket.getpeername(), socket.family)
+    except BaseException:
+        socket.close()
+        raise
+    return socket, peername
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/client/udp.py` & `easynetwork-1.0.0rc1/src/easynetwork/api_async/client/tcp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,357 +1,360 @@
 # -*- coding: Utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
-"""Network client module"""
+"""Asynchronous network client module"""
 
 from __future__ import annotations
 
-__all__ = ["UDPNetworkClient", "UDPNetworkEndpoint"]
+__all__ = ["AsyncTCPNetworkClient"]
 
+import contextlib as _contextlib
+import errno as _errno
 import socket as _socket
-from operator import itemgetter as _itemgetter
-from threading import Lock as _Lock
-from typing import TYPE_CHECKING, Any, Generic, Iterator, TypeVar, final, overload
-
-from ..exceptions import ClientClosedError, DatagramProtocolParseError
-from ..protocol import DatagramProtocol
-from ..tools._utils import check_real_socket_state as _check_real_socket_state, restore_timeout_at_end as _restore_timeout_at_end
-from ..tools.socket import MAX_DATAGRAM_BUFSIZE, SocketAddress, SocketProxy, new_socket_address
-from .abc import AbstractNetworkClient
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generic,
+    Iterator,
+    Literal,
+    Mapping,
+    NoReturn,
+    TypedDict,
+    TypeVar,
+    final,
+    overload,
+)
+
+from ...exceptions import ClientClosedError, StreamProtocolParseError
+from ...protocol import StreamProtocol
+from ...tools._utils import (
+    check_real_socket_state as _check_real_socket_state,
+    check_socket_family as _check_socket_family,
+    check_socket_no_ssl as _check_socket_no_ssl,
+    concatenate_chunks as _concatenate_chunks,
+    error_from_errno as _error_from_errno,
+    set_tcp_keepalive as _set_tcp_keepalive,
+    set_tcp_nodelay as _set_tcp_nodelay,
+)
+from ...tools.socket import (
+    CLOSED_SOCKET_ERRNOS,
+    MAX_STREAM_BUFSIZE,
+    SSL_HANDSHAKE_TIMEOUT,
+    SSL_SHUTDOWN_TIMEOUT,
+    SocketAddress,
+    SocketProxy,
+    new_socket_address,
+)
+from ...tools.stream import StreamDataConsumer
+from ..backend.abc import AbstractAsyncBackend, AbstractAsyncStreamSocketAdapter, ILock
+from ..backend.factory import AsyncBackendFactory
+from ..backend.tasks import SingleTaskRunner
+from .abc import AbstractAsyncNetworkClient
 
 if TYPE_CHECKING:
-    from types import TracebackType
+    from ssl import SSLContext as _SSLContext
 
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
 _SentPacketT = TypeVar("_SentPacketT")
 
 
-class UDPNetworkEndpoint(Generic[_SentPacketT, _ReceivedPacketT]):
+class _ClientInfo(TypedDict):
+    proxy: SocketProxy
+    local_address: SocketAddress
+    remote_address: SocketAddress
+
+
+class AsyncTCPNetworkClient(AbstractAsyncNetworkClient[_SentPacketT, _ReceivedPacketT], Generic[_SentPacketT, _ReceivedPacketT]):
     __slots__ = (
         "__socket",
-        "__socket_proxy",
+        "__backend",
+        "__socket_connector",
+        "__info",
+        "__receive_lock",
+        "__send_lock",
+        "__producer",
+        "__consumer",
         "__addr",
         "__peer",
-        "__owner",
-        "__protocol",
-        "__lock",
-        "__weakref__",
+        "__eof_reached",
+        "__max_recv_size",
     )
 
-    if TYPE_CHECKING:
-        __Self = TypeVar("__Self", bound="UDPNetworkEndpoint[Any, Any]")
-
     @overload
     def __init__(
         self,
+        address: tuple[str, int],
         /,
-        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
         *,
-        family: int = ...,
-        remote_address: tuple[str, int] | None = ...,
-        source_address: tuple[str, int] | None = ...,
+        local_address: tuple[str, int] | None = ...,
+        happy_eyeballs_delay: float | None = ...,
+        ssl: _SSLContext | bool | None = ...,
+        server_hostname: str | None = ...,
+        ssl_handshake_timeout: float | None = ...,
+        ssl_shutdown_timeout: float | None = ...,
+        max_recv_size: int | None = ...,
+        backend: str | AbstractAsyncBackend | None = ...,
+        backend_kwargs: Mapping[str, Any] | None = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
+        socket: _socket.socket,
         /,
-        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
         *,
-        socket: _socket.socket,
-        give: bool,
+        ssl: _SSLContext | bool | None = ...,
+        server_hostname: str | None = ...,
+        ssl_handshake_timeout: float | None = ...,
+        ssl_shutdown_timeout: float | None = ...,
+        max_recv_size: int | None = ...,
+        backend: str | AbstractAsyncBackend | None = ...,
+        backend_kwargs: Mapping[str, Any] | None = ...,
     ) -> None:
         ...
 
     def __init__(
         self,
+        __arg: tuple[str, int] | _socket.socket,
         /,
-        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
+        *,
+        ssl: _SSLContext | bool | None = None,
+        server_hostname: str | None = None,
+        ssl_handshake_timeout: float | None = None,
+        ssl_shutdown_timeout: float | None = None,
+        max_recv_size: int | None = None,
+        backend: str | AbstractAsyncBackend | None = None,
+        backend_kwargs: Mapping[str, Any] | None = None,
         **kwargs: Any,
     ) -> None:
-        self.__socket: _socket.socket | None = None  # If any exception occurs, the client will already be in a closed state
         super().__init__()
-        self.__lock = _Lock()
-
-        assert isinstance(protocol, DatagramProtocol)
-
-        self.__protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT] = protocol
 
-        socket: _socket.socket
-        peername: SocketAddress | None = None
-        external_socket: bool
-        if "socket" in kwargs:
-            external_socket = True
-            socket = kwargs.pop("socket")
-            if not isinstance(socket, _socket.socket):  # pragma: no cover
-                raise TypeError("Invalid arguments")
-            try:
-                give: bool = kwargs.pop("give")
-            except KeyError:
-                raise TypeError("Missing keyword argument 'give'") from None
-            if kwargs:  # pragma: no cover
-                raise TypeError("Invalid arguments")
-            if socket.family not in (_socket.AF_INET, _socket.AF_INET6):
-                raise ValueError("Only AF_INET and AF_INET6 families are supported")
-            self.__owner = bool(give)
+        backend = AsyncBackendFactory.ensure(backend, backend_kwargs)
+        if max_recv_size is None:
+            max_recv_size = MAX_STREAM_BUFSIZE
+        if not isinstance(max_recv_size, int) or max_recv_size <= 0:
+            raise ValueError("'max_recv_size' must be a strictly positive integer")
+
+        self.__socket: AbstractAsyncStreamSocketAdapter | None = None
+        self.__backend: AbstractAsyncBackend = backend
+        self.__info: _ClientInfo | None = None
+
+        if ssl:
+            if isinstance(ssl, bool):
+                from ssl import create_default_context
+
+                ssl = create_default_context()
+                if server_hostname is not None and not server_hostname:
+                    ssl.check_hostname = False
         else:
-            external_socket = False
-            family = kwargs.pop("family", _socket.AF_INET)
-            remote_address: tuple[str, int] | None = kwargs.pop("remote_address", None)
-            source_address: tuple[str, int] | None = kwargs.pop("source_address", None)
-            if kwargs:  # pragma: no cover
-                raise TypeError("Invalid arguments")
-            if family not in (_socket.AF_INET, _socket.AF_INET6):
-                raise ValueError("Only AF_INET and AF_INET6 families are supported")
-            socket = _socket.socket(family, _socket.SOCK_DGRAM)
-            try:
-                if source_address is None:
-                    socket.bind(("", 0))
-                else:
-                    source_host, source_port = source_address
-                    socket.bind((source_host, source_port))
-                if remote_address is not None:
-                    remote_host, remote_port = remote_address
-                    socket.connect((remote_host, remote_port))
-                    peername = new_socket_address(socket.getpeername(), socket.family)
-            except BaseException:
-                socket.close()
-                raise
+            if server_hostname is not None:
+                raise ValueError("server_hostname is only meaningful with ssl")
 
-            self.__owner = True
+            if ssl_handshake_timeout is not None:
+                raise ValueError("ssl_handshake_timeout is only meaningful with ssl")
 
-        try:
-            if socket.type != _socket.SOCK_DGRAM:
-                raise ValueError("Invalid socket type")
+            if ssl_shutdown_timeout is not None:
+                raise ValueError("ssl_shutdown_timeout is only meaningful with ssl")
 
-            if external_socket:
-                if socket.getsockname()[1] == 0:
-                    socket.bind(("", 0))
-                try:
-                    peername = new_socket_address(socket.getpeername(), socket.family)
-                except OSError:
-                    peername = None
-
-            self.__addr: SocketAddress = new_socket_address(socket.getsockname(), socket.family)
-            self.__peer: SocketAddress | None = peername
-            self.__socket_proxy = SocketProxy(socket, lock=self.__lock)
-        except BaseException:
-            if self.__owner:
-                socket.close()
-            raise
-        self.__socket = socket
+        def _value_or_default(value: float | None, default: float) -> float:
+            return value if value is not None else default
+
+        self.__socket_connector: SingleTaskRunner[AbstractAsyncStreamSocketAdapter] | None = None
+        match __arg:
+            case _socket.socket() as socket:
+                _check_socket_no_ssl(socket)
+                if ssl:
+                    if server_hostname is None:
+                        raise ValueError("You must set server_hostname when using ssl without a host")
+                    self.__socket_connector = SingleTaskRunner(
+                        backend,
+                        backend.wrap_ssl_over_tcp_client_socket,
+                        socket,
+                        ssl_context=ssl,
+                        server_hostname=server_hostname,
+                        ssl_handshake_timeout=_value_or_default(ssl_handshake_timeout, SSL_HANDSHAKE_TIMEOUT),
+                        ssl_shutdown_timeout=_value_or_default(ssl_shutdown_timeout, SSL_SHUTDOWN_TIMEOUT),
+                        **kwargs,
+                    )
+                else:
+                    self.__socket_connector = SingleTaskRunner(backend, backend.wrap_tcp_client_socket, socket, **kwargs)
+            case (host, port):
+                if ssl:
+                    self.__socket_connector = SingleTaskRunner(
+                        backend,
+                        backend.create_ssl_over_tcp_connection,
+                        host,
+                        port,
+                        ssl_context=ssl,
+                        server_hostname=server_hostname,
+                        ssl_handshake_timeout=_value_or_default(ssl_handshake_timeout, SSL_HANDSHAKE_TIMEOUT),
+                        ssl_shutdown_timeout=_value_or_default(ssl_shutdown_timeout, SSL_SHUTDOWN_TIMEOUT),
+                        **kwargs,
+                    )
+                else:
+                    self.__socket_connector = SingleTaskRunner(backend, backend.create_tcp_connection, host, port, **kwargs)
+            case _:  # pragma: no cover
+                raise TypeError("Invalid arguments")
 
-    def __del__(self) -> None:  # pragma: no cover
-        try:
-            socket: _socket.socket | None = self.__socket
-            owner: bool = self.__owner
-        except AttributeError:
-            return
-        if owner and socket is not None:
-            socket.close()
+        assert self.__socket_connector is not None
+
+        self.__receive_lock: ILock = backend.create_lock()
+        self.__send_lock: ILock = backend.create_lock()
+        self.__producer: Callable[[_SentPacketT], Iterator[bytes]] = protocol.generate_chunks
+        self.__consumer: StreamDataConsumer[_ReceivedPacketT] = StreamDataConsumer(protocol)
+        self.__eof_reached: bool = False
+        self.__max_recv_size: int = max_recv_size
 
     def __repr__(self) -> str:
         try:
             socket = self.__socket
         except AttributeError:
-            return f"<{type(self).__name__} closed>"
+            return f"<{type(self).__name__} (partially initialized)>"
         return f"<{type(self).__name__} socket={socket!r}>"
 
-    def __enter__(self: __Self) -> __Self:
-        return self
-
-    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
-        self.close()
+    async def wait_connected(self) -> None:
+        if self.__socket is None:
+            if self.__socket_connector is None:
+                raise ClientClosedError("Client is closing, or is already closed")
+            self.__socket = await self.__socket_connector.run()
+            self.__socket_connector = None
+        if self.__info is None:
+            socket_proxy = SocketProxy(self.__socket.socket())
+            _check_socket_family(socket_proxy.family)
+            local_address: SocketAddress = new_socket_address(self.__socket.get_local_address(), socket_proxy.family)
+            remote_address: SocketAddress = new_socket_address(self.__socket.get_remote_address(), socket_proxy.family)
+            self.__info = {
+                "proxy": socket_proxy,
+                "local_address": local_address,
+                "remote_address": remote_address,
+            }
+            _set_tcp_nodelay(socket_proxy)
+            _set_tcp_keepalive(socket_proxy)
 
-    def __getstate__(self) -> Any:  # pragma: no cover
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+    def is_connected(self) -> bool:
+        return self.__socket is not None and self.__info is not None
 
     @final
-    def is_closed(self) -> bool:
-        with self.__lock:
-            return self.__socket is None
-
-    def close(self) -> None:
-        with self.__lock:
-            if (socket := self.__socket) is None:
-                return
-            self.__socket = None
-            if not self.__owner:
+    def is_closing(self) -> bool:
+        if self.__socket_connector is not None:
+            return False
+        socket = self.__socket
+        return socket is None or socket.is_closing()
+
+    async def aclose(self) -> None:
+        if self.__socket_connector is not None:
+            self.__socket_connector.cancel()
+            self.__socket_connector = None
+        async with self.__send_lock:
+            socket, self.__socket = self.__socket, None
+            if socket is None:
                 return
-            socket.close()
-
-    def send_packet_to(
-        self,
-        packet: _SentPacketT,
-        address: tuple[str, int] | tuple[str, int, int, int] | None,
-    ) -> None:
-        with self.__lock:
-            if (socket := self.__socket) is None:
-                raise ClientClosedError("Closed client")
-            if (remote_addr := self.__peer) is not None:
-                if address is not None:
-                    if new_socket_address(address, socket.family) != remote_addr:
-                        raise ValueError(f"Invalid address: must be None or {remote_addr}")
-                    address = None
-            elif address is None:
-                raise ValueError("Invalid address: must not be None")
-            data: bytes = self.__protocol.make_datagram(packet)
-            with _restore_timeout_at_end(socket):
-                socket.settimeout(None)
-                if address is None:
-                    socket.send(data)
-                else:
-                    socket.sendto(data, address)
-                _check_real_socket_state(socket)
-
-    def recv_packet_from(self, timeout: float | None = None) -> tuple[_ReceivedPacketT, SocketAddress]:
-        with self.__lock:
-            if (socket := self.__socket) is None:
-                raise ClientClosedError("Closed client")
-            with _restore_timeout_at_end(socket):
-                socket.settimeout(timeout)
-                try:
-                    data, sender = socket.recvfrom(MAX_DATAGRAM_BUFSIZE)
-                except (TimeoutError, BlockingIOError) as exc:
-                    if timeout is None:  # pragma: no cover
-                        raise RuntimeError("socket.recvfrom() timed out with timeout=None ?") from exc
-                    raise TimeoutError("recv_packet() timed out") from None
+            try:
+                await socket.aclose()
+            except (ConnectionError, TimeoutError):
+                # It is normal if there was connection errors during operations. But do not propagate this exception,
+                # as we will never reuse this socket
+                pass
+
+    async def send_packet(self, packet: _SentPacketT) -> None:
+        async with self.__send_lock:
+            with self.__convert_socket_error():
+                socket = await self.__ensure_connected()
+                await socket.sendall(_concatenate_chunks(self.__producer(packet)))
+                _check_real_socket_state(self.socket)
+
+    async def recv_packet(self) -> _ReceivedPacketT:
+        async with self.__receive_lock:
+            with self.__convert_socket_error():
+                consumer = self.__consumer
+                next_packet = self.__next_packet
                 try:
-                    return self.__protocol.build_packet_from_datagram(data), new_socket_address(sender, socket.family)
-                except DatagramProtocolParseError:
-                    raise
-                except Exception as exc:  # pragma: no cover
-                    raise RuntimeError(str(exc)) from exc
-                finally:
-                    del data
-
-    def iter_received_packets_from(self, timeout: float | None = 0) -> Iterator[tuple[_ReceivedPacketT, SocketAddress]]:
-        recv_packet_from = self.recv_packet_from
+                    return next_packet(consumer)  # If there is enough data from last call to create a packet, return immediately
+                except StopIteration:
+                    pass
+                socket = await self.__ensure_connected()
+                bufsize: int = self.__max_recv_size
+                backend = self.__backend
+                while True:
+                    chunk: bytes = await socket.recv(bufsize)
+                    if not chunk:
+                        self.__eof_error(False)
+                    consumer.feed(chunk)
+                    del chunk
+                    try:
+                        return next_packet(consumer)
+                    except StopIteration:
+                        pass
+                    # Attempt failed, wait for one iteration
+                    await backend.coro_yield()
 
-        while True:
-            if self.__socket is None:
-                return
-            try:
-                packet_tuple = recv_packet_from(timeout=timeout)
-            except OSError:
-                return
-            yield packet_tuple  # yield out of lock scope
+    @staticmethod
+    def __next_packet(consumer: StreamDataConsumer[_ReceivedPacketT]) -> _ReceivedPacketT:
+        try:
+            return next(consumer)
+        except (StopIteration, StreamProtocolParseError):
+            raise
+        except Exception as exc:  # pragma: no cover
+            raise RuntimeError(str(exc)) from exc
 
     def get_local_address(self) -> SocketAddress:
-        return self.__addr
+        if self.__info is None:
+            raise _error_from_errno(_errno.ENOTSOCK)
+        return self.__info["local_address"]
 
-    def get_remote_address(self) -> SocketAddress | None:
-        return self.__peer
+    def get_remote_address(self) -> SocketAddress:
+        if self.__info is None:
+            raise _error_from_errno(_errno.ENOTSOCK)
+        return self.__info["remote_address"]
 
     def fileno(self) -> int:
-        with self.__lock:
-            if (socket := self.__socket) is None:
-                return -1
-            return socket.fileno()
-
-    @property
-    @final
-    def socket(self) -> SocketProxy:
-        return self.__socket_proxy
-
-
-class UDPNetworkClient(AbstractNetworkClient[_SentPacketT, _ReceivedPacketT], Generic[_SentPacketT, _ReceivedPacketT]):
-    __slots__ = ("__endpoint", "__peer")
-
-    @overload
-    def __init__(
-        self,
-        address: tuple[str, int],
-        /,
-        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
-        *,
-        family: int = ...,
-        source_address: tuple[str, int] | None = ...,
-    ) -> None:
-        ...
-
-    @overload
-    def __init__(
-        self,
-        socket: _socket.socket,
-        /,
-        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
-        *,
-        give: bool = ...,
-    ) -> None:
-        ...
-
-    def __init__(
-        self,
-        __arg: _socket.socket | tuple[str, int],
-        /,
-        protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
-        **kwargs: Any,
-    ) -> None:
-        super().__init__()
-
-        endpoint: UDPNetworkEndpoint[_SentPacketT, _ReceivedPacketT]
-        if isinstance(__arg, _socket.socket):
-            socket = __arg
-            endpoint = UDPNetworkEndpoint(protocol=protocol, socket=socket, **kwargs)
-        elif isinstance(__arg, tuple):
-            address = __arg
-            endpoint = UDPNetworkEndpoint(protocol=protocol, remote_address=address, **kwargs)
-        else:
-            raise TypeError("Invalid arguments")  # pragma: no cover
+        socket = self.__socket
+        if socket is None:
+            return -1
+        return socket.socket().fileno()
+
+    def get_backend(self) -> AbstractAsyncBackend:
+        return self.__backend
+
+    async def __ensure_connected(self) -> AbstractAsyncStreamSocketAdapter:
+        await self.wait_connected()
+        assert self.__socket is not None
+        if self.__socket.is_closing() or self.__eof_reached:
+            raise _error_from_errno(_errno.ECONNABORTED)
+        return self.__socket
 
+    @_contextlib.contextmanager
+    def __convert_socket_error(self) -> Iterator[None]:
         try:
-            self.__endpoint: UDPNetworkEndpoint[_SentPacketT, _ReceivedPacketT] = endpoint
-            remote_address = endpoint.get_remote_address()
-            if remote_address is None:
-                raise OSError("No remote address configured")
-            self.__peer: SocketAddress = remote_address
-        except BaseException:
-            endpoint.close()
+            yield
+        except (ConnectionAbortedError, ClientClosedError):
+            raise
+        except ConnectionError as exc:
+            self.__eof_error(exc)
+        except OSError as exc:
+            if exc.errno in CLOSED_SOCKET_ERRNOS:
+                self.__eof_error(exc)
             raise
 
-    def __repr__(self) -> str:
-        try:
-            return f"<{type(self).__name__} endpoint={self.__endpoint!r}>"
-        except AttributeError:
-            return f"<{type(self).__name__} (partially initialized)>"
+    def __eof_error(self, cause: BaseException | None | Literal[False]) -> NoReturn:
+        self.__eof_reached = True
+        if cause is False:
+            raise _error_from_errno(_errno.ECONNABORTED)
+        raise _error_from_errno(_errno.ECONNABORTED) from cause
 
+    @property
     @final
-    def is_closed(self) -> bool:
-        try:
-            endpoint = self.__endpoint
-        except AttributeError:  # pragma: no cover
-            return True
-        return endpoint.is_closed()
-
-    def close(self) -> None:
-        try:
-            endpoint = self.__endpoint
-        except AttributeError:  # pragma: no cover
-            return
-        return endpoint.close()
-
-    def get_local_address(self) -> SocketAddress:
-        return self.__endpoint.get_local_address()
-
-    def get_remote_address(self) -> SocketAddress:
-        return self.__peer
-
-    def send_packet(self, packet: _SentPacketT) -> None:
-        return self.__endpoint.send_packet_to(packet, None)
-
-    def recv_packet(self, timeout: float | None = None) -> _ReceivedPacketT:
-        packet, _ = self.__endpoint.recv_packet_from(timeout=timeout)
-        return packet
-
-    def iter_received_packets(self, timeout: float | None = 0) -> Iterator[_ReceivedPacketT]:
-        return map(_itemgetter(0), self.__endpoint.iter_received_packets_from(timeout=timeout))
-
-    def fileno(self) -> int:
-        return self.__endpoint.fileno()
+    def socket(self) -> SocketProxy:
+        if self.__info is None:
+            raise _error_from_errno(_errno.ENOTSOCK)
+        return self.__info["proxy"]
 
     @property
     @final
-    def socket(self) -> SocketProxy:
-        return self.__endpoint.socket
+    def max_recv_size(self) -> int:
+        return self.__max_recv_size
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/__init__.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,29 @@
     "CBORSerializer",
     "EncryptorSerializer",
     "FileBasedPacketSerializer",
     "FixedSizePacketSerializer",
     "JSONDecoderConfig",
     "JSONEncoderConfig",
     "JSONSerializer",
+    "MessagePackSerializer",
+    "MessagePackerConfig",
+    "MessageUnpackerConfig",
     "NamedTupleStructSerializer",
     "PickleSerializer",
     "PicklerConfig",
+    "StringLineSerializer",
     "UnpicklerConfig",
     "ZlibCompressorSerializer",
 ]
 
 
 ############ Package initialization ############
 from .abc import *
 from .base_stream import *
 from .cbor import *
 from .json import *
+from .line import *
+from .msgpack import *
 from .pickle import *
 from .struct import *
 from .wrapper import *
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/abc.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         raise NotImplementedError
 
     @abstractmethod
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
         raise NotImplementedError
 
     def serialize(self, packet: _ST_contra) -> bytes:
-        # The list call should be roughly
-        # equivalent to the PySequence_Fast that ''.join() would do.
-        return b"".join(list(self.incremental_serialize(packet)))
+        from ..tools._utils import concatenate_chunks
+
+        return concatenate_chunks(self.incremental_serialize(packet))
 
     def deserialize(self, data: bytes) -> _DT_co:
         from ..exceptions import DeserializeError
 
         consumer: Generator[None, bytes, tuple[_DT_co, bytes]] = self.incremental_deserialize()
         try:
             next(consumer)
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/base_stream.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/base_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 ]
 
 from abc import abstractmethod
 from io import BytesIO
 from typing import IO, Any, Generator, TypeVar, final
 
 from ..exceptions import DeserializeError, IncrementalDeserializeError
-from .abc import AbstractIncrementalPacketSerializer
+from .abc import AbstractIncrementalPacketSerializer, AbstractPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 class AutoSeparatedPacketSerializer(AbstractIncrementalPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__separator", "__keepends")
+    __slots__ = ("__separator",)
 
-    def __init__(self, separator: bytes, *, keepends: bool = False, **kwargs: Any) -> None:
+    def __init__(self, separator: bytes, **kwargs: Any) -> None:
         super().__init__(**kwargs)
-        assert isinstance(separator, bytes)
+        assert isinstance(separator, (bytes, bytearray))
+        separator = bytes(separator)
         if len(separator) < 1:
             raise ValueError("Empty separator")
         self.__separator: bytes = separator
-        self.__keepends: bool = bool(keepends)
 
     @abstractmethod
     def serialize(self, packet: _ST_contra) -> bytes:
         raise NotImplementedError
 
     @final
     def incremental_serialize(self, packet: _ST_contra) -> Generator[bytes, None, None]:
@@ -50,30 +50,31 @@
 
     @abstractmethod
     def deserialize(self, data: bytes) -> _DT_co:
         raise NotImplementedError
 
     @final
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
-        buffer: bytes = yield
+        buffer: bytearray = bytearray((yield))
         separator: bytes = self.__separator
+        separator_length: int = len(separator)
         while True:
             data, found_separator, buffer = buffer.partition(separator)
             if found_separator:
                 if not data:  # There was successive separators
                     continue
                 break
             assert not buffer
-            buffer = data + (yield)
-        if self.__keepends:
-            data += separator
+            buffer = data
+            buffer.extend((yield))
+        del found_separator
         while buffer.startswith(separator):  # Remove successive separators which can already be eliminated
-            buffer = buffer.removeprefix(separator)
+            del buffer[:separator_length]
         try:
-            packet = self.deserialize(data)
+            packet = self.deserialize(bytes(data))
         except DeserializeError as exc:
             raise IncrementalDeserializeError(
                 f"Error when deserializing data: {exc}",
                 remaining_data=buffer,
                 error_info=exc.error_info,
             ) from exc
         finally:
@@ -81,19 +82,14 @@
         return packet, buffer
 
     @property
     @final
     def separator(self) -> bytes:
         return self.__separator
 
-    @property
-    @final
-    def keepends(self) -> bool:
-        return self.__keepends
-
 
 class FixedSizePacketSerializer(AbstractIncrementalPacketSerializer[_ST_contra, _DT_co]):
     __slots__ = ("__size",)
 
     def __init__(self, size: int, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         size = int(size)
@@ -121,38 +117,40 @@
         buffer = bytearray((yield))
         packet_size: int = self.__size
         while len(buffer) < packet_size:
             buffer.extend((yield))
         data = buffer[:packet_size]
         del buffer[:packet_size]
         try:
-            packet = self.deserialize(data)
+            packet = self.deserialize(bytes(data))
         except DeserializeError as exc:
             raise IncrementalDeserializeError(
                 f"Error when deserializing data: {exc}",
                 remaining_data=buffer,
                 error_info=exc.error_info,
             ) from exc
+        finally:
+            del data
         return packet, buffer
 
     @property
     @final
     def packet_size(self) -> int:
         return self.__size
 
 
-class FileBasedPacketSerializer(AbstractIncrementalPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__expected_error",)
+class FileBasedPacketSerializer(AbstractPacketSerializer[_ST_contra, _DT_co]):
+    __slots__ = ("__expected_errors",)
 
     def __init__(self, expected_load_error: type[Exception] | tuple[type[Exception], ...], **kwargs: Any) -> None:
         super().__init__(**kwargs)
         if not isinstance(expected_load_error, tuple):
             expected_load_error = (expected_load_error,)
         assert all(issubclass(e, Exception) for e in expected_load_error)
-        self.__expected_error: tuple[type[Exception], ...] = expected_load_error
+        self.__expected_errors: tuple[type[Exception], ...] = expected_load_error
 
     @abstractmethod
     def dump_to_file(self, packet: _ST_contra, file: IO[bytes]) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def load_from_file(self, file: IO[bytes]) -> _DT_co:
@@ -161,51 +159,52 @@
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         with BytesIO() as buffer:
             self.dump_to_file(packet, buffer)
             return buffer.getvalue()
 
     @final
-    def incremental_serialize(self, packet: _ST_contra) -> Generator[bytes, None, None]:
-        with BytesIO() as buffer:
-            self.dump_to_file(packet, buffer)
-            data = buffer.getvalue()
-        if data:
-            yield data
-
-    @final
     def deserialize(self, data: bytes) -> _DT_co:
         with BytesIO(data) as buffer:
             del data
             try:
                 packet: _DT_co = self.load_from_file(buffer)
             except EOFError as exc:
-                raise DeserializeError("Missing data to create packet") from exc
-            except self.__expected_error as exc:
-                raise DeserializeError(str(exc)) from exc
-            if buffer.read():  # There is still data after deserialization
-                raise DeserializeError("Extra data caught")
+                raise DeserializeError("Missing data to create packet", error_info={"data": buffer.getvalue()}) from exc
+            except self.__expected_errors as exc:
+                raise DeserializeError(str(exc), error_info={"data": buffer.getvalue()}) from exc
+            if extra := buffer.read():  # There is still data after deserialization
+                raise DeserializeError("Extra data caught", error_info={"packet": packet, "extra": extra})
         return packet
 
     @final
+    def incremental_serialize(self, packet: _ST_contra) -> Generator[bytes, None, None]:
+        with BytesIO() as buffer:
+            self.dump_to_file(packet, buffer)
+            data = buffer.getvalue()
+        if data:
+            yield data
+
+    @final
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
         with BytesIO() as buffer:
             while True:
                 while not (chunk := (yield)):
                     continue
                 buffer.write(chunk)
                 del chunk
                 buffer.seek(0)
                 try:
                     packet: _DT_co = self.load_from_file(buffer)
                 except EOFError:
                     continue
-                except self.__expected_error as exc:
+                except self.__expected_errors as exc:
                     remaining_data: bytes = buffer.read()
                     if not remaining_data:  # Possibly an EOF error, give it a chance
                         continue
                     raise IncrementalDeserializeError(
                         f"Deserialize error: {exc}",
                         remaining_data=remaining_data,
+                        error_info={"data": buffer.getvalue()},
                     ) from exc
                 else:
                     return packet, buffer.read()
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/cbor.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/cbor.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/json.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/json.py`

 * *Files 15% similar despite different names*

```diff
@@ -99,23 +99,23 @@
                 continue
             break
         buffer_array.extend(chunk[:non_printable_idx])
         return buffer_array, chunk[non_printable_idx:]
 
 
 class JSONSerializer(AbstractIncrementalPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__encoder", "__decoder", "__encoding", "__str_errors")
+    __slots__ = ("__encoder", "__decoder", "__encoding", "__unicode_errors")
 
     def __init__(
         self,
         encoder_config: JSONEncoderConfig | None = None,
         decoder_config: JSONDecoderConfig | None = None,
         *,
         encoding: str = "utf-8",
-        str_errors: str = "strict",
+        unicode_errors: str = "strict",
     ) -> None:
         from json import JSONDecoder, JSONEncoder
 
         super().__init__()
         self.__encoder: JSONEncoder
         self.__decoder: JSONDecoder
 
@@ -129,65 +129,80 @@
         elif not isinstance(decoder_config, JSONDecoderConfig):
             raise TypeError(f"Invalid decoder config: expected {JSONDecoderConfig.__name__}, got {type(decoder_config).__name__}")
 
         self.__encoder = JSONEncoder(**dataclass_asdict(encoder_config))
         self.__decoder = JSONDecoder(**dataclass_asdict(decoder_config))
 
         self.__encoding: str = encoding
-        self.__str_errors: str = str_errors
+        self.__unicode_errors: str = unicode_errors
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
-        return self.__encoder.encode(packet).encode(self.__encoding, self.__str_errors)
+        return self.__encoder.encode(packet).encode(self.__encoding, self.__unicode_errors)
 
     @final
     def incremental_serialize(self, packet: _ST_contra) -> Generator[bytes, None, None]:
         encoding: str = self.__encoding
-        str_errors: str = self.__str_errors
+        str_errors: str = self.__unicode_errors
         for chunk in self.__encoder.iterencode(packet):
             yield chunk.encode(encoding, str_errors)
         yield b"\n"
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
         from json import JSONDecodeError
 
         try:
-            document: str = data.decode(self.__encoding, self.__str_errors)
+            document: str = data.decode(self.__encoding, self.__unicode_errors)
         except UnicodeError as exc:
-            raise DeserializeError(f"Unicode decode error: {exc}") from exc
+            raise DeserializeError(f"Unicode decode error: {exc}", error_info={"data": data}) from exc
         try:
             packet: _DT_co = self.__decoder.decode(document)
         except JSONDecodeError as exc:
-            raise DeserializeError(f"JSON decode error: {exc}") from exc
+            raise DeserializeError(
+                f"JSON decode error: {exc}",
+                error_info={
+                    "document": exc.doc,
+                    "position": exc.pos,
+                    "lineno": exc.lineno,
+                    "colno": exc.colno,
+                },
+            ) from exc
         return packet
 
     @final
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
         from json import JSONDecodeError
 
         complete_document, remaining_data = yield from _JSONParser.raw_parse()
 
         if not complete_document:
             complete_document = remaining_data
             remaining_data = b""
 
         packet: _DT_co
         try:
-            document: str = complete_document.decode(self.__encoding, self.__str_errors)
+            document: str = complete_document.decode(self.__encoding, self.__unicode_errors)
         except UnicodeError as exc:
             raise IncrementalDeserializeError(
                 f"Unicode decode error: {exc}",
                 remaining_data=remaining_data,
+                error_info={"data": complete_document},
             ) from exc
         try:
             packet, end = self.__decoder.raw_decode(document)
         except JSONDecodeError as exc:
             raise IncrementalDeserializeError(
-                f"JSON decode error: {exc} (document={document!r})",
+                f"JSON decode error: {exc}",
                 remaining_data=remaining_data,
+                error_info={
+                    "document": exc.doc,
+                    "position": exc.pos,
+                    "lineno": exc.lineno,
+                    "colno": exc.colno,
+                },
             ) from exc
         try:
-            remaining_data = document[end:].encode(self.__encoding, self.__str_errors) + remaining_data
+            remaining_data = document[end:].encode(self.__encoding, self.__unicode_errors) + remaining_data
         except UnicodeError:  # pragma: no cover  # Should not happen but it must not pass
             pass
         return packet, remaining_data.lstrip(b" \t\n\r")  # Optimization: Skip leading spaces
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/pickle.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/pickle.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import pickle as _pickle
 import pickletools as _pickletools
 from dataclasses import asdict as dataclass_asdict, dataclass
 from functools import partial
 from io import BytesIO
 from typing import IO, Callable, TypeVar, final
 
-from .base_stream import FileBasedPacketSerializer
+from ..exceptions import DeserializeError
+from .abc import AbstractPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 @dataclass(kw_only=True)
 class PicklerConfig:
@@ -34,32 +35,27 @@
 @dataclass(kw_only=True)
 class UnpicklerConfig:
     fix_imports: bool = False
     encoding: str = "utf-8"
     errors: str = "strict"
 
 
-class PickleSerializer(FileBasedPacketSerializer[_ST_contra, _DT_co]):
+class PickleSerializer(AbstractPacketSerializer[_ST_contra, _DT_co]):
     __slots__ = ("__optimize", "__pickler_cls", "__unpickler_cls")
 
     def __init__(
         self,
         pickler_config: PicklerConfig | None = None,
         unpickler_config: UnpicklerConfig | None = None,
         *,
         pickler_cls: type[_pickle.Pickler] | None = None,
         unpickler_cls: type[_pickle.Unpickler] | None = None,
         optimize: bool = False,
     ) -> None:
-        super().__init__(
-            expected_load_error=(
-                _pickle.UnpicklingError,
-                ValueError,
-            ),  # pickle.Unpickler does not only raise UnpicklingError... :)
-        )
+        super().__init__()
         self.__optimize = bool(optimize)
         self.__pickler_cls: Callable[[IO[bytes]], _pickle.Pickler]
         self.__unpickler_cls: Callable[[IO[bytes]], _pickle.Unpickler]
 
         if pickler_config is None:
             pickler_config = PicklerConfig()
         elif not isinstance(pickler_config, PicklerConfig):
@@ -72,18 +68,26 @@
                 f"Invalid unpickler config: expected {UnpicklerConfig.__name__}, got {type(unpickler_config).__name__}"
             )
 
         self.__pickler_cls = partial(pickler_cls or _pickle.Pickler, **dataclass_asdict(pickler_config), buffer_callback=None)
         self.__unpickler_cls = partial(unpickler_cls or _pickle.Unpickler, **dataclass_asdict(unpickler_config), buffers=None)
 
     @final
-    def dump_to_file(self, packet: _ST_contra, file: IO[bytes]) -> None:
-        if not self.__optimize:
-            self.__pickler_cls(file).dump(packet)
-            return
+    def serialize(self, packet: _ST_contra) -> bytes:
         with BytesIO() as buffer:
             self.__pickler_cls(buffer).dump(packet)
-            file.write(_pickletools.optimize(buffer.getvalue()))
+            pickle: bytes = buffer.getvalue()
+        if self.__optimize:
+            pickle = _pickletools.optimize(pickle)
+        return pickle
 
     @final
-    def load_from_file(self, file: IO[bytes]) -> _DT_co:
-        return self.__unpickler_cls(file).load()
+    def deserialize(self, data: bytes) -> _DT_co:
+        with BytesIO(data) as buffer:
+            del data
+            try:
+                packet: _DT_co = self.__unpickler_cls(buffer).load()
+            except Exception as exc:
+                raise DeserializeError(str(exc) or "Invalid token", error_info={"data": buffer.getvalue()}) from exc
+            if extra := buffer.read():  # There is still data after deserialization
+                raise DeserializeError("Extra data caught", {"packet": packet, "extra": extra})
+        return packet
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/struct.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/struct.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,78 +48,80 @@
         raise NotImplementedError
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
         try:
             packet_tuple: tuple[Any, ...] = self.__s.unpack(data)
         except _struct.error as exc:
-            raise DeserializeError(f"Invalid value: {exc}") from exc
+            raise DeserializeError(f"Invalid value: {exc}", error_info={"data": data}) from exc
         try:
             return self.from_tuple(packet_tuple)
         except Exception as exc:
-            raise DeserializeError(f"Error when building packet from unpacked struct value: {exc}") from exc
+            raise DeserializeError(
+                f"Error when building packet from unpacked struct value: {exc}",
+                error_info={"unpacked_struct": packet_tuple},
+            ) from exc
 
     @property
     @final
     def struct(self) -> _struct.Struct:
         return self.__s
 
 
 _NT = TypeVar("_NT", bound=NamedTuple)
 
 
 class NamedTupleStructSerializer(AbstractStructSerializer[_NT, _NT], Generic[_NT]):
-    __slots__ = ("__namedtuple_cls", "__string_fields", "__encoding", "__str_errors", "__strip_trailing_nul")
+    __slots__ = ("__namedtuple_cls", "__string_fields", "__encoding", "__unicode_errors", "__strip_trailing_nul")
 
     def __init__(
         self,
         namedtuple_cls: type[_NT],
         field_formats: SupportsKeysAndGetItem[str, str],
         format_endianness: str = "",
         encoding: str | None = "utf-8",
-        errors: str = "strict",
+        unicode_errors: str = "strict",
         strip_string_trailing_nul_bytes: bool = True,
     ) -> None:
         string_fields: set[str] = set()
 
         for field in field_formats.keys():
             field_fmt = field_formats[field]
             if any(c in _ENDIANNESS_CHARACTERS for c in field_fmt):
                 raise ValueError(f"{field!r}: Invalid field format")
             if field_fmt and field_fmt[-1] == "s":
-                if len(field_fmt) > 1 and not field_fmt[:-1].isdigit():
+                if len(field_fmt) > 1 and not field_fmt[:-1].isdecimal():
                     raise ValueError(f"{field!r}: Invalid field format")
                 string_fields.add(field)
             elif len(field_fmt) != 1 or not field_fmt.isalpha():
                 raise ValueError(f"{field!r}: Invalid field format")
         super().__init__(f"{format_endianness}{''.join(map(field_formats.__getitem__, namedtuple_cls._fields))}")
         self.__namedtuple_cls: type[_NT] = namedtuple_cls
         self.__string_fields: frozenset[str] = frozenset(string_fields)
         self.__encoding: str | None = encoding
-        self.__str_errors: str = errors
+        self.__unicode_errors: str = unicode_errors
         self.__strip_trailing_nul = bool(strip_string_trailing_nul_bytes)
 
     @final
     def iter_values(self, packet: _NT) -> _NT:
         assert isinstance(packet, self.__namedtuple_cls)
-        if (encoding := self.__encoding) is not None:
+        if (encoding := self.__encoding) is not None and self.__string_fields:
             string_fields: dict[str, str] = {field: getattr(packet, field) for field in self.__string_fields}
-            if string_fields:
-                str_errors: str = self.__str_errors
-                packet = packet._replace(**{field: value.encode(encoding, str_errors) for field, value in string_fields.items()})
+            unicode_errors: str = self.__unicode_errors
+            packet = packet._replace(**{field: value.encode(encoding, unicode_errors) for field, value in string_fields.items()})
         return packet
 
     @final
     def from_tuple(self, t: tuple[Any, ...]) -> _NT:
         p = self.__namedtuple_cls._make(t)
         string_fields: dict[str, bytes] = {field: getattr(p, field) for field in self.__string_fields}
         if string_fields:
             to_replace: dict[str, Any] | None = None
             if self.__strip_trailing_nul:
                 string_fields = {field: value.rstrip(b"\0") for field, value in string_fields.items()}
                 to_replace = string_fields
             if (encoding := self.__encoding) is not None:
-                str_errors: str = self.__str_errors
-                to_replace = {field: value.decode(encoding, str_errors) for field, value in string_fields.items()}
+                unicode_errors: str = self.__unicode_errors
+                to_replace = {field: value.decode(encoding, unicode_errors) for field, value in string_fields.items()}
             if to_replace is not None:
                 p = p._replace(**to_replace)
         return p
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/wrapper/base64.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/encryptor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 # -*- coding: Utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
-"""base64 encoding serializer module"""
+"""encrypted data serializer module"""
 
 from __future__ import annotations
 
 __all__ = [
-    "Base64EncodedSerializer",
+    "EncryptorSerializer",
 ]
 
-import base64
-import binascii
-from hmac import compare_digest, digest as hmac_digest
 from typing import TypeVar, final
 
 from ...exceptions import DeserializeError
 from ..abc import AbstractPacketSerializer
 from ..base_stream import AutoSeparatedPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
-class Base64EncodedSerializer(AutoSeparatedPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__serializer", "__signing_key")
+class EncryptorSerializer(AutoSeparatedPacketSerializer[_ST_contra, _DT_co]):
+    __slots__ = ("__serializer", "__fernet", "__token_ttl")
 
     def __init__(
         self,
         serializer: AbstractPacketSerializer[_ST_contra, _DT_co],
-        signing_key: str | bytes | None = None,
+        key: str | bytes,
+        *,
+        token_ttl: int | None = None,
+        separator: bytes = b"\r\n",
     ) -> None:
-        super().__init__(separator=b"\r\n", keepends=False)
+        try:
+            import cryptography.fernet
+        except ModuleNotFoundError as exc:  # pragma: no cover
+            raise ModuleNotFoundError("encryption dependencies are missing. Consider adding 'encryption' extra") from exc
+
+        super().__init__(separator=separator)
         assert isinstance(serializer, AbstractPacketSerializer)
         self.__serializer: AbstractPacketSerializer[_ST_contra, _DT_co] = serializer
-        if signing_key is not None:
-            try:
-                signing_key = base64.urlsafe_b64decode(signing_key)
-            except binascii.Error as exc:
-                raise ValueError("signing key must be 32 url-safe base64-encoded bytes.") from exc
-            if len(signing_key) != 32:
-                raise ValueError("signing key must be 32 url-safe base64-encoded bytes.")
-        self.__signing_key: bytes | None = signing_key
+        self.__fernet = cryptography.fernet.Fernet(key)
+        self.__token_ttl = token_ttl
 
     @classmethod
     def generate_key(cls) -> bytes:
-        from os import urandom
+        try:
+            import cryptography.fernet
+        except ModuleNotFoundError as exc:  # pragma: no cover
+            raise ModuleNotFoundError("encryption dependencies are missing. Consider adding 'encryption' extra") from exc
 
-        return base64.urlsafe_b64encode(urandom(32))
+        return cryptography.fernet.Fernet.generate_key()
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         data = self.__serializer.serialize(packet)
-        if key := self.__signing_key:
-            data += hmac_digest(key, data, "sha256")
-        return base64.urlsafe_b64encode(data)
+        return self.__fernet.encrypt(data)
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
+        from cryptography.fernet import InvalidToken
+
         try:
-            data = base64.urlsafe_b64decode(data)
-        except binascii.Error:
-            raise DeserializeError("Invalid token") from None
-        if key := self.__signing_key:
-            data, signature = data[:-32], data[-32:]
-            if not compare_digest(hmac_digest(key, data, "sha256"), signature):
-                raise DeserializeError("Invalid token")
+            data = self.__fernet.decrypt(data, ttl=self.__token_ttl)
+        except InvalidToken:
+            raise DeserializeError("Invalid token", error_info=None) from None
         return self.__serializer.deserialize(data)
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/serializers/wrapper/compressor.py` & `easynetwork-1.0.0rc1/src/easynetwork/serializers/wrapper/compressor.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,19 +88,25 @@
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
         decompressor: DecompressorInterface = self.new_decompressor_stream()
         try:
             data = decompressor.decompress(data)
         except self.__expected_error as exc:
-            raise DeserializeError(str(exc)) from exc
+            raise DeserializeError(str(exc), error_info={"data": data}) from exc
         if not decompressor.eof:
-            raise DeserializeError("Compressed data ended before the end-of-stream marker was reached")
-        if decompressor.unused_data:
-            raise DeserializeError("Trailing data error")
+            raise DeserializeError(
+                "Compressed data ended before the end-of-stream marker was reached",
+                error_info={"already_decompressed_data": data},
+            )
+        if unused_data := decompressor.unused_data:
+            raise DeserializeError(
+                "Trailing data error",
+                error_info={"decompressed_data": data, "extra": unused_data},
+            )
         del decompressor
         return self.__serializer.deserialize(data)
 
     @final
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
         results: deque[bytes] = deque()
         decompressor = self.new_decompressor_stream()
@@ -109,14 +115,18 @@
                 continue
             try:
                 chunk = decompressor.decompress(chunk)
             except self.__expected_error as exc:
                 raise IncrementalDeserializeError(
                     message=f"Decompression error: {exc}",
                     remaining_data=b"",
+                    error_info={
+                        "already_decompressed_chunks": results,
+                        "invalid_chunk": chunk,
+                    },
                 ) from exc
             if chunk:
                 results.append(chunk)
             del chunk
 
         data = b"".join(results)
         unused_data: bytes = decompressor.unused_data
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/server/abc.py` & `easynetwork-1.0.0rc1/src/easynetwork/api_async/client/abc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 # -*- coding: Utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
-"""Network server abstract base classes module"""
+"""Asynchronous network client module"""
 
 from __future__ import annotations
 
-__all__ = [
-    "AbstractNetworkServer",
-]
+__all__ = ["AbstractAsyncNetworkClient"]
 
 from abc import ABCMeta, abstractmethod
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from typing import TYPE_CHECKING, Any, AsyncIterator, Generic, Self, TypeVar
 
-from ..tools.socket import SocketAddress
+from ...tools.socket import SocketAddress
 
 if TYPE_CHECKING:
     from types import TracebackType
 
-_RequestT = TypeVar("_RequestT")
-_ResponseT = TypeVar("_ResponseT")
+    from ..backend.abc import AbstractAsyncBackend
 
+_ReceivedPacketT = TypeVar("_ReceivedPacketT")
+_SentPacketT = TypeVar("_SentPacketT")
 
-class AbstractNetworkServer(Generic[_RequestT, _ResponseT], metaclass=ABCMeta):
-    __slots__ = ("__weakref__",)
 
-    if TYPE_CHECKING:
-        __Self = TypeVar("__Self", bound="AbstractNetworkServer[Any, Any]")
+class AbstractAsyncNetworkClient(Generic[_SentPacketT, _ReceivedPacketT], metaclass=ABCMeta):
+    __slots__ = ("__weakref__",)
 
-    def __enter__(self: __Self) -> __Self:
+    async def __aenter__(self) -> Self:
+        await self.wait_connected()
         return self
 
-    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
-        self.server_close()
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        await self.aclose()
 
     def __getstate__(self) -> Any:  # pragma: no cover
         raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
 
     @abstractmethod
-    def is_closed(self) -> bool:
+    def is_connected(self) -> bool:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def wait_connected(self) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    def is_closing(self) -> bool:
         raise NotImplementedError
 
     @abstractmethod
-    def serve_forever(self) -> None:
+    async def aclose(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def server_close(self) -> None:
+    def get_local_address(self) -> SocketAddress:
         raise NotImplementedError
 
     @abstractmethod
-    def running(self) -> bool:
+    def get_remote_address(self) -> SocketAddress:
         raise NotImplementedError
 
     @abstractmethod
-    def shutdown(self) -> None:
+    async def send_packet(self, packet: _SentPacketT) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def recv_packet(self) -> _ReceivedPacketT:
+        raise NotImplementedError
+
+    async def iter_received_packets(self) -> AsyncIterator[_ReceivedPacketT]:
+        recv_packet = self.recv_packet
+        while True:
+            try:
+                packet = await recv_packet()
+            except OSError:
+                return
+            yield packet
+
+    @abstractmethod
+    def fileno(self) -> int:
         raise NotImplementedError
 
     @abstractmethod
-    def get_address(self) -> SocketAddress:
+    def get_backend(self) -> AbstractAsyncBackend:
         raise NotImplementedError
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/server/udp.py` & `easynetwork-1.0.0rc1/src/easynetwork/api_async/server/udp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,438 +1,474 @@
 # -*- coding: Utf-8 -*-
 # Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine
 #
 #
-"""Network server abstract base classes module"""
+"""Asynchronous network server module"""
 
 from __future__ import annotations
 
-__all__ = ["AbstractUDPNetworkServer"]
+__all__ = ["AsyncUDPNetworkServer"]
 
-import collections as _collections
 import contextlib as _contextlib
 import logging as _logging
-import os as _os
-import selectors as _selectors
-import socket as _socket
-import sys as _sys
-import threading as _threading
-from abc import abstractmethod
-from concurrent.futures import ThreadPoolExecutor as _ThreadPoolExecutor
-from typing import Any, Callable, Generic, TypeVar, final
-
-from ..exceptions import DatagramProtocolParseError
-from ..protocol import DatagramProtocol
-from ..tools._utils import check_real_socket_state as _check_real_socket_state
-from ..tools.socket import MAX_DATAGRAM_BUFSIZE, SocketAddress, new_socket_address
-from .abc import AbstractNetworkServer
+from collections import Counter, deque
+from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterator, Callable, Generic, Iterator, Mapping, TypeVar, final
+from weakref import WeakValueDictionary
+
+from ...exceptions import ClientClosedError, DatagramProtocolParseError
+from ...protocol import DatagramProtocol
+from ...tools._utils import (
+    check_real_socket_state as _check_real_socket_state,
+    recursively_clear_exception_traceback_frames as _recursively_clear_exception_traceback_frames,
+)
+from ...tools.socket import SocketAddress, SocketProxy, new_socket_address
+from ..backend.factory import AsyncBackendFactory
+from ..backend.tasks import SingleTaskRunner
+from .abc import AbstractAsyncNetworkServer
+from .handler import AsyncBaseRequestHandler, AsyncClientInterface
+
+if TYPE_CHECKING:
+    from ..backend.abc import (
+        AbstractAsyncBackend,
+        AbstractAsyncDatagramSocketAdapter,
+        AbstractTask,
+        AbstractTaskGroup,
+        ICondition,
+        IEvent,
+        ILock,
+    )
+
 
 _RequestT = TypeVar("_RequestT")
 _ResponseT = TypeVar("_ResponseT")
 
 
-class AbstractUDPNetworkServer(AbstractNetworkServer[_RequestT, _ResponseT], Generic[_RequestT, _ResponseT]):
+class AsyncUDPNetworkServer(AbstractAsyncNetworkServer, Generic[_RequestT, _ResponseT]):
     __slots__ = (
+        "__backend",
         "__socket",
-        "__addr",
-        "__sendto_lock",
-        "__looping",
-        "__is_shutdown",
-        "__is_up",
+        "__socket_factory",
         "__protocol",
-        "__selector_factory",
-        "__server_selector",
-        "__unsent_datagrams",
-        "__poll_interval",
-        "__thread_pool_size",
+        "__request_handler",
+        "__is_shutdown",
+        "__shutdown_asked",
+        "__sendto_lock",
+        "__client_manager",
+        "__client_datagram_queue",
+        "__mainloop_task",
+        "__service_actions_interval",
         "__logger",
     )
 
     def __init__(
         self,
-        host: str,
+        host: str | None,
         port: int,
         protocol: DatagramProtocol[_ResponseT, _RequestT],
+        request_handler: AsyncBaseRequestHandler[_RequestT, _ResponseT],
         *,
-        family: int = _socket.AF_INET,
+        family: int = 0,
         reuse_port: bool = False,
-        selector_factory: Callable[[], _selectors.BaseSelector] | None = None,
-        poll_interval: float = 0.1,
-        thread_pool_size: int = 0,
+        backend: str | AbstractAsyncBackend | None = None,
+        backend_kwargs: Mapping[str, Any] | None = None,
+        service_actions_interval: float | None = None,
         logger: _logging.Logger | None = None,
     ) -> None:
         super().__init__()
 
-        assert isinstance(protocol, DatagramProtocol)
-
-        if family not in (_socket.AF_INET, _socket.AF_INET6):
-            raise ValueError("Only AF_INET and AF_INET6 families are supported")
+        backend = AsyncBackendFactory.ensure(backend, backend_kwargs)
 
-        self.__socket: _socket.socket | None = None
-        socket = _create_udp_server((host, port), family, reuse_port)
-        try:
-            socket.setblocking(False)
-            self.__addr: SocketAddress = new_socket_address(socket.getsockname(), socket.family)
-            self.__thread_pool_size: int = int(thread_pool_size)
-            self.__sendto_lock: _threading.RLock = _threading.RLock()
-            self.__looping: bool = False
-            self.__is_shutdown: _threading.Event = _threading.Event()
-            self.__is_shutdown.set()
-            self.__is_up: _threading.Event = _threading.Event()
-            self.__is_up.clear()
-            self.__protocol: DatagramProtocol[_ResponseT, _RequestT] = protocol
-            self.__unsent_datagrams: _collections.deque[tuple[bytes, SocketAddress]] = _collections.deque()
-            self.__poll_interval: float = float(poll_interval)
-            if selector_factory is None:
-                selector_factory = _selectors.DefaultSelector
-            self.__selector_factory: Callable[[], _selectors.BaseSelector] = selector_factory
-            self.__server_selector: _selectors.BaseSelector | None = None
-            self.__logger: _logging.Logger = logger or _logging.getLogger(__name__)
-        except BaseException:
-            try:
-                socket.close()
-            finally:
-                raise
+        assert isinstance(protocol, DatagramProtocol)
 
-        self.__socket = socket
+        self.__socket_factory: SingleTaskRunner[AbstractAsyncDatagramSocketAdapter] | None
+        self.__socket_factory = SingleTaskRunner(
+            backend,
+            backend.create_udp_endpoint,
+            local_address=(host, port),
+            remote_address=None,
+            family=family,
+            reuse_port=reuse_port,
+        )
+
+        if service_actions_interval is None:
+            service_actions_interval = 0.1
+
+        self.__service_actions_interval: float = max(service_actions_interval, 0)
+        self.__backend: AbstractAsyncBackend = backend
+        self.__socket: AbstractAsyncDatagramSocketAdapter | None = None
+        self.__protocol: DatagramProtocol[_ResponseT, _RequestT] = protocol
+        self.__request_handler: AsyncBaseRequestHandler[_RequestT, _ResponseT] = request_handler
+        self.__is_shutdown: IEvent = self.__backend.create_event()
+        self.__is_shutdown.set()
+        self.__shutdown_asked: bool = False
+        self.__sendto_lock: ILock = backend.create_lock()
+        self.__mainloop_task: AbstractTask[None] | None = None
+        self.__logger: _logging.Logger = logger or _logging.getLogger(__name__)
+        self.__client_manager: _ClientAPIManager[_ResponseT] = _ClientAPIManager(
+            self.__backend,
+            self.__protocol,
+            self.__sendto_lock,
+            self.__logger,
+        )
+        self.__client_datagram_queue: dict[_ClientAPI[_ResponseT], deque[bytes]] = {}
+
+    def is_serving(self) -> bool:
+        return self.__socket is not None
+
+    async def server_close(self) -> None:
+        if self.__socket_factory is not None:
+            self.__socket_factory.cancel()
+            self.__socket_factory = None
+        self.__stop_mainloop()
+        await self.__close_socket()
+
+    async def __close_socket(self) -> None:
+        async with self.__sendto_lock:
+            socket, self.__socket = self.__socket, None
+            if socket is None:
+                return
+            await socket.aclose()
 
-    def __del__(self) -> None:  # pragma: no cover
+    async def shutdown(self) -> None:
+        self.__stop_mainloop()
+        self.__shutdown_asked = True
         try:
-            socket: _socket.socket | None = self.__socket
-        except AttributeError:
-            return
-        self.__socket = None
-        if socket is not None:
-            socket.close()
-
-    @final
-    def is_closed(self) -> bool:
-        return self.__socket is None
-
-    @final
-    def running(self) -> bool:
-        return not self.__is_shutdown.is_set()
-
-    @final
-    def wait_for_server_to_be_up(self, timeout: float | None = None) -> bool:
-        return self.__is_up.wait(timeout=timeout)
+            await self.__is_shutdown.wait()
+        finally:
+            self.__shutdown_asked = False
 
-    def server_close(self) -> None:
-        if (socket := self.__socket) is None:
-            return
-        self.shutdown()
-        self.__socket = None
-        socket.close()
-
-    def shutdown(self) -> None:
-        self.__looping = False
-        self.__is_shutdown.wait()
+    def __stop_mainloop(self) -> None:
+        if self.__mainloop_task is not None:
+            self.__mainloop_task.cancel()
+            self.__mainloop_task = None
 
-    def serve_forever(self) -> None:
-        if (socket := self.__socket) is None:
-            raise RuntimeError("Closed server")
+    async def serve_forever(self, *, is_up_event: IEvent | None = None) -> None:
         if not self.__is_shutdown.is_set():
             raise RuntimeError("Server is already running")
 
-        with _contextlib.ExitStack() as server_exit_stack:
-            # Final log
-            server_exit_stack.callback(self.__logger.info, "Server stopped")
-            ###########
-
+        async with _contextlib.AsyncExitStack() as server_exit_stack:
             # Wake up server
             self.__is_shutdown.clear()
             server_exit_stack.callback(self.__is_shutdown.set)
+            if is_up_event is not None:
+                # Force is_up_event to be set, in order not to stuck the waiting task
+                server_exit_stack.callback(is_up_event.set)
             ################
 
-            # Setup selector
-            server_selector: _selectors.BaseSelector = self.__selector_factory()
+            # Bind and activate
+            assert self.__socket is None
+            if self.__socket_factory is None:
+                raise RuntimeError("Closed server")
+            self.__socket = await self.__socket_factory.run()
+            self.__socket_factory = None
+            ###################
 
-            def _reset_selector(self: AbstractUDPNetworkServer[Any, Any]) -> None:
-                self.__server_selector = None
-
-            self.__server_selector = server_selector
-            server_exit_stack.callback(_reset_selector, self)
-            server_exit_stack.callback(server_selector.close)
+            # Final teardown
+            server_exit_stack.callback(self.__logger.info, "Server stopped")
+            server_exit_stack.push_async_callback(lambda: self.__backend.ignore_cancellation(self.server_close()))
             ################
 
-            # Flush unsent datagrams before shutdown
-            server_exit_stack.callback(self.__unsent_datagrams.clear)
-            server_exit_stack.callback(self.__flush_unsent_datagrams)
-            ###############
-
-            # Setup client requests' thread pool
-            request_executor: _ThreadPoolExecutor | None = None
-            if self.__thread_pool_size != 0:
-                request_executor = _ThreadPoolExecutor(
-                    max_workers=self.__thread_pool_size if self.__thread_pool_size != -1 else None,
-                    thread_name_prefix=f"{self.__class__.__name__}[request_executor]",
-                )
-                server_exit_stack.callback(request_executor.shutdown, wait=True, cancel_futures=False)
-                server_exit_stack.callback(self.__logger.info, "Server loop break, waiting for thread pool to be closed...")
-            ####################################
+            # Initialize request handler
+            self.__request_handler.set_async_backend(self.__backend)
+            await self.__request_handler.service_init()
+            server_exit_stack.callback(self.__client_manager.clear)
+            server_exit_stack.push_async_callback(self.__request_handler.service_quit)
+            server_exit_stack.push_async_callback(self.__close_socket)
+            ############################
+
+            # Setup task group
+            task_group: AbstractTaskGroup = await server_exit_stack.enter_async_context(self.__backend.create_task_group())
+            server_exit_stack.callback(self.__logger.info, "Server loop break, waiting for remaining tasks...")
+            ##################
 
             # Enable socket
-            server_selector.register(socket, _selectors.EVENT_READ)
-            self.__logger.info("Start serving at %s", self.__addr)
+            address: SocketAddress = new_socket_address(self.__socket.get_local_address(), self.__socket.socket().family)
+            self.__logger.info("Start serving at %s", address)
+            del address
             #################
 
-            # Pull methods to local namespace
-            select = server_selector.select
-            flush_unsent_datagrams = self.__flush_unsent_datagrams
-            handle_received_datagram = self.__handle_received_datagram
-            #################################
-
-            # Pull globals to local namespace
-            poll_interval: float = self.__poll_interval
-            EVENT_READ: int = _selectors.EVENT_READ
-            EVENT_WRITE: int = _selectors.EVENT_WRITE
-            #################################
-
             # Server is up
-            def _reset_loop_state(self: AbstractUDPNetworkServer[Any, Any]) -> None:
-                self.__looping = False
-
-            self.__looping = True
-            server_exit_stack.callback(_reset_loop_state, self)
-            self.__is_up.set()
-            server_exit_stack.callback(self.__is_up.clear)
+            if is_up_event is not None:
+                is_up_event.set()
+            task_group.start_soon(self.__service_actions_task)
             ##############
 
             # Main loop
-            while self.__looping:
-                ready: int
-                try:
-                    _, ready = select(poll_interval)[0]
-                except IndexError:
-                    ready = 0
-                if not self.__looping:  # shutdown() called during select()
-                    break  # type: ignore[unreachable]
-
-                if ready & EVENT_WRITE:
-                    flush_unsent_datagrams()
-
-                if socket not in server_selector.get_map():  # Error occured during process
-                    break
-
-                if ready & EVENT_READ:
-                    handle_received_datagram(request_executor)
-
-                if socket not in server_selector.get_map():  # Error occured during process
-                    break
-
-                try:
-                    self.service_actions()
-                except Exception:
-                    self.__logger.exception("Error occured in self.service_actions()")
-
-    def service_actions(self) -> None:
-        pass
-
-    def __handle_received_datagram(self, request_executor: _ThreadPoolExecutor | None) -> None:
-        selector = self.__server_selector
-        socket: _socket.socket | None = self.__socket
-        assert selector is not None and socket is not None, "Closed server"
-        logger: _logging.Logger = self.__logger
-        try:
-            datagram, client_address = socket.recvfrom(MAX_DATAGRAM_BUFSIZE)
-        except (TimeoutError, BlockingIOError, InterruptedError):
-            return
-        except OSError:
-            logger.exception("socket.recvfrom(): Error occured")
-            _remove_event_mask(selector, socket, _selectors.EVENT_READ | _selectors.EVENT_WRITE)
-            self.__looping = False  # The socket is not usable anymore, shutdown server loop
-            return
-        client_address = new_socket_address(client_address, socket.family)
-        logger.debug("Received a datagram from %s", client_address)
+            self.__mainloop_task = task_group.start_soon(self.__receive_datagrams_task, self.__socket, task_group)
+            if self.__shutdown_asked:
+                self.__mainloop_task.cancel()
+            try:
+                await self.__mainloop_task.join()
+            finally:
+                self.__mainloop_task = None
 
-        if not self.accept_request_from(client_address):
+    async def __receive_datagrams_task(
+        self,
+        socket: AbstractAsyncDatagramSocketAdapter,
+        task_group: AbstractTaskGroup,
+    ) -> None:
+        socket_family: int = socket.socket().family
+        datagram_received_task = self.__datagram_received_task
+        logger = self.__logger
+        while True:
+            datagram, client_address = await socket.recvfrom()
+            client_address = new_socket_address(client_address, socket_family)
+            logger.debug("Received a datagram from %s", client_address)
+            task_group.start_soon(datagram_received_task, socket, datagram, client_address, task_group)
+            del datagram, client_address
+
+    async def __service_actions_task(self) -> None:
+        request_handler = self.__request_handler
+        backend = self.__backend
+        if self.__service_actions_interval == float("+inf"):
             return
-
-        try:
-            request: _RequestT = self.__protocol.build_packet_from_datagram(datagram)
-        except DatagramProtocolParseError as exc:
-            logger.debug("Malformed request sent by %s", client_address)
+        while True:
+            await backend.sleep(self.__service_actions_interval)
             try:
-                self.bad_request(client_address, exc.error_type, exc.message, exc.error_info)
+                await request_handler.service_actions()
             except Exception:
-                self.handle_error(client_address, _get_exception)
-            return
-        except Exception:
-            self.handle_error(client_address, _get_exception)
-            return
-        else:
-            del datagram
-
-        logger.debug("Processing request sent by %s", client_address)
-        if request_executor is None:
-            self.__execute_request(request, client_address)
-        else:
-            try:
-                request_executor.submit(self.__execute_request, request, client_address)
-            except RuntimeError:  # shutdown() has been called()
-                pass
+                self.__logger.exception("Error occurred in request_handler.service_actions()")
 
-    def __execute_request(self, request: _RequestT, client_address: SocketAddress) -> None:
-        try:
-            self.process_request(request, client_address)
-        except BaseException:
-            self.handle_error(client_address, _get_exception)
-
-    def accept_request_from(self, client_address: SocketAddress) -> bool:
-        return True
-
-    @abstractmethod
-    def process_request(self, request: _RequestT, client_address: SocketAddress) -> None:
-        raise NotImplementedError
-
-    def bad_request(
+    async def __datagram_received_task(
         self,
+        socket: AbstractAsyncDatagramSocketAdapter,
+        datagram: bytes,
         client_address: SocketAddress,
-        error_type: DatagramProtocolParseError.ParseErrorType,
-        message: str,
-        error_info: Any,
+        task_group: AbstractTaskGroup,
     ) -> None:
-        pass
+        client = self.__client_manager.get(socket, client_address)
+        backend = self.__backend
 
-    def handle_error(self, client_address: SocketAddress, exc_info: Callable[[], BaseException | None]) -> None:
-        exception = exc_info()
-        if exception is None:
-            return
+        async with self.__client_manager.lock(client) as condition:
+            datagram_queue: deque[bytes] | None = self.__client_datagram_queue.get(client)
+            if datagram_queue is not None:
+                datagram_queue.append(datagram)
+                condition.notify()
+                del client
+                return
+            request_handler_generator: AsyncGenerator[None, _RequestT] | None = None
+            datagram_queue = deque()  # Add datagram after creating the generator
+            with self.__suppress_and_log_remaining_exception(client_address):
+                try:
+                    request_handler_generator = await self.__new_request_handler(client)
+                    datagram_queue.append(datagram)
+                    while True:
+                        if not datagram_queue:
+                            self.__client_datagram_queue[client] = datagram_queue
+                            try:
+                                await condition.wait()
+                            finally:
+                                del self.__client_datagram_queue[client]
+                            assert len(datagram_queue) > 0, f"{len(datagram_queue)=}"
+                        datagram = datagram_queue.popleft()
+                        try:
+                            request: _RequestT = self.__protocol.build_packet_from_datagram(datagram)
+                        except DatagramProtocolParseError as exc:
+                            self.__logger.debug("Malformed request sent by %s", client.address)
+                            try:
+                                _recursively_clear_exception_traceback_frames(exc)
+                            except RecursionError:
+                                self.__logger.warning("Recursion depth reached when clearing exception's traceback frames")
+                            await self.__request_handler.bad_request(client, exc)
+                            await backend.coro_yield()
+                            continue
+                        finally:
+                            del datagram
+
+                        self.__logger.debug("Processing request sent by %s", client.address)
+                        try:
+                            await request_handler_generator.asend(request)
+                        except StopAsyncIteration:
+                            request_handler_generator = None
+                            return
+                        except BaseException:
+                            request_handler_generator = None
+                            raise
+                        finally:
+                            del request
+                        await backend.coro_yield()
+                except (Exception, self.__backend.get_cancelled_exc_class()) as exc:
+                    await self.__throw_error(request_handler_generator, exc)
+                    raise
+                finally:
+                    del client
+                    async with (
+                        _contextlib.aclosing(request_handler_generator)
+                        if request_handler_generator is not None
+                        else _contextlib.nullcontext()
+                    ):
+                        datagram_received_task = self.__datagram_received_task
+                        for datagram in datagram_queue:
+                            task_group.start_soon(datagram_received_task, socket, datagram, client_address, task_group)
 
+    async def __new_request_handler(self, client: AsyncClientInterface[_ResponseT]) -> AsyncGenerator[None, _RequestT]:
+        request_handler_generator = self.__request_handler.handle(client)
         try:
-            logger: _logging.Logger = self.__logger
+            await anext(request_handler_generator)
+        except StopAsyncIteration:
+            raise RuntimeError("request_handler.handle() async generator did not yield") from None
+        return request_handler_generator
 
-            logger.error("-" * 40)
-            logger.error("Exception occurred during processing of request from %s", client_address, exc_info=exception)
-            logger.error("-" * 40)
+    async def __throw_error(self, request_handler_generator: AsyncGenerator[None, _RequestT] | None, exc: BaseException) -> None:
+        try:
+            if request_handler_generator is not None:
+                with _contextlib.suppress(StopAsyncIteration):
+                    await request_handler_generator.athrow(exc)
         finally:
-            del exception
+            del exc
 
-    def send_packet_to(self, packet: _ResponseT, client_address: SocketAddress) -> None:
-        selector = self.__server_selector
-        assert selector is not None, "Closed server"
+    @_contextlib.contextmanager
+    def __suppress_and_log_remaining_exception(self, client_address: SocketAddress) -> Iterator[None]:
         try:
-            response: bytes = self.__protocol.make_datagram(packet)
+            yield
         except Exception:
-            self.handle_error(client_address, _get_exception)
-            return
-        with self.__sendto_lock:
-            socket = self.__socket
-            assert socket is not None
-
-            logger: _logging.Logger = self.__logger
-            unsent_datagrams = self.__unsent_datagrams
-
-            if unsent_datagrams:
-                logger.debug("A response has been queued for %s", client_address)
-                unsent_datagrams.append((response, client_address))
-                return
-            logger.debug("A response will be sent to %s", client_address)
-            try:
-                socket.sendto(response, client_address)
-                _check_real_socket_state(socket)
-            except (TimeoutError, BlockingIOError, InterruptedError):
-                logger.debug("Failed to send datagram to %s, queue it.", client_address)
-                unsent_datagrams.append((response, client_address))
-                _add_event_mask(selector, socket, _selectors.EVENT_WRITE)
-            except OSError:
-                logger.exception("Failed to send datagram to %s", client_address)
-                _remove_event_mask(selector, socket, _selectors.EVENT_READ | _selectors.EVENT_WRITE)
-                self.__looping = False  # The socket is not usable anymore, shutdown server loop
-            else:
-                logger.debug("Datagram successfully sent to %s.", client_address)
-
-    def __flush_unsent_datagrams(self) -> None:
-        selector = self.__server_selector
-        assert selector is not None, "Closed server"
-
-        with self.__sendto_lock:
-            socket = self.__socket
-            assert socket is not None
-
-            logger: _logging.Logger = self.__logger
-            unsent_datagrams = self.__unsent_datagrams
-            while unsent_datagrams:
-                response, client_address = unsent_datagrams.popleft()
-                logger.debug("Try to send saved datagram to %s", client_address)
-                try:
-                    socket.sendto(response, client_address)
-                    _check_real_socket_state(socket)
-                except (TimeoutError, BlockingIOError, InterruptedError):
-                    unsent_datagrams.appendleft((response, client_address))
-                    logger.debug("Failed to send datagram to %s, bail out.", client_address)
-                    return
-                except OSError:
-                    logger.exception("Failed to send datagram to %s", client_address)
-                    _remove_event_mask(selector, socket, _selectors.EVENT_READ | _selectors.EVENT_WRITE)
-                    self.__looping = False  # The socket is not usable anymore, shutdown server loop
-                    return
-                else:
-                    logger.debug("Datagram successfully sent to %s.", client_address)
-            # end while
-            _remove_event_mask(selector, socket, _selectors.EVENT_WRITE)
+            self.__logger.error("-" * 40)
+            self.__logger.exception("Exception occurred during processing of request from %s", client_address)
+            self.__logger.error("-" * 40)
+
+    def get_backend(self) -> AbstractAsyncBackend:
+        return self.__backend
 
-    @final
-    def protocol(self) -> DatagramProtocol[_ResponseT, _RequestT]:
+    def get_protocol(self) -> DatagramProtocol[_ResponseT, _RequestT]:
         return self.__protocol
 
-    @final
-    def get_address(self) -> SocketAddress:
-        return self.__addr
+    @property
+    def socket(self) -> SocketProxy | None:
+        if (socket := self.__socket) is None:
+            return None
+        return SocketProxy(socket.socket())
 
     @property
-    @final
     def logger(self) -> _logging.Logger:
         return self.__logger
 
 
-def _create_udp_server(address: tuple[str, int], family: int, reuse_port: bool) -> _socket.socket:
-    socket = _socket.socket(family, _socket.SOCK_DGRAM)
-    try:
-        if _os.name not in ("nt", "cygwin") and hasattr(_socket, "SO_REUSEADDR"):
-            try:
-                socket.setsockopt(_socket.SOL_SOCKET, _socket.SO_REUSEADDR, 1)
-            except OSError:
-                pass
-
-        if reuse_port:
-            if not hasattr(_socket, "SO_REUSEPORT"):
-                raise ValueError("SO_REUSEPORT not supported on this platform")
-            socket.setsockopt(_socket.SOL_SOCKET, getattr(_socket, "SO_REUSEPORT"), 1)
+class _ClientAPIManager(Generic[_ResponseT]):
+    __slots__ = (
+        "__clients",
+        "__per_client_lock",
+        "__per_client_lock_count",
+        "__backend",
+        "__protocol",
+        "__send_lock",
+        "__logger",
+        "__weakref__",
+    )
+
+    def __init__(
+        self,
+        backend: AbstractAsyncBackend,
+        protocol: DatagramProtocol[_ResponseT, Any],
+        send_lock: ILock,
+        logger: _logging.Logger,
+    ) -> None:
+        super().__init__()
+
+        self.__clients: WeakValueDictionary[tuple[AbstractAsyncDatagramSocketAdapter, SocketAddress], _ClientAPI[_ResponseT]]
+        self.__clients = WeakValueDictionary()
+        self.__backend: AbstractAsyncBackend = backend
+        self.__protocol: DatagramProtocol[_ResponseT, Any] = protocol
+        self.__send_lock: ILock = send_lock
+        self.__logger: _logging.Logger = logger
+        self.__per_client_lock: dict[_ClientAPI[_ResponseT], ICondition] = {}
+        self.__per_client_lock_count: Counter[_ClientAPI[_ResponseT]] = Counter()
+
+    def clear(self) -> None:
+        self.__clients.clear()
+
+    def get(self, socket: AbstractAsyncDatagramSocketAdapter, address: SocketAddress) -> _ClientAPI[_ResponseT]:
+        key = (socket, address)
+        try:
+            return self.__clients[key]
+        except KeyError:
+            client = _ClientAPI(self.__backend, address, socket, self.__protocol, self.__send_lock, self.__logger)
+            self.__clients[key] = client
+            return client
+
+    @_contextlib.asynccontextmanager
+    async def lock(self, client: _ClientAPI[_ResponseT]) -> AsyncIterator[ICondition]:
+        condition = self.__per_client_lock.get(client)
+        if condition is None:
+            self.__per_client_lock[client] = condition = self.__backend.create_condition_var()
+        self.__per_client_lock_count[client] += 1
+        try:
+            async with condition:
+                yield condition
+        finally:
+            self.__per_client_lock_count[client] -= 1
+            assert self.__per_client_lock_count[client] >= 0, f"{self.__per_client_lock_count[client]=}"
+            if self.__per_client_lock_count[client] == 0:
+                del self.__per_client_lock_count[client], self.__per_client_lock[client]
+            del client
+
+
+@final
+class _ClientAPI(AsyncClientInterface[_ResponseT]):
+    __slots__ = (
+        "__backend",
+        "__socket_ref",
+        "__socket_proxy",
+        "__protocol",
+        "__send_lock",
+        "__h",
+        "__logger",
+    )
+
+    def __init__(
+        self,
+        backend: AbstractAsyncBackend,
+        address: SocketAddress,
+        socket: AbstractAsyncDatagramSocketAdapter,
+        protocol: DatagramProtocol[_ResponseT, Any],
+        send_lock: ILock,
+        logger: _logging.Logger,
+    ) -> None:
+        super().__init__(address)
 
-        if _socket.has_ipv6 and family == _socket.AF_INET6:
+        import weakref
+
+        self.__backend: AbstractAsyncBackend = backend
+        self.__socket_ref: Callable[[], AbstractAsyncDatagramSocketAdapter | None] = weakref.ref(socket)
+        self.__socket_proxy: SocketProxy = SocketProxy(socket.socket())
+        self.__h: int | None = None
+        self.__protocol: DatagramProtocol[_ResponseT, Any] = protocol
+        self.__send_lock: ILock = send_lock
+        self.__logger: _logging.Logger = logger
+
+    def __hash__(self) -> int:
+        if (h := self.__h) is None:
+            self.__h = h = hash((_ClientAPI, self.address, 0xFF))
+        return h
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, _ClientAPI):
+            return NotImplemented
+        return self.address == other.address
+
+    def is_closing(self) -> bool:
+        return (socket := self.__socket_ref()) is None or socket.is_closing()
+
+    async def aclose(self) -> None:
+        await self.__backend.coro_yield()
+
+    async def send_packet(self, packet: _ResponseT, /) -> None:
+        async with self.__send_lock:
+            socket = self.__check_closed()
+            datagram: bytes = self.__protocol.make_datagram(packet)
             try:
-                socket.setsockopt(_socket.IPPROTO_IPV6, _socket.IPV6_V6ONLY, 1)
-            except (OSError, AttributeError):
-                pass
-
-        socket.bind(address)
-    except BaseException:
-        socket.close()
-        raise
-
-    return socket
-
-
-def _get_exception() -> BaseException | None:
-    return _sys.exc_info()[1]
-
-
-def _add_event_mask(selector: _selectors.BaseSelector, socket: _socket.socket, event_mask: int) -> None:
-    try:
-        events: int = selector.get_key(socket).events
-    except KeyError:
-        selector.register(socket, event_mask)
-        return
-    selector.modify(socket, events | event_mask)
-
-
-def _remove_event_mask(selector: _selectors.BaseSelector, socket: _socket.socket, event_mask: int) -> None:
-    try:
-        events: int = selector.get_key(socket).events
-    except KeyError:
-        return
-    events = events & ~event_mask
-    if events:
-        selector.modify(socket, events)
-    else:
-        selector.unregister(socket)
+                del packet
+                self.__logger.debug("A datagram will be sent to %s", self.address)
+                await socket.sendto(datagram, self.address)
+                _check_real_socket_state(self.socket)
+                self.__logger.debug("Datagram successfully sent to %s.", self.address)
+            finally:
+                del datagram
+
+    def __check_closed(self) -> AbstractAsyncDatagramSocketAdapter:
+        socket = self.__socket_ref()
+        if socket is None or socket.is_closing():
+            raise ClientClosedError("Closed client")
+        return socket
+
+    @property
+    def socket(self) -> SocketProxy:
+        return self.__socket_proxy
```

### Comparing `easynetwork-1.0.0.dev1/src/easynetwork/tools/stream.py` & `easynetwork-1.0.0rc1/src/easynetwork/tools/stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 __all__ = [
     "StreamDataConsumer",
     "StreamDataProducer",
 ]
 
 from collections import deque
-from threading import Lock
 from typing import Any, Generator, Generic, Iterator, TypeVar, final
 
 from ..exceptions import StreamProtocolParseError
 from ..protocol import StreamProtocol
+from .lock import ForkSafeLock
 
 _SentPacketT = TypeVar("_SentPacketT")
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
 
 
 @final
 @Iterator.register
@@ -32,15 +32,18 @@
 
     def __init__(self, protocol: StreamProtocol[_SentPacketT, Any]) -> None:
         super().__init__()
         assert isinstance(protocol, StreamProtocol)
         self.__p: StreamProtocol[_SentPacketT, Any] = protocol
         self.__g: Generator[bytes, None, None] | None = None
         self.__q: deque[_SentPacketT] = deque()
-        self.__lock = Lock()
+
+        from threading import Lock
+
+        self.__lock = ForkSafeLock(Lock)
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             generator, self.__g = self.__g, None
         except AttributeError:
             return
         try:
@@ -49,15 +52,15 @@
         finally:
             del generator
 
     def __iter__(self) -> Iterator[bytes]:
         return self
 
     def __next__(self) -> bytes:
-        with self.__lock:
+        with self.__lock.get():
             protocol = self.__p
             queue: deque[_SentPacketT] = self.__q
             generator: Generator[bytes, None, None] | None
             while (generator := self.__g) is not None or queue:
                 if generator is None:
                     generator = protocol.generate_chunks(queue.popleft())
                 else:
@@ -71,29 +74,29 @@
                     self.__g = generator
                     return chunk
                 finally:
                     del generator
             raise StopIteration
 
     def pending_packets(self) -> bool:
-        with self.__lock:
+        with self.__lock.get():
             return self.__g is not None or bool(self.__q)
 
     def queue(self, *packets: _SentPacketT) -> None:
         if not packets:
             return
-        with self.__lock:
+        with self.__lock.get():
             self.__q.extend(packets)
 
     def clear(self) -> None:
-        with self.__lock:
+        with self.__lock.get():
+            self.__q.clear()
             generator, self.__g = self.__g, None
             if generator is not None:
                 generator.close()
-            self.__q.clear()
 
 
 @final
 @Iterator.register
 class StreamDataConsumer(Generic[_ReceivedPacketT]):
     __slots__ = ("__p", "__b", "__c", "__lock")
 
@@ -102,15 +105,18 @@
 
     def __init__(self, protocol: StreamProtocol[Any, _ReceivedPacketT]) -> None:
         super().__init__()
         assert isinstance(protocol, StreamProtocol)
         self.__p: StreamProtocol[Any, _ReceivedPacketT] = protocol
         self.__c: Generator[None, bytes, tuple[_ReceivedPacketT, bytes]] | None = None
         self.__b: bytes = b""
-        self.__lock = Lock()
+
+        from threading import Lock
+
+        self.__lock = ForkSafeLock(Lock)
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             consumer, self.__c = self.__c, None
         except AttributeError:
             return
         try:
@@ -119,15 +125,15 @@
         finally:
             del consumer
 
     def __iter__(self) -> Iterator[_ReceivedPacketT]:
         return self
 
     def __next__(self) -> _ReceivedPacketT:
-        with self.__lock:
+        with self.__lock.get():
             chunk: bytes = self.__b
             if not chunk:
                 raise StopIteration
             consumer, self.__c = self.__c, None
             if consumer is None:
                 consumer = self.__p.build_packet_from_chunks()
                 try:
@@ -137,34 +143,34 @@
             self.__b = b""
             packet: _ReceivedPacketT
             try:
                 consumer.send(chunk)
             except StopIteration as exc:
                 packet, chunk = exc.value
             except StreamProtocolParseError as exc:
-                self.__b, exc.remaining_data = exc.remaining_data, b""
+                self.__b, exc.remaining_data = bytes(exc.remaining_data), b""
                 raise
             else:
                 self.__c = consumer
                 raise StopIteration
             finally:
                 del consumer
             self.__b = bytes(chunk)
             return packet
 
     def feed(self, chunk: bytes) -> None:
         assert isinstance(chunk, (bytes, bytearray))
         if not chunk:
             return
-        with self.__lock:
+        with self.__lock.get():
             self.__b += chunk
 
     def get_buffer(self) -> bytes:
-        with self.__lock:
-            return self.__b[:]
+        with self.__lock.get():
+            return self.__b
 
     def clear(self) -> None:
-        with self.__lock:
+        with self.__lock.get():
+            self.__b = b""
             consumer, self.__c = self.__c, None
             if consumer is not None:
                 consumer.close()
-            self.__b = b""
```

### Comparing `easynetwork-1.0.0.dev1/tests/tools.py` & `easynetwork-1.0.0rc1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_communication/serializer.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_communication/serializer.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_client/test_tcp.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,25 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
+import socketserver
+import ssl
 from concurrent.futures import Future
 from socket import AF_INET, IPPROTO_TCP, SHUT_WR, TCP_NODELAY, socket as Socket
 from typing import Any, Callable, Iterator
 
-from easynetwork.client.tcp import TCPNetworkClient
+from easynetwork.api_sync.client.tcp import TCPNetworkClient
 from easynetwork.exceptions import ClientClosedError, StreamProtocolParseError
 from easynetwork.protocol import StreamProtocol
 from easynetwork.tools.socket import IPv4SocketAddress, IPv6SocketAddress
 
 import pytest
 
-from ....tools import TimeTest
-
-
-# Origin: https://gist.github.com/4325783, by Geert Jansen.  Public domain.
-# Cannot use socket.socketpair() vendored with Python on unix since it is required to use AF_UNIX family :)
-@pytest.fixture
-def socket_pair(localhost: str, tcp_socket_factory: Callable[[], Socket]) -> Iterator[tuple[Socket, Socket]]:
-    # We create a connected TCP socket. Note the trick with
-    # setblocking(False) that prevents us from having to create a thread.
-    lsock = tcp_socket_factory()
-    try:
-        lsock.bind((localhost, 0))
-        lsock.listen()
-        # On IPv6, ignore flow_info and scope_id
-        addr, port = lsock.getsockname()[:2]
-        csock = tcp_socket_factory()
-        try:
-            csock.setblocking(False)
-            try:
-                csock.connect((addr, port))
-            except (BlockingIOError, InterruptedError):
-                pass
-            csock.setblocking(True)
-            ssock, _ = lsock.accept()
-        except:  # noqa
-            csock.close()
-            raise
-    finally:
-        lsock.close()
-    with ssock:  # csock will be closed later by tcp_socket_factory() teardown
-        yield ssock, csock
+from .....tools import TimeTest
 
 
 class TestTCPNetworkClient:
     @pytest.fixture
     @staticmethod
     def server(socket_pair: tuple[Socket, Socket]) -> Socket:
         server = socket_pair[0]
@@ -56,60 +28,60 @@
 
     @pytest.fixture
     @staticmethod
     def client(
         socket_pair: tuple[Socket, Socket],
         stream_protocol: StreamProtocol[str, str],
     ) -> Iterator[TCPNetworkClient[str, str]]:
-        with TCPNetworkClient(socket_pair[1], stream_protocol, give=False) as client:
+        with TCPNetworkClient(socket_pair[1], stream_protocol) as client:
             client.socket.setsockopt(IPPROTO_TCP, TCP_NODELAY, 1)
             yield client
 
-    def test____close____double_close(self, client: TCPNetworkClient[str, str]) -> None:
+    def test____close____idempotent(self, client: TCPNetworkClient[str, str]) -> None:
         assert not client.is_closed()
         client.close()
         assert client.is_closed()
         client.close()
         assert client.is_closed()
 
     def test____send_packet____default(self, client: TCPNetworkClient[str, str], server: Socket) -> None:
         client.send_packet("ABCDEF")
         assert server.recv(1024) == b"ABCDEF\n"
 
-    @pytest.mark.platform_linux  # Windows and macOs raise ConnectionAbortedError but in the 2nd send() call
+    @pytest.mark.platform_linux  # Windows and MacOS raise ConnectionAbortedError but in the 2nd send() call
     def test____send_packet____connection_error____fresh_connection_closed_by_server(
         self,
         client: TCPNetworkClient[str, str],
         server: Socket,
     ) -> None:
         server.close()
-        with pytest.raises(ConnectionError):
+        with pytest.raises(ConnectionAbortedError):
             client.send_packet("ABCDEF")
 
-    @pytest.mark.platform_linux  # Windows and macOs raise ConnectionAbortedError but in the 2nd send() call
+    @pytest.mark.platform_linux  # Windows and MacOS raise ConnectionAbortedError but in the 2nd send() call
     def test____send_packet____connection_error____after_previous_successful_try(
         self,
         client: TCPNetworkClient[str, str],
         server: Socket,
     ) -> None:
         client.send_packet("ABCDEF")
         assert server.recv(1024) == b"ABCDEF\n"
         server.close()
-        with pytest.raises(ConnectionError):
+        with pytest.raises(ConnectionAbortedError):
             client.send_packet("ABCDEF")
 
     def test____send_packet____connection_error____partial_read_then_close(
         self,
         client: TCPNetworkClient[str, str],
         server: Socket,
     ) -> None:
         client.send_packet("ABC")
         assert server.recv(1) == b"A"
         server.close()
-        with pytest.raises(ConnectionError):
+        with pytest.raises(ConnectionAbortedError):
             client.send_packet("DEF")
 
     def test____send_packet____closed_client(self, client: TCPNetworkClient[str, str]) -> None:
         client.close()
         with pytest.raises(ClientClosedError):
             client.send_packet("ABCDEF")
 
@@ -219,7 +191,151 @@
     def test____get_remote_address____consistency(self, socket_family: int, client: TCPNetworkClient[str, str]) -> None:
         address = client.get_remote_address()
         if socket_family == AF_INET:
             assert isinstance(address, IPv4SocketAddress)
         else:
             assert isinstance(address, IPv6SocketAddress)
         assert address == client.socket.getpeername()
+
+
+class TCPServer(socketserver.TCPServer):
+    class RequestHandler(socketserver.StreamRequestHandler):
+        def handle(self) -> None:
+            data: bytes = self.rfile.readline()
+            self.wfile.write(data)
+
+    allow_reuse_address = True
+
+    def __init__(
+        self,
+        server_address: tuple[str, int],
+        socket_family: int,
+        ssl_context: ssl.SSLContext | None = None,
+    ) -> None:
+        self.address_family = socket_family
+        super().__init__(server_address, self.RequestHandler)
+        self.ssl_context: ssl.SSLContext | None = ssl_context
+
+    def get_request(self) -> tuple[Socket, Any]:
+        socket, client_address = super().get_request()
+
+        if self.ssl_context:
+            socket = self.ssl_context.wrap_socket(socket, server_side=True, do_handshake_on_connect=True)
+
+        return socket, client_address
+
+
+class TestTCPNetworkClientConnection:
+    @pytest.fixture(autouse=True)
+    @classmethod
+    def server(cls, localhost_ip: str, socket_family: int) -> Iterator[socketserver.TCPServer]:
+        from threading import Thread
+
+        with TCPServer((localhost_ip, 0), socket_family) as server:
+            server_thread = Thread(target=server.serve_forever)
+            server_thread.start()
+            yield server
+            server.shutdown()
+            server_thread.join()
+
+    @pytest.fixture
+    @staticmethod
+    def remote_address(server: socketserver.TCPServer) -> tuple[str, int]:
+        return server.server_address[:2]  # type: ignore[return-value]
+
+    def test____dunder_init____connect_to_server(
+        self,
+        localhost_ip: str,
+        remote_address: tuple[str, int],
+        stream_protocol: StreamProtocol[str, str],
+    ) -> None:
+        # Arrange
+
+        # Act & Assert
+        with TCPNetworkClient(remote_address, stream_protocol, local_address=(localhost_ip, 0)) as client:
+            client.send_packet("Test")
+            assert client.recv_packet() == "Test"
+
+
+class TestSSLOverTCPNetworkClient:
+    @pytest.fixture(autouse=True)
+    @classmethod
+    def server(
+        cls,
+        localhost_ip: str,
+        socket_family: int,
+        server_ssl_context: ssl.SSLContext,
+    ) -> Iterator[socketserver.TCPServer]:
+        from threading import Thread
+
+        with TCPServer((localhost_ip, 0), socket_family, ssl_context=server_ssl_context) as server:
+            server_thread = Thread(target=server.serve_forever)
+            server_thread.start()
+            yield server
+            server.shutdown()
+            server_thread.join()
+
+    @pytest.fixture
+    @staticmethod
+    def remote_address(server: socketserver.TCPServer) -> tuple[str, int]:
+        return server.server_address[:2]  # type: ignore[return-value]
+
+    def test____dunder_init____handshake_and_shutdown(
+        self,
+        remote_address: tuple[str, int],
+        stream_protocol: StreamProtocol[str, str],
+        client_ssl_context: ssl.SSLContext,
+    ) -> None:
+        # Arrange
+
+        # Act & Assert
+        with TCPNetworkClient(
+            remote_address,
+            stream_protocol,
+            ssl=client_ssl_context,
+            server_hostname="test.example.com",
+        ) as client:
+            client.send_packet("Test")
+            assert client.recv_packet() == "Test"
+
+    def test____dunder_init____use_default_context(
+        self,
+        remote_address: tuple[str, int],
+        stream_protocol: StreamProtocol[str, str],
+        client_ssl_context: ssl.SSLContext,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
+        # Arrange
+        monkeypatch.setattr(ssl, "create_default_context", lambda *args, **kwargs: client_ssl_context)
+
+        # Act & Assert
+        with TCPNetworkClient(
+            remote_address,
+            stream_protocol,
+            ssl=True,
+            server_hostname="test.example.com",
+        ) as client:
+            client.send_packet("Test")
+            assert client.recv_packet() == "Test"
+
+    def test____dunder_init____use_default_context____disable_hostname_check(
+        self,
+        remote_address: tuple[str, int],
+        stream_protocol: StreamProtocol[str, str],
+        client_ssl_context: ssl.SSLContext,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
+        # Arrange
+        check_hostname_by_default: bool = client_ssl_context.check_hostname
+        assert check_hostname_by_default
+        monkeypatch.setattr(ssl, "create_default_context", lambda *args, **kwargs: client_ssl_context)
+
+        # Act & Assert
+        with TCPNetworkClient(
+            remote_address,
+            stream_protocol,
+            ssl=True,
+            server_hostname="",
+        ) as client:
+            assert not client_ssl_context.check_hostname  # It must be set to False if server_hostname is an empty string
+            client.send_packet("Test")
+            assert client.recv_packet() == "Test"
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_communication/test_client/test_udp.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_communication/test_sync/test_client/test_udp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
 from socket import AF_INET, socket as Socket
 from typing import Any, Callable, Iterator
 
-from easynetwork.client.udp import UDPNetworkClient, UDPNetworkEndpoint
+from easynetwork.api_sync.client.udp import UDPNetworkClient, UDPNetworkEndpoint
 from easynetwork.exceptions import ClientClosedError, DatagramProtocolParseError
 from easynetwork.protocol import DatagramProtocol
 from easynetwork.tools.socket import IPv4SocketAddress, IPv6SocketAddress, new_socket_address
 
 import pytest
 
 
 @pytest.fixture
-def udp_socket_factory(request: pytest.FixtureRequest, localhost: str) -> Callable[[], Socket]:
+def udp_socket_factory(request: pytest.FixtureRequest, localhost_ip: str) -> Callable[[], Socket]:
     udp_socket_factory: Callable[[], Socket] = request.getfixturevalue("udp_socket_factory")
 
     def bound_udp_socket_factory() -> Socket:
         sock = udp_socket_factory()
-        sock.bind((localhost, 0))
+        sock.bind((localhost_ip, 0))
         return sock
 
     return bound_udp_socket_factory
 
 
 class TestUDPNetworkClient:
     @pytest.fixture
@@ -32,39 +32,39 @@
         return udp_socket_factory()
 
     @pytest.fixture
     @staticmethod
     def client(
         server: Socket,
         socket_family: int,
-        localhost: str,
+        localhost_ip: str,
         datagram_protocol: DatagramProtocol[str, str],
     ) -> Iterator[UDPNetworkClient[str, str]]:
         address: tuple[str, int] = server.getsockname()[:2]
-        with UDPNetworkClient(address, datagram_protocol, family=socket_family, source_address=(localhost, 0)) as client:
+        with UDPNetworkClient(address, datagram_protocol, family=socket_family, local_address=(localhost_ip, 0)) as client:
             yield client
 
-    def test____close____double_close(self, client: UDPNetworkClient[str, str]) -> None:
+    def test____close____idempotent(self, client: UDPNetworkClient[str, str]) -> None:
         assert not client.is_closed()
         client.close()
         assert client.is_closed()
         client.close()
         assert client.is_closed()
 
     def test____send_packet____default(self, client: UDPNetworkClient[str, str], server: Socket) -> None:
         client.send_packet("ABCDEF")
         assert server.recvfrom(1024) == (b"ABCDEF", client.get_local_address())
 
-    @pytest.mark.platform_linux  # Windows and macOS do not raise error
+    @pytest.mark.platform_linux  # Windows and MacOS do not raise error
     def test____send_packet____connection_refused(self, client: UDPNetworkClient[str, str], server: Socket) -> None:
         server.close()
         with pytest.raises(ConnectionRefusedError):
             client.send_packet("ABCDEF")
 
-    @pytest.mark.platform_linux  # Windows and macOS do not raise error
+    @pytest.mark.platform_linux  # Windows and MacOS do not raise error
     def test____send_packet____connection_refused____after_previous_successful_try(
         self,
         client: UDPNetworkClient[str, str],
         server: Socket,
     ) -> None:
         client.send_packet("ABC")
         assert server.recvfrom(1024) == (b"ABC", client.get_local_address())
@@ -100,15 +100,15 @@
         other_client = udp_socket_factory()
         other_client.sendto(b"ABCDEF", client.get_local_address())
         with pytest.raises(TimeoutError):
             client.recv_packet(timeout=0.1)
 
     def test____recv_packet____closed_client(self, client: UDPNetworkClient[str, str]) -> None:
         client.close()
-        with pytest.raises(OSError):
+        with pytest.raises(ClientClosedError):
             client.recv_packet()
 
     def test____recv_packet____invalid_data(self, client: UDPNetworkClient[str, str], server: Socket) -> None:
         server.sendto("\u00E9".encode("latin-1"), client.get_local_address())
         with pytest.raises(DatagramProtocolParseError):
             client.recv_packet()
 
@@ -117,15 +117,15 @@
         client: UDPNetworkClient[str, str],
         server: Socket,
     ) -> None:
         for p in [b"A", b"B", b"C", b"D", b"E", b"F"]:
             server.sendto(p, client.get_local_address())
 
         # NOTE: Comparison using set because equality check does not verify order
-        assert set(client.iter_received_packets(timeout=1)) == {"A", "B", "C", "D", "E", "F"}
+        assert set(client.iter_received_packets(timeout=0.1)) == {"A", "B", "C", "D", "E", "F"}
 
     def test____fileno____consistency(self, client: UDPNetworkClient[str, str]) -> None:
         assert client.fileno() == client.socket.fileno()
 
     def test____fileno____closed_client(self, client: UDPNetworkClient[str, str]) -> None:
         client.close()
         assert client.fileno() == -1
@@ -154,15 +154,15 @@
         return udp_socket_factory()
 
     @pytest.fixture(params=["WITH_REMOTE", "WITHOUT_REMOTE"])
     @staticmethod
     def client(
         request: pytest.FixtureRequest,
         socket_family: int,
-        localhost: str,
+        localhost_ip: str,
         datagram_protocol: DatagramProtocol[str, str],
     ) -> Iterator[UDPNetworkEndpoint[str, str]]:
         address: tuple[str, int] | None
         match getattr(request, "param"):
             case "WITH_REMOTE":
                 server: Socket = request.getfixturevalue("server")
                 address = server.getsockname()[:2]
@@ -170,19 +170,19 @@
                 address = None
             case invalid:
                 pytest.fail(f"Invalid fixture param, got {invalid!r}")
         with UDPNetworkEndpoint(
             datagram_protocol,
             remote_address=address,
             family=socket_family,
-            source_address=(localhost, 0),
+            local_address=(localhost_ip, 0),
         ) as client:
             yield client
 
-    def test____close____double_close(self, client: UDPNetworkEndpoint[str, str]) -> None:
+    def test____close____idempotent(self, client: UDPNetworkEndpoint[str, str]) -> None:
         assert not client.is_closed()
         client.close()
         assert client.is_closed()
         client.close()
         assert client.is_closed()
 
     @pytest.mark.parametrize("client", ["WITHOUT_REMOTE"], indirect=True)
@@ -236,23 +236,23 @@
 
             client.send_packet_to("ABCDEF", other_client_address)
         else:
             # The given address is not the configured remote address
             with pytest.raises(ValueError):
                 client.send_packet_to("ABCDEF", other_client_address)
 
-    @pytest.mark.platform_linux  # Windows and macOS do not raise error
+    @pytest.mark.platform_linux  # Windows and MacOS do not raise error
     @pytest.mark.parametrize("client", ["WITH_REMOTE"], indirect=True)
     def test____send_packet_to____connection_refused(self, client: UDPNetworkEndpoint[str, str], server: Socket) -> None:
         address = server.getsockname()
         server.close()
         with pytest.raises(ConnectionRefusedError):
             client.send_packet_to("ABCDEF", address)
 
-    @pytest.mark.platform_linux  # Windows and macOS do not raise error
+    @pytest.mark.platform_linux  # Windows and MacOS do not raise error
     @pytest.mark.parametrize("client", ["WITH_REMOTE"], indirect=True)
     def test____send_packet____connection_refused____after_previous_successful_try(
         self,
         client: UDPNetworkEndpoint[str, str],
         server: Socket,
     ) -> None:
         address = server.getsockname()
@@ -325,15 +325,15 @@
         other_client = udp_socket_factory()
         other_client.sendto(b"ABCDEF", client.get_local_address())
         with pytest.raises(TimeoutError):
             client.recv_packet_from(timeout=0.1)
 
     def test____recv_packet_from____closed_client(self, client: UDPNetworkEndpoint[str, str]) -> None:
         client.close()
-        with pytest.raises(OSError):
+        with pytest.raises(ClientClosedError):
             client.recv_packet_from()
 
     def test____recv_packet_from____invalid_data(self, client: UDPNetworkEndpoint[str, str], server: Socket) -> None:
         server.sendto("\u00E9".encode("latin-1"), client.get_local_address())
         with pytest.raises(DatagramProtocolParseError):
             client.recv_packet_from()
 
@@ -344,15 +344,15 @@
         server: Socket,
     ) -> None:
         server_address = new_socket_address(server.getsockname(), socket_family)
         for p in [b"A", b"B", b"C", b"D", b"E", b"F"]:
             server.sendto(p, client.get_local_address())
 
         # NOTE: Comparison using set because equality check does not verify order
-        assert set(client.iter_received_packets_from()) == {
+        assert set(client.iter_received_packets_from(timeout=0.1)) == {
             ("A", server_address),
             ("B", server_address),
             ("C", server_address),
             ("D", server_address),
             ("E", server_address),
             ("F", server_address),
         }
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/base.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,16 +227,14 @@
     def test____incremental_deserialize____invalid_data(
         self,
         serializer_for_deserialization: AbstractIncrementalPacketSerializer[Any, Any],
         invalid_partial_data: bytes,
         invalid_partial_data_extra_data: bytes | None,
     ) -> None:
         # Arrange
-        if invalid_partial_data_extra_data is not None:
-            assert len(invalid_partial_data_extra_data) > 0
         consumer = serializer_for_deserialization.incremental_deserialize()
         next(consumer)
 
         # Act
         with pytest.raises(IncrementalDeserializeError) as exc_info:
             if invalid_partial_data_extra_data:
                 consumer.send(invalid_partial_data + invalid_partial_data_extra_data)
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_base64.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_base64.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: Utf-8 -*-
+# mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import random
-from abc import abstractmethod
 from typing import Any, final
 
 from easynetwork.exceptions import DeserializeError
 from easynetwork.serializers.wrapper.base64 import Base64EncodedSerializer
 
 import pytest
 
@@ -27,23 +27,18 @@
     (random.randbytes(255), "255 random generated bytes"),
 ]
 
 
 class BaseTestBase64EncodedSerializer(BaseTestIncrementalSerializer):
     #### Serializers
 
-    @classmethod
-    @abstractmethod
-    def get_signing_key(cls) -> bytes | None:
-        raise NotImplementedError
-
     @pytest.fixture(scope="class")
     @classmethod
-    def serializer(cls) -> Base64EncodedSerializer[bytes, bytes]:
-        return Base64EncodedSerializer(NoSerialization(), signing_key=cls.get_signing_key())
+    def serializer(cls, checksum: bool | bytes) -> Base64EncodedSerializer[bytes, bytes]:
+        return Base64EncodedSerializer(NoSerialization(), checksum=checksum)
 
     @pytest.fixture(scope="class")
     @staticmethod
     def serializer_for_serialization(serializer: Base64EncodedSerializer[bytes, bytes]) -> Base64EncodedSerializer[bytes, bytes]:
         return serializer
 
     @pytest.fixture(scope="class")
@@ -60,22 +55,26 @@
     def packet_to_serialize(request: Any) -> Any:
         return request.param
 
     #### One-shot Serialize
 
     @pytest.fixture(scope="class")
     @classmethod
-    def expected_complete_data(cls, packet_to_serialize: bytes) -> bytes:
+    def expected_complete_data(cls, packet_to_serialize: bytes, checksum: bool | bytes) -> bytes:
         import base64
+        import hashlib
         import hmac
 
-        key: bytes | None = cls.get_signing_key()
-        if key is not None:
-            key = base64.urlsafe_b64decode(key)
-            packet_to_serialize += hmac.digest(key, packet_to_serialize, "sha256")
+        if checksum:
+            if isinstance(checksum, bytes):
+                key = base64.urlsafe_b64decode(checksum)
+                packet_to_serialize += hmac.digest(key, packet_to_serialize, "sha256")
+            else:
+                packet_to_serialize += hashlib.sha256(packet_to_serialize).digest()
+
         return base64.urlsafe_b64encode(packet_to_serialize)
 
     #### Incremental Serialize
 
     @pytest.fixture(scope="class")
     @staticmethod
     def expected_joined_data(expected_complete_data: bytes) -> bytes:
@@ -112,26 +111,32 @@
     @pytest.fixture(scope="class")
     @staticmethod
     def oneshot_extra_data() -> bytes:
         pytest.skip("Does not recognize extra data")
 
 
 @final
-class TestBase64EncodedSerializerNoKey(BaseTestBase64EncodedSerializer):
-    @classmethod
-    def get_signing_key(cls) -> None:
-        return None
+class TestBase64EncodedSerializerChecksum(BaseTestBase64EncodedSerializer):
+    @pytest.fixture(scope="class", params=[False, True], ids=lambda boolean: f"checksum=={boolean}")
+    @staticmethod
+    def checksum(request: pytest.FixtureRequest) -> bool:
+        return getattr(request, "param")
 
 
 @final
 class TestBase64EncodedSerializerWithKey(BaseTestBase64EncodedSerializer):
     @classmethod
     def get_signing_key(cls) -> bytes:
         return generate_key_from_string("key")
 
+    @pytest.fixture(scope="class")
+    @classmethod
+    def checksum(cls) -> bytes:
+        return cls.get_signing_key()
+
     def test____generate_key____create_url_safe_base64_encoded_bytes(self) -> None:
         # Arrange
         from base64 import urlsafe_b64decode
 
         # Act
         key = Base64EncodedSerializer.generate_key()
 
@@ -144,30 +149,30 @@
         import base64
         import binascii
 
         key: bytes = base64.urlsafe_b64encode(random.randbytes(32))[5:12]  # Removed a lot of data :)
 
         # Act
         with pytest.raises(ValueError, match=r"^signing key must be 32 url-safe base64-encoded bytes\.$") as exc_info:
-            _ = Base64EncodedSerializer(NoSerialization(), signing_key=key)
+            _ = Base64EncodedSerializer(NoSerialization(), checksum=key)
         exception = exc_info.value
 
         # Assert
         assert isinstance(exception.__cause__, binascii.Error)
 
     def test____dunder_init____invalid_key____invalid_base64_encoded_byte_length(self) -> None:
         # Arrange
         import base64
         import binascii
 
         key: bytes = base64.urlsafe_b64encode(random.randbytes(4))
 
         # Act
         with pytest.raises(ValueError, match=r"^signing key must be 32 url-safe base64-encoded bytes\.$") as exc_info:
-            _ = Base64EncodedSerializer(NoSerialization(), signing_key=key)
+            _ = Base64EncodedSerializer(NoSerialization(), checksum=key)
         exception = exc_info.value
 
         # Assert
         assert not isinstance(exception.__cause__, binascii.Error)
 
     def test____deserialize____invalid_signature(
         self,
@@ -175,18 +180,17 @@
         packet_to_serialize: bytes,
         expected_complete_data: bytes,
     ) -> None:
         # Arrange
         import base64
         import hmac
 
-        another_key = generate_key_from_string("another_key")
-        assert another_key != self.get_signing_key()
+        assert generate_key_from_string("another_key") != self.get_signing_key()
         data_with_another_signature = base64.urlsafe_b64encode(
-            packet_to_serialize + hmac.digest(another_key, packet_to_serialize, "sha256")
+            packet_to_serialize + hmac.digest(b"another_key", packet_to_serialize, "sha256")
         )
         assert data_with_another_signature != expected_complete_data
 
         # Act
         with pytest.raises(DeserializeError) as exc_info:
             serializer.deserialize(data_with_another_signature)
         exception = exc_info.value
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_cbor.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_cbor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: Utf-8 -*-
+# mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import dataclasses
 from typing import Any, final
 
 from easynetwork.serializers.cbor import CBOREncoderConfig, CBORSerializer
@@ -10,14 +11,15 @@
 import pytest
 
 from .base import BaseTestIncrementalSerializer
 from .samples.json import SAMPLES
 
 
 @final
+@pytest.mark.feature_cbor
 class TestCBORSerializer(BaseTestIncrementalSerializer):
     #### Serializers
 
     ENCODER_CONFIG = CBOREncoderConfig()
 
     @pytest.fixture(scope="class")
     @classmethod
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_compressors.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_compressors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: Utf-8 -*-
+# mypy: disable_error_code=override
 
 from __future__ import annotations
 
 import random
 from typing import Any, final
 
 from easynetwork.serializers.wrapper.compressor import BZ2CompressorSerializer, ZlibCompressorSerializer
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_encryptor.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_encryptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: Utf-8 -*-
+# mypy: disable_error_code=override
 
 from __future__ import annotations
 
 from typing import Any, Callable, final
 
 from easynetwork.serializers.wrapper.encryptor import EncryptorSerializer
 
 import pytest
 
 from .base import BaseTestIncrementalSerializer, NoSerialization
 from .test_base64 import SAMPLES, generate_key_from_string
 
 
 @final
+@pytest.mark.feature_encryption
 class TestEncryptorSerializer(BaseTestIncrementalSerializer):
     #### Serializers
 
     KEY = generate_key_from_string("key")
 
     @pytest.fixture(scope="class")
     @classmethod
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_json.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_json.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: Utf-8 -*-
+# mypy: disable-error-code=override
 
 from __future__ import annotations
 
 import dataclasses
 from typing import Any, final
 
 from easynetwork.serializers.json import JSONEncoderConfig, JSONSerializer
@@ -67,16 +68,23 @@
     @pytest.fixture(scope="class")
     @staticmethod
     def complete_data_for_incremental_deserialize(complete_data: bytes) -> bytes:
         return complete_data + b"\n"
 
     #### Invalid data
 
-    @pytest.fixture(scope="class")
+    @pytest.fixture(scope="class", params=[b"invalid", b"\0"])
     @staticmethod
-    def invalid_complete_data() -> bytes:
-        return b"invalid"
+    def invalid_complete_data(request: Any) -> bytes:
+        return getattr(request, "param")
 
-    @pytest.fixture(scope="class")
+    @pytest.fixture(scope="class", params=[b"[ invalid ]", b"\0"])
+    @staticmethod
+    def invalid_partial_data(request: Any) -> bytes:
+        return getattr(request, "param")
+
+    @pytest.fixture
     @staticmethod
-    def invalid_partial_data() -> bytes:
-        return b"[ invalid ]"
+    def invalid_partial_data_extra_data(invalid_partial_data: bytes) -> bytes:
+        if invalid_partial_data == b"\0":
+            return b""
+        return b"remaining_data"
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_namedtuple.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_namedtuple.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: Utf-8 -*-
+# mypy: disable_error_code=override
 
 from __future__ import annotations
 
 from typing import Any, NamedTuple, final
 
 from easynetwork.serializers.struct import NamedTupleStructSerializer
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/test_pickle.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/test_pickle.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import pickletools
 from typing import Any, final
 
 from easynetwork.serializers.pickle import PicklerConfig, PickleSerializer, UnpicklerConfig
 
 import pytest
 
-from .base import BaseTestIncrementalSerializer
+from .base import BaseTestSerializer
 from .samples.pickle import SAMPLES
 
 ALL_PROTOCOLS: tuple[int, ...] = tuple(range(0, pickle.HIGHEST_PROTOCOL + 1))
 
 
 @final
-class TestPickleSerializer(BaseTestIncrementalSerializer):
+class TestPickleSerializer(BaseTestSerializer):
     @pytest.fixture(scope="class", params=ALL_PROTOCOLS, ids=lambda p: f"pickle_data_protocol=={p}")
     @staticmethod
     def pickle_data_protocol(request: Any) -> int:
         return request.param
 
     #### Serializers
 
@@ -70,21 +70,14 @@
         if pickler_config is None:
             pickler_config = PicklerConfig()
         data = pickle.dumps(packet_to_serialize, **dataclasses.asdict(pickler_config), buffer_callback=None)
         if pickler_optimize:
             data = pickletools.optimize(data)
         return data
 
-    #### Incremental Serialize
-
-    @pytest.fixture(scope="class")
-    @staticmethod
-    def expected_joined_data(expected_complete_data: bytes) -> bytes:
-        return expected_complete_data
-
     #### One-shot Deserialize
 
     @pytest.fixture(scope="class")
     @staticmethod
     def complete_data(
         packet_to_serialize: Any,
         pickle_data_protocol: int,
@@ -94,21 +87,14 @@
         if unpickler_config is None:
             unpickler_config = UnpicklerConfig()
         data = pickle.dumps(packet_to_serialize, protocol=pickle_data_protocol, fix_imports=unpickler_config.fix_imports)
         if pickler_optimize:
             data = pickletools.optimize(data)
         return data
 
-    #### Incremental Deserialize
-
-    @pytest.fixture(scope="class")
-    @staticmethod
-    def complete_data_for_incremental_deserialize(complete_data: bytes) -> bytes:
-        return complete_data
-
     #### Invalid data
 
     @pytest.fixture
     @staticmethod
     def invalid_complete_data() -> bytes:
         pytest.skip("pickle.Unpickler() raises SystemError for some invalid inputs :)")
```

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/samples/json.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/json.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/tests/functional_test/test_serializers/samples/pickle.py` & `easynetwork-1.0.0rc1/tests/functional_test/test_serializers/samples/pickle.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/tests/other_test/test_import.py` & `easynetwork-1.0.0rc1/tests/other_test/test_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,21 +13,27 @@
     from pkgutil import ModuleInfo
 
 
 @cache
 def _catch_all_easynetwork_packages_and_modules() -> list[ModuleInfo]:
     from pkgutil import walk_packages
 
-    easynetwork_spec = import_module("easynetwork").__spec__
+    result: list[ModuleInfo] = []
 
-    assert easynetwork_spec is not None
+    for module_name in ["easynetwork", "easynetwork_asyncio"]:
+        module = import_module(module_name)
+        module_spec = module.__spec__
 
-    easynetwork_paths = easynetwork_spec.submodule_search_locations or import_module("easynetwork").__path__
+        assert module_spec is not None
 
-    return list(walk_packages(easynetwork_paths, prefix=f"{easynetwork_spec.name}."))
+        module_paths = module_spec.submodule_search_locations or module.__path__
+
+        result.extend(walk_packages(module_paths, prefix=f"{module_spec.name}."))
+
+    return result
 
 
 ALL_EASYNETWORK_PACKAGES = [info.name for info in _catch_all_easynetwork_packages_and_modules() if info.ispkg]
 ALL_EASYNETWORK_MODULES = [info.name for info in _catch_all_easynetwork_packages_and_modules()]
 
 
 @cache
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/conftest.py` & `easynetwork-1.0.0rc1/tests/unit_test/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
 import pathlib
 from socket import AF_INET, IPPROTO_TCP, IPPROTO_UDP, SOCK_DGRAM, SOCK_STREAM, socket as Socket
+from ssl import SSLContext, SSLSocket
 from typing import TYPE_CHECKING, Any, Callable
 
-from easynetwork.converter import AbstractPacketConverter
+from easynetwork.converter import AbstractPacketConverterComposite
 from easynetwork.protocol import DatagramProtocol, StreamProtocol
 from easynetwork.serializers.abc import AbstractIncrementalPacketSerializer, AbstractPacketSerializer
 from easynetwork.tools.stream import StreamDataConsumer, StreamDataProducer
 
 import pytest
 
 if TYPE_CHECKING:
@@ -22,63 +23,98 @@
 def pytest_collection_modifyitems(items: list[pytest.Item]) -> None:
     directory = pathlib.PurePath(__file__).parent
     for item in items:
         if pathlib.PurePath(item.fspath).is_relative_to(directory):
             item.add_marker(pytest.mark.unit)
 
 
-@pytest.fixture(scope="package", autouse=True)
-def dummy_lock_cls(package_mocker: MockerFixture) -> Any:
-    from ._utils import DummyLock
+@pytest.fixture
+def mock_socket_factory(mocker: MockerFixture) -> Callable[[], MagicMock]:
+    def factory() -> MagicMock:
+        mock_socket = mocker.NonCallableMagicMock(spec=Socket)
+        mock_socket.family = AF_INET
+        mock_socket.type = -1
+        mock_socket.proto = 0
+        return mock_socket
 
-    package_mocker.patch("threading.Lock", new=DummyLock)
-    package_mocker.patch("threading.RLock", new=DummyLock)
-    return DummyLock
+    return factory
 
 
 @pytest.fixture(scope="package", autouse=True)
 def original_socket_cls() -> type[Socket]:
     return Socket
 
 
 @pytest.fixture
-def mock_tcp_socket_factory(mocker: MockerFixture) -> Callable[[], MagicMock]:
+def mock_tcp_socket_factory(mock_socket_factory: Callable[[], MagicMock]) -> Callable[[], MagicMock]:
     def factory() -> MagicMock:
-        mock_socket = mocker.NonCallableMagicMock(spec=Socket)
-        mock_socket.family = AF_INET
+        mock_socket = mock_socket_factory()
         mock_socket.type = SOCK_STREAM
         mock_socket.proto = IPPROTO_TCP
         return mock_socket
 
     return factory
 
 
 @pytest.fixture
 def mock_tcp_socket(mock_tcp_socket_factory: Callable[[], MagicMock]) -> MagicMock:
     return mock_tcp_socket_factory()
 
 
 @pytest.fixture
-def mock_udp_socket_factory(mocker: MockerFixture) -> Callable[[], MagicMock]:
+def mock_udp_socket_factory(mock_socket_factory: Callable[[], MagicMock]) -> Callable[[], MagicMock]:
     def factory() -> MagicMock:
-        mock_socket = mocker.NonCallableMagicMock(spec=Socket)
-        mock_socket.family = AF_INET
+        mock_socket = mock_socket_factory()
         mock_socket.type = SOCK_DGRAM
         mock_socket.proto = IPPROTO_UDP
         return mock_socket
 
     return factory
 
 
 @pytest.fixture
 def mock_udp_socket(mock_udp_socket_factory: Callable[[], MagicMock]) -> MagicMock:
     return mock_udp_socket_factory()
 
 
 @pytest.fixture
+def mock_ssl_socket_factory(mocker: MockerFixture) -> Callable[[], MagicMock]:
+    def factory() -> MagicMock:
+        mock_socket = mocker.NonCallableMagicMock(spec=SSLSocket)
+        mock_socket.family = AF_INET
+        mock_socket.type = SOCK_STREAM
+        mock_socket.proto = IPPROTO_TCP
+        mock_socket.do_handshake.return_value = None
+        return mock_socket
+
+    return factory
+
+
+@pytest.fixture
+def mock_ssl_socket(mock_ssl_socket_factory: Callable[[], MagicMock]) -> MagicMock:
+    return mock_ssl_socket_factory()
+
+
+@pytest.fixture
+def mock_ssl_context_factory(mocker: MockerFixture) -> Callable[[], MagicMock]:
+    def factory() -> MagicMock:
+        mock_context = mocker.NonCallableMagicMock(spec=SSLContext)
+        mock_context.check_hostname = True
+        mock_context.options = 0
+        return mock_context
+
+    return factory
+
+
+@pytest.fixture
+def mock_ssl_context(mock_ssl_context_factory: Callable[[], MagicMock]) -> MagicMock:
+    return mock_ssl_context_factory()
+
+
+@pytest.fixture
 def mock_serializer_factory(mocker: MockerFixture) -> Callable[[], Any]:
     return lambda: mocker.NonCallableMagicMock(spec=AbstractPacketSerializer)
 
 
 @pytest.fixture
 def mock_serializer(mock_serializer_factory: Callable[[], Any]) -> Any:
     return mock_serializer_factory()
@@ -92,15 +128,15 @@
 @pytest.fixture
 def mock_incremental_serializer(mock_incremental_serializer_factory: Callable[[], Any]) -> Any:
     return mock_incremental_serializer_factory()
 
 
 @pytest.fixture
 def mock_converter_factory(mocker: MockerFixture) -> Callable[[], Any]:
-    return lambda: mocker.NonCallableMagicMock(spec=AbstractPacketConverter)
+    return lambda: mocker.NonCallableMagicMock(spec=AbstractPacketConverterComposite)
 
 
 @pytest.fixture
 def mock_converter(mock_converter_factory: Callable[[], Any]) -> Any:
     return mock_converter_factory()
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_protocol.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generator
 
-from easynetwork.converter import PacketConversionError
 from easynetwork.exceptions import (
     DatagramProtocolParseError,
     DeserializeError,
     IncrementalDeserializeError,
+    PacketConversionError,
     StreamProtocolParseError,
 )
 from easynetwork.protocol import DatagramProtocol, StreamProtocol
 
 import pytest
 
 if TYPE_CHECKING:
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_client/base.py` & `easynetwork-1.0.0rc1/tests/unit_test/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
 from socket import AF_INET6
 from typing import TYPE_CHECKING, Any
 
+from easynetwork.tools.socket import AddressFamily
+
+from ._utils import get_all_socket_families
+
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
+SUPPORTED_FAMILIES: tuple[str, ...] = tuple(sorted(AddressFamily.__members__))
+UNSUPPORTED_FAMILIES: tuple[str, ...] = tuple(sorted(get_all_socket_families().difference(SUPPORTED_FAMILIES)))
 
-class BaseTestClient:
+
+class BaseTestSocket:
     @staticmethod
     def set_local_address_to_socket_mock(
         mock_socket: MagicMock,
         socket_family: int,
-        address: tuple[str, int],
+        address: tuple[str, int] | None,
     ) -> None:
         additional_address_components: tuple[Any, ...] = (0, 0) if socket_family == AF_INET6 else ()
 
+        if address is None:
+            if socket_family == AF_INET6:
+                address = ("::", 0)
+            else:
+                address = ("0.0.0.0", 0)
+
         mock_socket.getsockname.return_value = address + additional_address_components
 
     @staticmethod
     def set_remote_address_to_socket_mock(
         mock_socket: MagicMock,
         socket_family: int,
         address: tuple[str, int],
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_client/test_abc.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_abc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,91 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
-from collections import deque
 from typing import TYPE_CHECKING, Any, final
 
-from easynetwork.client.abc import AbstractNetworkClient
+from easynetwork.api_async.client.abc import AbstractAsyncNetworkClient
 from easynetwork.tools.socket import SocketAddress
 
 import pytest
 
 if TYPE_CHECKING:
+    from easynetwork.api_async.backend.abc import AbstractAsyncBackend
+
     from pytest_mock import MockerFixture
 
 
 @final
-class _ClientForTest(AbstractNetworkClient[Any, Any]):
-    def is_closed(self) -> bool:
+class MockAsyncClient(AbstractAsyncNetworkClient[Any, Any]):
+    def __init__(self, mocker: MockerFixture) -> None:
+        super().__init__()
+        self.mock_wait_connected = mocker.AsyncMock(return_value=None)
+        self.mock_close = mocker.AsyncMock(return_value=None)
+        self.mock_recv_packet = mocker.AsyncMock()
+
+    def is_connected(self) -> bool:
         return True
 
-    def close(self) -> None:
-        raise NotImplementedError
+    async def wait_connected(self) -> None:
+        return await self.mock_wait_connected()
+
+    def is_closing(self) -> bool:
+        return False
+
+    async def aclose(self) -> None:
+        return await self.mock_close()
 
     def get_local_address(self) -> SocketAddress:
         raise NotImplementedError
 
     def get_remote_address(self) -> SocketAddress:
         raise NotImplementedError
 
-    def send_packet(self, packet: Any) -> None:
+    async def send_packet(self, packet: Any) -> None:
         raise NotImplementedError
 
-    def recv_packet(self, timeout: float | None = ...) -> Any:
-        raise NotImplementedError
+    async def recv_packet(self) -> Any:
+        return await self.mock_recv_packet()
 
     def fileno(self) -> int:
         raise NotImplementedError
 
+    def get_backend(self) -> AbstractAsyncBackend:
+        raise NotImplementedError
 
-class TestAbstractNetworkClient:
-    def test____context____close_client_at_end(self, mocker: MockerFixture) -> None:
-        # Arrange
-        client = _ClientForTest()
-        mock_close = mocker.patch.object(client, "close")
-
-        # Act
-        with client:
-            mock_close.assert_not_called()
 
-        # Assert
-        mock_close.assert_called_once_with()
+@pytest.mark.asyncio
+class TestAbstractAsyncNetworkClient:
+    @pytest.fixture
+    @staticmethod
+    def client(mocker: MockerFixture) -> MockAsyncClient:
+        return MockAsyncClient(mocker)
 
-    def test____iter_received_packets____yields_available_packets_with_given_timeout(
-        self,
-        mocker: MockerFixture,
-    ) -> None:
+    async def test____context____close_client_at_end(self, client: MockAsyncClient) -> None:
         # Arrange
-        received_packets_queue = deque([mocker.sentinel.packet_a, mocker.sentinel.packet_b, mocker.sentinel.packet_c])
-
-        def side_effect(timeout: Any) -> Any:
-            try:
-                return received_packets_queue.popleft()
-            except IndexError:
-                raise TimeoutError
-
-        client = _ClientForTest()
-        mock_recv_packet = mocker.patch.object(client, "recv_packet", side_effect=side_effect)
 
         # Act
-        packets = list(client.iter_received_packets(timeout=123456789))
+        async with client:
+            client.mock_wait_connected.assert_awaited_once_with()
+            client.mock_close.assert_not_awaited()
 
         # Assert
-        assert mock_recv_packet.mock_calls == [mocker.call(123456789) for _ in range(4)]
-        assert packets == [mocker.sentinel.packet_a, mocker.sentinel.packet_b, mocker.sentinel.packet_c]
+        client.mock_wait_connected.assert_awaited_once_with()
+        client.mock_close.assert_awaited_once_with()
 
-    @pytest.mark.parametrize("timeout", [123456789, None])
     @pytest.mark.parametrize("error", [OSError])
-    def test____iter_received_packets____with_given_timeout_stop_if_an_error_occurs(
+    async def test____iter_received_packets____stop_if_an_error_occurs(
         self,
-        timeout: int | None,
+        client: MockAsyncClient,
         error: type[BaseException],
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        client = _ClientForTest()
-        mock_recv_packet = mocker.patch.object(
-            client,
-            "recv_packet",
-            side_effect=[
-                mocker.sentinel.packet_a,
-                error,
-            ],
-        )
+        client.mock_recv_packet.side_effect = [mocker.sentinel.packet_a, error]
 
         # Act
-        packets = list(client.iter_received_packets(timeout=timeout))
+        packets = [p async for p in client.iter_received_packets()]
 
         # Assert
-        assert mock_recv_packet.mock_calls == [mocker.call(timeout) for _ in range(2)]
+        assert client.mock_recv_packet.mock_calls == [mocker.call() for _ in range(2)]
         assert packets == [mocker.sentinel.packet_a]
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_client/test_tcp.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_sync/test_client/test_udp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
-from socket import AF_INET6
+from selectors import EVENT_READ, EVENT_WRITE
+from socket import AF_INET6, SOCK_DGRAM
 from typing import TYPE_CHECKING, Any
 
-from easynetwork.client.tcp import TCPNetworkClient
+from easynetwork.api_sync.client.udp import UDPNetworkClient, UDPNetworkEndpoint
 from easynetwork.exceptions import ClientClosedError
-from easynetwork.tools.socket import MAX_STREAM_BUFSIZE, IPv4SocketAddress, IPv6SocketAddress
+from easynetwork.tools.socket import MAX_DATAGRAM_BUFSIZE, IPv4SocketAddress, IPv6SocketAddress
 
 import pytest
 
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
     from pytest_mock import MockerFixture
 
+from ...base import UNSUPPORTED_FAMILIES
 from .base import BaseTestClient
 
 
-@pytest.fixture(scope="module", autouse=True)
-def setup_dummy_lock(module_mocker: MockerFixture, dummy_lock_cls: Any) -> None:
-    module_mocker.patch(f"{TCPNetworkClient.__module__}._Lock", new=dummy_lock_cls)
-
-
-class TestTCPNetworkClient(BaseTestClient):
-    @pytest.fixture
-    @staticmethod
-    def mock_stream_data_producer() -> MagicMock:
-        pytest.fail("StreamDataProducer is not used")
-
+class TestUDPNetworkEndpoint(BaseTestClient):
     @pytest.fixture(scope="class", params=["AF_INET", "AF_INET6"])
     @staticmethod
     def socket_family(request: Any) -> Any:
         import socket
 
         return getattr(socket, request.param)
 
@@ -45,1063 +37,1153 @@
     @pytest.fixture(scope="class")
     @staticmethod
     def global_remote_address() -> tuple[str, int]:
         return ("remote_address", 5000)
 
     @pytest.fixture(autouse=True)
     @staticmethod
-    def mock_socket_create_connection(mocker: MockerFixture, mock_tcp_socket: MagicMock) -> MagicMock:
-        return mocker.patch("socket.create_connection", return_value=mock_tcp_socket)
-
-    @pytest.fixture(autouse=True)
-    @staticmethod
-    def mock_socket_proxy_cls(mocker: MockerFixture, mock_tcp_socket: MagicMock) -> MagicMock:
-        return mocker.patch(f"{TCPNetworkClient.__module__}.SocketProxy", return_value=mock_tcp_socket)
-
-    @pytest.fixture(autouse=True)
-    @staticmethod
-    def mock_stream_data_consumer_cls(mocker: MockerFixture, mock_stream_data_consumer: MagicMock) -> MagicMock:
-        return mocker.patch(f"{TCPNetworkClient.__module__}.StreamDataConsumer", return_value=mock_stream_data_consumer)
+    def mock_socket_proxy_cls(mocker: MockerFixture, mock_udp_socket: MagicMock) -> MagicMock:
+        return mocker.patch(f"{UDPNetworkClient.__module__}.SocketProxy", return_value=mock_udp_socket)
 
     @pytest.fixture(autouse=True)
     @classmethod
     def local_address(
         cls,
-        mock_tcp_socket: MagicMock,
+        request: Any,
+        mock_udp_socket: MagicMock,
         socket_family: int,
         global_local_address: tuple[str, int],
     ) -> tuple[str, int]:
-        cls.set_local_address_to_socket_mock(mock_tcp_socket, socket_family, global_local_address)
+        address: tuple[str, int] | None = getattr(request, "param", global_local_address)
+        cls.set_local_address_to_socket_mock(mock_udp_socket, socket_family, address)
         return global_local_address
 
-    @pytest.fixture(autouse=True)
+    @pytest.fixture(autouse=True, params=[False, True], ids=lambda p: f"remote_address=={p}")
     @classmethod
     def remote_address(
         cls,
-        mock_tcp_socket: MagicMock,
+        request: Any,
+        mock_udp_socket: MagicMock,
         socket_family: int,
         global_remote_address: tuple[str, int],
-    ) -> tuple[str, int]:
-        cls.set_remote_address_to_socket_mock(mock_tcp_socket, socket_family, global_remote_address)
-        return global_remote_address
+    ) -> tuple[str, int] | None:
+        match request.param:
+            case True:
+                cls.set_remote_address_to_socket_mock(mock_udp_socket, socket_family, global_remote_address)
+                return global_remote_address
+            case False:
+                cls.configure_socket_mock_to_raise_ENOTCONN(mock_udp_socket)
+                return None
+            case invalid:
+                pytest.fail(f"Invalid fixture param: Got {invalid!r}")
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def set_default_socket_mock_configuration(
-        mock_tcp_socket: MagicMock,
+        mock_udp_socket: MagicMock,
         socket_family: int,
-        mocker: MockerFixture,
     ) -> None:
-        mock_tcp_socket.family = socket_family
-        mock_tcp_socket.gettimeout.return_value = mocker.sentinel.default_timeout
-        mock_tcp_socket.getsockopt.return_value = 0  # Needed for tests dealing with send_packet()
+        mock_udp_socket.family = socket_family
+        mock_udp_socket.gettimeout.return_value = 0
+        mock_udp_socket.getsockopt.return_value = 0  # Needed for tests dealing with send_packet_to()
+        mock_udp_socket.send.side_effect = lambda data: len(data)
+        mock_udp_socket.sendto.side_effect = lambda data, address: len(data)
+        del mock_udp_socket.sendall
 
     @pytest.fixture  # DO NOT set autouse=True
     @staticmethod
-    def setup_producer_mock(mock_stream_protocol: MagicMock) -> None:
-        mock_stream_protocol.generate_chunks.side_effect = lambda packet: iter(
-            [str(packet).encode("ascii").removeprefix(b"sentinel.") + b"\n"]
-        )
-
-    @pytest.fixture  # DO NOT set autouse=True
-    @staticmethod
-    def setup_consumer_mock(mock_stream_data_consumer: MagicMock, mocker: MockerFixture) -> None:
-        bytes_buffer: bytes = b""
-
+    def setup_protocol_mock(mock_datagram_protocol: MagicMock, mocker: MockerFixture) -> None:
         sentinel = mocker.sentinel
 
-        def feed_side_effect(chunk: bytes) -> None:
-            nonlocal bytes_buffer
-            bytes_buffer += chunk
-
-        def next_side_effect() -> Any:
-            nonlocal bytes_buffer
-            data, separator, bytes_buffer = bytes_buffer.partition(b"\n")
-            if not separator:
-                assert not bytes_buffer
-                bytes_buffer = data
-                raise StopIteration
-            return getattr(sentinel, data.decode("ascii"))
+        def make_datagram_side_effect(packet: Any) -> bytes:
+            return str(packet).encode("ascii").removeprefix(b"sentinel.")
 
-        mock_stream_data_consumer.feed.side_effect = feed_side_effect
-        mock_stream_data_consumer.__iter__.side_effect = lambda: mock_stream_data_consumer
-        mock_stream_data_consumer.__next__.side_effect = next_side_effect
+        def build_packet_from_datagram_side_effect(data: bytes) -> Any:
+            return getattr(sentinel, data.decode("ascii"))
 
-    @pytest.fixture
-    @staticmethod
-    def max_recv_size(request: Any) -> int | None:
-        return getattr(request, "param", None)
+        mock_datagram_protocol.make_datagram.side_effect = make_datagram_side_effect
+        mock_datagram_protocol.build_packet_from_datagram.side_effect = build_packet_from_datagram_side_effect
 
-    @pytest.fixture(params=["REMOTE_ADDRESS", "SOCKET_WITH_EXPLICIT_GIVE"])
+    @pytest.fixture(params=["REMOTE_ADDRESS", "EXTERNAL_SOCKET"])
     @staticmethod
-    def client_with_socket_ownership(
-        request: Any,
-        max_recv_size: int | None,
-        remote_address: tuple[str, int],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
-    ) -> TCPNetworkClient[Any, Any]:
-        match request.param:
-            case "REMOTE_ADDRESS":
-                return TCPNetworkClient(remote_address, mock_stream_protocol, max_recv_size=max_recv_size)
-            case "SOCKET_WITH_EXPLICIT_GIVE":
-                return TCPNetworkClient(mock_tcp_socket, mock_stream_protocol, give=True, max_recv_size=max_recv_size)
-            case invalid:
-                pytest.fail(f"Invalid fixture param: Got {invalid!r}")
+    def use_external_socket(request: Any) -> str:
+        return request.param
 
-    @pytest.fixture
+    @pytest.fixture()
     @staticmethod
-    def client_without_socket_ownership(
-        max_recv_size: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
-    ) -> TCPNetworkClient[Any, Any]:
-        return TCPNetworkClient(mock_tcp_socket, mock_stream_protocol, give=False, max_recv_size=max_recv_size)
+    def client(
+        use_external_socket: str,
+        remote_address: tuple[str, int] | None,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mocker: MockerFixture,
+    ) -> UDPNetworkEndpoint[Any, Any]:
+        try:
+            match use_external_socket:
+                case "REMOTE_ADDRESS":
+                    mocker.patch("socket.socket", return_value=mock_udp_socket)
+                    return UDPNetworkEndpoint(protocol=mock_datagram_protocol, remote_address=remote_address)
+                case "EXTERNAL_SOCKET":
+                    return UDPNetworkEndpoint(socket=mock_udp_socket, protocol=mock_datagram_protocol)
+                case invalid:
+                    pytest.fail(f"Invalid fixture param: Got {invalid!r}")
+        finally:
+            mock_udp_socket.settimeout.reset_mock()
 
     @pytest.fixture
     @staticmethod
-    def client(client_without_socket_ownership: TCPNetworkClient[Any, Any]) -> TCPNetworkClient[Any, Any]:
-        return client_without_socket_ownership
+    def sender_address(request: Any, global_remote_address: tuple[str, int]) -> tuple[str, int]:
+        try:
+            param: Any = request.param
+        except AttributeError:
+            return global_remote_address
+        if param == "REMOTE":
+            return global_remote_address
+        host, port = param
+        return host, port
 
     @pytest.fixture(
         params=[
             pytest.param(None, id="blocking"),
             pytest.param(0, id="non_blocking"),
             pytest.param(123456789, id="with_timeout"),
         ]
     )
     @staticmethod
     def recv_timeout(request: Any) -> Any:
         return request.param
 
-    def test____dunder_init____connect_to_remote(
+    def test____dunder_init____create_datagram_endpoint____default(
         self,
-        remote_address: tuple[str, int],
-        mock_tcp_socket: MagicMock,
-        mock_socket_create_connection: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
-        mock_stream_protocol: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        mock_socket_proxy_cls.return_value = mocker.sentinel.proxy
-
-        # Act
-        client: TCPNetworkClient[Any, Any] = TCPNetworkClient(
-            remote_address,
-            protocol=mock_stream_protocol,
-            timeout=mocker.sentinel.timeout,
-            source_address=mocker.sentinel.source_address,
-        )
-
-        # Assert
-        mock_stream_data_consumer_cls.assert_called_once_with(mock_stream_protocol)
-        mock_socket_create_connection.assert_called_once_with(
-            remote_address,
-            timeout=mocker.sentinel.timeout,
-            source_address=mocker.sentinel.source_address,
-        )
-        mock_socket_proxy_cls.assert_called_once_with(mock_tcp_socket, lock=mocker.ANY)
-        mock_tcp_socket.getsockname.assert_called_once_with()
-        mock_tcp_socket.getpeername.assert_called_once_with()
-        assert client.socket is mocker.sentinel.proxy
-
-    @pytest.mark.parametrize("give_ownership", [False, True], ids=lambda p: f"give=={p}")
-    def test____dunder_init____use_given_socket(
-        self,
-        give_ownership: bool,
-        mock_tcp_socket: MagicMock,
-        mock_socket_create_connection: MagicMock,
+        socket_family: int,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mock_socket_proxy_cls: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
-        mock_stream_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
+        mock_socket_cls = mocker.patch("socket.socket", return_value=mock_udp_socket)
         mock_socket_proxy_cls.return_value = mocker.sentinel.proxy
 
         # Act
-        client: TCPNetworkClient[Any, Any] = TCPNetworkClient(mock_tcp_socket, protocol=mock_stream_protocol, give=give_ownership)
+        endpoint: UDPNetworkEndpoint[Any, Any] = UDPNetworkEndpoint(protocol=mock_datagram_protocol, family=socket_family)
 
         # Assert
-        mock_stream_data_consumer_cls.assert_called_once_with(mock_stream_protocol)
-        mock_socket_create_connection.assert_not_called()
-        mock_socket_proxy_cls.assert_called_once_with(mock_tcp_socket, lock=mocker.ANY)
-        mock_tcp_socket.getsockname.assert_called_once_with()
-        mock_tcp_socket.getpeername.assert_called_once_with()
-        assert client.socket is mocker.sentinel.proxy
+        mock_socket_cls.assert_called_once_with(socket_family, SOCK_DGRAM)
+        mock_udp_socket.bind.assert_called_once_with(("", 0))
+        mock_udp_socket.connect.assert_not_called()
+        mock_udp_socket.settimeout.assert_called_once_with(0)
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_udp_socket.getpeername.assert_not_called()
+        mock_socket_proxy_cls.assert_called_once_with(mock_udp_socket, lock=mocker.ANY)
+        assert endpoint.socket is mocker.sentinel.proxy
 
-    @pytest.mark.parametrize("give_ownership", [False, True], ids=lambda p: f"give=={p}")
-    def test____dunder_init____invalid_socket_type_error(
+    @pytest.mark.parametrize(
+        "local_address", [None, ("local_address", 12345)], ids=lambda p: f"local_address=={p}", indirect=True
+    )
+    def test____dunder_init____create_datagram_endpoint____with_parameters(
         self,
-        give_ownership: bool,
+        socket_family: int,
+        local_address: tuple[str, int] | None,
+        remote_address: tuple[str, int] | None,
         mock_udp_socket: MagicMock,
-        mock_socket_create_connection: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mock_socket_proxy_cls: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
-        mock_stream_protocol: MagicMock,
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
+        mock_socket_cls = mocker.patch("socket.socket", return_value=mock_udp_socket)
 
         # Act
-        with pytest.raises(ValueError, match=r"^Invalid socket type$"):
-            _ = TCPNetworkClient(mock_udp_socket, protocol=mock_stream_protocol, give=give_ownership)
+        _ = UDPNetworkEndpoint(
+            protocol=mock_datagram_protocol,
+            family=socket_family,
+            local_address=local_address,
+            remote_address=remote_address,
+        )
 
         # Assert
-        mock_stream_data_consumer_cls.assert_not_called()
-        mock_socket_create_connection.assert_not_called()
-        mock_socket_proxy_cls.assert_not_called()
-        mock_udp_socket.getsockname.assert_not_called()
-        mock_udp_socket.getpeername.assert_not_called()
-        ## If ownership was given, the socket must be closed
-        if give_ownership:
-            mock_udp_socket.close.assert_called_once_with()
+        mock_socket_cls.assert_called_once_with(socket_family, SOCK_DGRAM)
+        if local_address is None:
+            mock_udp_socket.bind.assert_called_once_with(("", 0))
         else:
-            mock_udp_socket.close.assert_not_called()
-
-    @pytest.mark.parametrize("give_ownership", [False, True], ids=lambda p: f"give=={p}")
-    def test____dunder_init____socket_given_is_not_connected_error(
-        self,
-        give_ownership: bool,
-        mock_tcp_socket: MagicMock,
-        mock_socket_create_connection: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
-        mock_stream_protocol: MagicMock,
-    ) -> None:
-        # Arrange
-        enotconn_exception = self.configure_socket_mock_to_raise_ENOTCONN(mock_tcp_socket)
-
-        # Act
-        with pytest.raises(OSError) as exc_info:
-            _ = TCPNetworkClient(mock_tcp_socket, protocol=mock_stream_protocol, give=give_ownership)
-
-        # Assert
-        assert exc_info.value is enotconn_exception
-        mock_stream_data_consumer_cls.assert_not_called()
-        mock_socket_create_connection.assert_not_called()
-        mock_socket_proxy_cls.assert_not_called()
-        mock_tcp_socket.getsockname.assert_called_once_with()
-        mock_tcp_socket.getpeername.assert_called_once_with()
-        ## If ownership was given, the socket must be closed
-        if give_ownership:
-            mock_tcp_socket.close.assert_called_once_with()
+            mock_udp_socket.bind.assert_called_once_with(local_address)
+        if remote_address is None:
+            mock_udp_socket.connect.assert_not_called()
+            mock_udp_socket.getpeername.assert_not_called()
         else:
-            mock_tcp_socket.close.assert_not_called()
+            mock_udp_socket.connect.assert_called_once_with(remote_address)
+            mock_udp_socket.getpeername.assert_called_once_with()
+        mock_udp_socket.settimeout.assert_called_once_with(0)
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_socket_proxy_cls.assert_called_once_with(mock_udp_socket, lock=mocker.ANY)
 
-    def test____dunder_init____ownership_parameter_missing(
+    @pytest.mark.parametrize("socket_family", list(UNSUPPORTED_FAMILIES), indirect=True)
+    def test____dunder_init____create_datagram_endpoint____invalid_socket_family(
         self,
-        mock_tcp_socket: MagicMock,
-        mock_socket_create_connection: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
-        mock_stream_protocol: MagicMock,
+        socket_family: int,
+        mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
 
-        # Act
-        with pytest.raises(TypeError, match=r"^Missing keyword argument 'give'$"):
-            _ = TCPNetworkClient(mock_tcp_socket, protocol=mock_stream_protocol)
-
-        # Assert
-        mock_stream_data_consumer_cls.assert_not_called()
-        mock_socket_create_connection.assert_not_called()
-        mock_socket_proxy_cls.assert_not_called()
-        mock_tcp_socket.close.assert_not_called()
+        # Act & Assert
+        with pytest.raises(ValueError, match=r"^Only these families are supported: .+$"):
+            _ = UDPNetworkEndpoint(protocol=mock_datagram_protocol, family=socket_family)
 
-    @pytest.mark.parametrize("max_recv_size", [None, 1, 2**64], ids=lambda p: f"max_recv_size=={p}")
-    @pytest.mark.parametrize("use_socket", [False, True], ids=lambda p: f"use_socket=={p}")
-    def test____dunder_init____with_ownership____max_size____valid_value(
+    @pytest.mark.parametrize("error_on", ["bind", "connect"])
+    @pytest.mark.parametrize("remote_address", [True], indirect=True)
+    def test____dunder_init____create_datagram_endpoint____close_socket_if_an_error_occurs(
         self,
-        max_recv_size: int | None,
-        use_socket: bool,
+        error_on: str,
+        local_address: tuple[str, int],
         remote_address: tuple[str, int],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
+        socket_family: int,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        expected_size: int = max_recv_size if max_recv_size is not None else MAX_STREAM_BUFSIZE
+        mocker.patch("socket.socket", return_value=mock_udp_socket)
+        mock_method: MagicMock = getattr(mock_udp_socket, error_on)
+        mock_method.side_effect = OSError()
 
-        # Act
-        client: TCPNetworkClient[Any, Any]
-        if use_socket:
-            client = TCPNetworkClient(
-                mock_tcp_socket,
-                protocol=mock_stream_protocol,
-                give=True,
-                max_recv_size=max_recv_size,
-            )
-        else:
-            client = TCPNetworkClient(
-                remote_address,
-                protocol=mock_stream_protocol,
-                max_recv_size=max_recv_size,
+        # Act & Assert
+        with pytest.raises(type(mock_method.side_effect)) as exc_info:
+            _ = UDPNetworkEndpoint(
+                protocol=mock_datagram_protocol,
+                family=socket_family,
+                local_address=local_address,
+                remote_address=remote_address,
             )
+        assert exc_info.value is mock_method.side_effect
+        mock_udp_socket.close.assert_called_once_with()
 
-        # Assert
-        assert client.max_recv_bufsize == expected_size
-
-    @pytest.mark.parametrize("max_recv_size", [0, -1, 10.4], ids=lambda p: f"max_recv_size=={p}")
-    @pytest.mark.parametrize("use_socket", [False, True], ids=lambda p: f"use_socket=={p}")
-    def test____dunder_init____with_ownership____max_size____invalid_value(
+    @pytest.mark.parametrize("bound", [False, True], ids=lambda p: f"bound=={p}")
+    def test____dunder_init____use_given_socket____default(
         self,
-        max_recv_size: Any,
-        use_socket: bool,
-        remote_address: tuple[str, int],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
+        bound: bool,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mock_socket_proxy_cls: MagicMock,
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
+        mock_socket_proxy_cls.return_value = mocker.sentinel.proxy
+        if not bound:
+            mock_udp_socket.getsockname.return_value = ("0.0.0.0", 0)
 
         # Act
-        with pytest.raises(ValueError, match=r"^max_size must be a strict positive integer$"):
-            if use_socket:
-                _ = TCPNetworkClient(
-                    mock_tcp_socket,
-                    protocol=mock_stream_protocol,
-                    give=True,
-                    max_recv_size=max_recv_size,
-                )
-            else:
-                _ = TCPNetworkClient(
-                    remote_address,
-                    protocol=mock_stream_protocol,
-                    max_recv_size=max_recv_size,
-                )
+        endpoint: UDPNetworkEndpoint[Any, Any] = UDPNetworkEndpoint(
+            protocol=mock_datagram_protocol,
+            socket=mock_udp_socket,
+        )
 
         # Assert
-        mock_stream_data_consumer_cls.assert_not_called()
-        mock_socket_proxy_cls.assert_not_called()
-        mock_tcp_socket.getsockname.assert_not_called()
-        mock_tcp_socket.getpeername.assert_not_called()
-        mock_tcp_socket.close.assert_called_once_with()
+        if bound:
+            mock_udp_socket.bind.assert_not_called()
+        else:
+            mock_udp_socket.bind.assert_called_once_with(("", 0))
+        mock_udp_socket.connect.assert_not_called()
+        mock_udp_socket.settimeout.assert_called_once_with(0)
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_udp_socket.getpeername.assert_called_once_with()
+        mock_socket_proxy_cls.assert_called_once_with(mock_udp_socket, lock=mocker.ANY)
+        assert endpoint.socket is mocker.sentinel.proxy
 
-    @pytest.mark.parametrize("max_recv_size", [None, 1, 2**64], ids=lambda p: f"max_recv_size=={p}")
-    def test____dunder_init____without_ownership____max_size____valid_value(
+    @pytest.mark.parametrize("socket_family", list(UNSUPPORTED_FAMILIES), indirect=True)
+    def test____dunder_init____use_given_socket____invalid_socket_family(
         self,
-        max_recv_size: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
-        expected_size: int = max_recv_size if max_recv_size is not None else MAX_STREAM_BUFSIZE
 
-        # Act
-        client: TCPNetworkClient[Any, Any] = TCPNetworkClient(
-            mock_tcp_socket,
-            protocol=mock_stream_protocol,
-            give=False,
-            max_recv_size=max_recv_size,
-        )
-
-        # Assert
-        assert client.max_recv_bufsize == expected_size
+        # Act & Assert
+        with pytest.raises(ValueError, match=r"^Only these families are supported: .+$"):
+            _ = UDPNetworkEndpoint(
+                protocol=mock_datagram_protocol,
+                socket=mock_udp_socket,
+            )
 
-    @pytest.mark.parametrize("max_recv_size", [0, -1, 10.4], ids=lambda p: f"max_recv_size=={p}")
-    def test____dunder_init____without_ownership____max_size____invalid_value(
+    def test____dunder_init____use_given_socket____invalid_socket_type_error(
         self,
-        max_recv_size: Any,
         mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
-        mock_stream_data_consumer_cls: MagicMock,
         mock_socket_proxy_cls: MagicMock,
+        mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
 
         # Act
-        with pytest.raises(ValueError, match=r"^max_size must be a strict positive integer$"):
-            _ = TCPNetworkClient(
-                mock_tcp_socket,
-                protocol=mock_stream_protocol,
-                give=False,
-                max_recv_size=max_recv_size,
+        with pytest.raises(ValueError, match=r"^Invalid socket type$"):
+            _ = UDPNetworkEndpoint(
+                protocol=mock_datagram_protocol,
+                socket=mock_tcp_socket,
             )
 
         # Assert
-        mock_stream_data_consumer_cls.assert_not_called()
         mock_socket_proxy_cls.assert_not_called()
         mock_tcp_socket.getsockname.assert_not_called()
         mock_tcp_socket.getpeername.assert_not_called()
-        mock_tcp_socket.close.assert_not_called()
+        mock_tcp_socket.close.assert_called_once_with()
 
-    def test____close____with_ownership(
+    def test____context____close_endpoint_at_end(
         self,
-        client_with_socket_ownership: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        assert not client_with_socket_ownership.is_closed()
+        mock_close = mocker.patch.object(UDPNetworkEndpoint, "close")
 
         # Act
-        client_with_socket_ownership.close()
+        with client:
+            mock_close.assert_not_called()
 
         # Assert
-        assert client_with_socket_ownership.is_closed()
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_tcp_socket.close.assert_called_once_with()
+        mock_close.assert_called_once_with()
 
-    def test____close____without_ownership(
+    def test____close____default(
         self,
-        client_without_socket_ownership: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
     ) -> None:
         # Arrange
-        assert not client_without_socket_ownership.is_closed()
+        assert not client.is_closed()
 
         # Act
-        client_without_socket_ownership.close()
+        client.close()
 
         # Assert
-        assert client_without_socket_ownership.is_closed()
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_tcp_socket.close.assert_not_called()
+        assert client.is_closed()
+        mock_udp_socket.close.assert_called_once_with()
 
     @pytest.mark.parametrize("client_closed", [False, True], ids=lambda p: f"client_closed=={p}")
     def test____get_local_address____return_saved_address(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
         client_closed: bool,
         socket_family: int,
         local_address: tuple[str, int],
-        mock_tcp_socket: MagicMock,
+        mock_udp_socket: MagicMock,
     ) -> None:
         # Arrange
-        mock_tcp_socket.getsockname.reset_mock()
+        mock_udp_socket.getsockname.reset_mock()
         if client_closed:
             client.close()
             assert client.is_closed()
 
         # Act
         address = client.get_local_address()
 
         # Assert
         if socket_family == AF_INET6:
             assert isinstance(address, IPv6SocketAddress)
         else:
             assert isinstance(address, IPv4SocketAddress)
-        mock_tcp_socket.getsockname.assert_not_called()
+        mock_udp_socket.getsockname.assert_not_called()
         assert address.host == local_address[0]
         assert address.port == local_address[1]
 
     @pytest.mark.parametrize("client_closed", [False, True], ids=lambda p: f"client_closed=={p}")
     def test____get_remote_address____return_saved_address(
         self,
-        client: TCPNetworkClient[Any, Any],
+        use_external_socket: str,
+        client: UDPNetworkEndpoint[Any, Any],
         client_closed: bool,
-        remote_address: tuple[str, int],
+        remote_address: tuple[str, int] | None,
         socket_family: int,
-        mock_tcp_socket: MagicMock,
+        mock_udp_socket: MagicMock,
     ) -> None:
         # Arrange
         ## NOTE: The client should have the remote address saved. Therefore this test check if there is no new call.
-        mock_tcp_socket.getpeername.assert_called_once()
+        if use_external_socket == "REMOTE_ADDRESS" and remote_address is None:
+            mock_udp_socket.getpeername.assert_not_called()
+        else:
+            mock_udp_socket.getpeername.assert_called_once()
+        mock_udp_socket.getpeername.reset_mock()
         if client_closed:
             client.close()
             assert client.is_closed()
 
         # Act
         address = client.get_remote_address()
 
         # Assert
-        if socket_family == AF_INET6:
-            assert isinstance(address, IPv6SocketAddress)
+        if remote_address is None:
+            assert address is None
         else:
-            assert isinstance(address, IPv4SocketAddress)
-        mock_tcp_socket.getpeername.assert_called_once()
-        assert address.host == remote_address[0]
-        assert address.port == remote_address[1]
+            if socket_family == AF_INET6:
+                assert isinstance(address, IPv6SocketAddress)
+            else:
+                assert isinstance(address, IPv4SocketAddress)
+            assert address.host == remote_address[0]
+            assert address.port == remote_address[1]
+        mock_udp_socket.getpeername.assert_not_called()
 
     def test____fileno____default(
         self,
-        client: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.fileno.return_value = mocker.sentinel.fileno
+        mock_udp_socket.fileno.return_value = mocker.sentinel.fileno
 
         # Act
         fd = client.fileno()
 
         # Assert
-        mock_tcp_socket.fileno.assert_called_once_with()
+        mock_udp_socket.fileno.assert_called_once_with()
         assert fd is mocker.sentinel.fileno
 
     def test____fileno____closed_client(
         self,
-        client: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
     ) -> None:
         # Arrange
         client.close()
         assert client.is_closed()
 
         # Act
         fd = client.fileno()
 
         # Assert
-        mock_tcp_socket.fileno.assert_not_called()
+        mock_udp_socket.fileno.assert_not_called()
         assert fd == -1
 
-    @pytest.mark.parametrize("shutdown_flag_name", ["SHUT_RD", "SHUT_WR", "SHUT_RDWR"])
-    def test____shutdown____default(
+    @pytest.mark.parametrize("remote_address", [False], indirect=True)
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____send_bytes_to_socket____without_remote____default(
         self,
-        client: TCPNetworkClient[Any, Any],
-        shutdown_flag_name: str,
-        mock_tcp_socket: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mock_selector_select: MagicMock,
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        import socket
+        from socket import SO_ERROR, SOL_SOCKET
 
-        shutdown_flag = int(getattr(socket, shutdown_flag_name))
+        target_address: tuple[str, int] = ("remote_address", 5000)
 
         # Act
-        client.shutdown(shutdown_flag)
+        client.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        mock_tcp_socket.shutdown.assert_called_once_with(shutdown_flag)
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.send.assert_not_called()
+        mock_udp_socket.sendto.assert_called_once_with(b"packet", target_address)
+        mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
+        mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
-    @pytest.mark.parametrize("shutdown_flag_name", ["SHUT_RD", "SHUT_WR", "SHUT_RDWR"])
-    def test____shutdown____closed_client(
+    @pytest.mark.parametrize("remote_address", [False], indirect=True)
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____send_bytes_to_socket____without_remote____blocking_operation(
         self,
-        client: TCPNetworkClient[Any, Any],
-        shutdown_flag_name: str,
-        mock_tcp_socket: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mock_selector_register: MagicMock,
+        mock_selector_select: MagicMock,
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        import socket
+        from socket import SO_ERROR, SOL_SOCKET
 
-        shutdown_flag = int(getattr(socket, shutdown_flag_name))
-        client.close()
+        target_address: tuple[str, int] = ("remote_address", 5000)
+
+        mock_udp_socket.sendto.side_effect = [BlockingIOError, len(b"packet")]
 
         # Act
-        with pytest.raises(ClientClosedError):
-            client.shutdown(shutdown_flag)
+        client.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        mock_tcp_socket.shutdown.assert_not_called()
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_register.assert_called_once_with(mock_udp_socket, EVENT_WRITE)
+        mock_selector_select.assert_called_once_with(None)
+        mock_udp_socket.send.assert_not_called()
+        assert mock_udp_socket.sendto.mock_calls == [mocker.call(b"packet", target_address) for _ in range(2)]
+        mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
+        mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
-    @pytest.mark.usefixtures("setup_producer_mock")
-    def test____send_packet____send_bytes_to_socket(
+    @pytest.mark.parametrize("remote_address", [False], indirect=True)
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____send_bytes_to_socket____without_remote____None_address_error(
         self,
-        client: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        from socket import SO_ERROR, SOL_SOCKET
 
         # Act
-        client.send_packet(mocker.sentinel.packet)
+        with pytest.raises(ValueError, match=r"^Invalid address: must not be None$"):
+            client.send_packet_to(mocker.sentinel.packet, None)
 
         # Assert
-        assert mock_tcp_socket.settimeout.mock_calls == [mocker.call(None), mocker.call(mocker.sentinel.default_timeout)]
-        mock_stream_protocol.generate_chunks.assert_called_once_with(mocker.sentinel.packet)
-        mock_tcp_socket.sendall.assert_called_once_with(b"packet\n")
-        mock_tcp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
+        mock_udp_socket.send.assert_not_called()
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.sendto.assert_not_called()
+        mock_datagram_protocol.make_datagram.assert_not_called()
+        mock_udp_socket.getsockopt.assert_not_called()
 
-    @pytest.mark.usefixtures("setup_producer_mock")
-    def test____send_packet____raise_error_saved_in_SO_ERROR_option(
+    @pytest.mark.parametrize("target_address", [None, ("remote_address", 5000)], ids=lambda p: f"target_address=={p}")
+    @pytest.mark.parametrize("remote_address", [True], indirect=True)
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____send_bytes_to_socket____with_remote____default(
         self,
-        client: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        target_address: tuple[str, int] | None,
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        from errno import ECONNRESET
         from socket import SO_ERROR, SOL_SOCKET
 
-        mock_tcp_socket.getsockopt.return_value = ECONNRESET
-
         # Act
-        with pytest.raises(OSError) as exc_info:
-            client.send_packet(mocker.sentinel.packet)
+        client.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        assert exc_info.value.errno == ECONNRESET
-        assert mock_tcp_socket.settimeout.mock_calls == [mocker.call(None), mocker.call(mocker.sentinel.default_timeout)]
-        mock_stream_protocol.generate_chunks.assert_called_once_with(mocker.sentinel.packet)
-        mock_tcp_socket.sendall.assert_called_once_with(b"packet\n")
-        mock_tcp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
-
-    @pytest.mark.usefixtures("setup_producer_mock")
-    def test____send_packet____closed_client_error(
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.sendto.assert_not_called()
+        mock_udp_socket.send.assert_called_once_with(b"packet")
+        mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
+        mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
+
+    @pytest.mark.parametrize("target_address", [None, ("remote_address", 5000)], ids=lambda p: f"target_address=={p}")
+    @pytest.mark.parametrize("remote_address", [True], indirect=True)
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____send_bytes_to_socket____with_remote____blocking_operation(
         self,
-        client: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        target_address: tuple[str, int] | None,
+        mock_udp_socket: MagicMock,
+        mock_selector_register: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        client.close()
-        assert client.is_closed()
+        from socket import SO_ERROR, SOL_SOCKET
+
+        mock_udp_socket.send.side_effect = [BlockingIOError, len(b"packet")]
 
         # Act
-        with pytest.raises(ClientClosedError):
-            client.send_packet(mocker.sentinel.packet)
+        client.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        mock_tcp_socket.settimeout.assert_not_called()
-        mock_stream_protocol.generate_chunks.assert_not_called()
-        mock_tcp_socket.sendall.assert_not_called()
-        mock_tcp_socket.getsockopt.assert_not_called()
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_register.assert_called_once_with(mock_udp_socket, EVENT_WRITE)
+        mock_selector_select.assert_called_once_with(None)
+        mock_udp_socket.sendto.assert_not_called()
+        assert mock_udp_socket.send.mock_calls == [mocker.call(b"packet") for _ in range(2)]
+        mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
+        mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet_blocking_or_not____receive_bytes_from_socket(
+    @pytest.mark.parametrize("remote_address", [True], indirect=True)
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____send_bytes_to_socket____with_remote____invalid_target_address(
         self,
-        client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b"packet\n"]
+        target_address: tuple[str, int] = ("address_other_than_remote", 9999)
 
         # Act
-        packet: Any = client.recv_packet(timeout=recv_timeout)
+        with pytest.raises(ValueError, match=r"^Invalid address: must be None or .+$"):
+            client.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        assert mock_tcp_socket.settimeout.mock_calls == [mocker.call(recv_timeout), mocker.call(mocker.sentinel.default_timeout)]
-        mock_tcp_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
-        mock_stream_data_consumer.feed.assert_called_once_with(b"packet\n")
-        assert packet is mocker.sentinel.packet
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.sendto.assert_not_called()
+        mock_datagram_protocol.make_datagram.assert_not_called()
+        mock_udp_socket.getsockopt.assert_not_called()
 
-    @pytest.mark.parametrize("recv_timeout", [None, 123456789], indirect=True)  # Do not test with timeout==0
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet____blocking____partial_data(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____raise_error_saved_in_SO_ERROR_option(
         self,
-        client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        global_remote_address: tuple[str, int],
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b"pac", b"ket\n"]
+        from errno import ECONNREFUSED
+        from socket import SO_ERROR, SOL_SOCKET
+
+        mock_udp_socket.getsockopt.return_value = ECONNREFUSED
 
         # Act
-        packet: Any = client.recv_packet(timeout=recv_timeout)
+        with pytest.raises(OSError) as exc_info:
+            client.send_packet_to(mocker.sentinel.packet, global_remote_address)
 
         # Assert
-        if recv_timeout is None:
-            assert mock_tcp_socket.settimeout.mock_calls == [
-                mocker.call(recv_timeout),
-                mocker.call(mocker.sentinel.default_timeout),
-            ]
+        assert exc_info.value.errno == ECONNREFUSED
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        if client.get_remote_address() is not None:
+            mock_udp_socket.sendto.assert_not_called()
+            mock_udp_socket.send.assert_called_once()
         else:
-            assert mock_tcp_socket.settimeout.mock_calls == [
-                mocker.call(recv_timeout),
-                mocker.call(mocker.ANY),
-                mocker.call(mocker.sentinel.default_timeout),
-            ]
-        assert mock_tcp_socket.recv.mock_calls == [mocker.call(MAX_STREAM_BUFSIZE) for _ in range(2)]
-        assert mock_stream_data_consumer.feed.mock_calls == [mocker.call(b"pac"), mocker.call(b"ket\n")]
-        assert packet is mocker.sentinel.packet
+            mock_udp_socket.sendto.assert_called_once()
+            mock_udp_socket.send.assert_not_called()
+        mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
+        mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
-    @pytest.mark.parametrize("recv_timeout", [0], indirect=True)  # Only test with timeout==0
-    @pytest.mark.parametrize(
-        "max_recv_size",
-        [
-            pytest.param(3, id="chunk_matching_bufsize"),
-            pytest.param(1024, id="chunk_not_matching_bufsize"),
-        ],
-        indirect=True,
-    )
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet_____non_blocking____partial_data(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____send_packet_to____closed_client_error(
         self,
-        client: TCPNetworkClient[Any, Any],
-        max_recv_size: int,
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        mock_tcp_socket.recv.side_effect = [b"pac", b"ket", b"\n"]
-
-        # Act & Assert
-        if max_recv_size == 3:
-            packet: Any = client.recv_packet(timeout=recv_timeout)
-
-            assert mock_tcp_socket.recv.mock_calls == [mocker.call(max_recv_size) for _ in range(3)]
-            assert mock_stream_data_consumer.feed.mock_calls == [mocker.call(b"pac"), mocker.call(b"ket"), mocker.call(b"\n")]
-            assert packet is mocker.sentinel.packet
-        else:
-            with pytest.raises(TimeoutError, match=r"^recv_packet\(\) timed out$"):
-                client.recv_packet(timeout=recv_timeout)
-
-            mock_tcp_socket.recv.assert_called_once_with(max_recv_size)
-            mock_stream_data_consumer.feed.assert_called_once_with(b"pac")
-
-        assert mock_tcp_socket.settimeout.mock_calls == [
-            mocker.call(recv_timeout),
-            mocker.call(mocker.sentinel.default_timeout),
-        ]
-
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet____blocking_or_not____extra_data(
-        self,
-        client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        client: UDPNetworkEndpoint[Any, Any],
+        remote_address: tuple[str, int] | None,
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b"packet_1\npacket_2\n"]
+        client.close()
+        assert client.is_closed()
 
         # Act
-        packet_1: Any = client.recv_packet(timeout=recv_timeout)
-        mock_tcp_socket.settimeout.reset_mock()
-        packet_2: Any = client.recv_packet(timeout=recv_timeout)
+        with pytest.raises(ClientClosedError):
+            client.send_packet_to(mocker.sentinel.packet, remote_address)
 
         # Assert
-        mock_tcp_socket.recv.assert_called_once()
-        mock_tcp_socket.settimeout.assert_not_called()
-        mock_stream_data_consumer.feed.assert_called_once_with(b"packet_1\npacket_2\n")
-        assert packet_1 is mocker.sentinel.packet_1
-        assert packet_2 is mocker.sentinel.packet_2
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.sendto.assert_not_called()
+        mock_datagram_protocol.make_datagram.assert_not_called()
+        mock_udp_socket.getsockopt.assert_not_called()
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet____blocking_or_not____eof_error____default(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____recv_packet_from____blocking_or_not____receive_bytes_from_socket(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
+        sender_address: tuple[str, int],
         recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_selector_register: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b""]
+        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
 
         # Act
-        with pytest.raises(ConnectionAbortedError):
-            _ = client.recv_packet(timeout=recv_timeout)
+        packet, sender = client.recv_packet_from(timeout=recv_timeout)
 
         # Assert
-        assert mock_tcp_socket.settimeout.mock_calls == [mocker.call(recv_timeout), mocker.call(mocker.sentinel.default_timeout)]
-        mock_tcp_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
-        mock_stream_data_consumer.feed.assert_not_called()
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+
+        mock_selector_register.assert_not_called()
+        mock_selector_select.assert_not_called()
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet____blocking_or_not____protocol_parse_error(
+        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
+        assert packet is mocker.sentinel.packet
+        assert (sender.host, sender.port) == sender_address
+
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____recv_packet_from____blocking_or_not____protocol_parse_error(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
+        sender_address: tuple[str, int],
         recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
-        mocker: MockerFixture,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
-        from easynetwork.exceptions import StreamProtocolParseError
+        from easynetwork.exceptions import DatagramProtocolParseError
 
-        mock_tcp_socket.recv.side_effect = [b"packet\n"]
-        expected_error = StreamProtocolParseError(b"", "deserialization", "Sorry")
-        mock_stream_data_consumer.__next__.side_effect = [StopIteration, expected_error]
+        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
+        expected_error = DatagramProtocolParseError("deserialization", "Sorry")
+        mock_datagram_protocol.build_packet_from_datagram.side_effect = expected_error
 
         # Act
-        with pytest.raises(StreamProtocolParseError) as exc_info:
-            _ = client.recv_packet(timeout=recv_timeout)
+        with pytest.raises(DatagramProtocolParseError) as exc_info:
+            _ = client.recv_packet_from(timeout=recv_timeout)
         exception = exc_info.value
 
         # Assert
-        assert mock_tcp_socket.settimeout.mock_calls == [mocker.call(recv_timeout), mocker.call(mocker.sentinel.default_timeout)]
-        mock_tcp_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
-        mock_stream_data_consumer.feed.assert_called_once_with(b"packet\n")
+        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
         assert exception is expected_error
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet____blocking_or_not____closed_client_error(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____recv_packet_from____blocking_or_not____closed_client_error(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
         recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_selector_register: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
         client.close()
         assert client.is_closed()
 
         # Act
         with pytest.raises(ClientClosedError):
-            _ = client.recv_packet(timeout=recv_timeout)
+            _ = client.recv_packet_from(timeout=recv_timeout)
 
         # Assert
-        mock_tcp_socket.settimeout.assert_not_called()
-        mock_stream_data_consumer.feed.assert_not_called()
-        mock_tcp_socket.recv.assert_not_called()
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_register.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.recvfrom.assert_not_called()
+        mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
 
     @pytest.mark.parametrize(
-        ["recv_timeout", "recv_exception"],
+        "recv_timeout",
         [
-            pytest.param(0, BlockingIOError, id="null timeout"),
-            pytest.param(123456789, TimeoutError, id="strictly positive timeout"),
+            pytest.param(0, id="null timeout"),
+            pytest.param(123456789, id="strictly positive timeout"),
         ],
     )
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____recv_packet____timeout(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____recv_packet_from____no_block____timeout(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
         recv_timeout: int,
-        recv_exception: type[BaseException],
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_selector_register: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = recv_exception
+        mock_udp_socket.recvfrom.side_effect = BlockingIOError
+        self.selector_timeout_after_n_calls(mock_selector_select, mocker, nb_calls=1)
 
         # Act & Assert
         with pytest.raises(TimeoutError, match=r"^recv_packet\(\) timed out$"):
-            _ = client.recv_packet(timeout=recv_timeout)
+            _ = client.recv_packet_from(timeout=recv_timeout)
 
-        mock_tcp_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
-        mock_stream_data_consumer.feed.assert_not_called()
+        if recv_timeout == 0:
+            assert len(mock_udp_socket.recvfrom.mock_calls) == 1
+            mock_selector_register.assert_not_called()
+            mock_selector_select.assert_not_called()
+        else:
+            assert len(mock_udp_socket.recvfrom.mock_calls) == 2
+            mock_selector_register.assert_called_with(mock_udp_socket, EVENT_READ)
+            mock_selector_select.assert_any_call(recv_timeout)
+        mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
 
     @pytest.mark.parametrize(
-        ["recv_timeout", "recv_exception"],
+        "recv_timeout",
         [
-            pytest.param(0, BlockingIOError, id="null timeout"),
-            pytest.param(123456789, TimeoutError, id="strictly positive timeout"),
+            pytest.param(0, id="null timeout"),
+            pytest.param(123456789, id="strictly positive timeout"),
         ],
     )
-    @pytest.mark.parametrize("max_recv_size", [3], indirect=True)  # Needed for timeout==0
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____yields_available_packets_with_given_timeout(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____iter_received_packets_from____yields_available_packets_with_given_timeout(
         self,
-        client: TCPNetworkClient[Any, Any],
-        max_recv_size: int,
+        client: UDPNetworkEndpoint[Any, Any],
+        sender_address: tuple[str, int],
         recv_timeout: int,
-        recv_exception: type[BaseException],
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b"pac", b"ket", b"_1\np", b"ack", b"et_", b"2\n", recv_exception]
-
-        # Act
-        packets = list(client.iter_received_packets(timeout=recv_timeout))
-
-        # Assert
-        assert mock_tcp_socket.recv.mock_calls == [mocker.call(max_recv_size) for _ in range(7)]
-        assert mock_stream_data_consumer.feed.mock_calls == [
-            mocker.call(b"pac"),
-            mocker.call(b"ket"),
-            mocker.call(b"_1\np"),
-            mocker.call(b"ack"),
-            mocker.call(b"et_"),
-            mocker.call(b"2\n"),
+        mock_udp_socket.recvfrom.side_effect = [
+            (b"packet_1", sender_address),
+            (b"packet_2", sender_address),
+            BlockingIOError,
         ]
-        assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2]
-
-    @pytest.mark.parametrize("max_recv_size", [3], indirect=True)  # Needed for timeout==0
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____yields_available_packets_until_eof(
-        self,
-        client: TCPNetworkClient[Any, Any],
-        max_recv_size: int,
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        mock_tcp_socket.recv.side_effect = [b"pac", b"ket", b"_1\np", b"ack", b"et_", b"2\n", b""]
+        self.selector_timeout_after_n_calls(mock_selector_select, mocker, nb_calls=0)
 
         # Act
-        packets = list(client.iter_received_packets(timeout=recv_timeout))
+        packets = [(p, (s.host, s.port)) for p, s in client.iter_received_packets_from(timeout=recv_timeout)]
 
         # Assert
-        assert mock_tcp_socket.recv.mock_calls == [mocker.call(max_recv_size) for _ in range(7)]
-        assert mock_stream_data_consumer.feed.mock_calls == [
-            mocker.call(b"pac"),
-            mocker.call(b"ket"),
-            mocker.call(b"_1\np"),
-            mocker.call(b"ack"),
-            mocker.call(b"et_"),
-            mocker.call(b"2\n"),
+        assert mock_udp_socket.recvfrom.mock_calls == [mocker.call(MAX_DATAGRAM_BUFSIZE) for _ in range(3)]
+        assert mock_datagram_protocol.build_packet_from_datagram.mock_calls == [
+            mocker.call(b"packet_1"),
+            mocker.call(b"packet_2"),
+        ]
+        assert packets == [
+            (mocker.sentinel.packet_1, sender_address),
+            (mocker.sentinel.packet_2, sender_address),
         ]
-        assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2]
 
-    @pytest.mark.parametrize("max_recv_size", [3], indirect=True)  # Needed for timeout==0
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____yields_available_packets_until_error(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____iter_received_packets_from____yields_available_packets_until_error(
         self,
-        client: TCPNetworkClient[Any, Any],
-        max_recv_size: int,
+        client: UDPNetworkEndpoint[Any, Any],
+        sender_address: tuple[str, int],
         recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b"pac", b"ket", b"_1\np", b"ack", b"et_", b"2\n", OSError]
+        mock_udp_socket.recvfrom.side_effect = [
+            (b"packet_1", sender_address),
+            (b"packet_2", sender_address),
+            OSError,
+        ]
 
         # Act
-        packets = list(client.iter_received_packets(timeout=recv_timeout))
+        packets = [(p, (s.host, s.port)) for p, s in client.iter_received_packets_from(timeout=recv_timeout)]
 
         # Assert
-        assert mock_tcp_socket.recv.mock_calls == [mocker.call(max_recv_size) for _ in range(7)]
-        assert mock_stream_data_consumer.feed.mock_calls == [
-            mocker.call(b"pac"),
-            mocker.call(b"ket"),
-            mocker.call(b"_1\np"),
-            mocker.call(b"ack"),
-            mocker.call(b"et_"),
-            mocker.call(b"2\n"),
+        assert mock_udp_socket.recvfrom.mock_calls == [mocker.call(MAX_DATAGRAM_BUFSIZE) for _ in range(3)]
+        assert mock_datagram_protocol.build_packet_from_datagram.mock_calls == [
+            mocker.call(b"packet_1"),
+            mocker.call(b"packet_2"),
+        ]
+        assert packets == [
+            (mocker.sentinel.packet_1, sender_address),
+            (mocker.sentinel.packet_2, sender_address),
         ]
-        assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2]
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____protocol_parse_error(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____iter_received_packets_from____protocol_parse_error(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
         recv_timeout: int | None,
-        mock_stream_data_consumer: MagicMock,
+        sender_address: tuple[str, int],
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
-        from easynetwork.exceptions import StreamProtocolParseError
+        from easynetwork.exceptions import DatagramProtocolParseError
 
-        mock_stream_data_consumer.__next__.side_effect = StreamProtocolParseError(b"", "deserialization", "Sorry")
+        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
+        expected_error = DatagramProtocolParseError("deserialization", "Sorry")
+        mock_datagram_protocol.build_packet_from_datagram.side_effect = expected_error
 
         # Act
-        with pytest.raises(StreamProtocolParseError) as exc_info:
-            _ = next(client.iter_received_packets(timeout=recv_timeout))
+        with pytest.raises(DatagramProtocolParseError) as exc_info:
+            _ = next(client.iter_received_packets_from(timeout=recv_timeout))
         exception = exc_info.value
 
         # Assert
-        assert exception is mock_stream_data_consumer.__next__.side_effect
-
-    @pytest.mark.parametrize("several_generators", [False, True], ids=lambda t: f"several_generators=={t}")
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____avoid_unnecessary_socket_recv_call(
-        self,
-        client: TCPNetworkClient[Any, Any],
-        several_generators: bool,
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
-        mock_stream_data_consumer: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        mock_tcp_socket.recv.side_effect = [b"packet_1\npacket_2\n"]
-
-        # Act
-        if several_generators:
-            packet_1 = next(client.iter_received_packets(timeout=recv_timeout))
-            packet_2 = next(client.iter_received_packets(timeout=recv_timeout))
-        else:
-            iterator = client.iter_received_packets(timeout=recv_timeout)
-            packet_1 = next(iterator)
-            packet_2 = next(iterator)
-
-        # Assert
-        mock_tcp_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
-        mock_stream_data_consumer.feed.assert_called_once_with(b"packet_1\npacket_2\n")
-        assert packet_1 is mocker.sentinel.packet_1
-        assert packet_2 is mocker.sentinel.packet_2
+        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
+        assert exception is expected_error
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____release_internal_lock_before_yield(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____iter_received_packets_from____release_internal_lock_before_yield(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
+        sender_address: tuple[str, int],
         recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
+        mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from threading import Lock
 
         mock_acquire = mocker.patch.object(Lock, "acquire", return_value=True)
         mock_release = mocker.patch.object(Lock, "release", return_value=None)
-        mock_tcp_socket.recv.side_effect = [b"packet_1\npacket_2\n"]
+        mock_udp_socket.recvfrom.side_effect = [(b"packet_1", sender_address), (b"packet_2", sender_address)]
 
         # Act & Assert
-        iterator = client.iter_received_packets(timeout=recv_timeout)
+        iterator = client.iter_received_packets_from(timeout=recv_timeout)
         mock_acquire.assert_not_called()
         mock_release.assert_not_called()
         packet_1 = next(iterator)
         mock_acquire.assert_called_once_with()
         mock_release.assert_called_once_with()
         mock_acquire.reset_mock()
         mock_release.reset_mock()
         packet_2 = next(iterator)
         mock_acquire.assert_called_once_with()
         mock_release.assert_called_once_with()
-        assert packet_1 is mocker.sentinel.packet_1
-        assert packet_2 is mocker.sentinel.packet_2
+        assert packet_1[0] is mocker.sentinel.packet_1
+        assert packet_2[0] is mocker.sentinel.packet_2
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____iter_received_packets____closed_client_during_iteration(
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    def test____iter_received_packets_from____closed_client_during_iteration(
         self,
-        client: TCPNetworkClient[Any, Any],
+        client: UDPNetworkEndpoint[Any, Any],
+        sender_address: tuple[str, int],
         recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
+        mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b"packet_1\n"]
+        mock_udp_socket.recvfrom.side_effect = [(b"packet_1", sender_address)]
 
         # Act & Assert
-        iterator = client.iter_received_packets(timeout=recv_timeout)
+        iterator = client.iter_received_packets_from(timeout=recv_timeout)
         packet_1 = next(iterator)
-        assert packet_1 is mocker.sentinel.packet_1
+        assert packet_1[0] is mocker.sentinel.packet_1
         client.close()
         assert client.is_closed()
         with pytest.raises(StopIteration):
             _ = next(iterator)
 
-    @pytest.mark.usefixtures("setup_producer_mock", "setup_consumer_mock")
-    def test____special_case____send_packet____eof_error____do_not_try_socket_send(
+
+class TestUDPNetworkClient:
+    @pytest.fixture
+    @staticmethod
+    def mock_udp_endpoint(mock_udp_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
+        mock = mocker.NonCallableMagicMock(spec=UDPNetworkEndpoint)
+        mock.get_local_address.return_value = ("local_address", 12345)
+        mock.get_remote_address.return_value = ("remote_address", 5000)
+        mock.socket = mock_udp_socket
+        return mock
+
+    @pytest.fixture(autouse=True)
+    @staticmethod
+    def mock_udp_endpoint_cls(mocker: MockerFixture, mock_udp_endpoint: MagicMock) -> MagicMock:
+        return mocker.patch(f"{UDPNetworkEndpoint.__module__}.UDPNetworkEndpoint", return_value=mock_udp_endpoint)
+
+    @pytest.fixture
+    @staticmethod
+    def client(
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+    ) -> UDPNetworkClient[Any, Any]:
+        return UDPNetworkClient(
+            mock_udp_socket,
+            mock_datagram_protocol,
+        )
+
+    def test____dunder_init____with_remote_address(
         self,
-        client: TCPNetworkClient[Any, Any],
-        mock_tcp_socket: MagicMock,
-        mock_stream_protocol: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mock_udp_endpoint_cls: MagicMock,
+        mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b""]
-        with pytest.raises(ConnectionAbortedError):
-            _ = client.recv_packet()
+        remote_address = ("remote_address", 5000)
+
+        # Act
+        client: UDPNetworkClient[Any, Any] = UDPNetworkClient(
+            remote_address,
+            mock_datagram_protocol,
+            family=mocker.sentinel.family,
+            local_address=mocker.sentinel.local_address,
+        )
 
-        mock_tcp_socket.recv.reset_mock()
-        mock_tcp_socket.settimeout.reset_mock()
+        # Assert
+        mock_udp_endpoint_cls.assert_called_once_with(
+            protocol=mock_datagram_protocol,
+            remote_address=remote_address,
+            family=mocker.sentinel.family,
+            local_address=mocker.sentinel.local_address,
+        )
+        mock_udp_endpoint.get_remote_address.assert_called_once_with()
+        assert client.socket is mock_udp_socket
+
+    def test____dunder_init____with_socket(
+        self,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mock_udp_endpoint_cls: MagicMock,
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
 
         # Act
-        with pytest.raises(ConnectionAbortedError):
-            client.send_packet(mocker.sentinel.packet)
+        client: UDPNetworkClient[Any, Any] = UDPNetworkClient(
+            mock_udp_socket,
+            mock_datagram_protocol,
+        )
 
         # Assert
-        mock_stream_protocol.generate_chunks.assert_not_called()
-        mock_tcp_socket.settimeout.assert_not_called()
-        mock_tcp_socket.sendall.assert_not_called()
+        mock_udp_endpoint_cls.assert_called_once_with(
+            protocol=mock_datagram_protocol,
+            socket=mock_udp_socket,
+        )
+        mock_udp_endpoint.get_remote_address.assert_called_once_with()
+        assert client.socket is mock_udp_socket
 
-    @pytest.mark.usefixtures("setup_consumer_mock")
-    def test____special_case____recv_packet____blocking_or_not____eof_error____do_not_try_socket_recv_on_next_call(
+    def test____dunder_init____error_no_remote_address(
         self,
-        client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
-        mock_tcp_socket: MagicMock,
+        mock_udp_socket: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.get_remote_address.return_value = None
+
+        # Act & Assert
+        with pytest.raises(OSError, match=r"^No remote address configured$"):
+            _ = UDPNetworkClient(
+                mock_udp_socket,
+                mock_datagram_protocol,
+            )
+        mock_udp_endpoint.close.assert_called_once_with()
+
+    def test____is_closed____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.is_closed.return_value = mocker.sentinel.status
+
+        # Act
+        status = client.is_closed()
+
+        # Assert
+        mock_udp_endpoint.is_closed.assert_called_once_with()
+        assert status is mocker.sentinel.status
+
+    def test____close____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.close.return_value = None
+
+        # Act
+        client.close()
+
+        # Assert
+        mock_udp_endpoint.close.assert_called_once_with()
+
+    def test____get_local_address____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+    ) -> None:
+        # Arrange
+
+        # Act
+        address = client.get_local_address()
+
+        # Assert
+        mock_udp_endpoint.get_local_address.assert_called_once_with()
+        assert address == ("local_address", 12345)
+
+    def test____get_remote_address____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+    ) -> None:
+        # Arrange
+        ## NOTE: The client should have the remote address saved. Therefore this test check if there is no new call.
+        mock_udp_endpoint.get_remote_address.assert_called_once()
+
+        # Act
+        address = client.get_remote_address()
+
+        # Assert
+        mock_udp_endpoint.get_remote_address.assert_called_once()
+        assert address == ("remote_address", 5000)
+
+    def test____send_packet____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.send_packet_to.return_value = None
+
+        # Act
+        client.send_packet(mocker.sentinel.packet)
+
+        # Assert
+        mock_udp_endpoint.send_packet_to.assert_called_once_with(mocker.sentinel.packet, None)
+
+    def test____recv_packet____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.recv_packet_from.return_value = (mocker.sentinel.packet, ("remote_address", 5000))
+
+        # Act
+        packet = client.recv_packet(timeout=mocker.sentinel.timeout)
+
+        # Assert
+        mock_udp_endpoint.recv_packet_from.assert_called_once_with(timeout=mocker.sentinel.timeout)
+        assert packet is mocker.sentinel.packet
+
+    def test____recv_packet____timeout_error(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.recv_packet_from.side_effect = TimeoutError("recv_packet() timed out")
+
+        # Act
+        with pytest.raises(TimeoutError) as exc_info:
+            _ = client.recv_packet(timeout=mocker.sentinel.timeout)
+        exception = exc_info.value
+
+        # Assert
+        mock_udp_endpoint.recv_packet_from.assert_called_once_with(timeout=mocker.sentinel.timeout)
+        assert exception is mock_udp_endpoint.recv_packet_from.side_effect
+
+    def test____iter_received_packets____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_tcp_socket.recv.side_effect = [b""]
-        with pytest.raises(ConnectionAbortedError):
-            _ = client.recv_packet(timeout=recv_timeout)
+        mock_udp_endpoint.iter_received_packets_from.side_effect = lambda timeout: iter(
+            [
+                (mocker.sentinel.packet_1, ("remote_address", 5000)),
+                (mocker.sentinel.packet_2, ("remote_address", 5000)),
+                (mocker.sentinel.packet_3, ("remote_address", 5000)),
+            ]
+        )
+
+        # Act
+        packets = list(client.iter_received_packets(timeout=mocker.sentinel.timeout))
+
+        # Assert
+        mock_udp_endpoint.iter_received_packets_from.assert_called_once_with(timeout=mocker.sentinel.timeout)
+        assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2, mocker.sentinel.packet_3]
 
-        mock_tcp_socket.recv.reset_mock()
-        mock_tcp_socket.settimeout.reset_mock()
+    def test____fileno____default(
+        self,
+        client: UDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.fileno.return_value = mocker.sentinel.fd
 
         # Act
-        with pytest.raises(ConnectionAbortedError):
-            _ = client.recv_packet(timeout=recv_timeout)
+        fd = client.fileno()
 
         # Assert
-        mock_tcp_socket.recv.assert_not_called()
-        mock_tcp_socket.settimeout.assert_not_called()
+        mock_udp_endpoint.fileno.assert_called_once_with()
+        assert fd is mocker.sentinel.fd
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_client/test_udp.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_async/test_api/test_client/test_udp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
-from socket import AF_INET6, SOCK_DGRAM
-from typing import TYPE_CHECKING, Any
+from socket import AF_INET6
+from typing import TYPE_CHECKING, Any, cast
 
-from easynetwork.client.udp import UDPNetworkClient, UDPNetworkEndpoint
+from easynetwork.api_async.client.udp import AsyncUDPNetworkClient, AsyncUDPNetworkEndpoint
 from easynetwork.exceptions import ClientClosedError
-from easynetwork.tools.socket import MAX_DATAGRAM_BUFSIZE, IPv4SocketAddress, IPv6SocketAddress
+from easynetwork.tools.socket import IPv4SocketAddress, IPv6SocketAddress, SocketProxy
 
 import pytest
+import pytest_asyncio
 
 if TYPE_CHECKING:
-    from unittest.mock import MagicMock
+    from unittest.mock import MagicMock, AsyncMock
 
     from pytest_mock import MockerFixture
 
 from .base import BaseTestClient
 
 
-@pytest.fixture(scope="module", autouse=True)
-def setup_dummy_lock(module_mocker: MockerFixture, dummy_lock_cls: Any) -> None:
-    module_mocker.patch(f"{UDPNetworkEndpoint.__module__}._Lock", new=dummy_lock_cls)
+@pytest.fixture(autouse=True)
+def mock_new_backend(mocker: MockerFixture, mock_backend: MagicMock) -> MagicMock:
+    from easynetwork.api_async.backend.factory import AsyncBackendFactory
 
+    return mocker.patch.object(AsyncBackendFactory, "new", return_value=mock_backend)
 
-def _get_all_socket_families() -> list[str]:
-    import socket
 
-    return [v for v in dir(socket) if v.startswith("AF_")]
-
-
-class TestUDPNetworkEndpoint(BaseTestClient):
+@pytest.mark.asyncio
+class TestAsyncUDPNetworkEndpoint(BaseTestClient):
     @pytest.fixture(scope="class", params=["AF_INET", "AF_INET6"])
     @staticmethod
     def socket_family(request: Any) -> Any:
         import socket
 
         return getattr(socket, request.param)
 
@@ -45,71 +43,72 @@
 
     @pytest.fixture(scope="class")
     @staticmethod
     def global_remote_address() -> tuple[str, int]:
         return ("remote_address", 5000)
 
     @pytest.fixture(autouse=True)
-    @staticmethod
-    def mock_socket_cls(mocker: MockerFixture, mock_udp_socket: MagicMock, original_socket_cls: type[Any]) -> MagicMock:
-        mock_socket_cls = mocker.patch("socket.socket", return_value=mock_udp_socket, autospec=True)
-
-        def patch_isinstance(obj: Any, type: Any) -> bool:
-            if type is mock_socket_cls:
-                type = original_socket_cls
-            return isinstance(obj, type)
-
-        mocker.patch(f"{UDPNetworkEndpoint.__module__}.isinstance", patch_isinstance)
-        return mock_socket_cls
-
-    @pytest.fixture(autouse=True)
-    @staticmethod
-    def mock_socket_proxy_cls(mocker: MockerFixture, mock_udp_socket: MagicMock) -> MagicMock:
-        return mocker.patch(f"{UDPNetworkClient.__module__}.SocketProxy", return_value=mock_udp_socket)
-
-    @pytest.fixture(autouse=True)
     @classmethod
     def local_address(
         cls,
+        mock_datagram_socket_adapter: MagicMock,
         mock_udp_socket: MagicMock,
         socket_family: int,
         global_local_address: tuple[str, int],
     ) -> tuple[str, int]:
         cls.set_local_address_to_socket_mock(mock_udp_socket, socket_family, global_local_address)
+        cls.set_local_address_to_async_socket_adapter_mock(
+            mock_datagram_socket_adapter,
+            socket_family,
+            global_local_address,
+        )
         return global_local_address
 
     @pytest.fixture(autouse=True, params=[False, True], ids=lambda p: f"remote_address=={p}")
     @classmethod
     def remote_address(
         cls,
         request: Any,
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         socket_family: int,
         global_remote_address: tuple[str, int],
     ) -> tuple[str, int] | None:
         match request.param:
             case True:
-                cls.set_remote_address_to_socket_mock(mock_udp_socket, socket_family, global_remote_address)
+                cls.set_remote_address_to_async_socket_adapter_mock(
+                    mock_datagram_socket_adapter,
+                    socket_family,
+                    global_remote_address,
+                )
                 return global_remote_address
             case False:
-                cls.configure_socket_mock_to_raise_ENOTCONN(mock_udp_socket)
+                mock_datagram_socket_adapter.get_remote_address.return_value = None
                 return None
             case invalid:
                 pytest.fail(f"Invalid fixture param: Got {invalid!r}")
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def set_default_socket_mock_configuration(
         mock_udp_socket: MagicMock,
         socket_family: int,
-        mocker: MockerFixture,
+        mock_backend: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         mock_udp_socket.family = socket_family
-        mock_udp_socket.gettimeout.return_value = mocker.sentinel.default_timeout
         mock_udp_socket.getsockopt.return_value = 0  # Needed for tests dealing with send_packet_to()
+        del mock_udp_socket.getpeername
+        del mock_udp_socket.send
+        del mock_udp_socket.sendto
+        del mock_udp_socket.recvfrom
+
+        mock_backend.create_udp_endpoint.return_value = mock_datagram_socket_adapter
+        mock_backend.wrap_udp_socket.return_value = mock_datagram_socket_adapter
+
+        mock_datagram_socket_adapter.socket.return_value = mock_udp_socket
 
     @pytest.fixture  # DO NOT set autouse=True
     @staticmethod
     def setup_protocol_mock(mock_datagram_protocol: MagicMock, mocker: MockerFixture) -> None:
         sentinel = mocker.sentinel
 
         def make_datagram_side_effect(packet: Any) -> bytes:
@@ -117,1063 +116,1058 @@
 
         def build_packet_from_datagram_side_effect(data: bytes) -> Any:
             return getattr(sentinel, data.decode("ascii"))
 
         mock_datagram_protocol.make_datagram.side_effect = make_datagram_side_effect
         mock_datagram_protocol.build_packet_from_datagram.side_effect = build_packet_from_datagram_side_effect
 
-    @pytest.fixture(params=["REMOTE_ADDRESS", "SOCKET_WITH_EXPLICIT_GIVE"])
+    @pytest.fixture
     @staticmethod
-    def client_with_socket_ownership(
-        request: Any,
-        remote_address: tuple[str, int] | None,
+    def client_not_bound(
+        mock_backend: MagicMock,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
-    ) -> UDPNetworkEndpoint[Any, Any]:
-        match request.param:
-            case "REMOTE_ADDRESS":
-                return UDPNetworkEndpoint(protocol=mock_datagram_protocol, remote_address=remote_address)
-            case "SOCKET_WITH_EXPLICIT_GIVE":
-                return UDPNetworkEndpoint(socket=mock_udp_socket, protocol=mock_datagram_protocol, give=True)
-            case invalid:
-                pytest.fail(f"Invalid fixture param: Got {invalid!r}")
+    ) -> AsyncUDPNetworkEndpoint[Any, Any]:
+        client: AsyncUDPNetworkEndpoint[Any, Any] = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
+            socket=mock_udp_socket,
+            backend=mock_backend,
+        )
+        assert not client.is_bound()
+        return client
 
-    @pytest.fixture
+    @pytest_asyncio.fixture
     @staticmethod
-    def client_without_socket_ownership(
-        mock_udp_socket: MagicMock,
-        mock_datagram_protocol: MagicMock,
-        remote_address: tuple[str, int] | None,  # Only for fixture dependency, do not remove
-    ) -> UDPNetworkEndpoint[Any, Any]:
-        return UDPNetworkEndpoint(mock_datagram_protocol, socket=mock_udp_socket, give=False)
+    async def client_bound(client_not_bound: AsyncUDPNetworkEndpoint[Any, Any]) -> AsyncUDPNetworkEndpoint[Any, Any]:
+        await client_not_bound.wait_bound()
+        assert client_not_bound.is_bound()
+        return client_not_bound
 
-    @pytest.fixture
+    @pytest.fixture(params=[False, True], ids=lambda boolean: f"client_bound=={boolean}")
     @staticmethod
-    def client(client_without_socket_ownership: UDPNetworkEndpoint[Any, Any]) -> UDPNetworkEndpoint[Any, Any]:
-        return client_without_socket_ownership
+    def client_bound_or_not(request: pytest.FixtureRequest) -> AsyncUDPNetworkEndpoint[Any, Any]:
+        client_to_use: str = {False: "client_not_bound", True: "client_bound"}[getattr(request, "param")]
+        return request.getfixturevalue(client_to_use)
 
     @pytest.fixture
     @staticmethod
     def sender_address(request: Any, global_remote_address: tuple[str, int]) -> tuple[str, int]:
-        try:
-            param: Any = request.param
-        except AttributeError:
-            return global_remote_address
+        param: Any = getattr(request, "param", "REMOTE")
         if param == "REMOTE":
             return global_remote_address
         host, port = param
         return host, port
 
-    @pytest.fixture(
-        params=[
-            pytest.param(None, id="blocking"),
-            pytest.param(0, id="non_blocking"),
-            pytest.param(123456789, id="with_timeout"),
-        ]
-    )
-    @staticmethod
-    def recv_timeout(request: Any) -> Any:
-        return request.param
-
-    def test____dunder_init____create_datagram_endpoint____default(
+    async def test____dunder_init____with_remote_address(
         self,
+        remote_address: tuple[str, int] | None,
         socket_family: int,
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mock_socket_cls: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
+        mock_new_backend: MagicMock,
+        mock_backend: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_socket_proxy_cls.return_value = mocker.sentinel.proxy
 
         # Act
-        endpoint: UDPNetworkEndpoint[Any, Any] = UDPNetworkEndpoint(protocol=mock_datagram_protocol, family=socket_family)
+        client: AsyncUDPNetworkEndpoint[Any, Any] = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
+            family=socket_family,
+            remote_address=remote_address,
+            local_address=mocker.sentinel.local_address,
+            reuse_port=mocker.sentinel.reuse_port,
+        )
+        await client.wait_bound()
 
         # Assert
-        mock_socket_cls.assert_called_once_with(socket_family, SOCK_DGRAM)
-        mock_udp_socket.bind.assert_called_once_with(("", 0))
-        mock_udp_socket.connect.assert_not_called()
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_udp_socket.getpeername.assert_not_called()
-        mock_socket_proxy_cls.assert_called_once_with(mock_udp_socket, lock=mocker.ANY)
-        assert endpoint.socket is mocker.sentinel.proxy
+        mock_new_backend.assert_called_once_with(None)
+        mock_backend.create_udp_endpoint.assert_awaited_once_with(
+            family=socket_family,
+            remote_address=remote_address,
+            local_address=mocker.sentinel.local_address,
+            reuse_port=mocker.sentinel.reuse_port,
+        )
+        mock_datagram_socket_adapter.socket.assert_called_once_with()
+        mock_datagram_socket_adapter.get_local_address.assert_called_once_with()
+        mock_datagram_socket_adapter.get_remote_address.assert_called_once_with()
+        assert isinstance(client.socket, SocketProxy)
 
-    @pytest.mark.parametrize("source_address", [None, ("local_address", 12345)], ids=lambda p: f"source_address=={p}")
-    def test____dunder_init____create_datagram_endpoint____with_parameters(
+    async def test____dunder_init____with_remote_address____force_local_address(
         self,
-        socket_family: int,
-        source_address: tuple[str, int] | None,
         remote_address: tuple[str, int] | None,
-        mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mock_socket_cls: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
+        mock_backend: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
 
         # Act
-        _ = UDPNetworkEndpoint(
-            protocol=mock_datagram_protocol,
-            family=socket_family,
-            source_address=source_address,
+        client: AsyncUDPNetworkEndpoint[Any, Any] = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
             remote_address=remote_address,
+            local_address=None,
         )
+        await client.wait_bound()
 
         # Assert
-        mock_socket_cls.assert_called_once_with(socket_family, SOCK_DGRAM)
-        if source_address is None:
-            mock_udp_socket.bind.assert_called_once_with(("", 0))
-        else:
-            mock_udp_socket.bind.assert_called_once_with(source_address)
-        if remote_address is None:
-            mock_udp_socket.connect.assert_not_called()
-            mock_udp_socket.getpeername.assert_not_called()
-        else:
-            mock_udp_socket.connect.assert_called_once_with(remote_address)
-            mock_udp_socket.getpeername.assert_called_once_with()
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_socket_proxy_cls.assert_called_once_with(mock_udp_socket, lock=mocker.ANY)
-
-    @pytest.mark.parametrize(
-        "socket_family", list(set(_get_all_socket_families()).difference(["AF_INET", "AF_INET6"])), indirect=True
-    )
-    def test____dunder_init____create_datagram_endpoint____invalid_socket_family(
+        mock_backend.create_udp_endpoint.assert_awaited_once_with(
+            remote_address=remote_address,
+            local_address=(None, 0),
+        )
+
+    async def test____dunder_init____backend____from_string(
         self,
-        socket_family: int,
+        remote_address: tuple[str, int] | None,
         mock_datagram_protocol: MagicMock,
+        mock_new_backend: MagicMock,
     ) -> None:
         # Arrange
 
-        # Act & Assert
-        with pytest.raises(ValueError, match=r"^Only AF_INET and AF_INET6 families are supported$"):
-            _ = UDPNetworkEndpoint(protocol=mock_datagram_protocol, family=socket_family)
+        # Act
+        _ = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
+            remote_address=remote_address,
+            backend="custom_backend",
+            backend_kwargs={"arg1": 1, "arg2": "2"},
+        )
 
-    @pytest.mark.parametrize("error_on", ["bind", "connect"])
-    @pytest.mark.parametrize("remote_address", [True], indirect=True)
-    def test____dunder_init____create_datagram_endpoint____close_socket_if_an_error_occurs(
+        # Assert
+        mock_new_backend.assert_called_once_with("custom_backend", arg1=1, arg2="2")
+
+    async def test____dunder_init____backend____explicit_argument(
         self,
-        error_on: str,
-        local_address: tuple[str, int],
-        remote_address: tuple[str, int],
-        socket_family: int,
-        mock_udp_socket: MagicMock,
+        remote_address: tuple[str, int] | None,
         mock_datagram_protocol: MagicMock,
+        mock_backend: MagicMock,
+        mock_new_backend: MagicMock,
     ) -> None:
         # Arrange
-        mock_method: MagicMock = getattr(mock_udp_socket, error_on)
-        mock_method.side_effect = OSError()
 
-        # Act & Assert
-        with pytest.raises(type(mock_method.side_effect)) as exc_info:
-            _ = UDPNetworkEndpoint(
-                protocol=mock_datagram_protocol,
-                family=socket_family,
-                source_address=local_address,
-                remote_address=remote_address,
-            )
-        assert exc_info.value is mock_method.side_effect
-        mock_udp_socket.close.assert_called_once_with()
-
-    @pytest.mark.parametrize("give_ownership", [False, True], ids=lambda p: f"give=={p}")
-    @pytest.mark.parametrize("bound", [False, True], ids=lambda p: f"bound=={p}")
-    def test____dunder_init____use_given_socket____default(
+        # Act
+        _ = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
+            remote_address=remote_address,
+            backend=mock_backend,
+        )
+
+        # Assert
+        mock_new_backend.assert_not_called()
+
+    async def test____dunder_init____use_given_socket(
         self,
-        give_ownership: bool,
-        bound: bool,
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mock_socket_cls: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
-        mocker: MockerFixture,
+        mock_new_backend: MagicMock,
+        mock_backend: MagicMock,
     ) -> None:
         # Arrange
-        mock_socket_proxy_cls.return_value = mocker.sentinel.proxy
-        if not bound:
-            mock_udp_socket.getsockname.return_value = ("0.0.0.0", 0)
 
         # Act
-        endpoint: UDPNetworkEndpoint[Any, Any] = UDPNetworkEndpoint(
-            protocol=mock_datagram_protocol,
+        client: AsyncUDPNetworkEndpoint[Any, Any] = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
             socket=mock_udp_socket,
-            give=give_ownership,
         )
+        await client.wait_bound()
 
         # Assert
-        mock_socket_cls.assert_not_called()
-        if bound:
-            mock_udp_socket.bind.assert_not_called()
-        else:
-            mock_udp_socket.bind.assert_called_once_with(("", 0))
-        mock_udp_socket.connect.assert_not_called()
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_udp_socket.getpeername.assert_called_once_with()
-        mock_socket_proxy_cls.assert_called_once_with(mock_udp_socket, lock=mocker.ANY)
-        assert endpoint.socket is mocker.sentinel.proxy
-
-    @pytest.mark.parametrize(
-        "socket_family", list(set(_get_all_socket_families()).difference(["AF_INET", "AF_INET6"])), indirect=True
-    )
-    def test____dunder_init____use_given_socket____invalid_socket_family(
+        mock_udp_socket.bind.assert_not_called()
+        mock_new_backend.assert_called_once_with(None)
+        mock_backend.wrap_udp_socket.assert_awaited_once_with(mock_udp_socket)
+        mock_datagram_socket_adapter.socket.assert_called_once_with()
+        mock_datagram_socket_adapter.get_local_address.assert_called_once_with()
+        mock_datagram_socket_adapter.get_remote_address.assert_called_once_with()
+        assert isinstance(client.socket, SocketProxy)
+
+    async def test____dunder_init____use_given_socket____force_local_address(
         self,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
+        mock_udp_socket.getsockname.return_value = ("0.0.0.0", 0)
+
+        # Act
+        _ = AsyncUDPNetworkEndpoint(
+            mock_datagram_protocol,
+            socket=mock_udp_socket,
+        )
+
+        # Assert
+        mock_udp_socket.bind.assert_called_once_with(("", 0))
+
+    async def test____context____close_endpoint_at_end(
+        self,
+        client_not_bound: AsyncUDPNetworkEndpoint[Any, Any],
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_wait_bound = cast("AsyncMock", mocker.patch.object(AsyncUDPNetworkEndpoint, "wait_bound"))
+        mock_close = cast("AsyncMock", mocker.patch.object(AsyncUDPNetworkEndpoint, "aclose"))
+
+        # Act
+        async with client_not_bound:
+            mock_wait_bound.assert_awaited_once_with()
+            mock_close.assert_not_awaited()
+
+        # Assert
+        mock_wait_bound.assert_awaited_once_with()
+        mock_close.assert_awaited_once_with()
+
+    async def test___is_closing___connection_not_performed_yet(
+        self,
+        client_not_bound: AsyncUDPNetworkEndpoint[Any, Any],
+    ) -> None:
+        # Arrange
 
         # Act & Assert
-        with pytest.raises(ValueError, match=r"^Only AF_INET and AF_INET6 families are supported$"):
-            _ = UDPNetworkEndpoint(
-                protocol=mock_datagram_protocol,
-                socket=mock_udp_socket,
-                give=False,
-            )
+        assert not client_not_bound.is_closing()
+        await client_not_bound.wait_bound()
+        assert not client_not_bound.is_closing()
 
-    @pytest.mark.parametrize("give_ownership", [False, True], ids=lambda p: f"give=={p}")
-    def test____dunder_init____use_given_socket____invalid_socket_type_error(
+    async def test____aclose____await_socket_close(
         self,
-        give_ownership: bool,
-        mock_tcp_socket: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
-        mock_datagram_protocol: MagicMock,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
+        assert not client_bound.is_closing()
 
         # Act
-        with pytest.raises(ValueError, match=r"^Invalid socket type$"):
-            _ = UDPNetworkEndpoint(
-                protocol=mock_datagram_protocol,
-                socket=mock_tcp_socket,
-                give=give_ownership,
-            )
+        await client_bound.aclose()
 
         # Assert
-        mock_socket_proxy_cls.assert_not_called()
-        mock_tcp_socket.getsockname.assert_not_called()
-        mock_tcp_socket.getpeername.assert_not_called()
-        ## If ownership was given, the socket must be closed
-        if give_ownership:
-            mock_tcp_socket.close.assert_called_once_with()
-        else:
-            mock_tcp_socket.close.assert_not_called()
+        assert client_bound.is_closing()
+        mock_datagram_socket_adapter.aclose.assert_awaited_once_with()
 
-    def test____dunder_init____use_given_socket____ownership_parameter_missing(
+    async def test____aclose____connection_not_performed_yet(
         self,
-        mock_udp_socket: MagicMock,
-        mock_socket_proxy_cls: MagicMock,
-        mock_datagram_protocol: MagicMock,
-        mocker: MockerFixture,
+        client_not_bound: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
+        assert not client_not_bound.is_closing()
 
         # Act
-        with pytest.raises(TypeError, match=r"^Missing keyword argument 'give'$"):
-            _ = UDPNetworkEndpoint(  # type: ignore[call-overload]
-                protocol=mock_datagram_protocol,
-                socket=mock_udp_socket,
-            )
+        await client_not_bound.aclose()
 
         # Assert
-        mock_socket_proxy_cls.assert_not_called()
-        mock_udp_socket.close.assert_not_called()
+        assert client_not_bound.is_closing()
+        mock_datagram_socket_adapter.aclose.assert_not_awaited()
 
-    def test____context____close_endpoint_at_end(
+    async def test____aclose____await_socket_close____error_occurred(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        mocker: MockerFixture,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
-        mock_close = mocker.patch.object(UDPNetworkEndpoint, "close")
+        error = OSError("Bad file descriptor")
+        mock_datagram_socket_adapter.aclose.side_effect = error
+        assert not client_bound.is_closing()
 
         # Act
-        with client:
-            mock_close.assert_not_called()
+        with pytest.raises(OSError) as exc_info:
+            await client_bound.aclose()
 
         # Assert
-        mock_close.assert_called_once_with()
+        assert client_bound.is_closing()
+        assert exc_info.value is error
+        mock_datagram_socket_adapter.aclose.assert_awaited_once_with()
 
-    def test____close____with_ownership(
+    async def test____aclose____await_socket_close____hide_connection_error(
         self,
-        client_with_socket_ownership: UDPNetworkEndpoint[Any, Any],
-        mock_udp_socket: MagicMock,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
-        assert not client_with_socket_ownership.is_closed()
+        error = ConnectionAbortedError()
+        mock_datagram_socket_adapter.aclose.side_effect = error
+        assert not client_bound.is_closing()
 
         # Act
-        client_with_socket_ownership.close()
+        await client_bound.aclose()
 
         # Assert
-        assert client_with_socket_ownership.is_closed()
-        mock_udp_socket.close.assert_called_once_with()
+        assert client_bound.is_closing()
+        mock_datagram_socket_adapter.aclose.assert_awaited_once_with()
 
-    def test____close____without_ownership(
+    async def test____aclose____already_closed(
         self,
-        client_without_socket_ownership: UDPNetworkEndpoint[Any, Any],
-        mock_udp_socket: MagicMock,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
-        assert not client_without_socket_ownership.is_closed()
+        await client_bound.aclose()
+        assert client_bound.is_closing()
 
         # Act
-        client_without_socket_ownership.close()
+        await client_bound.aclose()
 
         # Assert
-        assert client_without_socket_ownership.is_closed()
-        mock_udp_socket.close.assert_not_called()
+        mock_datagram_socket_adapter.aclose.assert_awaited_once_with()
+
+    async def test____aclose____cancellation(
+        self,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
+        fake_cancellation_cls: type[BaseException],
+    ) -> None:
+        # Arrange
+        mock_datagram_socket_adapter.aclose.side_effect = fake_cancellation_cls
+
+        # Act
+        with pytest.raises(fake_cancellation_cls):
+            await client_bound.aclose()
+
+        # Assert
+        mock_datagram_socket_adapter.aclose.assert_awaited_once_with()
 
     @pytest.mark.parametrize("client_closed", [False, True], ids=lambda p: f"client_closed=={p}")
-    def test____get_local_address____return_saved_address(
+    async def test____get_local_address____return_saved_address(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
         client_closed: bool,
         socket_family: int,
         local_address: tuple[str, int],
-        mock_udp_socket: MagicMock,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
-        mock_udp_socket.getsockname.reset_mock()
+        mock_datagram_socket_adapter.get_local_address.reset_mock()
         if client_closed:
-            client.close()
-            assert client.is_closed()
+            await client_bound.aclose()
+            assert client_bound.is_closing()
 
         # Act
-        address = client.get_local_address()
+        address = client_bound.get_local_address()
 
         # Assert
         if socket_family == AF_INET6:
             assert isinstance(address, IPv6SocketAddress)
         else:
             assert isinstance(address, IPv4SocketAddress)
-        mock_udp_socket.getsockname.assert_not_called()
+        mock_datagram_socket_adapter.get_local_address.assert_not_called()
         assert address.host == local_address[0]
         assert address.port == local_address[1]
 
+    async def test____get_local_address____error_connection_not_performed(
+        self,
+        client_not_bound: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
+    ) -> None:
+        # Arrange
+
+        # Act
+        with pytest.raises(OSError):
+            client_not_bound.get_local_address()
+
+        # Assert
+        mock_datagram_socket_adapter.get_local_address.assert_not_called()
+
     @pytest.mark.parametrize("client_closed", [False, True], ids=lambda p: f"client_closed=={p}")
-    def test____get_remote_address____return_saved_address(
+    async def test____get_remote_address____return_saved_address(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
         client_closed: bool,
         remote_address: tuple[str, int] | None,
         socket_family: int,
-        mock_udp_socket: MagicMock,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
     ) -> None:
         # Arrange
         ## NOTE: The client should have the remote address saved. Therefore this test check if there is no new call.
-        mock_udp_socket.getpeername.assert_called_once()
+        mock_datagram_socket_adapter.get_remote_address.assert_called_once()
         if client_closed:
-            client.close()
-            assert client.is_closed()
+            await client_bound.aclose()
+            assert client_bound.is_closing()
 
         # Act
-        address = client.get_remote_address()
+        address = client_bound.get_remote_address()
 
         # Assert
         if remote_address is None:
             assert address is None
         else:
             if socket_family == AF_INET6:
                 assert isinstance(address, IPv6SocketAddress)
             else:
                 assert isinstance(address, IPv4SocketAddress)
-            mock_udp_socket.getpeername.assert_called_once()
             assert address.host == remote_address[0]
             assert address.port == remote_address[1]
+        mock_datagram_socket_adapter.get_remote_address.assert_called_once()
 
-    def test____fileno____default(
+    async def test____get_remote_address____error_connection_not_performed(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_not_bound: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
+    ) -> None:
+        # Arrange
+
+        # Act
+        with pytest.raises(OSError):
+            client_not_bound.get_remote_address()
+
+        # Assert
+        mock_datagram_socket_adapter.get_remote_address.assert_not_called()
+
+    async def test____fileno____default(
+        self,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
         mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_udp_socket.fileno.return_value = mocker.sentinel.fileno
 
         # Act
-        fd = client.fileno()
+        fd = client_bound.fileno()
 
         # Assert
         mock_udp_socket.fileno.assert_called_once_with()
         assert fd is mocker.sentinel.fileno
 
-    def test____fileno____closed_client(
+    async def test____fileno____connection_not_performed(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_not_bound: AsyncUDPNetworkEndpoint[Any, Any],
         mock_udp_socket: MagicMock,
     ) -> None:
         # Arrange
-        client.close()
-        assert client.is_closed()
 
         # Act
-        fd = client.fileno()
+        fd = client_not_bound.fileno()
+
+        # Assert
+        mock_udp_socket.fileno.assert_not_called()
+        assert fd == -1
+
+    async def test____fileno____closed_client(
+        self,
+        client_bound: AsyncUDPNetworkClient[Any, Any],
+        mock_udp_socket: MagicMock,
+    ) -> None:
+        # Arrange
+        await client_bound.aclose()
+        assert client_bound.is_closing()
+
+        # Act
+        fd = client_bound.fileno()
 
         # Assert
         mock_udp_socket.fileno.assert_not_called()
         assert fd == -1
 
     @pytest.mark.parametrize("remote_address", [False], indirect=True)
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____send_packet_to____send_bytes_to_socket____without_remote____dedault(
+    async def test____send_packet_to____send_bytes_to_socket____without_remote____default(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        mock_udp_socket: MagicMock,
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
+        mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from socket import SO_ERROR, SOL_SOCKET
 
         target_address: tuple[str, int] = ("remote_address", 5000)
 
         # Act
-        client.send_packet_to(mocker.sentinel.packet, target_address)
+        await client_bound_or_not.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        assert mock_udp_socket.settimeout.mock_calls == [mocker.call(None), mocker.call(mocker.sentinel.default_timeout)]
-        mock_udp_socket.sendto.assert_called_once_with(b"packet", target_address)
+        mock_datagram_socket_adapter.sendto.assert_awaited_once_with(b"packet", target_address)
         mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
         mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
     @pytest.mark.parametrize("remote_address", [False], indirect=True)
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____send_packet_to____send_bytes_to_socket____without_remote____None_address_error(
+    async def test____send_packet_to____send_bytes_to_socket____without_remote____None_address_error(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
 
         # Act
         with pytest.raises(ValueError, match=r"^Invalid address: must not be None$"):
-            client.send_packet_to(mocker.sentinel.packet, None)
+            await client_bound_or_not.send_packet_to(mocker.sentinel.packet, None)
 
         # Assert
-        mock_udp_socket.send.assert_not_called()
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_udp_socket.sendto.assert_not_called()
+        mock_datagram_socket_adapter.sendto.assert_not_awaited()
         mock_datagram_protocol.make_datagram.assert_not_called()
         mock_udp_socket.getsockopt.assert_not_called()
 
     @pytest.mark.parametrize("target_address", [None, ("remote_address", 5000)], ids=lambda p: f"target_address=={p}")
     @pytest.mark.parametrize("remote_address", [True], indirect=True)
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____send_packet_to____send_bytes_to_socket____with_remote____default(
+    async def test____send_packet_to____send_bytes_to_socket____with_remote____default(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         target_address: tuple[str, int] | None,
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from socket import SO_ERROR, SOL_SOCKET
 
         # Act
-        client.send_packet_to(mocker.sentinel.packet, target_address)
+        await client_bound_or_not.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        assert mock_udp_socket.settimeout.mock_calls == [mocker.call(None), mocker.call(mocker.sentinel.default_timeout)]
-        mock_udp_socket.sendto.assert_not_called()
-        mock_udp_socket.send.assert_called_once_with(b"packet")
+        mock_datagram_socket_adapter.sendto.assert_awaited_once_with(b"packet", None)
         mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
         mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
     @pytest.mark.parametrize("remote_address", [True], indirect=True)
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____send_packet_to____send_bytes_to_socket____with_remote____invalid_target_address(
+    async def test____send_packet_to____send_bytes_to_socket____with_remote____invalid_target_address(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         target_address: tuple[str, int] = ("address_other_than_remote", 9999)
 
         # Act
         with pytest.raises(ValueError, match=r"^Invalid address: must be None or .+$"):
-            client.send_packet_to(mocker.sentinel.packet, target_address)
+            await client_bound_or_not.send_packet_to(mocker.sentinel.packet, target_address)
 
         # Assert
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_udp_socket.sendto.assert_not_called()
+        mock_datagram_socket_adapter.sendto.assert_not_awaited()
         mock_datagram_protocol.make_datagram.assert_not_called()
         mock_udp_socket.getsockopt.assert_not_called()
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____send_packet_to____raise_error_saved_in_SO_ERROR_option(
+    async def test____send_packet_to____raise_error_saved_in_SO_ERROR_option(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         global_remote_address: tuple[str, int],
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from errno import ECONNREFUSED
         from socket import SO_ERROR, SOL_SOCKET
 
         mock_udp_socket.getsockopt.return_value = ECONNREFUSED
 
         # Act
         with pytest.raises(OSError) as exc_info:
-            client.send_packet_to(mocker.sentinel.packet, global_remote_address)
+            await client_bound_or_not.send_packet_to(mocker.sentinel.packet, global_remote_address)
 
         # Assert
         assert exc_info.value.errno == ECONNREFUSED
-        assert mock_udp_socket.settimeout.mock_calls == [mocker.call(None), mocker.call(mocker.sentinel.default_timeout)]
-        if client.get_remote_address() is not None:
-            mock_udp_socket.sendto.assert_not_called()
-            mock_udp_socket.send.assert_called_once()
-        else:
-            mock_udp_socket.sendto.assert_called_once()
-            mock_udp_socket.send.assert_not_called()
+        mock_datagram_socket_adapter.sendto.assert_awaited_once()
         mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
         mock_udp_socket.getsockopt.assert_called_once_with(SOL_SOCKET, SO_ERROR)
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____send_packet_to____closed_client_error(
+    async def test____send_packet_to____closed_client_error(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         remote_address: tuple[str, int] | None,
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        client.close()
-        assert client.is_closed()
+        await client_bound_or_not.aclose()
+        assert client_bound_or_not.is_closing()
 
         # Act
         with pytest.raises(ClientClosedError):
-            client.send_packet_to(mocker.sentinel.packet, remote_address)
+            await client_bound_or_not.send_packet_to(mocker.sentinel.packet, remote_address)
 
         # Assert
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_udp_socket.sendto.assert_not_called()
+        mock_datagram_socket_adapter.sendto.assert_not_awaited()
         mock_datagram_protocol.make_datagram.assert_not_called()
         mock_udp_socket.getsockopt.assert_not_called()
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____recv_packet_from_blocking_or_not____receive_bytes_from_socket(
+    async def test____send_packet_to____unexpected_socket_close(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        sender_address: tuple[str, int],
-        recv_timeout: int | None,
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
+        remote_address: tuple[str, int] | None,
         mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
+        mock_datagram_socket_adapter.is_closing.return_value = True
 
         # Act
-        packet, sender = client.recv_packet_from(timeout=recv_timeout)
+        with pytest.raises(ConnectionAbortedError):
+            await client_bound_or_not.send_packet_to(mocker.sentinel.packet, remote_address)
 
         # Assert
-        assert mock_udp_socket.settimeout.mock_calls == [mocker.call(recv_timeout), mocker.call(mocker.sentinel.default_timeout)]
-        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
-        mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
-        assert packet is mocker.sentinel.packet
-        assert (sender.host, sender.port) == sender_address
+        mock_datagram_socket_adapter.sendto.assert_not_awaited()
+        mock_datagram_protocol.make_datagram.assert_not_called()
+        mock_udp_socket.getsockopt.assert_not_called()
 
-    @pytest.mark.parametrize("sender_address", ["REMOTE", ("any_other_address", 9999)], indirect=True)
-    @pytest.mark.parametrize("remote_address", [False], indirect=True)
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____recv_packet_from_blocking_or_not____without_remote____receive_bytes_from_anyone(
+    async def test____recv_packet_from____receive_bytes_from_socket(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
+        mock_datagram_socket_adapter.recvfrom.side_effect = [(b"packet", sender_address)]
 
         # Act
-        packet, sender = client.recv_packet_from(timeout=recv_timeout)
+        packet, sender = await client_bound_or_not.recv_packet_from()
 
         # Assert
-        assert mock_udp_socket.settimeout.mock_calls == [mocker.call(recv_timeout), mocker.call(mocker.sentinel.default_timeout)]
-        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_socket_adapter.recvfrom.assert_awaited_once_with()
         mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
         assert packet is mocker.sentinel.packet
         assert (sender.host, sender.port) == sender_address
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____recv_packet_from_blocking_or_not____protocol_parse_error(
+    async def test____recv_packet_from____protocol_parse_error(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mocker: MockerFixture,
     ) -> None:
         # Arrange
         from easynetwork.exceptions import DatagramProtocolParseError
 
-        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
+        mock_datagram_socket_adapter.recvfrom.side_effect = [(b"packet", sender_address)]
         expected_error = DatagramProtocolParseError("deserialization", "Sorry")
         mock_datagram_protocol.build_packet_from_datagram.side_effect = expected_error
 
         # Act
         with pytest.raises(DatagramProtocolParseError) as exc_info:
-            _ = client.recv_packet_from(timeout=recv_timeout)
+            _ = await client_bound_or_not.recv_packet_from()
         exception = exc_info.value
 
         # Assert
-        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_socket_adapter.recvfrom.assert_awaited_once_with()
         mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
         assert exception is expected_error
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____recv_packet_from_blocking_or_not____closed_client_error(
+    async def test____recv_packet_from____closed_client_error(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        recv_timeout: int | None,
-        mock_udp_socket: MagicMock,
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
-        client.close()
-        assert client.is_closed()
+        await client_bound_or_not.aclose()
+        assert client_bound_or_not.is_closing()
 
         # Act
-        with pytest.raises(OSError, match=r"^Closed client$"):
-            _ = client.recv_packet_from(timeout=recv_timeout)
+        with pytest.raises(ClientClosedError):
+            _ = await client_bound_or_not.recv_packet_from()
 
         # Assert
-        mock_udp_socket.settimeout.assert_not_called()
-        mock_udp_socket.recvfrom.assert_not_called()
+        mock_datagram_socket_adapter.recvfrom.assert_not_awaited()
         mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
 
-    @pytest.mark.parametrize(
-        ["recv_timeout", "recv_exception"],
-        [
-            pytest.param(0, BlockingIOError, id="null timeout"),
-            pytest.param(123456789, TimeoutError, id="strictly positive timeout"),
-        ],
-    )
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____recv_packet_from_no_block____timeout(
+    async def test____recv_packet_from____unexpected_socket_close(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        recv_timeout: int,
-        recv_exception: type[BaseException],
-        mock_udp_socket: MagicMock,
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_socket.recvfrom.side_effect = recv_exception
-
-        # Act & Assert
-        with pytest.raises(TimeoutError, match=r"^recv_packet\(\) timed out$"):
-            _ = client.recv_packet_from(timeout=recv_timeout)
-
-        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
-        mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
-
-    @pytest.mark.parametrize(
-        ["recv_timeout", "recv_exception"],
-        [
-            pytest.param(0, BlockingIOError, id="null timeout"),
-            pytest.param(123456789, TimeoutError, id="strictly positive timeout"),
-        ],
-    )
-    @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____iter_received_packets_from____yields_available_packets_with_given_timeout(
-        self,
-        client: UDPNetworkEndpoint[Any, Any],
-        sender_address: tuple[str, int],
-        recv_timeout: int,
-        recv_exception: type[BaseException],
-        mock_udp_socket: MagicMock,
-        mock_datagram_protocol: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        mock_udp_socket.recvfrom.side_effect = [
-            (b"packet_1", sender_address),
-            (b"packet_2", sender_address),
-            recv_exception,
-        ]
+        mock_datagram_socket_adapter.is_closing.return_value = True
 
         # Act
-        packets = [(p, (s.host, s.port)) for p, s in client.iter_received_packets_from(timeout=recv_timeout)]
+        with pytest.raises(ConnectionAbortedError):
+            _ = await client_bound_or_not.recv_packet_from()
 
         # Assert
-        assert mock_udp_socket.recvfrom.mock_calls == [mocker.call(MAX_DATAGRAM_BUFSIZE) for _ in range(3)]
-        assert mock_datagram_protocol.build_packet_from_datagram.mock_calls == [
-            mocker.call(b"packet_1"),
-            mocker.call(b"packet_2"),
-        ]
-        assert packets == [
-            (mocker.sentinel.packet_1, sender_address),
-            (mocker.sentinel.packet_2, sender_address),
-        ]
+        mock_datagram_socket_adapter.recvfrom.assert_not_awaited()
+        mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____iter_received_packets_from____yields_available_packets_until_error(
+    async def test____iter_received_packets_from____yields_available_packets_until_error(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_socket.recvfrom.side_effect = [
+        mock_datagram_socket_adapter.recvfrom.side_effect = [
             (b"packet_1", sender_address),
             (b"packet_2", sender_address),
             OSError,
         ]
 
         # Act
-        packets = [(p, (s.host, s.port)) for p, s in client.iter_received_packets_from(timeout=recv_timeout)]
+        packets = [(p, (s.host, s.port)) async for p, s in client_bound_or_not.iter_received_packets_from()]
 
         # Assert
-        assert mock_udp_socket.recvfrom.mock_calls == [mocker.call(MAX_DATAGRAM_BUFSIZE) for _ in range(3)]
+        assert mock_datagram_socket_adapter.recvfrom.await_args_list == [mocker.call() for _ in range(3)]
         assert mock_datagram_protocol.build_packet_from_datagram.mock_calls == [
             mocker.call(b"packet_1"),
             mocker.call(b"packet_2"),
         ]
         assert packets == [
             (mocker.sentinel.packet_1, sender_address),
             (mocker.sentinel.packet_2, sender_address),
         ]
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____iter_received_packets_from____protocol_parse_error(
+    async def test____iter_received_packets_from____protocol_parse_error(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        recv_timeout: int | None,
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mocker: MockerFixture,
     ) -> None:
         # Arrange
         from easynetwork.exceptions import DatagramProtocolParseError
 
-        mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
+        mock_datagram_socket_adapter.recvfrom.side_effect = [(b"packet", sender_address)]
         expected_error = DatagramProtocolParseError("deserialization", "Sorry")
         mock_datagram_protocol.build_packet_from_datagram.side_effect = expected_error
 
         # Act
         with pytest.raises(DatagramProtocolParseError) as exc_info:
-            _ = next(client.iter_received_packets_from(timeout=recv_timeout))
+            _ = await anext(client_bound_or_not.iter_received_packets_from())
         exception = exc_info.value
 
         # Assert
-        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_socket_adapter.recvfrom.assert_awaited_once_with()
         mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
         assert exception is expected_error
 
     @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____iter_received_packets____release_internal_lock_before_yield(
+    async def test____iter_received_packets_from____closed_client_during_iteration(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
-        mock_udp_socket: MagicMock,
+        mock_datagram_socket_adapter: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        from threading import Lock
-
-        mock_acquire = mocker.patch.object(Lock, "acquire", return_value=True)
-        mock_release = mocker.patch.object(Lock, "release", return_value=None)
-        mock_udp_socket.recvfrom.side_effect = [(b"packet_1", sender_address), (b"packet_2", sender_address)]
+        mock_datagram_socket_adapter.recvfrom.side_effect = [(b"packet_1", sender_address)]
 
         # Act & Assert
-        iterator = client.iter_received_packets_from(timeout=recv_timeout)
-        mock_acquire.assert_not_called()
-        mock_release.assert_not_called()
-        packet_1 = next(iterator)
-        mock_acquire.assert_called_once_with()
-        mock_release.assert_called_once_with()
-        mock_acquire.reset_mock()
-        mock_release.reset_mock()
-        packet_2 = next(iterator)
-        mock_acquire.assert_called_once_with()
-        mock_release.assert_called_once_with()
+        iterator = client_bound_or_not.iter_received_packets_from()
+        packet_1 = await anext(iterator)
         assert packet_1[0] is mocker.sentinel.packet_1
-        assert packet_2[0] is mocker.sentinel.packet_2
+        await client_bound_or_not.aclose()
+        assert client_bound_or_not.is_closing()
+        with pytest.raises(StopAsyncIteration):
+            _ = await anext(iterator)
 
-    @pytest.mark.usefixtures("setup_protocol_mock")
-    def test____iter_received_packets____closed_client_during_iteration(
+    async def test____get_backend____default(
         self,
-        client: UDPNetworkEndpoint[Any, Any],
-        sender_address: tuple[str, int],
-        recv_timeout: int | None,
-        mock_udp_socket: MagicMock,
-        mocker: MockerFixture,
+        client_bound_or_not: AsyncUDPNetworkEndpoint[Any, Any],
+        mock_backend: MagicMock,
     ) -> None:
         # Arrange
-        mock_udp_socket.recvfrom.side_effect = [(b"packet_1", sender_address)]
 
         # Act & Assert
-        iterator = client.iter_received_packets_from(timeout=recv_timeout)
-        packet_1 = next(iterator)
-        assert packet_1[0] is mocker.sentinel.packet_1
-        client.close()
-        assert client.is_closed()
-        with pytest.raises(StopIteration):
-            _ = next(iterator)
+        assert client_bound_or_not.get_backend() is mock_backend
+
 
+@pytest.mark.asyncio
+class TestAsyncUDPNetworkClient(BaseTestClient):
+    @pytest.fixture(scope="class", params=["AF_INET", "AF_INET6"])
+    @staticmethod
+    def socket_family(request: Any) -> Any:
+        import socket
+
+        return getattr(socket, request.param)
+
+    @pytest.fixture
+    @staticmethod
+    def remote_address() -> tuple[str, int]:
+        return ("remote_address", 5000)
 
-class TestUDPNetworkClient:
     @pytest.fixture
     @staticmethod
     def mock_udp_endpoint(mock_udp_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
-        mock = mocker.NonCallableMagicMock(spec=UDPNetworkEndpoint)
+        mock = mocker.NonCallableMagicMock(spec=AsyncUDPNetworkEndpoint)
         mock.get_local_address.return_value = ("local_address", 12345)
         mock.get_remote_address.return_value = ("remote_address", 5000)
         mock.socket = mock_udp_socket
         return mock
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def mock_udp_endpoint_cls(mocker: MockerFixture, mock_udp_endpoint: MagicMock) -> MagicMock:
-        return mocker.patch(f"{UDPNetworkEndpoint.__module__}.UDPNetworkEndpoint", return_value=mock_udp_endpoint)
+        return mocker.patch(f"{AsyncUDPNetworkEndpoint.__module__}.AsyncUDPNetworkEndpoint", return_value=mock_udp_endpoint)
 
     @pytest.fixture
     @staticmethod
     def client(
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
-    ) -> UDPNetworkClient[Any, Any]:
-        return UDPNetworkClient(
-            mock_udp_socket,
-            mock_datagram_protocol,
-            give=False,
-        )
+    ) -> AsyncUDPNetworkClient[Any, Any]:
+        return AsyncUDPNetworkClient(mock_udp_socket, mock_datagram_protocol)
+
+    @pytest.fixture(autouse=True)
+    @staticmethod
+    def set_default_socket_mock_configuration(
+        mock_udp_socket: MagicMock,
+    ) -> None:
+        mock_udp_socket.getsockname.return_value = ("local_address", 12345)
+        mock_udp_socket.getpeername.return_value = ("remote_address", 5000)
 
-    def test____dunder_init____with_remote_address(
+    async def test____dunder_init____with_remote_address(
         self,
+        remote_address: tuple[str, int],
+        socket_family: int,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
         mock_udp_endpoint_cls: MagicMock,
-        mock_udp_endpoint: MagicMock,
+        mock_backend: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        remote_address = ("remote_address", 5000)
 
         # Act
-        client: UDPNetworkClient[Any, Any] = UDPNetworkClient(
+        client: AsyncUDPNetworkClient[Any, Any] = AsyncUDPNetworkClient(
             remote_address,
             mock_datagram_protocol,
-            family=mocker.sentinel.family,
-            source_address=mocker.sentinel.source_address,
+            family=socket_family,
+            local_address=mocker.sentinel.local_address,
+            reuse_port=mocker.sentinel.reuse_port,
+            backend=mock_backend,
+            backend_kwargs={"arg1": 1, "arg2": "2"},
         )
 
         # Assert
         mock_udp_endpoint_cls.assert_called_once_with(
             protocol=mock_datagram_protocol,
+            family=socket_family,
             remote_address=remote_address,
-            family=mocker.sentinel.family,
-            source_address=mocker.sentinel.source_address,
+            local_address=mocker.sentinel.local_address,
+            reuse_port=mocker.sentinel.reuse_port,
+            backend=mock_backend,
+            backend_kwargs={"arg1": 1, "arg2": "2"},
         )
-        mock_udp_endpoint.get_remote_address.assert_called_once_with()
         assert client.socket is mock_udp_socket
 
-    def test____dunder_init____with_socket(
+    async def test____dunder_init____use_given_socket(
         self,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
         mock_udp_endpoint_cls: MagicMock,
-        mock_udp_endpoint: MagicMock,
-        mocker: MockerFixture,
+        mock_backend: MagicMock,
     ) -> None:
         # Arrange
 
         # Act
-        client: UDPNetworkClient[Any, Any] = UDPNetworkClient(
+        client: AsyncUDPNetworkClient[Any, Any] = AsyncUDPNetworkClient(
             mock_udp_socket,
             mock_datagram_protocol,
-            give=mocker.sentinel.give_ownership,
+            backend=mock_backend,
+            backend_kwargs={"arg1": 1, "arg2": "2"},
         )
 
         # Assert
         mock_udp_endpoint_cls.assert_called_once_with(
             protocol=mock_datagram_protocol,
             socket=mock_udp_socket,
-            give=mocker.sentinel.give_ownership,
+            backend=mock_backend,
+            backend_kwargs={"arg1": 1, "arg2": "2"},
         )
-        mock_udp_endpoint.get_remote_address.assert_called_once_with()
         assert client.socket is mock_udp_socket
 
-    def test____dunder_init____error_no_remote_address(
+    async def test____dunder_init____error_no_remote_address(
         self,
+        mock_backend: MagicMock,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
-        mock_udp_endpoint: MagicMock,
-        mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_endpoint.get_remote_address.return_value = None
+        self.configure_socket_mock_to_raise_ENOTCONN(mock_udp_socket)
 
         # Act & Assert
         with pytest.raises(OSError, match=r"^No remote address configured$"):
-            _ = UDPNetworkClient(
-                mock_udp_socket,
-                mock_datagram_protocol,
-                give=mocker.sentinel.give_ownership,
-            )
-        mock_udp_endpoint.close.assert_called_once_with()
+            _ = AsyncUDPNetworkClient(mock_udp_socket, mock_datagram_protocol, backend=mock_backend)
 
-    def test____is_closed____default(
+    async def test____is_closing____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_endpoint.is_closed.return_value = mocker.sentinel.status
+        mock_udp_endpoint.is_closing.return_value = mocker.sentinel.status
 
         # Act
-        status = client.is_closed()
+        status = client.is_closing()
 
         # Assert
-        mock_udp_endpoint.is_closed.assert_called_once_with()
+        mock_udp_endpoint.is_closing.assert_called_once_with()
         assert status is mocker.sentinel.status
 
-    def test____close____default(
+    async def test____is_connected____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
     ) -> None:
         # Arrange
-        mock_udp_endpoint.close.return_value = None
+        mock_udp_endpoint.is_bound.return_value = True
 
         # Act
-        client.close()
+        status = client.is_connected()
 
         # Assert
-        mock_udp_endpoint.close.assert_called_once_with()
+        mock_udp_endpoint.is_bound.assert_called_once_with()
+        assert status is True
 
-    def test____get_local_address____default(
+    async def test____wait_connected____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.wait_bound.return_value = None
+
+        # Act
+        await client.wait_connected()
+
+        # Assert
+        mock_udp_endpoint.wait_bound.assert_awaited_once_with()
+
+    async def test____aclose____default(
+        self,
+        client: AsyncUDPNetworkClient[Any, Any],
+        mock_udp_endpoint: MagicMock,
+    ) -> None:
+        # Arrange
+        mock_udp_endpoint.aclose.return_value = None
+
+        # Act
+        await client.aclose()
+
+        # Assert
+        mock_udp_endpoint.aclose.assert_awaited_once_with()
+
+    async def test____get_local_address____default(
+        self,
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
     ) -> None:
         # Arrange
 
         # Act
         address = client.get_local_address()
 
         # Assert
         mock_udp_endpoint.get_local_address.assert_called_once_with()
         assert address == ("local_address", 12345)
 
-    def test____get_remote_address____default(
+    async def test____get_remote_address____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
     ) -> None:
         # Arrange
-        ## NOTE: The client should have the remote address saved. Therefore this test check if there is no new call.
-        mock_udp_endpoint.get_remote_address.assert_called_once()
 
         # Act
         address = client.get_remote_address()
 
         # Assert
         mock_udp_endpoint.get_remote_address.assert_called_once()
         assert address == ("remote_address", 5000)
 
-    def test____send_packet____default(
+    async def test____send_packet____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_udp_endpoint.send_packet_to.return_value = None
 
         # Act
-        client.send_packet(mocker.sentinel.packet)
+        await client.send_packet(mocker.sentinel.packet)
 
         # Assert
-        mock_udp_endpoint.send_packet_to.assert_called_once_with(mocker.sentinel.packet, None)
+        mock_udp_endpoint.send_packet_to.assert_awaited_once_with(mocker.sentinel.packet, None)
 
-    def test____recv_packet____default(
+    async def test____recv_packet____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_udp_endpoint.recv_packet_from.return_value = (mocker.sentinel.packet, ("remote_address", 5000))
 
         # Act
-        packet = client.recv_packet(timeout=mocker.sentinel.timeout)
+        packet = await client.recv_packet()
 
         # Assert
-        mock_udp_endpoint.recv_packet_from.assert_called_once_with(timeout=mocker.sentinel.timeout)
+        mock_udp_endpoint.recv_packet_from.assert_awaited_once_with()
         assert packet is mocker.sentinel.packet
 
-    def test____recv_packet____timeout_error(
+    async def test____iter_received_packets____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_endpoint.recv_packet_from.side_effect = TimeoutError("recv_packet() timed out")
+        async def side_effect() -> Any:
+            yield (mocker.sentinel.packet_1, ("remote_address", 5000))
+            yield (mocker.sentinel.packet_2, ("remote_address", 5000))
+            yield (mocker.sentinel.packet_3, ("remote_address", 5000))
+
+        mock_udp_endpoint.iter_received_packets_from.side_effect = side_effect
 
         # Act
-        with pytest.raises(TimeoutError) as exc_info:
-            _ = client.recv_packet(timeout=mocker.sentinel.timeout)
-        exception = exc_info.value
+        packets = [p async for p in client.iter_received_packets()]
 
         # Assert
-        mock_udp_endpoint.recv_packet_from.assert_called_once_with(timeout=mocker.sentinel.timeout)
-        assert exception is mock_udp_endpoint.recv_packet_from.side_effect
+        mock_udp_endpoint.iter_received_packets_from.assert_called_once_with()
+        assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2, mocker.sentinel.packet_3]
 
-    def test____iter_received_packets____default(
+    async def test____fileno____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_endpoint.iter_received_packets_from.side_effect = lambda timeout: iter(
-            [
-                (mocker.sentinel.packet_1, ("remote_address", 5000)),
-                (mocker.sentinel.packet_2, ("remote_address", 5000)),
-                (mocker.sentinel.packet_3, ("remote_address", 5000)),
-            ]
-        )
+        mock_udp_endpoint.fileno.return_value = mocker.sentinel.fd
 
         # Act
-        packets = list(client.iter_received_packets(timeout=mocker.sentinel.timeout))
+        fd = client.fileno()
 
         # Assert
-        mock_udp_endpoint.iter_received_packets_from.assert_called_once_with(timeout=mocker.sentinel.timeout)
-        assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2, mocker.sentinel.packet_3]
+        mock_udp_endpoint.fileno.assert_called_once_with()
+        assert fd is mocker.sentinel.fd
 
-    def test____fileno____default(
+    async def test____get_backend____default(
         self,
-        client: UDPNetworkClient[Any, Any],
+        client: AsyncUDPNetworkClient[Any, Any],
         mock_udp_endpoint: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        mock_udp_endpoint.fileno.return_value = mocker.sentinel.fd
+        mock_udp_endpoint.get_backend.return_value = mocker.sentinel.backend
 
         # Act
-        fd = client.fileno()
+        backend = client.get_backend()
 
         # Assert
-        mock_udp_endpoint.fileno.assert_called_once_with()
-        assert fd is mocker.sentinel.fd
+        mock_udp_endpoint.get_backend.assert_called_once_with()
+        assert backend is mocker.sentinel.backend
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/base.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/base.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_abc.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         mock_incremental_deserialize_func: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer = _IncrementalPacketSerializerForTest()
         mock_consumer_generator: MagicMock = mock_incremental_deserialize_func.return_value
         mock_consumer_generator.__next__.return_value = None
-        mock_consumer_generator.send.side_effect = StopIteration((mocker.sentinel.packet, b""))
+        mock_consumer_generator.send.side_effect = [StopIteration((mocker.sentinel.packet, b""))]
 
         # Act
         packet = serializer.deserialize(mocker.sentinel.data)
 
         # Assert
         mock_incremental_deserialize_func.assert_called_once_with()
         mock_consumer_generator.__next__.assert_called_once_with()
@@ -160,24 +160,22 @@
 
     @pytest.fixture
     @staticmethod
     def mock_deserialize_func(mocker: MockerFixture) -> MagicMock:
         return mocker.patch.object(_AutoSeparatedPacketSerializerForTest, "deserialize")
 
     @pytest.mark.parametrize("separator", [b"\n", b".", b"\r\n", b"--"], ids=lambda p: f"separator=={p}")
-    @pytest.mark.parametrize("keepends", [False, True], ids=lambda p: f"keepends=={p}")
-    def test____properties____right_values(self, separator: bytes, keepends: bool) -> None:
+    def test____properties____right_values(self, separator: bytes) -> None:
         # Arrange
 
         # Act
-        serializer = _AutoSeparatedPacketSerializerForTest(separator=separator, keepends=keepends)
+        serializer = _AutoSeparatedPacketSerializerForTest(separator=separator)
 
         # Assert
         assert serializer.separator == separator
-        assert serializer.keepends == keepends
 
     def test____dunder_init____empty_separator_bytes(self) -> None:
         # Arrange
 
         # Act & Assert
         with pytest.raises(ValueError, match=r"^Empty separator$"):
             _ = _AutoSeparatedPacketSerializerForTest(b"")
@@ -268,26 +266,24 @@
             pytest.param(b"", id="without remaining data"),
             pytest.param(b"remaining", id="with remaining data"),
             pytest.param(b"remaining\r\nother", id="with remaining data including separator"),
         ],
     )
     @pytest.mark.parametrize("several_trailing_separators", [False, True], ids=lambda b: f"several_trailing_separators=={b}")
     @pytest.mark.parametrize("several_leading_separators", [False, True], ids=lambda b: f"several_leading_separators=={b}")
-    @pytest.mark.parametrize("keepends", [False, True], ids=lambda b: f"keepends=={b}")
     def test____incremental_deserialize____one_shot_chunk(
         self,
         expected_remaining_data: bytes,
         several_trailing_separators: bool,
         several_leading_separators: bool,
-        keepends: bool,
         mock_deserialize_func: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
-        serializer = _AutoSeparatedPacketSerializerForTest(separator=b"\r\n", keepends=keepends)
+        serializer = _AutoSeparatedPacketSerializerForTest(separator=b"\r\n")
         mock_deserialize_func.return_value = mocker.sentinel.packet
         data_to_test: bytes = b"data\r\n"
         if several_trailing_separators:
             data_to_test = data_to_test + b"\r\n\r\n\r\n"
         if several_leading_separators:
             data_to_test = b"\r\n\r\n\r\n" + data_to_test
 
@@ -295,18 +291,15 @@
         consumer = serializer.incremental_deserialize()
         next(consumer)
         with pytest.raises(StopIteration) as exc_info:
             consumer.send(data_to_test + expected_remaining_data)
         packet, remaining_data = exc_info.value.value
 
         # Assert
-        if not keepends:
-            mock_deserialize_func.assert_called_once_with(b"data")
-        else:
-            mock_deserialize_func.assert_called_once_with(b"data\r\n")
+        mock_deserialize_func.assert_called_once_with(b"data")
         assert remaining_data == expected_remaining_data
         assert packet is mocker.sentinel.packet
 
     @pytest.mark.parametrize(
         "expected_remaining_data",
         [
             pytest.param(b"", id="without remaining data"),
@@ -581,52 +574,14 @@
         # Act
         data = serializer.serialize(mocker.sentinel.packet)
 
         # Assert
         mock_dump_to_file_func.assert_called_once_with(mocker.sentinel.packet, mocker.ANY)
         assert data == b"success"
 
-    def test____incremental_serialize____dump_to_file(
-        self,
-        mock_dump_to_file_func: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        def side_effect(_: Any, file: IO[bytes]) -> None:
-            file.write(b"success")
-
-        serializer = _FileBasedPacketSerializerForTest(expected_load_error=())
-        mock_dump_to_file_func.side_effect = side_effect
-
-        # Act
-        data = list(serializer.incremental_serialize(mocker.sentinel.packet))
-
-        # Assert
-        mock_dump_to_file_func.assert_called_once_with(mocker.sentinel.packet, mocker.ANY)
-        assert data == [b"success"]
-
-    def test____incremental_serialize____does_not_yield_if_there_is_no_data(
-        self,
-        mock_dump_to_file_func: MagicMock,
-        mocker: MockerFixture,
-    ) -> None:
-        # Arrange
-        def side_effect(_: Any, file: IO[bytes]) -> None:
-            pass
-
-        serializer = _FileBasedPacketSerializerForTest(expected_load_error=())
-        mock_dump_to_file_func.side_effect = side_effect
-
-        # Act
-        data = list(serializer.incremental_serialize(mocker.sentinel.packet))
-
-        # Assert
-        mock_dump_to_file_func.assert_called_once_with(mocker.sentinel.packet, mocker.ANY)
-        assert data == []
-
     def test____deserialize____load_from_file(
         self,
         mock_load_from_file_func: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         def side_effect(file: IO[bytes]) -> Any:
@@ -656,14 +611,15 @@
         with pytest.raises(DeserializeError, match=r"^Missing data to create packet$") as exc_info:
             _ = serializer.deserialize(b"data")
         exception = exc_info.value
 
         # Assert
         mock_load_from_file_func.assert_called_once_with(mocker.ANY)
         assert exception.__cause__ is mock_load_from_file_func.side_effect
+        assert exception.error_info == {"data": b"data"}
 
     @pytest.mark.parametrize("give_as_tuple", [False, True], ids=lambda boolean: f"give_as_tuple=={boolean}")
     def test____deserialize____translate_given_exceptions(
         self,
         give_as_tuple: bool,
         mock_load_from_file_func: MagicMock,
         mocker: MockerFixture,
@@ -685,14 +641,15 @@
         with pytest.raises(DeserializeError) as exc_info:
             _ = serializer.deserialize(b"data")
         exception = exc_info.value
 
         # Assert
         mock_load_from_file_func.assert_called_once_with(mocker.ANY)
         assert exception.__cause__ is mock_load_from_file_func.side_effect
+        assert exception.error_info == {"data": b"data"}
 
     def test____deserialize____with_remaining_data_to_read(
         self,
         mock_load_from_file_func: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
@@ -700,19 +657,59 @@
             assert file.read(2) == b"da"
             return mocker.sentinel.packet
 
         serializer = _FileBasedPacketSerializerForTest(expected_load_error=())
         mock_load_from_file_func.side_effect = side_effect
 
         # Act
-        with pytest.raises(DeserializeError, match=r"^Extra data caught$"):
+        with pytest.raises(DeserializeError, match=r"^Extra data caught$") as exc_info:
             _ = serializer.deserialize(b"data")
+        exception = exc_info.value
 
         # Assert
         mock_load_from_file_func.assert_called_once_with(mocker.ANY)
+        assert exception.error_info == {"packet": mocker.sentinel.packet, "extra": b"ta"}
+
+    def test____incremental_serialize____dump_to_file(
+        self,
+        mock_dump_to_file_func: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        def side_effect(_: Any, file: IO[bytes]) -> None:
+            file.write(b"success")
+
+        serializer = _FileBasedPacketSerializerForTest(expected_load_error=())
+        mock_dump_to_file_func.side_effect = side_effect
+
+        # Act
+        data = list(serializer.incremental_serialize(mocker.sentinel.packet))
+
+        # Assert
+        mock_dump_to_file_func.assert_called_once_with(mocker.sentinel.packet, mocker.ANY)
+        assert data == [b"success"]
+
+    def test____incremental_serialize____does_not_yield_if_there_is_no_data(
+        self,
+        mock_dump_to_file_func: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        def side_effect(_: Any, file: IO[bytes]) -> None:
+            pass
+
+        serializer = _FileBasedPacketSerializerForTest(expected_load_error=())
+        mock_dump_to_file_func.side_effect = side_effect
+
+        # Act
+        data = list(serializer.incremental_serialize(mocker.sentinel.packet))
+
+        # Assert
+        mock_dump_to_file_func.assert_called_once_with(mocker.sentinel.packet, mocker.ANY)
+        assert data == []
 
     def test____incremental_deserialize____load_from_file____read_all(
         self,
         mock_load_from_file_func: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
@@ -830,7 +827,8 @@
         with pytest.raises(IncrementalDeserializeError) as exc_info:  # There is new data and error still here
             consumer.send(b"other")
         exception = exc_info.value
 
         # Assert
         assert exception.remaining_data == b"other"
         assert type(exception.__cause__) is MyFileAPIValueError
+        assert exception.error_info == {"data": b"dataother"}
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_base64.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_base64.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_cbor.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_cbor.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
     from pytest_mock import MockerFixture
 
 
 @final
+@pytest.mark.feature_cbor
 class TestCBORSerializer(BaseSerializerConfigInstanceCheck):
     @pytest.fixture(scope="class")
     @staticmethod
     def serializer_cls() -> type[CBORSerializer[Any, Any]]:
         return CBORSerializer
 
     @pytest.fixture(params=["encoder", "decoder"])
@@ -28,45 +29,41 @@
     def config_param(request: Any) -> tuple[str, str]:
         name: str = request.param
         return (name, f"CBOR{name.capitalize()}Config")
 
     @pytest.fixture
     @staticmethod
     def mock_encoder(mocker: MockerFixture) -> MagicMock:
-        from io import BytesIO
-
         from cbor2 import CBOREncoder
 
-        return mocker.MagicMock(spec=CBOREncoder(BytesIO()))
+        return mocker.NonCallableMagicMock(spec=CBOREncoder)
 
     @pytest.fixture
     @staticmethod
     def mock_encoder_cls(mocker: MockerFixture, mock_encoder: MagicMock) -> MagicMock:
         return mocker.patch("cbor2.CBOREncoder", autospec=True, return_value=mock_encoder)
 
     @pytest.fixture
     @staticmethod
     def mock_decoder(mocker: MockerFixture) -> MagicMock:
-        from io import BytesIO
-
         from cbor2 import CBORDecoder
 
-        return mocker.MagicMock(spec=CBORDecoder(BytesIO()))
+        return mocker.NonCallableMagicMock(spec=CBORDecoder)
 
     @pytest.fixture
     @staticmethod
     def mock_decoder_cls(mocker: MockerFixture, mock_decoder: MagicMock) -> MagicMock:
         return mocker.patch("cbor2.CBORDecoder", autospec=True, return_value=mock_decoder)
 
     @pytest.fixture
     @staticmethod
     def mock_file(mocker: MockerFixture) -> MagicMock:
         from io import BytesIO
 
-        return mocker.MagicMock(spec=BytesIO())
+        return mocker.NonCallableMagicMock(spec=BytesIO)
 
     @pytest.fixture(params=[True, False], ids=lambda boolean: f"default_encoder_config=={boolean}")
     @staticmethod
     def encoder_config(request: Any, mocker: MockerFixture) -> CBOREncoderConfig | None:
         use_default_config: bool = request.param
         if use_default_config:
             return None
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_compressor.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_compressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,63 +179,72 @@
         # Assert
         mock_serializer_new_decompressor_stream.assert_called_once_with()
         mock_decompressor_stream.decompress.assert_called_once_with(mocker.sentinel.data)
         mock_decompressor_stream_eof.assert_not_called()
         mock_decompressor_stream_unused_data.assert_not_called()
         mock_serializer.deserialize.assert_not_called()
         assert exception.__cause__ is mock_decompressor_stream.decompress.side_effect
+        assert exception.error_info == {"data": mocker.sentinel.data}
 
     def test____deserialize____missing_data(
         self,
         mock_serializer: MagicMock,
         mock_serializer_new_decompressor_stream: MagicMock,
         mock_decompressor_stream: MagicMock,
         mock_decompressor_stream_eof: MagicMock,
         mock_decompressor_stream_unused_data: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer = _CompressorSerializerForTest(mock_serializer, ())
+        mock_decompressor_stream.decompress.return_value = mocker.sentinel.decompressed_data
         mock_decompressor_stream_eof.return_value = False
 
         # Act
-        with pytest.raises(DeserializeError, match=r"^Compressed data ended before the end-of-stream marker was reached$"):
+        with pytest.raises(
+            DeserializeError, match=r"^Compressed data ended before the end-of-stream marker was reached$"
+        ) as exc_info:
             _ = serializer.deserialize(mocker.sentinel.data)
+        exception = exc_info.value
 
         # Assert
         mock_serializer_new_decompressor_stream.assert_called_once_with()
         mock_decompressor_stream.decompress.assert_called_once_with(mocker.sentinel.data)
         mock_decompressor_stream_eof.assert_called_once()
         mock_decompressor_stream_unused_data.assert_not_called()
         mock_serializer.deserialize.assert_not_called()
+        assert exception.error_info == {"already_decompressed_data": mocker.sentinel.decompressed_data}
 
     def test____deserialize____extra_data(
         self,
         mock_serializer: MagicMock,
         mock_serializer_new_decompressor_stream: MagicMock,
         mock_decompressor_stream: MagicMock,
         mock_decompressor_stream_eof: MagicMock,
         mock_decompressor_stream_unused_data: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer = _CompressorSerializerForTest(mock_serializer, ())
+        mock_decompressor_stream.decompress.return_value = mocker.sentinel.decompressed_data
         mock_decompressor_stream_eof.return_value = True
         mock_decompressor_stream_unused_data.return_value = b"some extra data"
 
         # Act
-        with pytest.raises(DeserializeError, match=r"^Trailing data error$"):
+        with pytest.raises(DeserializeError, match=r"^Trailing data error$") as exc_info:
             _ = serializer.deserialize(mocker.sentinel.data)
+        exception = exc_info.value
 
         # Assert
         mock_serializer_new_decompressor_stream.assert_called_once_with()
         mock_decompressor_stream.decompress.assert_called_once_with(mocker.sentinel.data)
         mock_decompressor_stream_eof.assert_called_once()
         mock_decompressor_stream_unused_data.assert_called_once()
         mock_serializer.deserialize.assert_not_called()
+        assert exception.error_info == {"decompressed_data": mocker.sentinel.decompressed_data, "extra": b"some extra data"}
 
     def test____incremental_deserialize____decompress_chunks(
         self,
         mock_serializer: MagicMock,
         mock_serializer_new_decompressor_stream: MagicMock,
         mock_decompressor_stream: MagicMock,
         mock_decompressor_stream_eof: MagicMock,
@@ -273,14 +282,16 @@
         mock_serializer: MagicMock,
         mock_serializer_new_decompressor_stream: MagicMock,
         mock_decompressor_stream: MagicMock,
         mock_decompressor_stream_eof: MagicMock,
         mock_decompressor_stream_unused_data: MagicMock,
     ) -> None:
         # Arrange
+        from collections import deque
+
         class MyStreamAPIBaseException(Exception):
             pass
 
         class MyStreamAPIValueError(MyStreamAPIBaseException, ValueError):
             pass
 
         if give_as_tuple:
@@ -301,14 +312,18 @@
         mock_serializer_new_decompressor_stream.assert_called_once_with()
         mock_decompressor_stream.decompress.assert_called_once_with(b"chunk")
         mock_decompressor_stream_eof.assert_called_once()
         mock_decompressor_stream_unused_data.assert_not_called()
         mock_serializer.deserialize.assert_not_called()
         assert exception.__cause__ is mock_decompressor_stream.decompress.side_effect
         assert exception.remaining_data == b""
+        assert exception.error_info == {
+            "already_decompressed_chunks": deque([]),
+            "invalid_chunk": b"chunk",
+        }
 
     def test____incremental_deserialize____translate_deserialize_errors(
         self,
         mock_serializer: MagicMock,
         mock_serializer_new_decompressor_stream: MagicMock,
         mock_decompressor_stream: MagicMock,
         mock_decompressor_stream_eof: MagicMock,
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_encryptor.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_encryptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
     from pytest_mock import MockerFixture
 
 
+@pytest.mark.feature_encryption
 class TestEncryptorSerializer:
     @pytest.fixture
     @staticmethod
     def mock_fernet(mocker: MockerFixture) -> MagicMock:
         from cryptography.fernet import Fernet
 
-        return mocker.MagicMock(spec=Fernet)
+        return mocker.NonCallableMagicMock(spec=Fernet)
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def mock_fernet_cls(mocker: MockerFixture, mock_fernet: MagicMock) -> MagicMock:
         return mocker.patch("cryptography.fernet.Fernet", return_value=mock_fernet)
 
     @pytest.mark.parametrize("method", ["incremental_serialize", "incremental_deserialize"])
@@ -114,7 +115,8 @@
         exception = exc_info.value
 
         # Assert
         mock_fernet.decrypt.assert_called_once_with(mocker.sentinel.encrypted_data, ttl=mocker.sentinel.token_ttl)
         mock_serializer.deserialize.assert_not_called()
         assert exception.__context__ is mock_fernet.decrypt.side_effect
         assert exception.__cause__ is None
+        assert exception.error_info is None
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_json.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,27 @@
         return (name, f"JSON{name.capitalize()}Config")
 
     @pytest.fixture
     @staticmethod
     def mock_encoder(mocker: MockerFixture) -> MagicMock:
         from json import JSONEncoder
 
-        return mocker.MagicMock(spec=JSONEncoder)
+        return mocker.NonCallableMagicMock(spec=JSONEncoder)
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def mock_encoder_cls(mocker: MockerFixture, mock_encoder: MagicMock) -> MagicMock:
         return mocker.patch("json.JSONEncoder", return_value=mock_encoder)
 
     @pytest.fixture
     @staticmethod
     def mock_decoder(mocker: MockerFixture) -> MagicMock:
         from json import JSONDecoder
 
-        return mocker.MagicMock(spec=JSONDecoder)
+        return mocker.NonCallableMagicMock(spec=JSONDecoder)
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def mock_decoder_cls(mocker: MockerFixture, mock_decoder: MagicMock) -> MagicMock:
         return mocker.patch("json.JSONDecoder", return_value=mock_decoder)
 
     @pytest.fixture(params=[True, False], ids=lambda boolean: f"default_encoder_config=={boolean}")
@@ -137,17 +137,17 @@
         self,
         mock_encoder: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer: JSONSerializer[Any, Any] = JSONSerializer(
             encoding=mocker.sentinel.encoding,
-            str_errors=mocker.sentinel.str_errors,
+            unicode_errors=mocker.sentinel.str_errors,
         )
-        mock_string = mock_encoder.encode.return_value = mocker.MagicMock()
+        mock_string = mock_encoder.encode.return_value = mocker.NonCallableMagicMock()
         mock_string.encode.return_value = mocker.sentinel.data
 
         # Act
         data = serializer.serialize(mocker.sentinel.packet)
 
         # Assert
         mock_encoder.encode.assert_called_once_with(mocker.sentinel.packet)
@@ -158,19 +158,19 @@
         self,
         mock_encoder: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer: JSONSerializer[Any, Any] = JSONSerializer(
             encoding=mocker.sentinel.encoding,
-            str_errors=mocker.sentinel.str_errors,
+            unicode_errors=mocker.sentinel.str_errors,
         )
-        chunk_a = mocker.MagicMock(**{"encode.return_value": mocker.sentinel.chunk_a})
-        chunk_b = mocker.MagicMock(**{"encode.return_value": mocker.sentinel.chunk_b})
-        chunk_c = mocker.MagicMock(**{"encode.return_value": mocker.sentinel.chunk_c})
+        chunk_a = mocker.NonCallableMagicMock(**{"encode.return_value": mocker.sentinel.chunk_a})
+        chunk_b = mocker.NonCallableMagicMock(**{"encode.return_value": mocker.sentinel.chunk_b})
+        chunk_c = mocker.NonCallableMagicMock(**{"encode.return_value": mocker.sentinel.chunk_c})
         mock_encoder.iterencode.return_value = iter([chunk_a, chunk_b, chunk_c])
 
         # Act & Assert
         generator = serializer.incremental_serialize(mocker.sentinel.packet)
         first_chunk = next(generator)
         chunk_a.encode.assert_called_once_with(mocker.sentinel.encoding, mocker.sentinel.str_errors)
         assert first_chunk is mocker.sentinel.chunk_a
@@ -195,17 +195,17 @@
         self,
         mock_decoder: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer: JSONSerializer[Any, Any] = JSONSerializer(
             encoding=mocker.sentinel.encoding,
-            str_errors=mocker.sentinel.str_errors,
+            unicode_errors=mocker.sentinel.str_errors,
         )
-        mock_bytes = mocker.MagicMock()
+        mock_bytes = mocker.NonCallableMagicMock()
         mock_bytes.decode.return_value = mocker.sentinel.document
         mock_decoder.decode.return_value = mocker.sentinel.packet
 
         # Act
         packet = serializer.deserialize(mock_bytes)
 
         # Assert
@@ -216,48 +216,55 @@
     def test____deserialize____translate_unicode_decode_errors(
         self,
         mock_decoder: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         serializer: JSONSerializer[Any, Any] = JSONSerializer()
-        mock_bytes = mocker.MagicMock()
+        mock_bytes = mocker.NonCallableMagicMock()
         mock_bytes.decode.side_effect = UnicodeDecodeError("some encoding", b"invalid data", 0, 2, "Bad encoding ?")
 
         # Act
         with pytest.raises(DeserializeError) as exc_info:
             _ = serializer.deserialize(mock_bytes)
         exception = exc_info.value
 
         # Assert
         mock_bytes.decode.assert_called_once()
         mock_decoder.decode.assert_not_called()
         assert exception.__cause__ is mock_bytes.decode.side_effect
+        assert exception.error_info == {"data": mock_bytes}
 
     def test____deserialize____translate_json_decode_errors(
         self,
         mock_decoder: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from json import JSONDecodeError
 
         serializer: JSONSerializer[Any, Any] = JSONSerializer()
-        mock_bytes = mocker.MagicMock()
-        mock_decoder.decode.side_effect = JSONDecodeError("Invalid payload", "document", 0)
+        mock_bytes = mocker.NonCallableMagicMock()
+        mock_decoder.decode.side_effect = JSONDecodeError("Invalid payload", "invalid\ndocument", 8)
 
         # Act
         with pytest.raises(DeserializeError) as exc_info:
             _ = serializer.deserialize(mock_bytes)
         exception = exc_info.value
 
         # Assert
         mock_bytes.decode.assert_called_once()
         mock_decoder.decode.assert_called_once()
         assert exception.__cause__ is mock_decoder.decode.side_effect
+        assert exception.error_info == {
+            "document": "invalid\ndocument",
+            "position": 8,
+            "lineno": 2,
+            "colno": 1,
+        }
 
     def test____incremental_deserialize____parse_and_decode_data(
         self,
         mock_decoder: MagicMock,
         mock_json_parser: MagicMock,
         mocker: MockerFixture,
     ) -> None:
@@ -265,19 +272,19 @@
         def raw_parse_side_effect() -> Generator[None, bytes, tuple[bytes, bytes]]:
             data = yield
             assert data is mocker.sentinel.data
             return mock_bytes, b"Hello World !"
 
         serializer: JSONSerializer[Any, Any] = JSONSerializer(
             encoding=mocker.sentinel.encoding,
-            str_errors=mocker.sentinel.str_errors,
+            unicode_errors=mocker.sentinel.str_errors,
         )
-        mock_bytes = mocker.MagicMock()
-        mock_string_document = mock_bytes.decode.return_value = mocker.MagicMock()
-        mock_sliced_string = mock_string_document.__getitem__.return_value = mocker.MagicMock()
+        mock_bytes = mocker.NonCallableMagicMock()
+        mock_string_document = mock_bytes.decode.return_value = mocker.NonCallableMagicMock()
+        mock_sliced_string = mock_string_document.__getitem__.return_value = mocker.NonCallableMagicMock()
         mock_sliced_string.encode.return_value = b"Trailing data + "
         mock_decoder.raw_decode.return_value = mocker.sentinel.packet, 123456789
         mock_json_parser.side_effect = raw_parse_side_effect
 
         # Act
         consumer = serializer.incremental_deserialize()
         next(consumer)
@@ -302,17 +309,17 @@
         def raw_parse_side_effect() -> Generator[None, bytes, tuple[bytes, bytes]]:
             data = yield
             assert data is mocker.sentinel.data
             return mock_bytes, mocker.sentinel.remaining_data
 
         serializer: JSONSerializer[Any, Any] = JSONSerializer(
             encoding=mocker.sentinel.encoding,
-            str_errors=mocker.sentinel.str_errors,
+            unicode_errors=mocker.sentinel.str_errors,
         )
-        mock_bytes = mocker.MagicMock()
+        mock_bytes = mocker.NonCallableMagicMock()
         mock_bytes.decode.side_effect = UnicodeDecodeError("some encoding", b"invalid data", 0, 2, "Bad encoding ?")
         mock_json_parser.side_effect = raw_parse_side_effect
 
         # Act
         consumer = serializer.incremental_deserialize()
         next(consumer)
         with pytest.raises(IncrementalDeserializeError) as exc_info:
@@ -320,14 +327,15 @@
         exception = exc_info.value
 
         # Assert
         mock_bytes.decode.assert_called_once()
         mock_decoder.raw_decode.assert_not_called()
         assert exception.remaining_data is mocker.sentinel.remaining_data
         assert exception.__cause__ is mock_bytes.decode.side_effect
+        assert exception.error_info == {"data": mock_bytes}
 
     def test____incremental_deserialize____translate_json_decode_errors(
         self,
         mock_decoder: MagicMock,
         mock_json_parser: MagicMock,
         mocker: MockerFixture,
     ) -> None:
@@ -337,25 +345,31 @@
         def raw_parse_side_effect() -> Generator[None, bytes, tuple[bytes, bytes]]:
             data = yield
             assert data is mocker.sentinel.data
             return mock_bytes, mocker.sentinel.remaining_data
 
         serializer: JSONSerializer[Any, Any] = JSONSerializer(
             encoding=mocker.sentinel.encoding,
-            str_errors=mocker.sentinel.str_errors,
+            unicode_errors=mocker.sentinel.str_errors,
         )
-        mock_bytes = mocker.MagicMock()
-        mock_decoder.raw_decode.side_effect = JSONDecodeError("Invalid payload", "document", 0)
+        mock_bytes = mocker.NonCallableMagicMock()
+        mock_decoder.raw_decode.side_effect = JSONDecodeError("Invalid payload", "invalid\ndocument", 8)
         mock_json_parser.side_effect = raw_parse_side_effect
 
         # Act
         consumer = serializer.incremental_deserialize()
         next(consumer)
         with pytest.raises(IncrementalDeserializeError) as exc_info:
             _ = consumer.send(mocker.sentinel.data)
         exception = exc_info.value
 
         # Assert
         mock_bytes.decode.assert_called_once()
         mock_decoder.raw_decode.assert_called_once()
         assert exception.remaining_data is mocker.sentinel.remaining_data
         assert exception.__cause__ is mock_decoder.raw_decode.side_effect
+        assert exception.error_info == {
+            "document": "invalid\ndocument",
+            "position": 8,
+            "lineno": 2,
+            "colno": 1,
+        }
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_serializers/test_struct.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_serializers/test_struct.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 class BaseTestStructBasedSerializer:
     @pytest.fixture
     @staticmethod
     def mock_struct(mocker: MockerFixture) -> MagicMock:
         from struct import Struct
 
-        mock = mocker.MagicMock(spec=Struct)
+        mock = mocker.NonCallableMagicMock(spec=Struct)
         mock.size = 123456789
         return mock
 
     @pytest.fixture(autouse=True)
     @staticmethod
     def mock_struct_cls(mocker: MockerFixture, mock_struct: MagicMock) -> MagicMock:
         return mocker.patch("struct.Struct", return_value=mock_struct)
@@ -141,14 +141,15 @@
             _ = serializer.deserialize(mocker.sentinel.data)
         exception = exc_info.value
 
         # Assert
         mock_struct_unpack.assert_called_once_with(mocker.sentinel.data)
         mock_serializer_from_tuple.assert_not_called()
         assert exception.__cause__ is mock_struct_unpack.side_effect
+        assert exception.error_info == {"data": mocker.sentinel.data}
 
     def test____deserialize____translate_any_exception_raised_by_from_tuple_method(
         self,
         mock_struct: MagicMock,
         mock_serializer_from_tuple: MagicMock,
         mocker: MockerFixture,
     ) -> None:
@@ -164,14 +165,15 @@
             _ = serializer.deserialize(mocker.sentinel.data)
         exception = exc_info.value
 
         # Assert
         mock_struct_unpack.assert_called_once_with(mocker.sentinel.data)
         mock_serializer_from_tuple.assert_called_once_with(mocker.sentinel.packet_tuple)
         assert exception.__cause__ is mock_serializer_from_tuple.side_effect
+        assert exception.error_info == {"unpacked_struct": mocker.sentinel.packet_tuple}
 
 
 class TestNamedTupleStructSerializer(BaseTestStructBasedSerializer):
     @pytest.mark.parametrize("method", ["serialize", "incremental_serialize", "deserialize", "incremental_deserialize"])
     def test____base_class____implements_default_methods(self, method: str) -> None:
         # Arrange
 
@@ -180,14 +182,16 @@
 
     @pytest.mark.parametrize(
         ["fields", "field_formats", "expected_format"],
         [
             pytest.param((), {}, "", id="no fields"),
             pytest.param(("string", "int"), {"string": "10s", "int": "Q"}, "10sQ", id="10sQ"),
             pytest.param(("int", "string"), {"string": "10s", "int": "Q"}, "Q10s", id="Q10s"),
+            pytest.param(("string", "int"), {"string": "s", "int": "Q"}, "sQ", id="sQ"),
+            pytest.param(("int", "string"), {"string": "s", "int": "Q"}, "Qs", id="Qs"),
         ],
     )
     @pytest.mark.parametrize("endianness", sorted(_ENDIANNESS_CHARACTERS.union([""])), ids=repr)
     def test____dunder_init____compute_right_format(
         self,
         fields: tuple[str, ...],
         field_formats: dict[str, str],
@@ -240,14 +244,71 @@
 
         # Act & Assert
         with pytest.raises(KeyError, match=r"^{!r}$".format(field)):
             _ = NamedTupleStructSerializer(namedtuple_cls, field_formats)
 
         mock_struct_cls.assert_not_called()
 
+    @pytest.mark.parametrize("format", ["4Q", "10c", "abc"], ids=repr)
+    @pytest.mark.parametrize("field", ["x", "y"], ids=repr)
+    def test____dunder_init____field_format_not_a_single_character_error(
+        self,
+        format: str,
+        field: str,
+        mock_struct_cls: MagicMock,
+    ) -> None:
+        # Arrange
+        namedtuple_cls = collections.namedtuple("namedtuple_cls", ["x", "y"])
+        field_formats: dict[str, str] = {"x": "Q", "y": "I"}
+        field_formats[field] = format
+
+        # Act & Assert
+        with pytest.raises(ValueError, match=r"^{!r}: Invalid field format$".format(field)):
+            _ = NamedTupleStructSerializer(namedtuple_cls, field_formats)
+
+        mock_struct_cls.assert_not_called()
+
+    @pytest.mark.parametrize("format", ["4", "#", "\\"], ids=repr)
+    @pytest.mark.parametrize("field", ["x", "y"], ids=repr)
+    def test____dunder_init____field_format_not_a_alphabet_character_error(
+        self,
+        format: str,
+        field: str,
+        mock_struct_cls: MagicMock,
+    ) -> None:
+        # Arrange
+        namedtuple_cls = collections.namedtuple("namedtuple_cls", ["x", "y"])
+        field_formats: dict[str, str] = {"x": "Q", "y": "I"}
+        field_formats[field] = format
+
+        # Act & Assert
+        with pytest.raises(ValueError, match=r"^{!r}: Invalid field format$".format(field)):
+            _ = NamedTupleStructSerializer(namedtuple_cls, field_formats)
+
+        mock_struct_cls.assert_not_called()
+
+    @pytest.mark.parametrize("format", ["²s", "b2s", "abcs"], ids=repr)
+    @pytest.mark.parametrize("field", ["x", "y"], ids=repr)
+    def test____dunder_init____string_field_format_with_non_number_sequence_error(
+        self,
+        format: str,
+        field: str,
+        mock_struct_cls: MagicMock,
+    ) -> None:
+        # Arrange
+        namedtuple_cls = collections.namedtuple("namedtuple_cls", ["x", "y"])
+        field_formats: dict[str, str] = {"x": "Q", "y": "I"}
+        field_formats[field] = format
+
+        # Act & Assert
+        with pytest.raises(ValueError, match=r"^{!r}: Invalid field format$".format(field)):
+            _ = NamedTupleStructSerializer(namedtuple_cls, field_formats)
+
+        mock_struct_cls.assert_not_called()
+
     def test____iter_values____return_given_instance_if_there_is_no_strings(self) -> None:
         # Arrange
         namedtuple_cls = collections.namedtuple("namedtuple_cls", ["x", "y"])
         namedtuple_instance = namedtuple_cls(1234, 56789)
         serializer = NamedTupleStructSerializer(namedtuple_cls, {"x": "I", "y": "I"})
 
         # Act
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_tools/test_socket.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_socket.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: Utf-8 -*-
 
 from __future__ import annotations
 
 import socket
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Callable
 
 from easynetwork.tools.socket import (
     AddressFamily,
     IPv4SocketAddress,
     IPv6SocketAddress,
     SocketAddress,
     SocketProxy,
     new_socket_address,
 )
 
 import pytest
 
+from .._utils import partial_eq
+
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
     from pytest_mock import MockerFixture
 
 
 @pytest.mark.parametrize("name", list(AddressFamily.__members__))
@@ -69,105 +71,169 @@
 
 class TestSocketProxy:
     @pytest.fixture
     @staticmethod
     def mock_new_socket_address(mocker: MockerFixture) -> MagicMock:
         return mocker.patch("easynetwork.tools.socket.new_socket_address", autospec=True)
 
+    @pytest.fixture(
+        params=[
+            pytest.param(False, id="without_runner"),
+            pytest.param(True, id="with_runner"),
+        ]
+    )
+    @staticmethod
+    def runner_stub(request: Any, mocker: MockerFixture) -> MagicMock | None:
+        use_runner: bool = request.param
+        if not use_runner:
+            return None
+
+        def runner(func: Callable[[], Any]) -> Any:
+            return func()
+
+        return mocker.MagicMock(spec=runner, side_effect=runner)
+
     @pytest.mark.parametrize("prop", ["family", "type", "proto"])
-    def test____property____access(self, prop: str, mock_tcp_socket: MagicMock) -> None:
+    def test____property____access(
+        self,
+        prop: str,
+        mock_tcp_socket: MagicMock,
+        runner_stub: MagicMock | None,
+    ) -> None:
         # Arrange
         expected_value = getattr(mock_tcp_socket, prop)
 
         # Act
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
         prop_value = getattr(socket_proxy, prop)
 
         # Assert
         assert prop_value == expected_value
+        if runner_stub is not None:
+            runner_stub.assert_not_called()
 
-    def test____fileno____sub_call(self, mock_tcp_socket: MagicMock, mocker: MockerFixture) -> None:
+    def test____fileno____sub_call(
+        self,
+        mock_tcp_socket: MagicMock,
+        mocker: MockerFixture,
+        runner_stub: MagicMock | None,
+    ) -> None:
         # Arrange
         mock_tcp_socket.fileno.return_value = mocker.sentinel.fd
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
 
         # Act
         fd = socket_proxy.fileno()
 
         # Assert
         mock_tcp_socket.fileno.assert_called_once_with()
         assert fd is mocker.sentinel.fd
+        if runner_stub is not None:
+            runner_stub.assert_called_once_with(mock_tcp_socket.fileno)
 
-    def test____dup____sub_call(self, mock_tcp_socket: MagicMock, mocker: MockerFixture) -> None:
+    def test____dup____sub_call(
+        self,
+        mock_tcp_socket: MagicMock,
+        mocker: MockerFixture,
+        runner_stub: MagicMock | None,
+    ) -> None:
         # Arrange
         mock_tcp_socket.dup.return_value = mocker.sentinel.dup_socket
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
 
         # Act
         socket = socket_proxy.dup()
 
         # Assert
         mock_tcp_socket.dup.assert_called_once_with()
         assert socket is mocker.sentinel.dup_socket
+        if runner_stub is not None:
+            runner_stub.assert_called_once_with(mock_tcp_socket.dup)
 
-    def test____get_inheritable____sub_call(self, mock_tcp_socket: MagicMock, mocker: MockerFixture) -> None:
+    def test____get_inheritable____sub_call(
+        self,
+        mock_tcp_socket: MagicMock,
+        mocker: MockerFixture,
+        runner_stub: MagicMock | None,
+    ) -> None:
         # Arrange
         mock_tcp_socket.get_inheritable.return_value = mocker.sentinel.status
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
 
         # Act
         status = socket_proxy.get_inheritable()
 
         # Assert
         mock_tcp_socket.get_inheritable.assert_called_once_with()
         assert status is mocker.sentinel.status
+        if runner_stub is not None:
+            runner_stub.assert_called_once_with(mock_tcp_socket.get_inheritable)
 
     @pytest.mark.parametrize("nb_args", [2, 3], ids=lambda nb: f"{nb} arguments")
-    def test____getsockopt____sub_call(self, nb_args: int, mock_tcp_socket: MagicMock, mocker: MockerFixture) -> None:
+    def test____getsockopt____sub_call(
+        self,
+        nb_args: int,
+        mock_tcp_socket: MagicMock,
+        mocker: MockerFixture,
+        runner_stub: MagicMock | None,
+    ) -> None:
         # Arrange
         mock_tcp_socket.getsockopt.return_value = mocker.sentinel.value
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
         args: tuple[Any, ...] = (mocker.sentinel.level, mocker.sentinel.optname)
         if nb_args == 3:
             args += (mocker.sentinel.buflen,)
 
         # Act
         value = socket_proxy.getsockopt(*args)
 
         # Assert
         mock_tcp_socket.getsockopt.assert_called_once_with(*args)
         assert value is mocker.sentinel.value
+        if runner_stub is not None:
+            runner_stub.assert_called_once_with(partial_eq(mock_tcp_socket.getsockopt, *args))
 
     @pytest.mark.parametrize("nb_args", [3, 4], ids=lambda nb: f"{nb} arguments")
-    def test____setsockopt____sub_call(self, nb_args: int, mock_tcp_socket: MagicMock, mocker: MockerFixture) -> None:
+    def test____setsockopt____sub_call(
+        self,
+        nb_args: int,
+        mock_tcp_socket: MagicMock,
+        mocker: MockerFixture,
+        runner_stub: MagicMock | None,
+    ) -> None:
         # Arrange
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
         args: tuple[Any, ...] = (mocker.sentinel.level, mocker.sentinel.optname, mocker.sentinel.value)
         if nb_args == 4:
             args += (mocker.sentinel.optlen,)
 
         # Act
         socket_proxy.setsockopt(*args)
 
         # Assert
         mock_tcp_socket.setsockopt.assert_called_once_with(*args)
+        if runner_stub is not None:
+            runner_stub.assert_called_once_with(partial_eq(mock_tcp_socket.setsockopt, *args))
 
     @pytest.mark.parametrize("method", ["getsockname", "getpeername"])
     def test____socket_address____sub_call(
         self,
         method: str,
         mock_tcp_socket: MagicMock,
         mock_new_socket_address: MagicMock,
         mocker: MockerFixture,
+        runner_stub: MagicMock | None,
     ) -> None:
         # Arrange
-        socket_proxy = SocketProxy(mock_tcp_socket)
+        socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
         getattr(mock_tcp_socket, method).return_value = mocker.sentinel.address_to_convert
         mock_new_socket_address.return_value = mocker.sentinel.converted_address
 
         # Act
         address = getattr(socket_proxy, method)()
 
         # Assert
         getattr(mock_tcp_socket, method).assert_called_once_with()
         mock_new_socket_address.assert_called_once_with(mocker.sentinel.address_to_convert, mock_tcp_socket.family)
         assert address is mocker.sentinel.converted_address
+        if runner_stub is not None:
+            runner_stub.assert_called_once_with(getattr(mock_tcp_socket, method))
```

### Comparing `easynetwork-1.0.0.dev1/tests/unit_test/test_tools/test_stream.py` & `easynetwork-1.0.0rc1/tests/unit_test/test_tools/test_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
     ) -> None:
         # Arrange
         from easynetwork.exceptions import StreamProtocolParseError
 
         def side_effect() -> Generator[None, bytes, tuple[Any, bytes]]:
             data = yield
             assert data == b"Hello"
-            raise StreamProtocolParseError(b"World", "deserialization", "Error occured")
+            raise StreamProtocolParseError(b"World", "deserialization", "Error occurred")
 
         mock_build_packet_from_chunks_func: MagicMock = mock_stream_protocol.build_packet_from_chunks
         mock_build_packet_from_chunks_func.side_effect = side_effect
         consumer.feed(b"Hello")
         assert consumer.get_buffer() == b"Hello"
 
         # Act
```

### Comparing `easynetwork-1.0.0.dev1/.gitignore` & `easynetwork-1.0.0rc1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # pdm
-.pdm.toml
+.pdm-python
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `easynetwork-1.0.0.dev1/LICENSE` & `easynetwork-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0.dev1/pyproject.toml` & `easynetwork-1.0.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,41 +5,66 @@
 [project]
 name = "easynetwork"
 description = "The easiest way to use sockets in Python"
 authors = [
     {name = "FrankySnow9", email = "clairicia.rcj.francis@gmail.com"}
 ]
 dependencies = []
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 readme = "README.md"
 license-files = { paths = ["LICENSE"] }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Internet",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Networking",
     "Typing :: Typed"
 ]
 dynamic = ["version"]
+keywords = [
+    "networking",
+    "socket",
+    "server",
+    "client",
+    "communication",
+    "serialization",
+    "async",
+    "asynchronous",
+]
 
 [project.urls]
 Homepage = "https://github.com/francis-clairicia/EasyNetwork"
 
 [project.optional-dependencies]
 cbor = [
-  "cbor2>=5.4,<6",
+    "cbor2>=5.4,<6",
+]
+msgpack = [
+    "msgpack>=1.0.5",
 ]
 encryption = [
-  "cryptography>=39,<40",
+    "cryptography>=39",
+]
+sniffio = [
+    "sniffio>=1.3.0",
+]
+uvloop = [
+    "uvloop~=0.17.0; sys_platform!='win32'",
 ]
 
+[project.entry-points."easynetwork.async.backends"]
+asyncio = "easynetwork_asyncio:AsyncioBackend"
+
 ############################ pdm configuration ############################
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit>=2.20.0",
     "bump2version>=1.0.1",
 ]
@@ -47,61 +72,66 @@
     "tox<5,>=4.0.8",
 ]
 format = [
     "isort!=5.11.0,>=5.10.1",
     "black>=22.6.0",
 ]
 mypy = [
-    "mypy==0.991",
+    "mypy==1.3.0",
+    "types-cryptography>=3.3.23.2",
+    "msgpack-types>=0.2.0",
 ]
 flake8 = [
     "flake8>=6.0",
     "flake8-pyi>=22.11.0",
-    "flake8-dunder-all @ git+https://github.com/francis-clairicia/flake8-dunder-all.git@main",
+    "flake8-dunder-all @ git+https://github.com/francis-clairicia/flake8-dunder-all.git@v0.1.0",
 ]
 test = [
-    "pytest~=7.2",
+    "pytest~=7.3",
+    "pytest-xdist>=3.3.1",
     "pytest-mock~=3.10.0",
     "pytest-cov<5,>=4.0",
-    "coverage[toml]",
+    "pytest-asyncio>=0.21.0",
+    "trove-classifiers==2023.5.2",
+    "trustme>=1.0.0",
 ]
 
 ############################ hatchling configuration ############################
 
 [tool.hatch.build]
 exclude = [
   ".github/",
   ".vscode/",
   ".bumpversion.cfg",
 ]
 
 [tool.hatch.build.targets.wheel]
-sources = ["src"]
+packages = ["src/easynetwork", "src/easynetwork_asyncio"]
 
 [tool.hatch.version]
 path = "src/easynetwork/__init__.py"
 
 
 ############################ Development tools configuration ############################
 
 [tool.isort]
 profile = "black"
 line_length = 130
 combine_as_imports = true
 sections = ["FUTURE", "STDLIB", "EASYNETWORK", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
-known_easynetwork = ["easynetwork"]
+known_easynetwork = ["easynetwork", "easynetwork_asyncio"]
 add_imports = ["from __future__ import annotations"]
 
 [tool.black]
 line-length = 130
-target-version = ["py310"]
+target-version = ["py311"]
 
 [tool.mypy]
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
-python_version = "3.10"
+python_version = "3.11"
 show_error_codes = true
 warn_unused_configs = true
 disallow_any_generics = true
 disallow_any_unimported = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
@@ -111,28 +141,24 @@
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_no_return = true
 warn_unreachable = true
 no_implicit_reexport = true
 strict_equality = true
-enable_error_code = ["truthy-bool", "ignore-without-code"]
+enable_error_code = ["truthy-bool", "ignore-without-code", "unused-awaitable"]
 
 [[tool.mypy.overrides]]
 module = [
     "cbor2",
-    "cryptography.*",
 ]
 ignore_missing_imports = true
 
-[[tool.mypy.overrides]]
-module = ["tests.*"]
-disable_error_code = ["override"]
-
 [tool.pytest.ini_options]
+asyncio_mode = "strict"  # Avoid some unwanted behaviour
 addopts = "--strict-markers"
 minversion = "7.1.2"
 testpaths = ["tests"]
 norecursedirs = ["scripts"]
 markers = [
     "slow: marks tests as slow",
     "functional: marks tests as functional tests",
@@ -144,14 +170,15 @@
     "platform_linux: marks tests as runnable on linux",
 ]
 
 [tool.coverage.run]
 branch = true
 source_pkgs = [
     "easynetwork",
+    "easynetwork_asyncio",
 ]
 relative_files = true
 
 [tool.coverage.paths]
 source = [
     "src/",
     ".tox/*/lib/python*/site-packages",
@@ -167,14 +194,15 @@
 
     # Don't complain about missing debug-only code:
     "def __repr__",
 
     # Don't complain if tests don't hit defensive assertion code:
     "raise AssertionError",
     "raise NotImplementedError",
+    "(typing\\.)?assert_never",
 
     # Don't complain if non-runnable code isn't run:
     "if __name__ == .__main__.:",
 
     # Don't complain about type hinting code:
     "if (typing\\.)?TYPE_CHECKING:",
     "@(typing\\.)?overload",
```

### Comparing `easynetwork-1.0.0.dev1/PKG-INFO` & `easynetwork-1.0.0rc1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: easynetwork
-Version: 1.0.0.dev1
+Version: 1.0.0rc1
 Summary: The easiest way to use sockets in Python
 Project-URL: Homepage, https://github.com/francis-clairicia/EasyNetwork
 Author-email: FrankySnow9 <clairicia.rcj.francis@gmail.com>
 License-File: LICENSE
+Keywords: async,asynchronous,client,communication,networking,serialization,server,socket
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Provides-Extra: cbor
 Requires-Dist: cbor2<6,>=5.4; extra == 'cbor'
 Provides-Extra: encryption
-Requires-Dist: cryptography<40,>=39; extra == 'encryption'
+Requires-Dist: cryptography>=39; extra == 'encryption'
+Provides-Extra: msgpack
+Requires-Dist: msgpack>=1.0.5; extra == 'msgpack'
+Provides-Extra: sniffio
+Requires-Dist: sniffio>=1.3.0; extra == 'sniffio'
+Provides-Extra: uvloop
+Requires-Dist: uvloop~=0.17.0; sys_platform != 'win32' and extra == 'uvloop'
 Description-Content-Type: text/markdown
 
 # EasyNetwork
 The easiest way to use sockets in Python
```

