# Comparing `tmp/scylla-cqlsh-6.0.8.tar.gz` & `tmp/scylla-cqlsh-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scylla-cqlsh-6.0.8.tar", last modified: Tue Apr 18 11:29:35 2023, max compression
+gzip compressed data, was "scylla-cqlsh-6.0.9.tar", last modified: Thu May 11 08:55:46 2023, max compression
```

## Comparing `scylla-cqlsh-6.0.8.tar` & `scylla-cqlsh-6.0.9.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.582742 scylla-cqlsh-6.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.566741 scylla-cqlsh-6.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.570741 scylla-cqlsh-6.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/.github/workflows/build-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-18 11:29:35.582742 scylla-cqlsh-6.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/SCYLLA-VERSION-GEN
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.570741 scylla-cqlsh-6.0.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3062 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/bin/cqlsh
--rwxr-xr-x   0 runner    (1001) docker     (123)   110575 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/bin/cqlsh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.570741 scylla-cqlsh-6.0.8/cqlsh/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlsh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlsh/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   110575 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlsh/cqlsh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.574741 scylla-cqlsh-6.0.8/cqlshlib/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/cqlshlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/authproviderhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)  4376775 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/cqlshlib/copyutil.c
--rw-r--r--   0 runner    (1001) docker     (123)   113002 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/copyutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    57506 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/cql3handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/cqlhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/cqlshhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/displaying.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/helptopics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/pylexotron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/saferscanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/sslhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/cqlshlib/wcwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.566741 scylla-cqlsh-6.0.8/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.574741 scylla-cqlsh-6.0.8/dist/debian/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/changelog.template
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/control.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.574741 scylla-cqlsh-6.0.8/dist/debian/debian/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (123)      427 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.574741 scylla-cqlsh-6.0.8/dist/debian/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/debian/source/options
--rwxr-xr-x   0 runner    (1001) docker     (123)     1999 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/debian/debian_files_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.574741 scylla-cqlsh-6.0.8/dist/redhat/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/dist/redhat/scylla-cqlsh.spec
--rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/install-dependencies.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3921 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.578741 scylla-cqlsh-6.0.8/pylib/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/Dockerfile.ubuntu.py3
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/Dockerfile.ubuntu.py37
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/Dockerfile.ubuntu.py38
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/README.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)     4013 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cassandra-cqlsh-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.578741 scylla-cqlsh-6.0.8/pylib/cqlshlib/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/authproviderhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)   113002 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/copyutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    57506 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/cql3handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/cqlhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/cqlshhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/displaying.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/helptopics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/pylexotron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/saferscanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/sslhandling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.578741 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/ansi_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/basecase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/cassconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/reserved_keywords.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/run_cqlsh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.578741 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/complex_auth_provider
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/complex_auth_provider_creds
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/complex_auth_provider_with_pass
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/empty_example
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/full_plain_text_example
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/illegal_example
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/no_classname_example
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/partial_example
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/plain_text_full_creds
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/plain_text_partial_creds
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling_config/plain_text_partial_example
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_copyutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    41459 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_cql_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    51732 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_cqlsh_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    38690 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_cqlsh_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_keyspace_init.cql
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/test/winpty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/cqlshlib/wcwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pylib/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.582742 scylla-cqlsh-6.0.8/reloc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/reloc/build_deb.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/reloc/build_reloc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/reloc/build_rpm.sh
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.582742 scylla-cqlsh-6.0.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/scripts/create-relocatable-package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:29:35.582742 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 11:29:35.000000 scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-18 11:29:35.582742 scylla-cqlsh-6.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-04-18 11:29:23.000000 scylla-cqlsh-6.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.288189 scylla-cqlsh-6.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.264189 scylla-cqlsh-6.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.268189 scylla-cqlsh-6.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/.github/workflows/build-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-11 08:55:46.288189 scylla-cqlsh-6.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/SCYLLA-VERSION-GEN
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.268189 scylla-cqlsh-6.0.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3062 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/bin/cqlsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110575 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/bin/cqlsh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.268189 scylla-cqlsh-6.0.9/cqlsh/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlsh/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110575 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlsh/cqlsh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.276189 scylla-cqlsh-6.0.9/cqlshlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/cqlshlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/authproviderhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4376775 2023-05-11 08:55:45.000000 scylla-cqlsh-6.0.9/cqlshlib/copyutil.c
+-rw-r--r--   0 runner    (1001) docker     (123)   113002 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/copyutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57506 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/cql3handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/cqlhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/cqlshhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/displaying.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/helptopics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/pylexotron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/saferscanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/sslhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/cqlshlib/wcwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.264189 scylla-cqlsh-6.0.9/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.276189 scylla-cqlsh-6.0.9/dist/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/changelog.template
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/control.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.276189 scylla-cqlsh-6.0.9/dist/debian/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)      427 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.280189 scylla-cqlsh-6.0.9/dist/debian/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/debian/source/options
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1999 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/debian/debian_files_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.280189 scylla-cqlsh-6.0.9/dist/redhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/dist/redhat/scylla-cqlsh.spec
+-rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/install-dependencies.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3921 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.280189 scylla-cqlsh-6.0.9/pylib/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/Dockerfile.ubuntu.py3
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/Dockerfile.ubuntu.py37
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/Dockerfile.ubuntu.py38
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/README.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4013 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cassandra-cqlsh-tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.280189 scylla-cqlsh-6.0.9/pylib/cqlshlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/authproviderhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113002 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/copyutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57506 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/cql3handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/cqlhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/cqlshhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/displaying.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/helptopics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/pylexotron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/saferscanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/sslhandling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.284189 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/basecase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/cassconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/reserved_keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/run_cqlsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.284189 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/complex_auth_provider
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/complex_auth_provider_creds
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/complex_auth_provider_with_pass
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/empty_example
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/full_plain_text_example
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/illegal_example
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/no_classname_example
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/partial_example
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/plain_text_full_creds
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/plain_text_partial_creds
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling_config/plain_text_partial_example
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_copyutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41459 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_cql_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51732 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_cqlsh_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38690 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_cqlsh_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_keyspace_init.cql
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/test/winpty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/cqlshlib/wcwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pylib/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.284189 scylla-cqlsh-6.0.9/reloc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/reloc/build_deb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2174 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/reloc/build_reloc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/reloc/build_rpm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.284189 scylla-cqlsh-6.0.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2211 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/scripts/create-relocatable-package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:55:46.288189 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 08:55:46.000000 scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-11 08:55:46.288189 scylla-cqlsh-6.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-05-11 08:55:26.000000 scylla-cqlsh-6.0.9/setup.py
```

### Comparing `scylla-cqlsh-6.0.8/.github/workflows/build-push.yml` & `scylla-cqlsh-6.0.9/.github/workflows/build-push.yml`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/LICENSE.txt` & `scylla-cqlsh-6.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/PKG-INFO` & `scylla-cqlsh-6.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scylla-cqlsh
-Version: 6.0.8
+Version: 6.0.9
 Summary: cqlsh is a Python-based command-line client for running CQL commands on a scylla cluster.
 Home-page: https://github.com/scylladb/scylla-cqlsh
 Author: Israel Fruchter
 Author-email: fruch@scylladb.com
 License: Apache
 Project-URL: Changelog, https://github.com/scylladb/scylla-cqlsh#changelog
 Project-URL: Documentation, https://cassandra.apache.org/doc/latest/tools/cqlsh.html
```

### Comparing `scylla-cqlsh-6.0.8/README.md` & `scylla-cqlsh-6.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/SCYLLA-VERSION-GEN` & `scylla-cqlsh-6.0.9/SCYLLA-VERSION-GEN`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/bin/cqlsh` & `scylla-cqlsh-6.0.9/bin/cqlsh`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/bin/cqlsh.py` & `scylla-cqlsh-6.0.9/bin/cqlsh.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlsh/cqlsh.py` & `scylla-cqlsh-6.0.9/cqlsh/cqlsh.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/__init__.py` & `scylla-cqlsh-6.0.9/cqlshlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,7 +69,22 @@
     @classmethod
     def after_table_cql(cls, table_meta, ext_key, ext_blob):
         # For scylla_tags, the blob is actually 
         # a serialized unorderd_map<string, string>. 
         mer = MapExtensionReader(ext_blob)
         return "%s = %s" % (ext_key, mer.read_map())
 
+
+# Add a handler for scylla_encryption_options extension to at least print
+# the info when doing "desc <table>".
+#
+# The end result will not be cut-and-paste usable; we'd need to modify the
+# driver for this. But it is something.
+class Encr(RegisteredTableExtension):
+    name = 'scylla_encryption_options'
+
+    @classmethod
+    def after_table_cql(cls, table_meta, ext_key, ext_blob):
+        # For scylla_encryption_options, the blob is actually
+        # a serialized unorderd_map<string, string>.
+        mer = MapExtensionReader(ext_blob)
+        return "%s = %s" % (ext_key, mer.read_map())
```

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/authproviderhandling.py` & `scylla-cqlsh-6.0.9/cqlshlib/authproviderhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/copyutil.c` & `scylla-cqlsh-6.0.9/cqlshlib/copyutil.c`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/copyutil.py` & `scylla-cqlsh-6.0.9/cqlshlib/copyutil.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/cql3handling.py` & `scylla-cqlsh-6.0.9/cqlshlib/cql3handling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/cqlhandling.py` & `scylla-cqlsh-6.0.9/cqlshlib/cqlhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/cqlshhandling.py` & `scylla-cqlsh-6.0.9/cqlshlib/cqlshhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/displaying.py` & `scylla-cqlsh-6.0.9/cqlshlib/displaying.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/formatting.py` & `scylla-cqlsh-6.0.9/cqlshlib/formatting.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/helptopics.py` & `scylla-cqlsh-6.0.9/cqlshlib/helptopics.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/pylexotron.py` & `scylla-cqlsh-6.0.9/cqlshlib/pylexotron.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/saferscanner.py` & `scylla-cqlsh-6.0.9/cqlshlib/saferscanner.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/sslhandling.py` & `scylla-cqlsh-6.0.9/cqlshlib/sslhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/tracing.py` & `scylla-cqlsh-6.0.9/cqlshlib/tracing.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/util.py` & `scylla-cqlsh-6.0.9/cqlshlib/util.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/cqlshlib/wcwidth.py` & `scylla-cqlsh-6.0.9/cqlshlib/wcwidth.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/dist/debian/debian/copyright` & `scylla-cqlsh-6.0.9/dist/debian/debian/copyright`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/dist/debian/debian_files_gen.py` & `scylla-cqlsh-6.0.9/dist/debian/debian_files_gen.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/dist/redhat/scylla-cqlsh.spec` & `scylla-cqlsh-6.0.9/dist/redhat/scylla-cqlsh.spec`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/install.sh` & `scylla-cqlsh-6.0.9/install.sh`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/README.asc` & `scylla-cqlsh-6.0.9/pylib/README.asc`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cassandra-cqlsh-tests.sh` & `scylla-cqlsh-6.0.9/pylib/cassandra-cqlsh-tests.sh`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/__init__.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,7 +69,22 @@
     @classmethod
     def after_table_cql(cls, table_meta, ext_key, ext_blob):
         # For scylla_tags, the blob is actually 
         # a serialized unorderd_map<string, string>. 
         mer = MapExtensionReader(ext_blob)
         return "%s = %s" % (ext_key, mer.read_map())
 
+
+# Add a handler for scylla_encryption_options extension to at least print
+# the info when doing "desc <table>".
+#
+# The end result will not be cut-and-paste usable; we'd need to modify the
+# driver for this. But it is something.
+class Encr(RegisteredTableExtension):
+    name = 'scylla_encryption_options'
+
+    @classmethod
+    def after_table_cql(cls, table_meta, ext_key, ext_blob):
+        # For scylla_encryption_options, the blob is actually
+        # a serialized unorderd_map<string, string>.
+        mer = MapExtensionReader(ext_blob)
+        return "%s = %s" % (ext_key, mer.read_map())
```

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/authproviderhandling.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/authproviderhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/copyutil.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/copyutil.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/cql3handling.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/cql3handling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/cqlhandling.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/cqlhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/cqlshhandling.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/cqlshhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/displaying.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/displaying.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/formatting.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/formatting.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/helptopics.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/helptopics.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/pylexotron.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/pylexotron.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/saferscanner.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/saferscanner.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/sslhandling.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/sslhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/__init__.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/ansi_colors.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/ansi_colors.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/basecase.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/basecase.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/cassconnect.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/cassconnect.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/run_cqlsh.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/run_cqlsh.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_authproviderhandling.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_authproviderhandling.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_constants.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_constants.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_copyutil.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_copyutil.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_cql_parsing.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_cql_parsing.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_cqlsh_completion.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_cqlsh_completion.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_cqlsh_output.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_cqlsh_output.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_keyspace_init.cql` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_keyspace_init.cql`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/test_unicode.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/test_unicode.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/test/winpty.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/test/winpty.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/tracing.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/tracing.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/util.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/util.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/cqlshlib/wcwidth.py` & `scylla-cqlsh-6.0.9/pylib/cqlshlib/wcwidth.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/pylib/setup.py` & `scylla-cqlsh-6.0.9/pylib/setup.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/reloc/build_deb.sh` & `scylla-cqlsh-6.0.9/reloc/build_deb.sh`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/reloc/build_reloc.sh` & `scylla-cqlsh-6.0.9/reloc/build_reloc.sh`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/reloc/build_rpm.sh` & `scylla-cqlsh-6.0.9/reloc/build_rpm.sh`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/scripts/create-relocatable-package.py` & `scylla-cqlsh-6.0.9/scripts/create-relocatable-package.py`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/PKG-INFO` & `scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scylla-cqlsh
-Version: 6.0.8
+Version: 6.0.9
 Summary: cqlsh is a Python-based command-line client for running CQL commands on a scylla cluster.
 Home-page: https://github.com/scylladb/scylla-cqlsh
 Author: Israel Fruchter
 Author-email: fruch@scylladb.com
 License: Apache
 Project-URL: Changelog, https://github.com/scylladb/scylla-cqlsh#changelog
 Project-URL: Documentation, https://cassandra.apache.org/doc/latest/tools/cqlsh.html
```

### Comparing `scylla-cqlsh-6.0.8/scylla_cqlsh.egg-info/SOURCES.txt` & `scylla-cqlsh-6.0.9/scylla_cqlsh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/setup.cfg` & `scylla-cqlsh-6.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `scylla-cqlsh-6.0.8/setup.py` & `scylla-cqlsh-6.0.9/setup.py`

 * *Files identical despite different names*

