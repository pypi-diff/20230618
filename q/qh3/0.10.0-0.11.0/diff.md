# Comparing `tmp/qh3-0.10.0.tar.gz` & `tmp/qh3-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/qh3/qh3/dist/.tmp-cn8c6h9z/qh3-0.10.0.tar", last modified: Fri Jun 16 06:26:21 2023, max compression
+gzip compressed data, was "/home/runner/work/qh3/qh3/dist/.tmp-vickcz8k/qh3-0.11.0.tar", last modified: Sun Jun 18 14:51:39 2023, max compression
```

## Comparing `qh3-0.10.0.tar` & `qh3-0.11.0.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-16 06:26:11.000000 qh3-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 06:26:11.000000 qh3-0.10.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-16 06:26:21.000000 qh3-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-16 06:26:11.000000 qh3-0.10.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/h3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-16 06:26:11.000000 qh3-0.10.0/docs/quic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-16 06:26:11.000000 qh3-0.10.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:26:21.000000 qh3-0.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-16 06:26:11.000000 qh3-0.10.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/_crypto.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/_vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/_vendor/OpenSSL/
--rw-r--r--   0 runner    (1001) docker     (123)   111333 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/_vendor/OpenSSL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/_vendor/pylsqpack/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/_vendor/pylsqpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/_vendor/pylsqpack/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/asyncio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/asyncio/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/h0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/h0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/h0/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/h3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/h3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39189 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/h3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/h3/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/h3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3/quic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)   122411 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/quic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    72691 2023-06-16 06:26:11.000000 qh3-0.10.0/src/qh3/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 06:26:21.000000 qh3-0.10.0/src/qh3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/initial_client.bin
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/initial_server.bin
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/pycacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/retry.bin
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/retry_draft_29.bin
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/short_header.bin
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/ssl_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/ssl_cert_with_chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/ssl_combined.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/ssl_key.pem
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)   115714 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14146 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_crypto_draft_29.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_h0.py
--rw-r--r--   0 runner    (1001) docker     (123)    63162 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_h3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_rangeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/test_webtransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_certificate.bin
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_certificate_verify.bin
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_client_hello.bin
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_client_hello_with_alpn.bin
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_client_hello_with_psk.bin
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_client_hello_with_sni.bin
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_encrypted_extensions.bin
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_encrypted_extensions_with_alpn.bin
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_encrypted_extensions_with_alpn_and_early_data.bin
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_finished.bin
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_new_session_ticket.bin
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_new_session_ticket_with_unknown_extension.bin
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_server_hello.bin
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_server_hello_with_psk.bin
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/tls_server_hello_with_unknown_extension.bin
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 06:26:11.000000 qh3-0.10.0/tests/version_negotiation.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 06:26:11.000000 qh3-0.10.0/vendor/ls-qpack/.git
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/bin/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/bin/encode-int.c
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/bin/fuzz-decode.c
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/bin/interop-decode.c
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/bin/interop-encode.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/deps/xxhash/
--rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/deps/xxhash/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/deps/xxhash/xxhash.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/README
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/preamble
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000390,op_havoc,rep_4
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000579,op_flip1,pos_14
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,src_000000,op_flip2,pos_12
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000001,sig_11,src_000579,op_havoc,rep_4
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,sig_11,src_000481,op_int16,pos_15,val_-1
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,src_000000,op_havoc,rep_8
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000006,src_000285,op_flip2,pos_14
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000008,src_000285,op_flip2,pos_20
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000010,src_000306,op_flip2,pos_75
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000011,src_000344,op_havoc,rep_2
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000014,src_000366,op_flip2,pos_28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/b/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/b/README
--rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/b/preamble
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/b/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/b/test-cases/seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/c/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/c/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/c/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/c/test-cases/fb-req.qif.proxygen.out.256.100.0-chopped
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/
--rw-r--r--   0 runner    (1001) docker     (123)    59117 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/preamble
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1
--rw-r--r--   0 runner    (1001) docker     (123)  4372759 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/huff-tables.h
--rw-r--r--   0 runner    (1001) docker     (123)   185368 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/lsqpack.c
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/lsqpack.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/lsqpack-test.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/test/qifs/
--rw-r--r--   0 runner    (1001) docker     (123)   235326 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/qifs/fb-req.qif
--rw-r--r--   0 runner    (1001) docker     (123)   351937 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/qifs/fb-resp.qif
--rw-r--r--   0 runner    (1001) docker     (123)   158092 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/qifs/long-codes.qif
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/qifs/netbsd.qif
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/run-qif.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1529 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/run-scenario.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/0.95-reset.sce
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/cancel-stream.sce
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/drain-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/drain.sce
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/end-dst-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/end-dst.sce
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/incl-name.sce
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/post-base-1.sce
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/post-base-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/post-base-nr.sce
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/scenarios/set-max-cap.sce
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/test_enc_str.c
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/test_get_stx_id.c
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/test_huff_dec.c
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/test_int.c
--rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/test_qpack.c
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/test/test_read_enc_stream.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/tools/har2qif.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/tools/randomize-cookies.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/tools/sort-qif.pl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/wincompat/
--rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/wincompat/getopt.c
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/wincompat/getopt.h
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/wincompat/getopt1.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:26:21.000000 qh3-0.10.0/vendor/ls-qpack/wincompat/sys/
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-06-16 06:26:12.000000 qh3-0.10.0/vendor/ls-qpack/wincompat/sys/queue.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-18 14:51:28.000000 qh3-0.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-18 14:51:28.000000 qh3-0.11.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-18 14:51:39.000000 qh3-0.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-18 14:51:28.000000 qh3-0.11.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/h3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/quic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-18 14:51:28.000000 qh3-0.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:51:39.000000 qh3-0.11.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-18 14:51:28.000000 qh3-0.11.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/_vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/_vendor/OpenSSL/
+-rw-r--r--   0 runner    (1001) docker     (123)   111333 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/OpenSSL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/_vendor/pylsqpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/pylsqpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/pylsqpack/binding.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/h0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h0/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/h3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39189 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/quic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122411 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72691 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/initial_client.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/initial_server.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/pycacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/retry.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/retry_draft_29.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/short_header.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_cert_with_chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_combined.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115714 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_crypto_draft_29.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_h0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63162 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_h3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_webtransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_certificate.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_certificate_verify.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello_with_alpn.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello_with_psk.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello_with_sni.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_encrypted_extensions.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_encrypted_extensions_with_alpn.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_encrypted_extensions_with_alpn_and_early_data.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_finished.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_new_session_ticket.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_new_session_ticket_with_unknown_extension.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_server_hello.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_server_hello_with_psk.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_server_hello_with_unknown_extension.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/version_negotiation.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/encode-int.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/fuzz-decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/interop-decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/interop-encode.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/deps/xxhash/
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/README
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/preamble
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000390,op_havoc,rep_4
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000579,op_flip1,pos_14
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,src_000000,op_flip2,pos_12
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000001,sig_11,src_000579,op_havoc,rep_4
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,sig_11,src_000481,op_int16,pos_15,val_-1
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,src_000000,op_havoc,rep_8
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000006,src_000285,op_flip2,pos_14
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000008,src_000285,op_flip2,pos_20
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000010,src_000306,op_flip2,pos_75
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000011,src_000344,op_havoc,rep_2
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000014,src_000366,op_flip2,pos_28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/README
+-rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/preamble
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/test-cases/seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/test-cases/fb-req.qif.proxygen.out.256.100.0-chopped
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/
+-rw-r--r--   0 runner    (1001) docker     (123)    59117 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/preamble
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1
+-rw-r--r--   0 runner    (1001) docker     (123)  4372759 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/huff-tables.h
+-rw-r--r--   0 runner    (1001) docker     (123)   185368 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/lsqpack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/lsqpack.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/lsqpack-test.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/
+-rw-r--r--   0 runner    (1001) docker     (123)   235326 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-req.qif
+-rw-r--r--   0 runner    (1001) docker     (123)   351937 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-resp.qif
+-rw-r--r--   0 runner    (1001) docker     (123)   158092 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/long-codes.qif
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/netbsd.qif
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/run-qif.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1529 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/run-scenario.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/0.95-reset.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/cancel-stream.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/end-dst-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/end-dst.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/incl-name.sce
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/post-base-1.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/post-base-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/post-base-nr.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/set-max-cap.sce
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_enc_str.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_get_stx_id.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_huff_dec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_qpack.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_read_enc_stream.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/tools/har2qif.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/tools/randomize-cookies.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/tools/sort-qif.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/
+-rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/getopt1.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/sys/queue.h
```

### Comparing `qh3-0.10.0/LICENSE` & `qh3-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/README.rst` & `qh3-0.11.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 qh3
 ===
 
-|rtd| |pypi-v| |pypi-pyversions| |pypi-l| |tests| |codecov| |black|
+|pypi-v| |pypi-pyversions| |pypi-l| |codecov|
 
-.. |rtd| image:: https://readthedocs.org/projects/aioquic/badge/?version=latest
-    :target: https://aioquic.readthedocs.io/
+.. |pypi-v| image:: https://img.shields.io/pypi/v/qh3.svg
+    :target: https://pypi.python.org/pypi/qh3
 
-.. |pypi-v| image:: https://img.shields.io/pypi/v/aioquic.svg
-    :target: https://pypi.python.org/pypi/aioquic
+.. |pypi-pyversions| image:: https://img.shields.io/pypi/pyversions/qh3.svg
+    :target: https://pypi.python.org/pypi/qh3
 
-.. |pypi-pyversions| image:: https://img.shields.io/pypi/pyversions/aioquic.svg
-    :target: https://pypi.python.org/pypi/aioquic
+.. |pypi-l| image:: https://img.shields.io/pypi/l/qh3.svg
+    :target: https://pypi.python.org/pypi/qh3
 
-.. |pypi-l| image:: https://img.shields.io/pypi/l/aioquic.svg
-    :target: https://pypi.python.org/pypi/aioquic
-
-.. |tests| image:: https://github.com/aiortc/aioquic/workflows/tests/badge.svg
-    :target: https://github.com/aiortc/aioquic/actions
-
-.. |codecov| image:: https://img.shields.io/codecov/c/github/aiortc/aioquic.svg
-    :target: https://codecov.io/gh/aiortc/aioquic
-
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/python/black
+.. |codecov| image:: https://img.shields.io/codecov/c/github/Ousret/qh3.svg
+    :target: https://codecov.io/gh/Ousret/qh3
 
 What is ``qh3``?
 ----------------
 
-``qh3`` is a fork of the awesome ``aioquic`` library pending its author return.
-Important changes / improvements are:
+``qh3`` is a fork of the awesome ``aioquic`` library pending its author return (or not).
+Important changes/improvements are:
+
 - Made abi3 compatible, no need to build the wheel all over again on each interpreter version.
 - Only one dependency left! Cryptography will remain as long as Python does not ship with proper QUIC implementation.
 - Mitigated deprecated match_hostname.
-- Mimic load_default_certs ssl context.
+- Mimic load_default_certs SSL context from native Python.
+- Remove the need for OpenSSL development headers.
+- Many, many more pre-built wheel for your convenience! Including PyPy 3.8 and 3.9 and musl linux distributions.
 
-``aioquic`` is a library for the QUIC network protocol in Python. It features
+``qh3`` is a library for the QUIC network protocol in Python. It features
 a minimal TLS 1.3 implementation, a QUIC stack and an HTTP/3 stack.
 
 QUIC was standardised in `RFC 9000`_ and HTTP/3 in `RFC 9114`_.
-``aioquic`` is regularly tested for interoperability against other
+``qh3`` is regularly tested for interoperability against other
 `QUIC implementations`_.
 
-To learn more about ``aioquic`` please `read the documentation`_.
+To learn more about ``qh3`` please `read the documentation`_.
 
 Why should I use ``aioquic``?
 -----------------------------
 
-``aioquic`` has been designed to be embedded into Python client and server
+``qh3`` has been designed to be embedded into Python client and server
 libraries wishing to support QUIC and / or HTTP/3. The goal is to provide a
 common codebase for Python libraries in the hope of avoiding duplicated effort.
 
 Both the QUIC and the HTTP/3 APIs follow the "bring your own I/O" pattern,
 leaving actual I/O operations to the API user. This approach has a number of
 advantages including making the code testable and allowing integration with
 different concurrency models.
@@ -66,74 +60,27 @@
 - logging TLS traffic secrets
 - logging QUIC events in QLOG format
 - HTTP/3 server push support
 
 Requirements
 ------------
 
-``aioquic`` requires Python 3.7 or better, and the OpenSSL development headers.
-
-Linux
-.....
-
-On Debian/Ubuntu run:
-
-.. code-block:: console
-
-   sudo apt install libssl-dev python3-dev
-
-On Alpine Linux run:
-
-.. code-block:: console
-
-   sudo apk add openssl-dev python3-dev bsd-compat-headers libffi-dev
-
-OS X
-....
-
-On OS X run:
-
-.. code-block:: console
-
-   brew install openssl
-
-You will need to set some environment variables to link against OpenSSL:
-
-.. code-block:: console
-
-   export CFLAGS=-I/usr/local/opt/openssl/include
-   export LDFLAGS=-L/usr/local/opt/openssl/lib
-
-Windows
-.......
-
-On Windows the easiest way to install OpenSSL is to use `Chocolatey`_.
-
-.. code-block:: console
-
-   choco install openssl
-
-You will need to set some environment variables to link against OpenSSL:
-
-.. code-block:: console
-
-  $Env:INCLUDE = "C:\Progra~1\OpenSSL-Win64\include"
-  $Env:LIB = "C:\Progra~1\OpenSSL-Win64\lib"
+``aioquic`` requires Python 3.7 or greater.
 
 Running the examples
 --------------------
 
-`aioquic` comes with a number of examples illustrating various QUIC usecases.
+`qh3` comes with a number of examples illustrating various QUIC use-cases.
 
-You can browse these examples here: https://github.com/aiortc/aioquic/tree/main/examples
+You can browse these examples here: https://github.com/Ousret/qh3/tree/main/examples
 
 License
 -------
 
-``aioquic`` is released under the `BSD license`_.
+``qh3`` is released under the `BSD license`_.
 
 .. _read the documentation: https://aioquic.readthedocs.io/en/latest/
 .. _QUIC implementations: https://github.com/quicwg/base-drafts/wiki/Implementations
 .. _cryptography: https://cryptography.io/
 .. _Chocolatey: https://chocolatey.org/
 .. _BSD license: https://aioquic.readthedocs.io/en/latest/license.html
 .. _RFC 8446: https://datatracker.ietf.org/doc/html/rfc8446
```

### Comparing `qh3-0.10.0/docs/Makefile` & `qh3-0.11.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/docs/asyncio.rst` & `qh3-0.11.0/docs/asyncio.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/docs/conf.py` & `qh3-0.11.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/docs/design.rst` & `qh3-0.11.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/docs/h3.rst` & `qh3-0.11.0/docs/h3.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/docs/index.rst` & `qh3-0.11.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/docs/quic.rst` & `qh3-0.11.0/docs/quic.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/pyproject.toml` & `qh3-0.11.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -61,7 +63,15 @@
     "F",  # Pyflakes
     "W",  # pycodestyle
     "I",  # isort
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "qh3.__version__"}
+
+# neat trick to add bsd compat headers only in musllinux images
+[tool.cibuildwheel.linux]
+before-all = "echo"
+
+[[tool.cibuildwheel.overrides]]
+select = "*-musllinux*"
+before-all = "apk add bsd-compat-headers"
```

### Comparing `qh3-0.10.0/setup.py` & `qh3-0.11.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import os
+import platform
 from wheel.bdist_wheel import bdist_wheel
 
 import setuptools
 
 include_dirs = [
     os.path.join("vendor", "ls-qpack"),
     os.path.join("vendor", "ls-qpack", "deps", "xxhash"),
@@ -33,39 +34,38 @@
 
         if python.startswith("cp"):
             return "cp37", "abi3", plat
 
         return python, abi, plat
 
 
+if platform.python_implementation() == "CPython":
+    extra_kwarg = {
+        "py_limited_api": True,
+        "define_macros": [("Py_LIMITED_API", "0x03070000")]
+    }
+else:
+    extra_kwarg = dict()
+
+
 setuptools.setup(
     ext_modules=[
         setuptools.Extension(
             "qh3._buffer",
             extra_compile_args=extra_compile_args,
             sources=["src/qh3/_buffer.c"],
-            define_macros=[("Py_LIMITED_API", "0x03070000")],
-            py_limited_api=True,
-        ),
-        setuptools.Extension(
-            "qh3._crypto",
-            extra_compile_args=extra_compile_args,
-            libraries=libraries,
-            sources=["src/qh3/_crypto.c"],
-            define_macros=[("Py_LIMITED_API", "0x03070000")],
-            py_limited_api=True,
+            **extra_kwarg
         ),
         setuptools.Extension(
             "qh3._vendor.pylsqpack._binding",
             extra_compile_args=extra_compile_args,
             include_dirs=include_dirs,
             sources=[
                 "src/qh3/_vendor/pylsqpack/binding.c",
                 "vendor/ls-qpack/lsqpack.c",
                 "vendor/ls-qpack/deps/xxhash/xxhash.c",
             ],
-            define_macros=[("Py_LIMITED_API", "0x03070000")],
-            py_limited_api=True,
+            **extra_kwarg
         ),
     ],
     cmdclass={"bdist_wheel": bdist_wheel_abi3},
 )
```

### Comparing `qh3-0.10.0/src/qh3/_buffer.c` & `qh3-0.11.0/src/qh3/_buffer.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/_vendor/OpenSSL/__init__.py` & `qh3-0.11.0/src/qh3/_vendor/OpenSSL/__init__.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/_vendor/pylsqpack/binding.c` & `qh3-0.11.0/src/qh3/_vendor/pylsqpack/binding.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/asyncio/client.py` & `qh3-0.11.0/src/qh3/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/asyncio/protocol.py` & `qh3-0.11.0/src/qh3/asyncio/protocol.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/asyncio/server.py` & `qh3-0.11.0/src/qh3/asyncio/server.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/buffer.py` & `qh3-0.11.0/src/qh3/buffer.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/h0/connection.py` & `qh3-0.11.0/src/qh3/h0/connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/h3/connection.py` & `qh3-0.11.0/src/qh3/h3/connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/h3/events.py` & `qh3-0.11.0/src/qh3/h3/events.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/configuration.py` & `qh3-0.11.0/src/qh3/quic/configuration.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/connection.py` & `qh3-0.11.0/src/qh3/quic/connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/crypto.py` & `qh3-0.11.0/src/qh3/quic/crypto.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/events.py` & `qh3-0.11.0/src/qh3/quic/events.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/logger.py` & `qh3-0.11.0/src/qh3/quic/logger.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/packet.py` & `qh3-0.11.0/src/qh3/quic/packet.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/packet_builder.py` & `qh3-0.11.0/src/qh3/quic/packet_builder.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/rangeset.py` & `qh3-0.11.0/src/qh3/quic/rangeset.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/recovery.py` & `qh3-0.11.0/src/qh3/quic/recovery.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/retry.py` & `qh3-0.11.0/src/qh3/quic/retry.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/quic/stream.py` & `qh3-0.11.0/src/qh3/quic/stream.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3/tls.py` & `qh3-0.11.0/src/qh3/tls.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/src/qh3.egg-info/SOURCES.txt` & `qh3-0.11.0/src/qh3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 docs/design.rst
 docs/h3.rst
 docs/index.rst
 docs/license.rst
 docs/quic.rst
 src/qh3/__init__.py
 src/qh3/_buffer.c
-src/qh3/_crypto.c
+src/qh3/_crypto.py
 src/qh3/buffer.py
 src/qh3/py.typed
 src/qh3/tls.py
 src/qh3.egg-info/PKG-INFO
 src/qh3.egg-info/SOURCES.txt
 src/qh3.egg-info/dependency_links.txt
 src/qh3.egg-info/requires.txt
```

### Comparing `qh3-0.10.0/tests/initial_client.bin` & `qh3-0.11.0/tests/initial_client.bin`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/pycacert.pem` & `qh3-0.11.0/tests/pycacert.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/ssl_cert.pem` & `qh3-0.11.0/tests/ssl_cert.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/ssl_cert_with_chain.pem` & `qh3-0.11.0/tests/ssl_cert_with_chain.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/ssl_combined.pem` & `qh3-0.11.0/tests/ssl_combined.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/ssl_key.pem` & `qh3-0.11.0/tests/ssl_key.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_asyncio.py` & `qh3-0.11.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_buffer.py` & `qh3-0.11.0/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_connection.py` & `qh3-0.11.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_crypto.py` & `qh3-0.11.0/tests/test_crypto_draft_29.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,97 +9,96 @@
     derive_key_iv_hp,
 )
 from qh3.quic.packet import PACKET_FIXED_BIT, QuicProtocolVersion
 from qh3.tls import CipherSuite
 
 from .utils import SKIP_TESTS
 
-PROTOCOL_VERSION = QuicProtocolVersion.VERSION_1
+PROTOCOL_VERSION = QuicProtocolVersion.DRAFT_29
 
-# https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.5
-CHACHA20_CLIENT_PACKET_NUMBER = 654360564
-CHACHA20_CLIENT_PLAIN_HEADER = binascii.unhexlify("4200bff4")
-CHACHA20_CLIENT_PLAIN_PAYLOAD = binascii.unhexlify("01")
+CHACHA20_CLIENT_PACKET_NUMBER = 2
+CHACHA20_CLIENT_PLAIN_HEADER = binascii.unhexlify(
+    "e1ff0000160880b57c7b70d8524b0850fc2a28e240fd7640170002"
+)
+CHACHA20_CLIENT_PLAIN_PAYLOAD = binascii.unhexlify("0201000000")
 CHACHA20_CLIENT_ENCRYPTED_PACKET = binascii.unhexlify(
-    "4cfe4189655e5cd55c41f69080575d7999c25a5bfb"
+    "e8ff0000160880b57c7b70d8524b0850fc2a28e240fd7640178313b04be98449"
+    "eb10567e25ce930381f2a5b7da2db8db"
 )
 
-# https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.2
 LONG_CLIENT_PACKET_NUMBER = 2
 LONG_CLIENT_PLAIN_HEADER = binascii.unhexlify(
-    "c300000001088394c8f03e5157080000449e00000002"
+    "c3ff00001d088394c8f03e5157080000449e00000002"
 )
 LONG_CLIENT_PLAIN_PAYLOAD = binascii.unhexlify(
-    "060040f1010000ed0303ebf8fa56f12939b9584a3896472ec40bb863cfd3e868"
-    "04fe3a47f06a2b69484c00000413011302010000c000000010000e00000b6578"
-    "616d706c652e636f6dff01000100000a00080006001d00170018001000070005"
-    "04616c706e000500050100000000003300260024001d00209370b2c9caa47fba"
-    "baf4559fedba753de171fa71f50f1ce15d43e994ec74d748002b000302030400"
-    "0d0010000e0403050306030203080408050806002d00020101001c0002400100"
-    "3900320408ffffffffffffffff05048000ffff07048000ffff08011001048000"
-    "75300901100f088394c8f03e51570806048000ffff"
-) + bytes(917)
+    "060040c4010000c003036660261ff947cea49cce6cfad687f457cf1b14531ba1"
+    "4131a0e8f309a1d0b9c4000006130113031302010000910000000b0009000006"
+    "736572766572ff01000100000a00140012001d00170018001901000101010201"
+    "03010400230000003300260024001d00204cfdfcd178b784bf328cae793b136f"
+    "2aedce005ff183d7bb1495207236647037002b0003020304000d0020001e0403"
+    "05030603020308040805080604010501060102010402050206020202002d0002"
+    "0101001c00024001"
+) + bytes(962)
 LONG_CLIENT_ENCRYPTED_PACKET = binascii.unhexlify(
-    "c000000001088394c8f03e5157080000449e7b9aec34d1b1c98dd7689fb8ec11"
-    "d242b123dc9bd8bab936b47d92ec356c0bab7df5976d27cd449f63300099f399"
-    "1c260ec4c60d17b31f8429157bb35a1282a643a8d2262cad67500cadb8e7378c"
-    "8eb7539ec4d4905fed1bee1fc8aafba17c750e2c7ace01e6005f80fcb7df6212"
-    "30c83711b39343fa028cea7f7fb5ff89eac2308249a02252155e2347b63d58c5"
-    "457afd84d05dfffdb20392844ae812154682e9cf012f9021a6f0be17ddd0c208"
-    "4dce25ff9b06cde535d0f920a2db1bf362c23e596d11a4f5a6cf3948838a3aec"
-    "4e15daf8500a6ef69ec4e3feb6b1d98e610ac8b7ec3faf6ad760b7bad1db4ba3"
-    "485e8a94dc250ae3fdb41ed15fb6a8e5eba0fc3dd60bc8e30c5c4287e53805db"
-    "059ae0648db2f64264ed5e39be2e20d82df566da8dd5998ccabdae053060ae6c"
-    "7b4378e846d29f37ed7b4ea9ec5d82e7961b7f25a9323851f681d582363aa5f8"
-    "9937f5a67258bf63ad6f1a0b1d96dbd4faddfcefc5266ba6611722395c906556"
-    "be52afe3f565636ad1b17d508b73d8743eeb524be22b3dcbc2c7468d54119c74"
-    "68449a13d8e3b95811a198f3491de3e7fe942b330407abf82a4ed7c1b311663a"
-    "c69890f4157015853d91e923037c227a33cdd5ec281ca3f79c44546b9d90ca00"
-    "f064c99e3dd97911d39fe9c5d0b23a229a234cb36186c4819e8b9c5927726632"
-    "291d6a418211cc2962e20fe47feb3edf330f2c603a9d48c0fcb5699dbfe58964"
-    "25c5bac4aee82e57a85aaf4e2513e4f05796b07ba2ee47d80506f8d2c25e50fd"
-    "14de71e6c418559302f939b0e1abd576f279c4b2e0feb85c1f28ff18f58891ff"
-    "ef132eef2fa09346aee33c28eb130ff28f5b766953334113211996d20011a198"
-    "e3fc433f9f2541010ae17c1bf202580f6047472fb36857fe843b19f5984009dd"
-    "c324044e847a4f4a0ab34f719595de37252d6235365e9b84392b061085349d73"
-    "203a4a13e96f5432ec0fd4a1ee65accdd5e3904df54c1da510b0ff20dcc0c77f"
-    "cb2c0e0eb605cb0504db87632cf3d8b4dae6e705769d1de354270123cb11450e"
-    "fc60ac47683d7b8d0f811365565fd98c4c8eb936bcab8d069fc33bd801b03ade"
-    "a2e1fbc5aa463d08ca19896d2bf59a071b851e6c239052172f296bfb5e724047"
-    "90a2181014f3b94a4e97d117b438130368cc39dbb2d198065ae3986547926cd2"
-    "162f40a29f0c3c8745c0f50fba3852e566d44575c29d39a03f0cda721984b6f4"
-    "40591f355e12d439ff150aab7613499dbd49adabc8676eef023b15b65bfc5ca0"
-    "6948109f23f350db82123535eb8a7433bdabcb909271a6ecbcb58b936a88cd4e"
-    "8f2e6ff5800175f113253d8fa9ca8885c2f552e657dc603f252e1a8e308f76f0"
-    "be79e2fb8f5d5fbbe2e30ecadd220723c8c0aea8078cdfcb3868263ff8f09400"
-    "54da48781893a7e49ad5aff4af300cd804a6b6279ab3ff3afb64491c85194aab"
-    "760d58a606654f9f4400e8b38591356fbf6425aca26dc85244259ff2b19c41b9"
-    "f96f3ca9ec1dde434da7d2d392b905ddf3d1f9af93d1af5950bd493f5aa731b4"
-    "056df31bd267b6b90a079831aaf579be0a39013137aac6d404f518cfd4684064"
-    "7e78bfe706ca4cf5e9c5453e9f7cfd2b8b4c8d169a44e55c88d4a9a7f9474241"
-    "e221af44860018ab0856972e194cd934"
+    "c5ff00001d088394c8f03e5157080000449e4a95245bfb66bc5f93032b7ddd89"
+    "fe0ff15d9c4f7050fccdb71c1cd80512d4431643a53aafa1b0b518b44968b18b"
+    "8d3e7a4d04c30b3ed9410325b2abb2dafb1c12f8b70479eb8df98abcaf95dd8f"
+    "3d1c78660fbc719f88b23c8aef6771f3d50e10fdfb4c9d92386d44481b6c52d5"
+    "9e5538d3d3942de9f13a7f8b702dc31724180da9df22714d01003fc5e3d165c9"
+    "50e630b8540fbd81c9df0ee63f94997026c4f2e1887a2def79050ac2d86ba318"
+    "e0b3adc4c5aa18bcf63c7cf8e85f569249813a2236a7e72269447cd1c755e451"
+    "f5e77470eb3de64c8849d292820698029cfa18e5d66176fe6e5ba4ed18026f90"
+    "900a5b4980e2f58e39151d5cd685b10929636d4f02e7fad2a5a458249f5c0298"
+    "a6d53acbe41a7fc83fa7cc01973f7a74d1237a51974e097636b6203997f921d0"
+    "7bc1940a6f2d0de9f5a11432946159ed6cc21df65c4ddd1115f86427259a196c"
+    "7148b25b6478b0dc7766e1c4d1b1f5159f90eabc61636226244642ee148b464c"
+    "9e619ee50a5e3ddc836227cad938987c4ea3c1fa7c75bbf88d89e9ada642b2b8"
+    "8fe8107b7ea375b1b64889a4e9e5c38a1c896ce275a5658d250e2d76e1ed3a34"
+    "ce7e3a3f383d0c996d0bed106c2899ca6fc263ef0455e74bb6ac1640ea7bfedc"
+    "59f03fee0e1725ea150ff4d69a7660c5542119c71de270ae7c3ecfd1af2c4ce5"
+    "51986949cc34a66b3e216bfe18b347e6c05fd050f85912db303a8f054ec23e38"
+    "f44d1c725ab641ae929fecc8e3cefa5619df4231f5b4c009fa0c0bbc60bc75f7"
+    "6d06ef154fc8577077d9d6a1d2bd9bf081dc783ece60111bea7da9e5a9748069"
+    "d078b2bef48de04cabe3755b197d52b32046949ecaa310274b4aac0d008b1948"
+    "c1082cdfe2083e386d4fd84c0ed0666d3ee26c4515c4fee73433ac703b690a9f"
+    "7bf278a77486ace44c489a0c7ac8dfe4d1a58fb3a730b993ff0f0d61b4d89557"
+    "831eb4c752ffd39c10f6b9f46d8db278da624fd800e4af85548a294c1518893a"
+    "8778c4f6d6d73c93df200960104e062b388ea97dcf4016bced7f62b4f062cb6c"
+    "04c20693d9a0e3b74ba8fe74cc01237884f40d765ae56a51688d985cf0ceaef4"
+    "3045ed8c3f0c33bced08537f6882613acd3b08d665fce9dd8aa73171e2d3771a"
+    "61dba2790e491d413d93d987e2745af29418e428be34941485c93447520ffe23"
+    "1da2304d6a0fd5d07d0837220236966159bef3cf904d722324dd852513df39ae"
+    "030d8173908da6364786d3c1bfcb19ea77a63b25f1e7fc661def480c5d00d444"
+    "56269ebd84efd8e3a8b2c257eec76060682848cbf5194bc99e49ee75e4d0d254"
+    "bad4bfd74970c30e44b65511d4ad0e6ec7398e08e01307eeeea14e46ccd87cf3"
+    "6b285221254d8fc6a6765c524ded0085dca5bd688ddf722e2c0faf9d0fb2ce7a"
+    "0c3f2cee19ca0ffba461ca8dc5d2c8178b0762cf67135558494d2a96f1a139f0"
+    "edb42d2af89a9c9122b07acbc29e5e722df8615c343702491098478a389c9872"
+    "a10b0c9875125e257c7bfdf27eef4060bd3d00f4c14fd3e3496c38d3c5d1a566"
+    "8c39350effbc2d16ca17be4ce29f02ed969504dda2a8c6b9ff919e693ee79e09"
+    "089316e7d1d89ec099db3b2b268725d888536a4b8bf9aee8fb43e82a4d919d48"
+    "43b1ca70a2d8d3f725ead1391377dcc0"
 )
 
-# https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.3
 LONG_SERVER_PACKET_NUMBER = 1
 LONG_SERVER_PLAIN_HEADER = binascii.unhexlify(
-    "c1000000010008f067a5502a4262b50040750001"
+    "c1ff00001d0008f067a5502a4262b50040740001"
 )
 LONG_SERVER_PLAIN_PAYLOAD = binascii.unhexlify(
-    "02000000000600405a020000560303eefce7f7b37ba1d1632e96677825ddf739"
-    "88cfc79825df566dc5430b9a045a1200130100002e00330024001d00209d3c94"
-    "0d89690b84d08a60993c144eca684d1081287c834d5311bcf32bb9da1a002b00"
-    "020304"
+    "0d0000000018410a020000560303eefce7f7b37ba1d1632e96677825ddf73988"
+    "cfc79825df566dc5430b9a045a1200130100002e00330024001d00209d3c940d"
+    "89690b84d08a60993c144eca684d1081287c834d5311bcf32bb9da1a002b0002"
+    "0304"
 )
 LONG_SERVER_ENCRYPTED_PACKET = binascii.unhexlify(
-    "cf000000010008f067a5502a4262b5004075c0d95a482cd0991cd25b0aac406a"
-    "5816b6394100f37a1c69797554780bb38cc5a99f5ede4cf73c3ec2493a1839b3"
-    "dbcba3f6ea46c5b7684df3548e7ddeb9c3bf9c73cc3f3bded74b562bfb19fb84"
-    "022f8ef4cdd93795d77d06edbb7aaf2f58891850abbdca3d20398c276456cbc4"
-    "2158407dd074ee"
+    "caff00001d0008f067a5502a4262b5004074aaf2f007823a5d3a1207c86ee491"
+    "32824f0465243d082d868b107a38092bc80528664cbf9456ebf27673fb5fa506"
+    "1ab573c9f001b81da028a00d52ab00b15bebaa70640e106cf2acd043e9c6b441"
+    "1c0a79637134d8993701fe779e58c2fe753d14b0564021565ea92e57bc6faf56"
+    "dfc7a40870e6"
 )
 
 SHORT_SERVER_PACKET_NUMBER = 3
 SHORT_SERVER_PLAIN_HEADER = binascii.unhexlify("41b01fd24a586a9cf30003")
 SHORT_SERVER_PLAIN_PAYLOAD = binascii.unhexlify(
     "06003904000035000151805a4bebf5000020b098c8dc4183e4c182572e10ac3e"
     "2b88897e0524c8461847548bd2dffa2c0ae60008002a0004ffffffff"
@@ -111,83 +110,58 @@
 )
 
 
 class CryptoTest(TestCase):
     """
     Test vectors from:
 
-    https://datatracker.ietf.org/doc/html/rfc9001#appendix-A
+    https://datatracker.ietf.org/doc/html/draft-ietf-quic-tls-18#appendix-A
     """
 
     def create_crypto(self, is_client):
         pair = CryptoPair()
         pair.setup_initial(
             cid=binascii.unhexlify("8394c8f03e515708"),
             is_client=is_client,
             version=PROTOCOL_VERSION,
         )
         return pair
 
     def test_derive_key_iv_hp(self):
-        # https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.1
-
         # client
         secret = binascii.unhexlify(
-            "c00cf151ca5be075ed0ebfb5c80323c42d6b7db67881289af4008f1f6c357aea"
+            "8a3515a14ae3c31b9c2d6d5bc58538ca5cd2baa119087143e60887428dcb52f6"
         )
         key, iv, hp = derive_key_iv_hp(INITIAL_CIPHER_SUITE, secret)
-        self.assertEqual(key, binascii.unhexlify("1f369613dd76d5467730efcbe3b1a22d"))
-        self.assertEqual(iv, binascii.unhexlify("fa044b2f42a3fd3b46fb255c"))
-        self.assertEqual(hp, binascii.unhexlify("9f50449e04a0e810283a1e9933adedd2"))
+        self.assertEqual(key, binascii.unhexlify("98b0d7e5e7a402c67c33f350fa65ea54"))
+        self.assertEqual(iv, binascii.unhexlify("19e94387805eb0b46c03a788"))
+        self.assertEqual(hp, binascii.unhexlify("0edd982a6ac527f2eddcbb7348dea5d7"))
 
         # server
         secret = binascii.unhexlify(
-            "3c199828fd139efd216c155ad844cc81fb82fa8d7446fa7d78be803acdda951b"
+            "47b2eaea6c266e32c0697a9e2a898bdf5c4fb3e5ac34f0e549bf2c58581a3811"
         )
         key, iv, hp = derive_key_iv_hp(INITIAL_CIPHER_SUITE, secret)
-        self.assertEqual(key, binascii.unhexlify("cf3a5331653c364c88f0f379b6067e37"))
-        self.assertEqual(iv, binascii.unhexlify("0ac1493ca1905853b0bba03e"))
-        self.assertEqual(hp, binascii.unhexlify("c206b8d9b9f0f37644430b490eeaa314"))
-
-    @skipIf("chacha20" in SKIP_TESTS, "Skipping chacha20 tests")
-    def test_derive_key_iv_hp_chacha20(self):
-        # https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.5
-
-        # server
-        secret = binascii.unhexlify(
-            "9ac312a7f877468ebe69422748ad00a15443f18203a07d6060f688f30f21632b"
-        )
-        key, iv, hp = derive_key_iv_hp(CipherSuite.CHACHA20_POLY1305_SHA256, secret)
-        self.assertEqual(
-            key,
-            binascii.unhexlify(
-                "c6d98ff3441c3fe1b2182094f69caa2ed4b716b65488960a7a984979fb23e1c8"
-            ),
-        )
-        self.assertEqual(iv, binascii.unhexlify("e0459b3474bdd0e44a41c144"))
-        self.assertEqual(
-            hp,
-            binascii.unhexlify(
-                "25a282b9e82f06f21f488917a4fc8f1b73573685608597d0efcb076b0ab7a7a4"
-            ),
-        )
+        self.assertEqual(key, binascii.unhexlify("9a8be902a9bdd91d16064ca118045fb4"))
+        self.assertEqual(iv, binascii.unhexlify("0a82086d32205ba22241d8dc"))
+        self.assertEqual(hp, binascii.unhexlify("94b9452d2b3c7c7f6da7fdd8593537fd"))
 
     @skipIf("chacha20" in SKIP_TESTS, "Skipping chacha20 tests")
     def test_decrypt_chacha20(self):
         pair = CryptoPair()
         pair.recv.setup(
             cipher_suite=CipherSuite.CHACHA20_POLY1305_SHA256,
             secret=binascii.unhexlify(
-                "9ac312a7f877468ebe69422748ad00a15443f18203a07d6060f688f30f21632b"
+                "b42772df33c9719a32820d302aa664d080d7f5ea7a71a330f87864cb289ae8c0"
             ),
             version=PROTOCOL_VERSION,
         )
 
         plain_header, plain_payload, packet_number = pair.decrypt_packet(
-            CHACHA20_CLIENT_ENCRYPTED_PACKET, 1, CHACHA20_CLIENT_PACKET_NUMBER
+            CHACHA20_CLIENT_ENCRYPTED_PACKET, 25, 0
         )
         self.assertEqual(plain_header, CHACHA20_CLIENT_PLAIN_HEADER)
         self.assertEqual(plain_payload, CHACHA20_CLIENT_PLAIN_PAYLOAD)
         self.assertEqual(packet_number, CHACHA20_CLIENT_PACKET_NUMBER)
 
     def test_decrypt_long_client(self):
         pair = self.create_crypto(is_client=False)
@@ -233,15 +207,15 @@
 
     @skipIf("chacha20" in SKIP_TESTS, "Skipping chacha20 tests")
     def test_encrypt_chacha20(self):
         pair = CryptoPair()
         pair.send.setup(
             cipher_suite=CipherSuite.CHACHA20_POLY1305_SHA256,
             secret=binascii.unhexlify(
-                "9ac312a7f877468ebe69422748ad00a15443f18203a07d6060f688f30f21632b"
+                "b42772df33c9719a32820d302aa664d080d7f5ea7a71a330f87864cb289ae8c0"
             ),
             version=PROTOCOL_VERSION,
         )
 
         packet = pair.encrypt_packet(
             CHACHA20_CLIENT_PLAIN_HEADER,
             CHACHA20_CLIENT_PLAIN_PAYLOAD,
```

### Comparing `qh3-0.10.0/tests/test_crypto_draft_29.py` & `qh3-0.11.0/tests/test_crypto.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 import binascii
 from unittest import TestCase, skipIf
+from unittest.mock import patch
 
 from qh3.buffer import Buffer
 from qh3.quic.crypto import (
+    AEAD,
+    CIPHER_SUITES,
     INITIAL_CIPHER_SUITE,
     CryptoError,
     CryptoPair,
+    HeaderProtection,
     derive_key_iv_hp,
 )
 from qh3.quic.packet import PACKET_FIXED_BIT, QuicProtocolVersion
 from qh3.tls import CipherSuite
 
 from .utils import SKIP_TESTS
 
-PROTOCOL_VERSION = QuicProtocolVersion.DRAFT_29
+PROTOCOL_VERSION = QuicProtocolVersion.VERSION_1
 
-CHACHA20_CLIENT_PACKET_NUMBER = 2
-CHACHA20_CLIENT_PLAIN_HEADER = binascii.unhexlify(
-    "e1ff0000160880b57c7b70d8524b0850fc2a28e240fd7640170002"
-)
-CHACHA20_CLIENT_PLAIN_PAYLOAD = binascii.unhexlify("0201000000")
+# https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.5
+CHACHA20_CLIENT_PACKET_NUMBER = 654360564
+CHACHA20_CLIENT_PLAIN_HEADER = binascii.unhexlify("4200bff4")
+CHACHA20_CLIENT_PLAIN_PAYLOAD = binascii.unhexlify("01")
 CHACHA20_CLIENT_ENCRYPTED_PACKET = binascii.unhexlify(
-    "e8ff0000160880b57c7b70d8524b0850fc2a28e240fd7640178313b04be98449"
-    "eb10567e25ce930381f2a5b7da2db8db"
+    "4cfe4189655e5cd55c41f69080575d7999c25a5bfb"
 )
 
+# https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.2
 LONG_CLIENT_PACKET_NUMBER = 2
 LONG_CLIENT_PLAIN_HEADER = binascii.unhexlify(
-    "c3ff00001d088394c8f03e5157080000449e00000002"
+    "c300000001088394c8f03e5157080000449e00000002"
 )
 LONG_CLIENT_PLAIN_PAYLOAD = binascii.unhexlify(
-    "060040c4010000c003036660261ff947cea49cce6cfad687f457cf1b14531ba1"
-    "4131a0e8f309a1d0b9c4000006130113031302010000910000000b0009000006"
-    "736572766572ff01000100000a00140012001d00170018001901000101010201"
-    "03010400230000003300260024001d00204cfdfcd178b784bf328cae793b136f"
-    "2aedce005ff183d7bb1495207236647037002b0003020304000d0020001e0403"
-    "05030603020308040805080604010501060102010402050206020202002d0002"
-    "0101001c00024001"
-) + bytes(962)
+    "060040f1010000ed0303ebf8fa56f12939b9584a3896472ec40bb863cfd3e868"
+    "04fe3a47f06a2b69484c00000413011302010000c000000010000e00000b6578"
+    "616d706c652e636f6dff01000100000a00080006001d00170018001000070005"
+    "04616c706e000500050100000000003300260024001d00209370b2c9caa47fba"
+    "baf4559fedba753de171fa71f50f1ce15d43e994ec74d748002b000302030400"
+    "0d0010000e0403050306030203080408050806002d00020101001c0002400100"
+    "3900320408ffffffffffffffff05048000ffff07048000ffff08011001048000"
+    "75300901100f088394c8f03e51570806048000ffff"
+) + bytes(917)
 LONG_CLIENT_ENCRYPTED_PACKET = binascii.unhexlify(
-    "c5ff00001d088394c8f03e5157080000449e4a95245bfb66bc5f93032b7ddd89"
-    "fe0ff15d9c4f7050fccdb71c1cd80512d4431643a53aafa1b0b518b44968b18b"
-    "8d3e7a4d04c30b3ed9410325b2abb2dafb1c12f8b70479eb8df98abcaf95dd8f"
-    "3d1c78660fbc719f88b23c8aef6771f3d50e10fdfb4c9d92386d44481b6c52d5"
-    "9e5538d3d3942de9f13a7f8b702dc31724180da9df22714d01003fc5e3d165c9"
-    "50e630b8540fbd81c9df0ee63f94997026c4f2e1887a2def79050ac2d86ba318"
-    "e0b3adc4c5aa18bcf63c7cf8e85f569249813a2236a7e72269447cd1c755e451"
-    "f5e77470eb3de64c8849d292820698029cfa18e5d66176fe6e5ba4ed18026f90"
-    "900a5b4980e2f58e39151d5cd685b10929636d4f02e7fad2a5a458249f5c0298"
-    "a6d53acbe41a7fc83fa7cc01973f7a74d1237a51974e097636b6203997f921d0"
-    "7bc1940a6f2d0de9f5a11432946159ed6cc21df65c4ddd1115f86427259a196c"
-    "7148b25b6478b0dc7766e1c4d1b1f5159f90eabc61636226244642ee148b464c"
-    "9e619ee50a5e3ddc836227cad938987c4ea3c1fa7c75bbf88d89e9ada642b2b8"
-    "8fe8107b7ea375b1b64889a4e9e5c38a1c896ce275a5658d250e2d76e1ed3a34"
-    "ce7e3a3f383d0c996d0bed106c2899ca6fc263ef0455e74bb6ac1640ea7bfedc"
-    "59f03fee0e1725ea150ff4d69a7660c5542119c71de270ae7c3ecfd1af2c4ce5"
-    "51986949cc34a66b3e216bfe18b347e6c05fd050f85912db303a8f054ec23e38"
-    "f44d1c725ab641ae929fecc8e3cefa5619df4231f5b4c009fa0c0bbc60bc75f7"
-    "6d06ef154fc8577077d9d6a1d2bd9bf081dc783ece60111bea7da9e5a9748069"
-    "d078b2bef48de04cabe3755b197d52b32046949ecaa310274b4aac0d008b1948"
-    "c1082cdfe2083e386d4fd84c0ed0666d3ee26c4515c4fee73433ac703b690a9f"
-    "7bf278a77486ace44c489a0c7ac8dfe4d1a58fb3a730b993ff0f0d61b4d89557"
-    "831eb4c752ffd39c10f6b9f46d8db278da624fd800e4af85548a294c1518893a"
-    "8778c4f6d6d73c93df200960104e062b388ea97dcf4016bced7f62b4f062cb6c"
-    "04c20693d9a0e3b74ba8fe74cc01237884f40d765ae56a51688d985cf0ceaef4"
-    "3045ed8c3f0c33bced08537f6882613acd3b08d665fce9dd8aa73171e2d3771a"
-    "61dba2790e491d413d93d987e2745af29418e428be34941485c93447520ffe23"
-    "1da2304d6a0fd5d07d0837220236966159bef3cf904d722324dd852513df39ae"
-    "030d8173908da6364786d3c1bfcb19ea77a63b25f1e7fc661def480c5d00d444"
-    "56269ebd84efd8e3a8b2c257eec76060682848cbf5194bc99e49ee75e4d0d254"
-    "bad4bfd74970c30e44b65511d4ad0e6ec7398e08e01307eeeea14e46ccd87cf3"
-    "6b285221254d8fc6a6765c524ded0085dca5bd688ddf722e2c0faf9d0fb2ce7a"
-    "0c3f2cee19ca0ffba461ca8dc5d2c8178b0762cf67135558494d2a96f1a139f0"
-    "edb42d2af89a9c9122b07acbc29e5e722df8615c343702491098478a389c9872"
-    "a10b0c9875125e257c7bfdf27eef4060bd3d00f4c14fd3e3496c38d3c5d1a566"
-    "8c39350effbc2d16ca17be4ce29f02ed969504dda2a8c6b9ff919e693ee79e09"
-    "089316e7d1d89ec099db3b2b268725d888536a4b8bf9aee8fb43e82a4d919d48"
-    "43b1ca70a2d8d3f725ead1391377dcc0"
+    "c000000001088394c8f03e5157080000449e7b9aec34d1b1c98dd7689fb8ec11"
+    "d242b123dc9bd8bab936b47d92ec356c0bab7df5976d27cd449f63300099f399"
+    "1c260ec4c60d17b31f8429157bb35a1282a643a8d2262cad67500cadb8e7378c"
+    "8eb7539ec4d4905fed1bee1fc8aafba17c750e2c7ace01e6005f80fcb7df6212"
+    "30c83711b39343fa028cea7f7fb5ff89eac2308249a02252155e2347b63d58c5"
+    "457afd84d05dfffdb20392844ae812154682e9cf012f9021a6f0be17ddd0c208"
+    "4dce25ff9b06cde535d0f920a2db1bf362c23e596d11a4f5a6cf3948838a3aec"
+    "4e15daf8500a6ef69ec4e3feb6b1d98e610ac8b7ec3faf6ad760b7bad1db4ba3"
+    "485e8a94dc250ae3fdb41ed15fb6a8e5eba0fc3dd60bc8e30c5c4287e53805db"
+    "059ae0648db2f64264ed5e39be2e20d82df566da8dd5998ccabdae053060ae6c"
+    "7b4378e846d29f37ed7b4ea9ec5d82e7961b7f25a9323851f681d582363aa5f8"
+    "9937f5a67258bf63ad6f1a0b1d96dbd4faddfcefc5266ba6611722395c906556"
+    "be52afe3f565636ad1b17d508b73d8743eeb524be22b3dcbc2c7468d54119c74"
+    "68449a13d8e3b95811a198f3491de3e7fe942b330407abf82a4ed7c1b311663a"
+    "c69890f4157015853d91e923037c227a33cdd5ec281ca3f79c44546b9d90ca00"
+    "f064c99e3dd97911d39fe9c5d0b23a229a234cb36186c4819e8b9c5927726632"
+    "291d6a418211cc2962e20fe47feb3edf330f2c603a9d48c0fcb5699dbfe58964"
+    "25c5bac4aee82e57a85aaf4e2513e4f05796b07ba2ee47d80506f8d2c25e50fd"
+    "14de71e6c418559302f939b0e1abd576f279c4b2e0feb85c1f28ff18f58891ff"
+    "ef132eef2fa09346aee33c28eb130ff28f5b766953334113211996d20011a198"
+    "e3fc433f9f2541010ae17c1bf202580f6047472fb36857fe843b19f5984009dd"
+    "c324044e847a4f4a0ab34f719595de37252d6235365e9b84392b061085349d73"
+    "203a4a13e96f5432ec0fd4a1ee65accdd5e3904df54c1da510b0ff20dcc0c77f"
+    "cb2c0e0eb605cb0504db87632cf3d8b4dae6e705769d1de354270123cb11450e"
+    "fc60ac47683d7b8d0f811365565fd98c4c8eb936bcab8d069fc33bd801b03ade"
+    "a2e1fbc5aa463d08ca19896d2bf59a071b851e6c239052172f296bfb5e724047"
+    "90a2181014f3b94a4e97d117b438130368cc39dbb2d198065ae3986547926cd2"
+    "162f40a29f0c3c8745c0f50fba3852e566d44575c29d39a03f0cda721984b6f4"
+    "40591f355e12d439ff150aab7613499dbd49adabc8676eef023b15b65bfc5ca0"
+    "6948109f23f350db82123535eb8a7433bdabcb909271a6ecbcb58b936a88cd4e"
+    "8f2e6ff5800175f113253d8fa9ca8885c2f552e657dc603f252e1a8e308f76f0"
+    "be79e2fb8f5d5fbbe2e30ecadd220723c8c0aea8078cdfcb3868263ff8f09400"
+    "54da48781893a7e49ad5aff4af300cd804a6b6279ab3ff3afb64491c85194aab"
+    "760d58a606654f9f4400e8b38591356fbf6425aca26dc85244259ff2b19c41b9"
+    "f96f3ca9ec1dde434da7d2d392b905ddf3d1f9af93d1af5950bd493f5aa731b4"
+    "056df31bd267b6b90a079831aaf579be0a39013137aac6d404f518cfd4684064"
+    "7e78bfe706ca4cf5e9c5453e9f7cfd2b8b4c8d169a44e55c88d4a9a7f9474241"
+    "e221af44860018ab0856972e194cd934"
 )
 
+# https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.3
 LONG_SERVER_PACKET_NUMBER = 1
 LONG_SERVER_PLAIN_HEADER = binascii.unhexlify(
-    "c1ff00001d0008f067a5502a4262b50040740001"
+    "c1000000010008f067a5502a4262b50040750001"
 )
 LONG_SERVER_PLAIN_PAYLOAD = binascii.unhexlify(
-    "0d0000000018410a020000560303eefce7f7b37ba1d1632e96677825ddf73988"
-    "cfc79825df566dc5430b9a045a1200130100002e00330024001d00209d3c940d"
-    "89690b84d08a60993c144eca684d1081287c834d5311bcf32bb9da1a002b0002"
-    "0304"
+    "02000000000600405a020000560303eefce7f7b37ba1d1632e96677825ddf739"
+    "88cfc79825df566dc5430b9a045a1200130100002e00330024001d00209d3c94"
+    "0d89690b84d08a60993c144eca684d1081287c834d5311bcf32bb9da1a002b00"
+    "020304"
 )
 LONG_SERVER_ENCRYPTED_PACKET = binascii.unhexlify(
-    "caff00001d0008f067a5502a4262b5004074aaf2f007823a5d3a1207c86ee491"
-    "32824f0465243d082d868b107a38092bc80528664cbf9456ebf27673fb5fa506"
-    "1ab573c9f001b81da028a00d52ab00b15bebaa70640e106cf2acd043e9c6b441"
-    "1c0a79637134d8993701fe779e58c2fe753d14b0564021565ea92e57bc6faf56"
-    "dfc7a40870e6"
+    "cf000000010008f067a5502a4262b5004075c0d95a482cd0991cd25b0aac406a"
+    "5816b6394100f37a1c69797554780bb38cc5a99f5ede4cf73c3ec2493a1839b3"
+    "dbcba3f6ea46c5b7684df3548e7ddeb9c3bf9c73cc3f3bded74b562bfb19fb84"
+    "022f8ef4cdd93795d77d06edbb7aaf2f58891850abbdca3d20398c276456cbc4"
+    "2158407dd074ee"
 )
 
 SHORT_SERVER_PACKET_NUMBER = 3
 SHORT_SERVER_PLAIN_HEADER = binascii.unhexlify("41b01fd24a586a9cf30003")
 SHORT_SERVER_PLAIN_PAYLOAD = binascii.unhexlify(
     "06003904000035000151805a4bebf5000020b098c8dc4183e4c182572e10ac3e"
     "2b88897e0524c8461847548bd2dffa2c0ae60008002a0004ffffffff"
@@ -110,58 +115,98 @@
 )
 
 
 class CryptoTest(TestCase):
     """
     Test vectors from:
 
-    https://datatracker.ietf.org/doc/html/draft-ietf-quic-tls-18#appendix-A
+    https://datatracker.ietf.org/doc/html/rfc9001#appendix-A
     """
 
     def create_crypto(self, is_client):
         pair = CryptoPair()
         pair.setup_initial(
             cid=binascii.unhexlify("8394c8f03e515708"),
             is_client=is_client,
             version=PROTOCOL_VERSION,
         )
         return pair
 
+    def create_aead(
+        self,
+        cipher_name: bytes = CIPHER_SUITES[INITIAL_CIPHER_SUITE][1],
+        key: bytes = b"topsecret16bytes",
+        iv: bytes = b"12!nullbytes",
+    ) -> AEAD:
+        return AEAD(cipher_name, key, iv)
+
+    def create_hp(
+        self,
+        cipher_name: bytes = CIPHER_SUITES[INITIAL_CIPHER_SUITE][0],
+        key: bytes = b"topsecret16bytes",
+    ) -> HeaderProtection:
+        return HeaderProtection(cipher_name, key)
+
     def test_derive_key_iv_hp(self):
+        # https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.1
+
         # client
         secret = binascii.unhexlify(
-            "8a3515a14ae3c31b9c2d6d5bc58538ca5cd2baa119087143e60887428dcb52f6"
+            "c00cf151ca5be075ed0ebfb5c80323c42d6b7db67881289af4008f1f6c357aea"
         )
         key, iv, hp = derive_key_iv_hp(INITIAL_CIPHER_SUITE, secret)
-        self.assertEqual(key, binascii.unhexlify("98b0d7e5e7a402c67c33f350fa65ea54"))
-        self.assertEqual(iv, binascii.unhexlify("19e94387805eb0b46c03a788"))
-        self.assertEqual(hp, binascii.unhexlify("0edd982a6ac527f2eddcbb7348dea5d7"))
+        self.assertEqual(key, binascii.unhexlify("1f369613dd76d5467730efcbe3b1a22d"))
+        self.assertEqual(iv, binascii.unhexlify("fa044b2f42a3fd3b46fb255c"))
+        self.assertEqual(hp, binascii.unhexlify("9f50449e04a0e810283a1e9933adedd2"))
 
         # server
         secret = binascii.unhexlify(
-            "47b2eaea6c266e32c0697a9e2a898bdf5c4fb3e5ac34f0e549bf2c58581a3811"
+            "3c199828fd139efd216c155ad844cc81fb82fa8d7446fa7d78be803acdda951b"
         )
         key, iv, hp = derive_key_iv_hp(INITIAL_CIPHER_SUITE, secret)
-        self.assertEqual(key, binascii.unhexlify("9a8be902a9bdd91d16064ca118045fb4"))
-        self.assertEqual(iv, binascii.unhexlify("0a82086d32205ba22241d8dc"))
-        self.assertEqual(hp, binascii.unhexlify("94b9452d2b3c7c7f6da7fdd8593537fd"))
+        self.assertEqual(key, binascii.unhexlify("cf3a5331653c364c88f0f379b6067e37"))
+        self.assertEqual(iv, binascii.unhexlify("0ac1493ca1905853b0bba03e"))
+        self.assertEqual(hp, binascii.unhexlify("c206b8d9b9f0f37644430b490eeaa314"))
+
+    @skipIf("chacha20" in SKIP_TESTS, "Skipping chacha20 tests")
+    def test_derive_key_iv_hp_chacha20(self):
+        # https://datatracker.ietf.org/doc/html/rfc9001#appendix-A.5
+
+        # server
+        secret = binascii.unhexlify(
+            "9ac312a7f877468ebe69422748ad00a15443f18203a07d6060f688f30f21632b"
+        )
+        key, iv, hp = derive_key_iv_hp(CipherSuite.CHACHA20_POLY1305_SHA256, secret)
+        self.assertEqual(
+            key,
+            binascii.unhexlify(
+                "c6d98ff3441c3fe1b2182094f69caa2ed4b716b65488960a7a984979fb23e1c8"
+            ),
+        )
+        self.assertEqual(iv, binascii.unhexlify("e0459b3474bdd0e44a41c144"))
+        self.assertEqual(
+            hp,
+            binascii.unhexlify(
+                "25a282b9e82f06f21f488917a4fc8f1b73573685608597d0efcb076b0ab7a7a4"
+            ),
+        )
 
     @skipIf("chacha20" in SKIP_TESTS, "Skipping chacha20 tests")
     def test_decrypt_chacha20(self):
         pair = CryptoPair()
         pair.recv.setup(
             cipher_suite=CipherSuite.CHACHA20_POLY1305_SHA256,
             secret=binascii.unhexlify(
-                "b42772df33c9719a32820d302aa664d080d7f5ea7a71a330f87864cb289ae8c0"
+                "9ac312a7f877468ebe69422748ad00a15443f18203a07d6060f688f30f21632b"
             ),
             version=PROTOCOL_VERSION,
         )
 
         plain_header, plain_payload, packet_number = pair.decrypt_packet(
-            CHACHA20_CLIENT_ENCRYPTED_PACKET, 25, 0
+            CHACHA20_CLIENT_ENCRYPTED_PACKET, 1, CHACHA20_CLIENT_PACKET_NUMBER
         )
         self.assertEqual(plain_header, CHACHA20_CLIENT_PLAIN_HEADER)
         self.assertEqual(plain_payload, CHACHA20_CLIENT_PLAIN_PAYLOAD)
         self.assertEqual(packet_number, CHACHA20_CLIENT_PACKET_NUMBER)
 
     def test_decrypt_long_client(self):
         pair = self.create_crypto(is_client=False)
@@ -207,15 +252,15 @@
 
     @skipIf("chacha20" in SKIP_TESTS, "Skipping chacha20 tests")
     def test_encrypt_chacha20(self):
         pair = CryptoPair()
         pair.send.setup(
             cipher_suite=CipherSuite.CHACHA20_POLY1305_SHA256,
             secret=binascii.unhexlify(
-                "b42772df33c9719a32820d302aa664d080d7f5ea7a71a330f87864cb289ae8c0"
+                "9ac312a7f877468ebe69422748ad00a15443f18203a07d6060f688f30f21632b"
             ),
             version=PROTOCOL_VERSION,
         )
 
         packet = pair.encrypt_packet(
             CHACHA20_CLIENT_PLAIN_HEADER,
             CHACHA20_CLIENT_PLAIN_PAYLOAD,
@@ -313,7 +358,86 @@
         pair1.update_key()
 
         # roundtrip
         send(pair2, pair1, 3)
         send(pair1, pair2, 3)
         self.assertEqual(pair1.key_phase, 1)
         self.assertEqual(pair2.key_phase, 1)
+
+    def test_aead_init_args_validation(self):
+        # invalid cipher
+        with self.assertRaises(CryptoError) as cm:
+            self.create_aead(cipher_name=b"tango9000")
+        self.assertEqual(str(cm.exception), "Invalid cipher name: tango9000")
+
+        # invalid key length
+        with self.assertRaises(CryptoError) as cm:
+            self.create_aead(key=bytes(33))
+        self.assertEqual(str(cm.exception), "Invalid key length")
+
+        # invalid iv length
+        with self.assertRaises(CryptoError) as cm:
+            self.create_aead(iv=bytes(11))
+        self.assertEqual(str(cm.exception), "Invalid iv length")
+        with self.assertRaises(CryptoError) as cm:
+            self.create_aead(iv=bytes(13))
+        self.assertEqual(str(cm.exception), "Invalid iv length")
+
+    def test_aead_data_length_validation(self):
+        aead = self.create_aead()
+        iv = aead._iv
+        zero_nonce = bytes(12)
+
+        # too large for encrypt, early abort
+        self.assertEqual(bytes(aead._nonce), zero_nonce)
+        with self.assertRaises(CryptoError) as cm:
+            aead.encrypt(bytes(1501), associated_data=b"", packet_number=0)
+        self.assertEqual(str(cm.exception), "Invalid payload length")
+        self.assertEqual(bytes(aead._nonce), zero_nonce)
+
+        # too large for encrypt, late tag check
+        with self.assertRaises(CryptoError) as cm:
+            aead.encrypt(bytes(1500), associated_data=b"", packet_number=0)
+        self.assertEqual(str(cm.exception), "Invalid payload length")
+        self.assertEqual(bytes(aead._nonce), iv)
+
+        # too small for decrypt
+        with self.assertRaises(CryptoError) as cm:
+            aead.decrypt(bytes(11), associated_data=b"", packet_number=0)
+        self.assertEqual(str(cm.exception), "Invalid payload length")
+
+        # too large for decrypt
+        with self.assertRaises(CryptoError) as cm:
+            aead.decrypt(bytes(1501), associated_data=b"", packet_number=0)
+        self.assertEqual(str(cm.exception), "Invalid payload length")
+
+    def test_hp_init_args_validation(self):
+        # invalid cipher
+        with self.assertRaises(CryptoError) as cm:
+            self.create_hp(cipher_name=b"tango9000")
+        self.assertEqual(str(cm.exception), "Invalid cipher name: tango9000")
+
+        # invalid key length
+        with self.assertRaises(CryptoError) as cm:
+            self.create_hp(key=bytes(33))
+        self.assertEqual(str(cm.exception), "Invalid key length")
+
+    def test_hp_data_length_validation(self):
+        hp = self.create_hp()
+
+        # too large for apply
+        with self.assertRaises(CryptoError) as cm:
+            hp.apply(plain_header=bytes(501), protected_payload=bytes(1000))
+        self.assertEqual(str(cm.exception), "Invalid payload length")
+
+        # too large for remove
+        with self.assertRaises(CryptoError) as cm:
+            hp.remove(packet=bytes(1501), encrypted_offset=0)
+        self.assertEqual(str(cm.exception), "Invalid payload length")
+
+    def test_handle_openssl_failure(self):
+        # ensure errors are cleared
+        aead = self.create_aead()
+        with patch.object(aead._binding.lib, "ERR_clear_error") as mock:
+            with self.assertRaises(CryptoError):
+                aead._handle_openssl_failure()
+            mock.assert_called_once()
```

### Comparing `qh3-0.10.0/tests/test_h0.py` & `qh3-0.11.0/tests/test_h0.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_h3.py` & `qh3-0.11.0/tests/test_h3.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_logger.py` & `qh3-0.11.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_packet.py` & `qh3-0.11.0/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_packet_builder.py` & `qh3-0.11.0/tests/test_packet_builder.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_rangeset.py` & `qh3-0.11.0/tests/test_rangeset.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_recovery.py` & `qh3-0.11.0/tests/test_recovery.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_retry.py` & `qh3-0.11.0/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_stream.py` & `qh3-0.11.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_tls.py` & `qh3-0.11.0/tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/test_webtransport.py` & `qh3-0.11.0/tests/test_webtransport.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/tls_certificate.bin` & `qh3-0.11.0/tests/tls_certificate.bin`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/tests/utils.py` & `qh3-0.11.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/.travis.yml` & `qh3-0.11.0/vendor/ls-qpack/.travis.yml`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/CMakeLists.txt` & `qh3-0.11.0/vendor/ls-qpack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/LICENSE` & `qh3-0.11.0/vendor/ls-qpack/LICENSE`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/README.md` & `qh3-0.11.0/vendor/ls-qpack/README.md`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/bin/CMakeLists.txt` & `qh3-0.11.0/vendor/ls-qpack/bin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/bin/encode-int.c` & `qh3-0.11.0/vendor/ls-qpack/bin/encode-int.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/bin/fuzz-decode.c` & `qh3-0.11.0/vendor/ls-qpack/bin/fuzz-decode.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/bin/interop-decode.c` & `qh3-0.11.0/vendor/ls-qpack/bin/interop-decode.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/bin/interop-encode.c` & `qh3-0.11.0/vendor/ls-qpack/bin/interop-encode.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/deps/xxhash/xxhash.c` & `qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/deps/xxhash/xxhash.h` & `qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.h`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/fuzz/decode/b/preamble` & `qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/preamble`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/preamble` & `qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/preamble`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack` & `qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1` & `qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1` & `qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1` & `qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/huff-tables.h` & `qh3-0.11.0/vendor/ls-qpack/huff-tables.h`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/lsqpack.c` & `qh3-0.11.0/vendor/ls-qpack/lsqpack.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/lsqpack.h` & `qh3-0.11.0/vendor/ls-qpack/lsqpack.h`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/CMakeLists.txt` & `qh3-0.11.0/vendor/ls-qpack/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/lsqpack-test.h` & `qh3-0.11.0/vendor/ls-qpack/test/lsqpack-test.h`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/qifs/fb-req.qif` & `qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-req.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/qifs/fb-resp.qif` & `qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-resp.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/qifs/long-codes.qif` & `qh3-0.11.0/vendor/ls-qpack/test/qifs/long-codes.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/qifs/netbsd.qif` & `qh3-0.11.0/vendor/ls-qpack/test/qifs/netbsd.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/run-qif.pl` & `qh3-0.11.0/vendor/ls-qpack/test/run-qif.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/run-scenario.sh` & `qh3-0.11.0/vendor/ls-qpack/test/run-scenario.sh`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/scenarios/drain-2.sce` & `qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain-2.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/scenarios/drain.sce` & `qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce` & `qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce` & `qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/test_enc_str.c` & `qh3-0.11.0/vendor/ls-qpack/test/test_enc_str.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/test_get_stx_id.c` & `qh3-0.11.0/vendor/ls-qpack/test/test_get_stx_id.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/test_huff_dec.c` & `qh3-0.11.0/vendor/ls-qpack/test/test_huff_dec.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/test_int.c` & `qh3-0.11.0/vendor/ls-qpack/test/test_int.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/test_qpack.c` & `qh3-0.11.0/vendor/ls-qpack/test/test_qpack.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/test/test_read_enc_stream.c` & `qh3-0.11.0/vendor/ls-qpack/test/test_read_enc_stream.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/tools/har2qif.pl` & `qh3-0.11.0/vendor/ls-qpack/tools/har2qif.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/tools/randomize-cookies.pl` & `qh3-0.11.0/vendor/ls-qpack/tools/randomize-cookies.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/tools/sort-qif.pl` & `qh3-0.11.0/vendor/ls-qpack/tools/sort-qif.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/wincompat/getopt.c` & `qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/wincompat/getopt.h` & `qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.h`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/wincompat/getopt1.c` & `qh3-0.11.0/vendor/ls-qpack/wincompat/getopt1.c`

 * *Files identical despite different names*

### Comparing `qh3-0.10.0/vendor/ls-qpack/wincompat/sys/queue.h` & `qh3-0.11.0/vendor/ls-qpack/wincompat/sys/queue.h`

 * *Files identical despite different names*

