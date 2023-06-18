# Comparing `tmp/qh3-0.11.0.tar.gz` & `tmp/qh3-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/qh3/qh3/dist/.tmp-vickcz8k/qh3-0.11.0.tar", last modified: Sun Jun 18 14:51:39 2023, max compression
+gzip compressed data, was "/home/runner/work/qh3/qh3/dist/.tmp-lhsmg66x/qh3-0.11.1.tar", last modified: Sun Jun 18 15:22:56 2023, max compression
```

## Comparing `qh3-0.11.0.tar` & `qh3-0.11.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-18 14:51:28.000000 qh3-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-18 14:51:28.000000 qh3-0.11.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-18 14:51:39.000000 qh3-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-18 14:51:28.000000 qh3-0.11.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/h3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-18 14:51:28.000000 qh3-0.11.0/docs/quic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-18 14:51:28.000000 qh3-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:51:39.000000 qh3-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-18 14:51:28.000000 qh3-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/_vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/_vendor/OpenSSL/
--rw-r--r--   0 runner    (1001) docker     (123)   111333 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/OpenSSL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/_vendor/pylsqpack/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/pylsqpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/_vendor/pylsqpack/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/asyncio/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/h0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h0/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/h3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39189 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/h3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3/quic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)   122411 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/quic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    72691 2023-06-18 14:51:28.000000 qh3-0.11.0/src/qh3/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 14:51:39.000000 qh3-0.11.0/src/qh3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/initial_client.bin
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/initial_server.bin
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/pycacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/retry.bin
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/retry_draft_29.bin
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/short_header.bin
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_cert_with_chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_combined.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/ssl_key.pem
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)   115714 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_crypto_draft_29.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_h0.py
--rw-r--r--   0 runner    (1001) docker     (123)    63162 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_h3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_rangeset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/test_webtransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_certificate.bin
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_certificate_verify.bin
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello.bin
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello_with_alpn.bin
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello_with_psk.bin
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_client_hello_with_sni.bin
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_encrypted_extensions.bin
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_encrypted_extensions_with_alpn.bin
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_encrypted_extensions_with_alpn_and_early_data.bin
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_finished.bin
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_new_session_ticket.bin
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_new_session_ticket_with_unknown_extension.bin
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_server_hello.bin
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_server_hello_with_psk.bin
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/tls_server_hello_with_unknown_extension.bin
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 14:51:28.000000 qh3-0.11.0/tests/version_negotiation.bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.git
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/encode-int.c
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/fuzz-decode.c
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/interop-decode.c
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/bin/interop-encode.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/deps/xxhash/
--rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/README
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/preamble
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000390,op_havoc,rep_4
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000579,op_flip1,pos_14
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,src_000000,op_flip2,pos_12
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000001,sig_11,src_000579,op_havoc,rep_4
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,sig_11,src_000481,op_int16,pos_15,val_-1
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,src_000000,op_havoc,rep_8
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000006,src_000285,op_flip2,pos_14
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000008,src_000285,op_flip2,pos_20
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000010,src_000306,op_flip2,pos_75
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000011,src_000344,op_havoc,rep_2
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000014,src_000366,op_flip2,pos_28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/README
--rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/preamble
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/test-cases/seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/c/test-cases/fb-req.qif.proxygen.out.256.100.0-chopped
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/
--rw-r--r--   0 runner    (1001) docker     (123)    59117 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/preamble
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/test-cases/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1
--rw-r--r--   0 runner    (1001) docker     (123)  4372759 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/huff-tables.h
--rw-r--r--   0 runner    (1001) docker     (123)   185368 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/lsqpack.c
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/lsqpack.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/lsqpack-test.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/
--rw-r--r--   0 runner    (1001) docker     (123)   235326 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-req.qif
--rw-r--r--   0 runner    (1001) docker     (123)   351937 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-resp.qif
--rw-r--r--   0 runner    (1001) docker     (123)   158092 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/long-codes.qif
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/qifs/netbsd.qif
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/run-qif.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1529 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/run-scenario.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/0.95-reset.sce
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/cancel-stream.sce
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain.sce
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/end-dst-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/end-dst.sce
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/incl-name.sce
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/post-base-1.sce
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/post-base-2.sce
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/post-base-nr.sce
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/scenarios/set-max-cap.sce
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_enc_str.c
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_get_stx_id.c
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_huff_dec.c
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_int.c
--rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_qpack.c
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/test/test_read_enc_stream.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/tools/har2qif.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/tools/randomize-cookies.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/tools/sort-qif.pl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/
--rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.c
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.h
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/getopt1.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:51:39.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/sys/
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-06-18 14:51:29.000000 qh3-0.11.0/vendor/ls-qpack/wincompat/sys/queue.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-18 15:22:46.000000 qh3-0.11.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-18 15:22:46.000000 qh3-0.11.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-18 15:22:56.000000 qh3-0.11.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-18 15:22:46.000000 qh3-0.11.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/h3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-18 15:22:46.000000 qh3-0.11.1/docs/quic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-18 15:22:46.000000 qh3-0.11.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:22:56.000000 qh3-0.11.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-18 15:22:46.000000 qh3-0.11.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/_vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/_vendor/OpenSSL/
+-rw-r--r--   0 runner    (1001) docker     (123)   111333 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/_vendor/OpenSSL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/_vendor/pylsqpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/_vendor/pylsqpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18318 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/_vendor/pylsqpack/binding.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/asyncio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/asyncio/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/h0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/h0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/h0/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/h3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/h3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39189 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/h3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/h3/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/h3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3/quic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122411 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/quic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72829 2023-06-18 15:22:46.000000 qh3-0.11.1/src/qh3/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 15:22:56.000000 qh3-0.11.1/src/qh3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/initial_client.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/initial_server.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/pycacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/retry.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/retry_draft_29.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/short_header.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/ssl_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/ssl_cert_with_chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/ssl_combined.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/ssl_key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115714 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_crypto_draft_29.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_h0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63162 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_h3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/test_webtransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_certificate.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_certificate_verify.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_client_hello.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_client_hello_with_alpn.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_client_hello_with_psk.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_client_hello_with_sni.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_encrypted_extensions.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_encrypted_extensions_with_alpn.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_encrypted_extensions_with_alpn_and_early_data.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_finished.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_new_session_ticket.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_new_session_ticket_with_unknown_extension.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_server_hello.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_server_hello_with_psk.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/tls_server_hello_with_unknown_extension.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 15:22:46.000000 qh3-0.11.1/tests/version_negotiation.bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 15:22:46.000000 qh3-0.11.1/vendor/ls-qpack/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/bin/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/bin/encode-int.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/bin/fuzz-decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/bin/interop-decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/bin/interop-encode.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/deps/xxhash/
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/deps/xxhash/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/deps/xxhash/xxhash.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/README
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/preamble
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000390,op_havoc,rep_4
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,sig_06,src_000579,op_flip1,pos_14
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000000,src_000000,op_flip2,pos_12
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000001,sig_11,src_000579,op_havoc,rep_4
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,sig_11,src_000481,op_int16,pos_15,val_-1
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000002,src_000000,op_havoc,rep_8
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000006,src_000285,op_flip2,pos_14
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000008,src_000285,op_flip2,pos_20
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000010,src_000306,op_flip2,pos_75
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000011,src_000344,op_havoc,rep_2
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/a/test-cases/id_000014,src_000366,op_flip2,pos_28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/b/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/b/README
+-rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/b/preamble
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/b/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/b/test-cases/seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/c/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/c/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/c/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/c/test-cases/fb-req.qif.proxygen.out.256.100.0-chopped
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/
+-rw-r--r--   0 runner    (1001) docker     (123)    59117 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/preamble
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/test-cases/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1
+-rw-r--r--   0 runner    (1001) docker     (123)  4372759 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/huff-tables.h
+-rw-r--r--   0 runner    (1001) docker     (123)   185368 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/lsqpack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/lsqpack.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/lsqpack-test.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/test/qifs/
+-rw-r--r--   0 runner    (1001) docker     (123)   235326 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/qifs/fb-req.qif
+-rw-r--r--   0 runner    (1001) docker     (123)   351937 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/qifs/fb-resp.qif
+-rw-r--r--   0 runner    (1001) docker     (123)   158092 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/qifs/long-codes.qif
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/qifs/netbsd.qif
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/run-qif.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1529 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/run-scenario.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/0.95-reset.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/cancel-stream.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/drain-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/drain.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/end-dst-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/end-dst.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/incl-name.sce
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/post-base-1.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/post-base-2.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/post-base-nr.sce
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/scenarios/set-max-cap.sce
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/test_enc_str.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/test_get_stx_id.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/test_huff_dec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/test_int.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24907 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/test_qpack.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/test/test_read_enc_stream.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/tools/har2qif.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/tools/randomize-cookies.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/tools/sort-qif.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/wincompat/
+-rw-r--r--   0 runner    (1001) docker     (123)    23097 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/wincompat/getopt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/wincompat/getopt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/wincompat/getopt1.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:22:56.000000 qh3-0.11.1/vendor/ls-qpack/wincompat/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-06-18 15:22:48.000000 qh3-0.11.1/vendor/ls-qpack/wincompat/sys/queue.h
```

### Comparing `qh3-0.11.0/LICENSE` & `qh3-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/PKG-INFO` & `qh3-0.11.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qh3
-Version: 0.11.0
+Version: 0.11.1
 Summary: An implementation of QUIC and HTTP/3
 Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/Ousret/qh3
 Project-URL: documentation, https://aioquic.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qh3-0.11.0/README.rst` & `qh3-0.11.1/README.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/Makefile` & `qh3-0.11.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/asyncio.rst` & `qh3-0.11.1/docs/asyncio.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/conf.py` & `qh3-0.11.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/design.rst` & `qh3-0.11.1/docs/design.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/h3.rst` & `qh3-0.11.1/docs/h3.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/index.rst` & `qh3-0.11.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/docs/quic.rst` & `qh3-0.11.1/docs/quic.rst`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/pyproject.toml` & `qh3-0.11.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/setup.py` & `qh3-0.11.1/setup.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/_buffer.c` & `qh3-0.11.1/src/qh3/_buffer.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/_crypto.py` & `qh3-0.11.1/src/qh3/_crypto.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/_vendor/OpenSSL/__init__.py` & `qh3-0.11.1/src/qh3/_vendor/OpenSSL/__init__.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/_vendor/pylsqpack/binding.c` & `qh3-0.11.1/src/qh3/_vendor/pylsqpack/binding.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/asyncio/client.py` & `qh3-0.11.1/src/qh3/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/asyncio/protocol.py` & `qh3-0.11.1/src/qh3/asyncio/protocol.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/asyncio/server.py` & `qh3-0.11.1/src/qh3/asyncio/server.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/buffer.py` & `qh3-0.11.1/src/qh3/buffer.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/h0/connection.py` & `qh3-0.11.1/src/qh3/h0/connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/h3/connection.py` & `qh3-0.11.1/src/qh3/h3/connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/h3/events.py` & `qh3-0.11.1/src/qh3/h3/events.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/configuration.py` & `qh3-0.11.1/src/qh3/quic/configuration.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/connection.py` & `qh3-0.11.1/src/qh3/quic/connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/crypto.py` & `qh3-0.11.1/src/qh3/quic/crypto.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/events.py` & `qh3-0.11.1/src/qh3/quic/events.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/logger.py` & `qh3-0.11.1/src/qh3/quic/logger.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/packet.py` & `qh3-0.11.1/src/qh3/quic/packet.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/packet_builder.py` & `qh3-0.11.1/src/qh3/quic/packet_builder.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/rangeset.py` & `qh3-0.11.1/src/qh3/quic/rangeset.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/recovery.py` & `qh3-0.11.1/src/qh3/quic/recovery.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/retry.py` & `qh3-0.11.1/src/qh3/quic/retry.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/quic/stream.py` & `qh3-0.11.1/src/qh3/quic/stream.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/src/qh3/tls.py` & `qh3-0.11.1/src/qh3/tls.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,14 +394,16 @@
             if attr.oid == x509.NameOID.COMMON_NAME:
                 subject.append((("commonName", attr.value),))
         for ext in certificate.extensions:
             if isinstance(ext.value, x509.SubjectAlternativeName):
                 for name in ext.value:
                     if isinstance(name, x509.DNSName):
                         subjectAltName.append(("DNS", name.value))
+                    elif isinstance(name, x509.IPAddress):
+                        subjectAltName.append(("IP Address", str(name.value)))
 
         try:
             match_hostname(
                 tuple(subject),
                 tuple(subjectAltName),
                 server_name,
                 hostname_checks_common_name=not bool(subjectAltName),
```

### Comparing `qh3-0.11.0/src/qh3.egg-info/PKG-INFO` & `qh3-0.11.1/src/qh3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qh3
-Version: 0.11.0
+Version: 0.11.1
 Summary: An implementation of QUIC and HTTP/3
 Author-email: Jeremy Lainé <jeremy.laine@m4x.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/Ousret/qh3
 Project-URL: documentation, https://aioquic.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qh3-0.11.0/src/qh3.egg-info/SOURCES.txt` & `qh3-0.11.1/src/qh3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/initial_client.bin` & `qh3-0.11.1/tests/initial_client.bin`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/pycacert.pem` & `qh3-0.11.1/tests/pycacert.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/ssl_cert.pem` & `qh3-0.11.1/tests/ssl_cert.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/ssl_cert_with_chain.pem` & `qh3-0.11.1/tests/ssl_cert_with_chain.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/ssl_combined.pem` & `qh3-0.11.1/tests/ssl_combined.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/ssl_key.pem` & `qh3-0.11.1/tests/ssl_key.pem`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_asyncio.py` & `qh3-0.11.1/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_buffer.py` & `qh3-0.11.1/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_connection.py` & `qh3-0.11.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_crypto.py` & `qh3-0.11.1/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_crypto_draft_29.py` & `qh3-0.11.1/tests/test_crypto_draft_29.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_h0.py` & `qh3-0.11.1/tests/test_h0.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_h3.py` & `qh3-0.11.1/tests/test_h3.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_logger.py` & `qh3-0.11.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_packet.py` & `qh3-0.11.1/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_packet_builder.py` & `qh3-0.11.1/tests/test_packet_builder.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_rangeset.py` & `qh3-0.11.1/tests/test_rangeset.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_recovery.py` & `qh3-0.11.1/tests/test_recovery.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_retry.py` & `qh3-0.11.1/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_stream.py` & `qh3-0.11.1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_tls.py` & `qh3-0.11.1/tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/test_webtransport.py` & `qh3-0.11.1/tests/test_webtransport.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/tls_certificate.bin` & `qh3-0.11.1/tests/tls_certificate.bin`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/tests/utils.py` & `qh3-0.11.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/.travis.yml` & `qh3-0.11.1/vendor/ls-qpack/.travis.yml`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/CMakeLists.txt` & `qh3-0.11.1/vendor/ls-qpack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/LICENSE` & `qh3-0.11.1/vendor/ls-qpack/LICENSE`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/README.md` & `qh3-0.11.1/vendor/ls-qpack/README.md`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/bin/CMakeLists.txt` & `qh3-0.11.1/vendor/ls-qpack/bin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/bin/encode-int.c` & `qh3-0.11.1/vendor/ls-qpack/bin/encode-int.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/bin/fuzz-decode.c` & `qh3-0.11.1/vendor/ls-qpack/bin/fuzz-decode.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/bin/interop-decode.c` & `qh3-0.11.1/vendor/ls-qpack/bin/interop-decode.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/bin/interop-encode.c` & `qh3-0.11.1/vendor/ls-qpack/bin/interop-encode.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.c` & `qh3-0.11.1/vendor/ls-qpack/deps/xxhash/xxhash.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/deps/xxhash/xxhash.h` & `qh3-0.11.1/vendor/ls-qpack/deps/xxhash/xxhash.h`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/fuzz/decode/b/preamble` & `qh3-0.11.1/vendor/ls-qpack/fuzz/decode/b/preamble`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/preamble` & `qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/preamble`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack` & `qh3-0.11.1/vendor/ls-qpack/fuzz/decode/d/test-cases/fb-resp.minhq.256.128.0.ack`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1` & `qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/fb-req.out.256.100.1`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1` & `qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/fb-resp.out.256.100.1`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1` & `qh3-0.11.1/vendor/ls-qpack/fuzz/input/256.100.1/netbsd.out.256.100.1`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/huff-tables.h` & `qh3-0.11.1/vendor/ls-qpack/huff-tables.h`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/lsqpack.c` & `qh3-0.11.1/vendor/ls-qpack/lsqpack.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/lsqpack.h` & `qh3-0.11.1/vendor/ls-qpack/lsqpack.h`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/CMakeLists.txt` & `qh3-0.11.1/vendor/ls-qpack/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/lsqpack-test.h` & `qh3-0.11.1/vendor/ls-qpack/test/lsqpack-test.h`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-req.qif` & `qh3-0.11.1/vendor/ls-qpack/test/qifs/fb-req.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/qifs/fb-resp.qif` & `qh3-0.11.1/vendor/ls-qpack/test/qifs/fb-resp.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/qifs/long-codes.qif` & `qh3-0.11.1/vendor/ls-qpack/test/qifs/long-codes.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/qifs/netbsd.qif` & `qh3-0.11.1/vendor/ls-qpack/test/qifs/netbsd.qif`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/run-qif.pl` & `qh3-0.11.1/vendor/ls-qpack/test/run-qif.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/run-scenario.sh` & `qh3-0.11.1/vendor/ls-qpack/test/run-scenario.sh`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain-2.sce` & `qh3-0.11.1/vendor/ls-qpack/test/scenarios/drain-2.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/scenarios/drain.sce` & `qh3-0.11.1/vendor/ls-qpack/test/scenarios/drain.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce` & `qh3-0.11.1/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-1.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce` & `qh3-0.11.1/vendor/ls-qpack/test/scenarios/multi-byte-int-dyn-ref-2.sce`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/test_enc_str.c` & `qh3-0.11.1/vendor/ls-qpack/test/test_enc_str.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/test_get_stx_id.c` & `qh3-0.11.1/vendor/ls-qpack/test/test_get_stx_id.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/test_huff_dec.c` & `qh3-0.11.1/vendor/ls-qpack/test/test_huff_dec.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/test_int.c` & `qh3-0.11.1/vendor/ls-qpack/test/test_int.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/test_qpack.c` & `qh3-0.11.1/vendor/ls-qpack/test/test_qpack.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/test/test_read_enc_stream.c` & `qh3-0.11.1/vendor/ls-qpack/test/test_read_enc_stream.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/tools/har2qif.pl` & `qh3-0.11.1/vendor/ls-qpack/tools/har2qif.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/tools/randomize-cookies.pl` & `qh3-0.11.1/vendor/ls-qpack/tools/randomize-cookies.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/tools/sort-qif.pl` & `qh3-0.11.1/vendor/ls-qpack/tools/sort-qif.pl`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.c` & `qh3-0.11.1/vendor/ls-qpack/wincompat/getopt.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/wincompat/getopt.h` & `qh3-0.11.1/vendor/ls-qpack/wincompat/getopt.h`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/wincompat/getopt1.c` & `qh3-0.11.1/vendor/ls-qpack/wincompat/getopt1.c`

 * *Files identical despite different names*

### Comparing `qh3-0.11.0/vendor/ls-qpack/wincompat/sys/queue.h` & `qh3-0.11.1/vendor/ls-qpack/wincompat/sys/queue.h`

 * *Files identical despite different names*

