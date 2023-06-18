# Comparing `tmp/PyFunceble-dev-4.2.0a9.tar.gz` & `tmp/PyFunceble-dev-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFunceble-dev-4.2.0a9.tar", last modified: Sat May 27 11:44:31 2023, max compression
+gzip compressed data, was "PyFunceble-dev-4.2.1.tar", last modified: Sun Jun 18 13:35:57 2023, max compression
```

## Comparing `PyFunceble-dev-4.2.0a9.tar` & `PyFunceble-dev-4.2.1.tar`

### file list

```diff
@@ -1,348 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.422926 PyFunceble-dev-4.2.0a9/PyFunceble/
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.422926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.426926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain_and_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.426926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/parked.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/subject_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/complex_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/params_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.426926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/status_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/second_lvl_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/credential_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/public_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    45945 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/execution_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/file_preloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/json_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/registrar_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/status_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/db_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/mining_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/file_and_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/miner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/miner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40349 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/ascii_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/config/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/adblock_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/cidr2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/internal_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_policy2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/subject2complements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/url2netloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/wildcard2subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/dir_structure_production.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/autocontinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/whois_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/all_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/base_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/csv_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/db_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/iana.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    32788 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/http_status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/hostbyaddr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/https.py
--rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/digit2digits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/expiration_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/month2unified.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PyFunceble/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.win.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.525590 PyFunceble-dev-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-06-18 13:35:57.525590 PyFunceble-dev-4.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.493589 PyFunceble-dev-4.2.1/PyFunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.493589 PyFunceble-dev-4.2.1/PyFunceble/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.497589 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38694 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/domain_and_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.497589 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/etoxic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/parked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/subject_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/availability/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/complex_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/params_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.497589 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/status_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.497589 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/domain_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/second_lvl_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.497589 PyFunceble-dev-4.2.1/PyFunceble/checker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/checker/utils/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.501589 PyFunceble-dev-4.2.1/PyFunceble/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.501589 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/credential_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.501589 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/public_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.501589 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45937 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/execution_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/file_preloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.501589 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.501589 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/json_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/registrar_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/status_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/db_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/mining_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/file_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.505589 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.509589 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/file_sorter_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.509589 PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.509589 PyFunceble-dev-4.2.1/PyFunceble/cli/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/system/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/system/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42775 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/system/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.509589 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/ascii_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.509589 PyFunceble-dev-4.2.1/PyFunceble/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/config/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/adblock_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/cidr2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/internal_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/rpz_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/rpz_policy2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/subject2complements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/url2netloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/converter/wildcard2subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/data/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/data/infrastructure/dir_structure_production.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.513589 PyFunceble-dev-4.2.1/PyFunceble/database/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/credential/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/credential/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/credential/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/credential/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/database/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/schemas/autocontinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/schemas/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/schemas/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/schemas/whois_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/all_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/base_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/csv_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/db_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/iana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.517589 PyFunceble-dev-4.2.1/PyFunceble/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/downloader/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/dns/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32788 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/dns/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/dns/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/http_status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/hostbyaddr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/record/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/record/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/record/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/requests/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.521589 PyFunceble-dev-4.2.1/PyFunceble/query/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.525590 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/digit2digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/expiration_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/month2unified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/query/whois/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.525590 PyFunceble-dev-4.2.1/PyFunceble/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/PyFunceble/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:35:57.525590 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-06-18 13:35:57.000000 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-06-18 13:35:57.000000 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:35:57.000000 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-18 13:35:57.000000 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-18 13:35:57.000000 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 13:35:57.000000 PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/requirements.win.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-18 13:35:57.525590 PyFunceble-dev-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-18 13:35:48.000000 PyFunceble-dev-4.2.1/version.yaml
```

### Comparing `PyFunceble-dev-4.2.0a9/CODE_OF_CONDUCT.rst` & `PyFunceble-dev-4.2.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/CONTRIBUTING.rst` & `PyFunceble-dev-4.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/LICENSE` & `PyFunceble-dev-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PKG-INFO` & `PyFunceble-dev-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.0a9
+Version: 4.2.1
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -15,15 +15,15 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: psql
 Provides-Extra: full
 License-File: LICENSE
 
@@ -86,24 +86,24 @@
 ------------
 
 :code:`pip`
 ^^^^^^^^^^^
 
 ::
 
-    $ pip install --upgrade --pre pyfunceble-dev
+    $ pip install --upgrade pyfunceble
     $ pyfunceble --version
 
 :code:`docker`
 ^^^^^^^^^^^^^^
 
 ::
 
-    $ docker pull pyfunceble/pyfunceble-dev
-    $ docker run -it pyfunceble/pyfunceble-dev --version
+    $ docker pull pyfunceble/pyfunceble
+    $ docker run -it pyfunceble/pyfunceble --version
 
 ___________________________________________
 
 Documentation as the place to be!
 ---------------------------------
 
 Want to know more about details **PyFunceble**?
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
 from PyFunceble.checker.availability.url import URLAvailabilityChecker
 from PyFunceble.checker.reputation.domain import DomainReputationChecker
 from PyFunceble.checker.reputation.domain_and_ip import DomainAndIPReputationChecker
 from PyFunceble.checker.reputation.ip import IPReputationChecker
 from PyFunceble.checker.reputation.url import URLReputationChecker
 from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.domain_and_ip import DomainAndIPSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.checker.syntax.ipv4 import IPv4SyntaxChecker
 from PyFunceble.checker.syntax.ipv6 import IPv6SyntaxChecker
 from PyFunceble.checker.syntax.second_lvl_domain import SecondLvlDomainSyntaxChecker
 from PyFunceble.checker.syntax.subdomain import SubDomainSyntaxChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
 from PyFunceble.converter.subject2complements import Subject2Complements
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 import PyFunceble.checker.utils.whois
 import PyFunceble.facility
 import PyFunceble.factory
 import PyFunceble.storage
 from PyFunceble.checker.availability.extras.base import ExtraRuleHandlerBase
 from PyFunceble.checker.availability.extras.dns import DNSRulesHandler
+from PyFunceble.checker.availability.extras.etoxic import EToxicHandler
 from PyFunceble.checker.availability.extras.rules import ExtraRulesHandler
 from PyFunceble.checker.availability.extras.subject_switch import (
     SubjectSwitchRulesHandler,
 )
 from PyFunceble.checker.availability.params import AvailabilityCheckerParams
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
 from PyFunceble.checker.base import CheckerBase
@@ -169,14 +170,15 @@
         self.domain_syntax_checker = DomainSyntaxChecker()
         self.ip_syntax_checker = IPSyntaxChecker()
         self.url_syntax_checker = URLSyntaxChecker()
         # WARNING: Put the aggressive one first!
         self.extra_rules_handlers = [
             SubjectSwitchRulesHandler(),
             DNSRulesHandler(),
+            EToxicHandler(),
             ExtraRulesHandler(),
         ]
         self.db_session = db_session
 
         self.params = AvailabilityCheckerParams()
 
         self.status = AvailabilityCheckerStatus()
@@ -510,24 +512,15 @@
         self.url_syntax_checker.subject = self.idna_subject
 
         self.status = AvailabilityCheckerStatus()
         self.status.params = self.params
         self.status.dns_lookup_record = self.dns_query_tool.lookup_record
         self.status.whois_lookup_record = self.whois_query_tool.lookup_record
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-        self.status.netloc = self.url2netloc.set_data_to_convert(
-            self.idna_subject
-        ).get_converted()
-        self.status.status = None
-
-        self.query_syntax_checker()
-
-        return self
+        return super().subject_propagator()
 
     def should_we_continue_test(self, status_post_syntax_checker: str) -> bool:
         """
         Checks if we are allowed to continue a standard testing.
 
         Rules:
             1. No status available yet. Continue to next test method.
@@ -651,15 +644,15 @@
             if method in to_ignore or not method.startswith("guess_"):
                 continue
 
             getattr(self, method)()
 
         return self
 
-    def query_syntax_checker(self) -> "AvailabilityCheckerBase":
+    def query_common_checker(self) -> "AvailabilityCheckerBase":
         """
         Queries the syntax checker.
         """
 
         PyFunceble.facility.Logger.info(
             "Started to check the syntax of %r", self.status.idna_subject
         )
@@ -679,15 +672,15 @@
         self.status.ip_syntax = bool(self.status.ipv4_syntax or self.status.ipv6_syntax)
         self.status.url_syntax = self.url_syntax_checker.is_valid()
 
         PyFunceble.facility.Logger.info(
             "Finished to check the syntax of %r", self.status.idna_subject
         )
 
-        return self
+        return super().query_common_checker()
 
     @CheckerBase.ensure_subject_is_given
     def query_dns_record(self) -> Optional[Dict[str, Optional[List[str]]]]:
         """
         Tries to query the DNS record(s) of the given subject.
 
         .. versionchanged:: 4.1.0b8.dev
@@ -888,24 +881,35 @@
         PyFunceble.facility.Logger.info(
             "Finished to try to query the status of %r from: NETINFO Lookup",
             self.status.idna_subject,
         )
 
         return self
 
-    def try_to_query_status_from_http_status_code(self) -> "AvailabilityCheckerBase":
+    def try_to_query_status_from_http_status_code(
+        self, *, from_domain_test: bool = False
+    ) -> "AvailabilityCheckerBase":
         """
         Tries to query the status from the HTTP status code.
+
+        :param bool from_domain_test:
+            Whether we wanted to test a test - actually.
+
+            Setting this argument to :py:class:`True` will exit the http_status_code
+            test if the given subject is already a URL.
         """
 
         PyFunceble.facility.Logger.info(
             "Started to try to query the status of %r from: HTTP Status code Lookup",
             self.status.idna_subject,
         )
 
+        if from_domain_test and self.status.url_syntax:
+            return self
+
         if not self.status.url_syntax and not RegexHelper("[^a-z0-9._]").match(
             self.idna_subject, return_match=False
         ):
             # The regex is there because while testing for domain, sometime we
             # may see something like mailto:xxx@yyy.de
 
             self.http_status_code_query_tool.set_subject(
@@ -948,29 +952,49 @@
         PyFunceble.facility.Logger.info(
             "Finished to try to query the status of %r from: HTTP Status code Lookup",
             self.status.idna_subject,
         )
 
         return self
 
-    def try_to_query_status_from_syntax_lookup(self) -> "AvailabilityCheckerBase":
+    def try_to_query_status_from_syntax_lookup(
+        self, from_domain_test: bool = False, from_url_test: bool = False
+    ) -> "AvailabilityCheckerBase":
         """
         Tries to query the status from the syntax.
+
+        :param bool from_domain_test:
+            Whether we wanted to test a domain - actually.
+
+            Setting this argument to :py:class:`True` will assume that we are
+            exclusively checking the syntax of domain/ip.
+        :param bool from_url_test:
+            Whether we wanted to test a url - actually.
+
+            Setting this argument to :py:class:`True` will assume that we are
+            exclusively checking the syntax of url.
         """
 
         PyFunceble.facility.Logger.info(
             "Started to try to query the status of %r from: Syntax Lookup",
             self.status.idna_subject,
         )
 
-        if (
-            not self.status.domain_syntax
-            and not self.status.ip_syntax
-            and not self.status.url_syntax
-        ):
+        if from_domain_test:
+            is_invalid = not self.status.domain_syntax and not self.status.ip_syntax
+        elif from_url_test:
+            is_invalid = not self.status.url_syntax
+        else:
+            is_invalid = (
+                not self.status.domain_syntax
+                and not self.status.ip_syntax
+                and not self.status.url_syntax
+            )
+
+        if is_invalid:
             self.status.status = PyFunceble.storage.STATUS.invalid
             self.status.status_source = "SYNTAX"
 
             PyFunceble.facility.Logger.info(
                 "Could define the status of %r from: Syntax Lookup",
                 self.status.idna_subject,
             )
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
         status_post_syntax_checker = None
 
         if not self.status.status and self.use_collection:
             self.try_to_query_status_from_collection()
 
         if not self.status.status and self.do_syntax_check_first:
-            self.try_to_query_status_from_syntax_lookup()
+            self.try_to_query_status_from_syntax_lookup(from_domain_test=True)
 
             if self.status.status:
                 status_post_syntax_checker = self.status.status
 
         if (
             self.use_whois_lookup
             and self.status.second_level_domain_syntax
@@ -161,15 +161,15 @@
         ):
             self.try_to_query_status_from_reputation()
 
         if self.use_extra_rules or (
             self.use_http_code_lookup
             and self.should_we_continue_test(status_post_syntax_checker)
         ):
-            self.try_to_query_status_from_http_status_code()
+            self.try_to_query_status_from_http_status_code(from_domain_test=True)
 
         if not self.status.status:
             self.status.status = PyFunceble.storage.STATUS.down
             self.status.status_source = "STDLOOKUP"
 
             PyFunceble.facility.Logger.info(
                 "Could not define status the status of %r. Setting to %r",
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain_and_ip.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the domains and IP availability checker.
+Provides the base of all datasets classes.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,72 +46,100 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Union
+import functools
+from typing import Any, Optional
 
-from PyFunceble.checker.availability.base import AvailabilityCheckerBase
-from PyFunceble.checker.availability.domain import DomainAvailabilityChecker
-from PyFunceble.checker.availability.ip import IPAvailabilityChecker
+import PyFunceble.storage
+from PyFunceble.downloader.base import DownloaderBase
+from PyFunceble.helpers.dict import DictHelper
+from PyFunceble.helpers.file import FileHelper
 
 
-class DomainAndIPAvailabilityChecker(AvailabilityCheckerBase):
+class DatasetBase:
     """
-    Provides the interface for checking the availability of a IP or domain.
-
-    :param str subject:
-        Optional, The subject to work with.
-    :param bool use_extra_rules:
-        Optional, Activates/Disables the usage of our own set of extra rules.
-    :param bool use_whois_lookup:
-        Optional, Activates/Disables the usage of the WHOIS lookup to gather
-        the status of the given :code:`subject`.
-    :param bool use_dns_lookup:
-        Optional, Activates/Disables the usage of the DNS lookup to gather the
-        status of the given :code:`subject`.
-    :param bool use_netinfo_lookup:
-        Optional, Activates/Disables the usage of the network information
-        lookup module to gather the status of the given :code:`subject`.
-    :param bool use_http_code_lookup:
-        Optional, Activates/Disables the usage of the HTTP status code lookup
-        to gather the status of the given :code:`subject`.
-    :param bool use_reputation_lookup:
-        Optional, Activates/Disables the usage of the reputation dataset
-        lookup to gather the status of the given :code:`subject`.
-    :param bool do_syntax_check_first:
-        Optional, Activates/Disables the check of the status before the actual
-        status gathering.
-    :param bool use_whois_db:
-        Optional, Activates/Disable the usage of a local database to store the
-        WHOIS datasets.
+    Provides the base of all dataset.
     """
 
-    @AvailabilityCheckerBase.ensure_subject_is_given
-    @AvailabilityCheckerBase.update_status_date_after_query
-    def query_status(
-        self,
-    ) -> "DomainAndIPAvailabilityChecker":  # pragma: no cover ## Just a switch.
+    STORAGE_INDEX: Optional[str] = None
+    DOWNLOADER: Optional[DownloaderBase] = None
+
+    source_file: Optional[str] = None
+
+    def __contains__(self, value: Any):  # pragma: no cover
+        raise NotImplementedError()
+
+    def __getattr__(self, value: Any):  # pragma: no cover
+        raise AttributeError(value)
+
+    def __getitem__(self, value: Any):  # pragma: no cover
+        raise KeyError(value)
+
+    def __getstate__(self):  # pragma: no cover
+        return vars(self)
+
+    def __setstate__(self, state):  # pragma: no cover
+        vars(self).update(state)
+
+    def ensure_source_file_exists(func):  # pylint: disable=no-self-argument
         """
-        Queries the result without anything more.
+        Ensures that the source file exists before running the decorated
+        method.
+
+        :raise TypeError:
+            When :code:`self.source_file` is not a :py:class:`str`.
+        :raise ValueError:
+            When :code:`self.source_file` is empty.
         """
 
-        query_object: Union[IPAvailabilityChecker, DomainAvailabilityChecker] = None
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if not isinstance(self.source_file, str):
+                raise TypeError(
+                    f"<self.source_file> should be {str}, "
+                    f"{type(self.source_file)} given."
+                )
+
+            if not self.source_file:
+                raise ValueError("<self.source_file> should not be empty.")
 
-        if self.status.ip_syntax:
-            query_object = IPAvailabilityChecker()
-        else:
-            query_object = DomainAvailabilityChecker()
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
 
-        query_object.__dict__ = self.__dict__
+        return wrapper
 
-        result = query_object.query_status()
+    @ensure_source_file_exists
+    def get_content(self) -> Optional[dict]:
+        """
+        Provides the cached or the real contend of the dataset (after caching)
 
-        self.__dict__.update(query_object.__dict__)
+        :raise FileNotFoundError:
+            When the declared file does not exists.
+        """
 
-        return result
+        if (
+            bool(self.STORAGE_INDEX)
+            and hasattr(PyFunceble.storage, self.STORAGE_INDEX)
+            and bool(getattr(PyFunceble.storage, self.STORAGE_INDEX))
+        ):
+            return getattr(PyFunceble.storage, self.STORAGE_INDEX)
+
+        file_helper = FileHelper(self.source_file)
+
+        if not file_helper.exists() and bool(
+            self.DOWNLOADER
+        ):  # pragma: no cover ## This is just a safety endpoint.
+            self.DOWNLOADER.start()
+
+            if not file_helper.exists():
+                raise FileNotFoundError(file_helper.path)
+
+        content = DictHelper().from_json_file(
+            self.source_file, return_dict_on_error=False
+        )
 
-    @staticmethod
-    def is_valid() -> bool:  # pylint: disable=arguments-differ
-        raise NotImplementedError()
+        setattr(PyFunceble.storage, self.STORAGE_INDEX, content)
+
+        return content
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/rules.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all extra handlers.
+Provides the extra rules handler based on the status code.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,228 +46,214 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
-from typing import Callable, List, Optional, Union
+from typing import Optional
 
-import requests
+from box import Box
 
+import PyFunceble.facility
 import PyFunceble.factory
+import PyFunceble.storage
+from PyFunceble.checker.availability.extras.base import ExtraRuleHandlerBase
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
-from PyFunceble.query.dns.query_tool import DNSQueryTool
+from PyFunceble.helpers.regex import RegexHelper
 
 
-class ExtraRuleHandlerBase:
+class ExtraRulesHandler(ExtraRuleHandlerBase):
     """
-    Provides the base of all extra rules handler.
+    Provides our very own extra rules handler.
 
-    :param statatus:
+    :param status:
         The previously gathered status.
     :type status:
         :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`
     """
 
-    _status: Optional[AvailabilityCheckerStatus] = None
-    req: Optional[requests.Response] = None
-    dns_query_tool: Optional[DNSQueryTool] = None
-    req_url: Optional[str] = None
+    regex_active2inactive: dict = {}
+    http_codes_dataset: Optional[Box] = None
 
     def __init__(self, status: Optional[AvailabilityCheckerStatus] = None) -> None:
-        if status is not None:
-            self.status = status
+        self.regex_active2inactive = {
+            r"\.000webhostapp\.com": [
+                (self.switch_to_down_if_status_code, 410),
+            ],
+            r"\.24\.eu$": [(self.switch_to_down_if_status_code, 503)],
+            r"\.altervista\.org$": [(self.switch_to_down_if_status_code, 403)],
+            r"\.angelfire\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.blogspot\.": [self.handle_blogspot],
+            r"\.canalblog\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.dr\.ag$": [(self.switch_to_down_if_status_code, 503)],
+            r"\.fc2\.com$": [self.handle_fc2_dot_com],
+            r"\.github\.io$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.godaddysites\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.hpg.com.br$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.imgur\.com$": [self.handle_imgur_dot_com],
+            r"\.liveadvert\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.skyrock\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.tumblr\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.wix\.com$": [(self.switch_to_down_if_status_code, 404)],
+            r"\.wordpress\.com$": [
+                (self.switch_to_down_if_status_code, 410),
+                self.handle_wordpress_dot_com,
+            ],
+            r"\.weebly\.com$": [(self.switch_to_down_if_status_code, {"404", "406"})],
+        }
 
-        # Be sure that all settings are loaded proprely!!
-        PyFunceble.factory.Requester.guess_all_settings()
-        self.dns_query_tool = DNSQueryTool()
-
-    def ensure_status_is_given(
-        func: Callable[..., "ExtraRuleHandlerBase"]
-    ):  # pylint: disable=no-self-argument
-        """
-        Ensures that the status is given before running the decorated method.
-
-        :raise TypeError:
-            If the subject is not a string.
-        """
-
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            if not self.status:
-                raise TypeError(
-                    f"<self.status> should be {AvailabilityCheckerStatus}, "
-                    f"{type(self.status)} given."
-                )
-
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
-
-        return wrapper
+        if PyFunceble.facility.ConfigLoader.is_already_loaded():
+            self.http_codes_dataset = PyFunceble.storage.HTTP_CODES
+        else:
+            self.http_codes_dataset = PyFunceble.storage.STD_HTTP_CODES
 
-    def setup_status_before(
-        func: Callable[..., "ExtraRuleHandlerBase"]
-    ):  # pylint: disable=no-self-argument
-        """
-        Ensures that the status is given before running the decorated method.
+        super().__init__(status)
 
-        :raise TypeError:
-            If the subject is not a string.
+    def __regex_registry_handler(self, regex_registry: dict) -> "ExtraRulesHandler":
         """
-
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            self.status.status_before_extra_rules = self.status.status
-            self.status.status_source_before_extra_rules = self.status.status_source
-
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
-
-        return wrapper
-
-    def setup_status_after(
-        func: Callable[..., "ExtraRuleHandlerBase"]
-    ):  # pylint: disable=no-self-argument
+        Handles the standard regex lookup case.
         """
-        Ensures that the status is given before running the decorated method.
 
-        :raise TypeError:
-            If the subject is not a string.
-        """
+        regex_helper = RegexHelper()
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            result = func(self, *args, **kwargs)  # pylint: disable=not-callable
+        for (
+            regex,
+            data,
+        ) in regex_registry.items():
+            broken = False
+            for element in data:
+                if not regex_helper.set_regex(regex).match(
+                    self.status.netloc, return_match=False
+                ):
+                    continue
 
-            if self.status.status_after_extra_rules:
-                self.status.status = self.status.status_after_extra_rules
-                self.status.status_source = self.status.status_source_after_extra_rules
+                if isinstance(element, tuple):
+                    element[0](*element[1:])
+                else:
+                    element()
 
-                PyFunceble.facility.Logger.info(
-                    "Could define the status of %r from our own set of rules.",
-                    self.status.idna_subject,
-                )
-            else:
-                self.status.status_before_extra_rules = None
-                self.status.status_source_before_extra_rules = None
-                self.status.status_after_extra_rules = None
-                self.status.status_source_after_extra_rules = None
+                if self.status.status_after_extra_rules:
+                    broken = True
+                    break
 
-            return result
+            if broken:
+                break
 
-        return wrapper
+        return self
 
-    @property
-    def status(self) -> Optional[AvailabilityCheckerStatus]:
-        """
-        Provides the current state of the :code:`_status` attribute.
+    def handle_blogspot(self) -> "ExtraRulesHandler":
         """
+        Handles the :code:`blogspot.*` case.
 
-        return self._status
-
-    @status.setter
-    def status(self, value: AvailabilityCheckerStatus) -> None:
+        .. warning::
+            This method assume that we know that we are handling a blogspot domain.
         """
-        Sets the status to work with.
 
-        :param value:
-            The status to work with.
+        regex_blogger = [r"create-blog.g?", r"87065", r"doesn&#8217;t&nbsp;exist"]
 
-        :raise TypeError:
-            When the given :code:`value` is not a
-            :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`.
-        """
-
-        if not isinstance(value, AvailabilityCheckerStatus):
-            raise TypeError(
-                f"<value> should be {AvailabilityCheckerStatus}, {type(value)} given."
-            )
+        self.do_on_body_match(
+            self.req_url,
+            regex_blogger,
+            method=self.switch_to_down,
+            allow_redirects=True,
+        )
 
-        self._status = value
+        return self
 
-    def set_status(self, value: AvailabilityCheckerStatus) -> "ExtraRuleHandlerBase":
+    def handle_wordpress_dot_com(self) -> "ExtraRulesHandler":
         """
-        Sets the status to work with.
+        Handles the :code:`wordpress.com` case.
 
-        :param value:
-            The status to work with.
+        .. warning::
+            This method assume that we know that we are handling a blogspot domain.
         """
 
-        self.status = value
+        regex_wordpress = [r"doesn&#8217;t&nbsp;exist", r"no\slonger\savailable"]
+
+        self.do_on_body_match(
+            self.req_url,
+            regex_wordpress,
+            method=self.switch_to_down,
+            allow_redirects=True,
+        )
 
         return self
 
-    def do_request(self, *, allow_redirects: bool = True) -> requests.Response:
+    def handle_fc2_dot_com(self) -> "ExtraRulesHandler":
         """
-        Do a request and store its response into the `req` attribute.
+        Handles the :code:`fc2.com` case.
 
-        :param bool allow_redirects:
-            Whether we shoold follow the redirection - or not.
+        .. warning::
+            This method assume that we know that we are handling a fc2 domain.
         """
 
-        if any(self.status.idna_subject.startswith(x) for x in ("http:", "https:")):
-            self.req_url = url = self.status.idna_subject
-        else:
-            self.req_url = url = f"http://{self.status.idna_subject}:80"
-
-        self.req = PyFunceble.factory.Requester.get(
-            url, allow_redirects=allow_redirects
+        self.do_on_header_match(
+            self.req_url,
+            {"location": ["error.fc2.com"]},
+            method=self.switch_to_down,
+            match_mode="std",
+            strict=True,
+            allow_redirects=False,
         )
 
         return self
 
-    def do_dns_lookup(self, *, subject: str, query_type: str) -> List[str]:
+    def handle_imgur_dot_com(self) -> "ExtraRulesHandler":
         """
-        Do a DNS lookup and return its response.
+        Handles the :code:`imgur.com` case.
 
-        :param subject:
-            The subject to query.
-        :param query_type:
-            The query type.
+        .. warning:.
+            This method assume that we know that we are handling a imgur.com
+            sub-domain.
         """
 
-        return (
-            self.dns_query_tool.set_query_record_type(query_type)
-            .set_subject(subject)
-            .query()
+        req = PyFunceble.factory.Requester.get(
+            self.req_url_https, allow_redirects=False
         )
+        username = self.status.netloc.replace(".imgur.com", "")
 
-    def start(self) -> "ExtraRuleHandlerBase":
-        """
-        Starts the gathering process.
-        """
+        if "Location" in req.headers:
+            if req.headers["Location"].endswith(("/removed.png", f"/user/{username}")):
+                self.switch_to_down()
 
-        raise NotImplementedError()
+        return self
 
-    def switch_to_down(self) -> "ExtraRuleHandlerBase":
+    def __handle_active2inactive(self) -> "ExtraRulesHandler":
         """
-        Switches the status to inactive.
+        Handles the status deescalation.
         """
 
-        self.status.status_after_extra_rules = PyFunceble.storage.STATUS.down
-        self.status.status_source_after_extra_rules = "SPECIAL"
+        if self.status.http_status_code:
+            self.__regex_registry_handler(self.regex_active2inactive)
 
         return self
 
-    def switch_to_down_if_status_code(
-        self, status_code: Union[int, List[int]]
-    ) -> "ExtraRuleHandlerBase":
+    @ExtraRuleHandlerBase.ensure_status_is_given
+    @ExtraRuleHandlerBase.setup_status_before
+    @ExtraRuleHandlerBase.setup_status_after
+    def start(self) -> "ExtraRulesHandler":
         """
-        Switches the status to inactive if the caught status code matches one
-        of the given one.
+        Starts the process.
         """
 
-        if not isinstance(status_code, (list, tuple)):
-            status_code = [status_code]
-
-        if any(self.status.http_status_code == x for x in status_code):
-            self.switch_to_down()
+        PyFunceble.facility.Logger.info(
+            "Started to check %r against our own set of extra rules.",
+            self.status.idna_subject,
+        )
 
-        return self
+        if self.status.status_before_extra_rules == PyFunceble.storage.STATUS.up:
+            self.__handle_active2inactive()
 
-    def switch_to_up(self) -> "ExtraRuleHandlerBase":
-        """
-        Switches the status to active.
-        """
+        if (
+            not self.status.status_after_extra_rules
+            and self.status.status_before_extra_rules in PyFunceble.storage.STATUS.down
+        ):
+            if self.status.ipv4_range_syntax or self.status.ipv6_range_syntax:
+                self.switch_to_up()
+
+        PyFunceble.facility.Logger.info(
+            "Finished to check %r against our own set of extra rules.",
+            self.status.idna_subject,
+        )
 
-        self.status.status_after_extra_rules = PyFunceble.storage.STATUS.up
-        self.status.status_source_after_extra_rules = "SPECIAL"
+        return self
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/dns.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/dns.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 """
 
 from typing import Optional
 
 import PyFunceble.facility
 from PyFunceble.checker.availability.extras.base import ExtraRuleHandlerBase
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
-from PyFunceble.helpers.regex import RegexHelper
 
 
 class DNSRulesHandler(ExtraRuleHandlerBase):
     """
     Provides our very own sets of DNS based rules.
 
     :param status:
@@ -103,39 +102,20 @@
             r"sendsmtp\.com|serveuser\.com|serveusers\.com|sexidude\.com|"
             r"sexxxy\.biz|sixth\.biz|squirly\.info|ssl443\.org|ssmailer\.com|"
             r"toh\.info|toshibanetcam\.com|toythieves\.com|trickip\.net|"
             r"trickip\.org|vizvaz\.com|wikaba\.com|www1\.biz|"
             r"wwwhost\.biz|wwwhost\.us|x24hr\.com|xxuz\.com|xxxy\.biz|"
             r"xxxy\.info|ygto\.com|youdontcare\.com|yourtrap\.com|"
             r"zyns\.com|zzux\.com)(\.|)$": [
-                (self._switch_down_if_match, ("SOA", ["abuse.changeip.com."]))
+                (self.switch_down_if_dns_match, ("SOA", ["abuse.changeip.com."]))
             ]
         }
 
         super().__init__(status)
 
-    def _switch_down_if_match(
-        self, query_type: str, matches: list
-    ) -> "DNSRulesHandler":
-        """
-        Tries to switch the status :code:`INACTIVE` if the query matched.
-        """
-
-        result = (
-            self.dns_query_tool.set_query_record_type(query_type)
-            .set_subject(self.status.netloc)
-            .query()
-        )
-
-        for record in result:
-            for match in matches:
-                if match in record:
-                    self.switch_to_down()
-                    break
-
     @ExtraRuleHandlerBase.ensure_status_is_given
     @ExtraRuleHandlerBase.setup_status_before
     @ExtraRuleHandlerBase.setup_status_after
     def start(self) -> "DNSRulesHandler":
         """
         Process the check and handling of the current subject.
         """
@@ -145,15 +125,17 @@
             self.status.idna_subject,
         )
 
         for regex, rulesets in self.rulesets.items():
             if self.status.status_after_extra_rules:
                 break
 
-            if not RegexHelper(regex).match(self.status.netloc, return_match=False):
+            if not self.regex_helper.set_regex(regex).match(
+                self.status.netloc, return_match=False
+            ):
                 break
 
             for ruler, params in rulesets:
                 if self.status.status_after_extra_rules:
                     break
 
                 ruler(*params)
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/parked.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/parked.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,18 +46,14 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Optional
-
-import requests
-
 import PyFunceble.factory
 import PyFunceble.storage
 from PyFunceble.checker.availability.extras.base import ExtraRuleHandlerBase
 
 
 class ParkedRulesHandler(ExtraRuleHandlerBase):
     """
@@ -66,37 +62,14 @@
 
     :param status:
         The previously gathered status.
     :type status:
         :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`
     """
 
-    req: Optional[requests.Response] = None
-
-    def _do_request(self, *, allow_redirects: bool = True) -> "ParkedRulesHandler":
-        """
-        Do a request and store its response into the `req` attribute.
-
-        :param bool allow_redirects:
-            Whether we shoold follow the redirection - or not.
-        """
-
-        if self.status.idna_subject.startswith(
-            "http:"
-        ) or self.status.idna_subject.startswith("https://"):
-            url = self.status.idna_subject
-        else:
-            url = f"http://{self.status.idna_subject}:80"
-
-        self.req = PyFunceble.factory.Requester.get(
-            url, allow_redirects=allow_redirects
-        )
-
-        return self
-
     def _switch_down_by_cookie(self) -> "ParkedRulesHandler":
         """
         Tries to switch the status to inactive if some special cookies where found.
         """
 
         if "parking_session" in self.req.cookies:
             self.switch_to_down()
@@ -138,15 +111,15 @@
     def start(self) -> "ParkedRulesHandler":
         PyFunceble.facility.Logger.info(
             "Started to check %r against our own set of parked rules.",
             self.status.idna_subject,
         )
 
         try:
-            self._do_request()
+            self.do_request()
 
             if self.status.status_before_extra_rules == PyFunceble.storage.STATUS.up:
                 self._switch_down_by_cookie()
 
             if not self.status.status_after_extra_rules:
                 self._swith_down_by_content()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/rules.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the extra rules handler based on the status code.
+Provides the base of all our printers.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,254 +46,296 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import socket
-from typing import Callable, List, Optional
+import copy
+import functools
+import string
+from typing import Dict, Optional
 
-from box import Box
 
-import PyFunceble.facility
-import PyFunceble.factory
-import PyFunceble.storage
-from PyFunceble.checker.availability.extras.base import ExtraRuleHandlerBase
-from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
-from PyFunceble.helpers.regex import RegexHelper
-
-
-class ExtraRulesHandler(ExtraRuleHandlerBase):
+class PrinterBase:
     """
-    Provides our very own extra rules handler.
+    Provides the base of all printer class.
 
-    :param status:
-        The previously gathered status.
-    :type status:
-        :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`
+    Printer classes are classes which derivate from this class. their objectives
+    should be the same: Unify and simplify the way to print something to a given
+    destination.
     """
 
-    regex_active2inactive: dict = {}
-    http_codes_dataset: Optional[Box] = None
+    STD_UNKNOWN: str = "Unknown"
 
-    def __init__(self, status: Optional[AvailabilityCheckerStatus] = None) -> None:
-        self.regex_active2inactive = {
-            r"\.000webhostapp\.com": [
-                (self.switch_to_down_if_status_code, 410),
-            ],
-            r"\.24\.eu$": [(self.switch_to_down_if_status_code, 503)],
-            r"\.altervista\.org$": [(self.switch_to_down_if_status_code, 403)],
-            r"\.angelfire\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.blogspot\.": [self.handle_blogspot],
-            r"\.canalblog\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.dr\.ag$": [(self.switch_to_down_if_status_code, 503)],
-            r"\.fc2\.com$": [self.handle_fc2_dot_com],
-            r"\.github\.io$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.godaddysites\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.hpg.com.br$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.imgur\.com$": [self.handle_imgur_dot_com],
-            r"\.liveadvert\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.skyrock\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.tumblr\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.wix\.com$": [(self.switch_to_down_if_status_code, 404)],
-            r"\.wordpress\.com$": [
-                (self.switch_to_down_if_status_code, 410),
-                self.handle_wordpress_dot_com,
-            ],
-            r"\.weebly\.com$": [(self.switch_to_down_if_status_code, {"404", "406"})],
-        }
-
-        if PyFunceble.facility.ConfigLoader.is_already_loaded():
-            self.http_codes_dataset = PyFunceble.storage.HTTP_CODES
-        else:
-            self.http_codes_dataset = PyFunceble.storage.STD_HTTP_CODES
+    STD_LENGTH: Dict[str, int] = {
+        "idna_subject": 100,
+        "status": 11,
+        "status_source": 10,
+        "http_status_code": 10,
+        "percentage": 12,
+        "expiration_date": 17,
+        "amount": 12,
+        "checker_type": 13,
+        "days": 2,
+        "hours": 2,
+        "minutes": 2,
+        "seconds": 6,
+        "registrar": 30,
+    }
+
+    TEMPLATES: Dict[str, string.Template] = {
+        "all": string.Template(
+            "$idna_subject $status $status_source $expiration_date $registrar "
+            "$http_status_code $checker_type"
+        ),
+        "less": string.Template("$idna_subject $status $status_source"),
+        "simple": string.Template("$idna_subject $status"),
+        "percentage": string.Template("$status $percentage $amount"),
+        "hosts": string.Template("$ip $idna_subject"),
+        "plain": string.Template("$idna_subject"),
+        "execution_time": string.Template(
+            "\nExecution Time: $days:$hours:$minutes:$seconds\n"
+        ),
+        "registrar": string.Template("$registrar $percentage $amount"),
+    }
+
+    HEADERS: Dict[str, str] = {
+        "idna_subject": "Subject",
+        "status": "Status",
+        "status_source": "Source",
+        "http_status_code": "HTTP Code",
+        "expiration_date": "Expiration Date",
+        "percentage": "Percentage",
+        "amount": "Amount",
+        "ip": "IP",
+        "checker_type": "Checker",
+        "days": "Days",
+        "hours": "Hours",
+        "minutes": "Minutes",
+        "seconds": "Seconds",
+        "registrar": "Registrar",
+    }
 
-        super().__init__(status)
+    _template_to_use: Optional[str] = None
+    _dataset: Optional[Dict[str, str]] = None
 
-    def __web_regex_handler(
+    def __init__(
         self,
-        url: str,
-        regex_list: List[str],
-        method: Callable[..., "ExtraRulesHandler"],
-    ) -> "ExtraRulesHandler":
-        """
-        Handles a web request along with a regex filter.
-        """
-
-        try:
-            req = PyFunceble.factory.Requester.get(url, allow_redirects=True)
-
-            for regex in regex_list:
-                if regex in req.text or RegexHelper(regex).match(
-                    req.text, return_match=False
-                ):
-                    method()
-                    break
-        except (
-            PyFunceble.factory.Requester.exceptions.RequestException,
-            PyFunceble.factory.Requester.exceptions.InvalidURL,
-            PyFunceble.factory.Requester.exceptions.Timeout,
-            PyFunceble.factory.Requester.exceptions.ConnectionError,
-            PyFunceble.factory.Requester.urllib3_exceptions.InvalidHeader,
-            socket.timeout,
-        ):
-            pass
+        template_to_use: Optional[str] = None,
+        *,
+        dataset: Optional[Dict[str, str]] = None,
+    ) -> None:
+        if template_to_use is not None:
+            self.template_to_use = template_to_use
 
-        return self
+        if dataset is not None:
+            self.dataset = dataset
 
-    def __regex_registry_handler(self, regex_registry: dict) -> "ExtraRulesHandler":
-        """
-        Handles the standard regex lookup case.
+    def ensure_template_to_use_is_given(func):  # pylint: disable=no-self-argument
         """
+        Ensures that the template to use is given before launching the
+        decorated method.
 
-        for (
-            regex,
-            data,
-        ) in regex_registry.items():
-            broken = False
-            for element in data:
-                if not RegexHelper(regex).match(self.status.netloc, return_match=False):
-                    continue
+        :raise TypeError:
+            When the current :code:`self.template_to_use` is not set.
+        """
 
-                if isinstance(element, tuple):
-                    element[0](*element[1:])
-                else:
-                    element()
-
-                if self.status.status_after_extra_rules:
-                    broken = True
-                    break
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if not isinstance(self.template_to_use, str):
+                raise TypeError("<self.template_to_use> is not given.")
 
-            if broken:
-                break
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
 
-        return self
+        return wrapper
 
-    def handle_blogspot(self) -> "ExtraRulesHandler":
+    def ensure_dataset_is_given(func):  # pylint: disable=no-self-argument
         """
-        Handles the :code:`blogspot.*` case.
+        Ensures that the dataset to write is given before launching the
+        decorated method.
 
-        .. warning::
-            This method assume that we know that we are handling a blogspot domain.
+        :raise TypeError:
+            When the current :code:`self.template_to_use` is not set.
         """
 
-        regex_blogger = [r"create-blog.g?", r"87065", r"doesn&#8217;t&nbsp;exist"]
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if not isinstance(self.dataset, dict):
+                raise TypeError("<self.dataset> is not given.")
 
-        if self.status.idna_subject.startswith(
-            "http:"
-        ) or self.status.idna_subject.startswith("https://"):
-            url = self.status.idna_subject
-        else:
-            url = f"http://{self.status.idna_subject}:80"
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
 
-        self.__web_regex_handler(url, regex_blogger, self.switch_to_down)
+        return wrapper
 
-        return self
+    @property
+    def template_to_use(self) -> Optional[str]:
+        """
+        Provides the current state of the :code:`_template_to_use` attribute.
+        """
+
+        return self._template_to_use
 
-    def handle_wordpress_dot_com(self) -> "ExtraRulesHandler":
+    @template_to_use.setter
+    def template_to_use(self, value: str) -> None:
         """
-        Handles the :code:`wordpress.com` case.
+        Sets the template to use.
+
+        :param value:
+            The value to set.
 
-        .. warning::
-            This method assume that we know that we are handling a blogspot domain.
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is not supported.
         """
 
-        regex_wordpress = [r"doesn&#8217;t&nbsp;exist", r"no\slonger\savailable"]
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        if self.status.idna_subject.startswith(
-            "http:"
-        ) or self.status.idna_subject.startswith("https://"):
-            url = self.status.idna_subject
-        else:
-            url = f"http://{self.status.idna_subject}:80"
+        if value not in self.TEMPLATES:
+            raise ValueError(
+                f"<value> ({value!r}) is not supported "
+                f"({list(self.TEMPLATES.keys())!r})."
+            )
 
-        self.__web_regex_handler(url, regex_wordpress, self.switch_to_down)
+        self._template_to_use = value
+
+    def set_template_to_use(self, value: str) -> "PrinterBase":
+        """
+        Sets the template to use.
+
+        :param value:
+            The value to set.
+        """
+
+        self.template_to_use = value
 
         return self
 
-    def handle_fc2_dot_com(self) -> "ExtraRulesHandler":
+    @property
+    def dataset(self) -> Optional[Dict[str, str]]:
+        """
+        Provides the current state of the :code:`_dataset` attribute.
         """
-        Handles the :code:`fc2.com` case.
 
-        .. warning::
-            This method assume that we know that we are handling a fc2 domain.
+        return self._dataset
+
+    @dataset.setter
+    def dataset(self, value: Dict[str, str]) -> None:
         """
+        Sets the dataset to apply to the template.
+
+        :param value:
+            The value to set.
 
-        if self.status.idna_subject.startswith(
-            "http:"
-        ) or self.status.idna_subject.startswith("https://"):
-            url = self.status.idna_subject
-        else:
-            url = f"http://{self.status.idna_subject}:80"
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`dict`
+        :raise ValueError:
+            When the given :code:`value` is empty.
+        """
 
-        req = PyFunceble.factory.Requester.get(url, allow_redirects=False)
+        if not isinstance(value, dict):
+            raise TypeError(f"<value> should be {dict}, {type(value)} given.")
 
-        if "Location" in req.headers and "error.fc2.com" in req.headers["Location"]:
-            self.switch_to_down()
+        if not value:
+            raise ValueError("<value> should not be empty.")
+
+        self._dataset = copy.deepcopy(value)
+
+    def set_dataset(self, value: Dict[str, str]) -> "PrinterBase":
+        """
+        Sets the dataset to apply to the template.
+
+        :param value:
+            The value to set.
+        """
+
+        self.dataset = value
 
         return self
 
-    def handle_imgur_dot_com(self) -> "ExtraRulesHandler":
+    @ensure_template_to_use_is_given
+    def get_header_to_print(self) -> str:
+        """
+        Provides the template header to print.
         """
-        Handles the :code:`imgur.com` case.
 
-        .. warning:.
-            This method assume that we know that we are handling a imgur.com
-            sub-domain.
+        ignore_header = ["simple", "hosts", "plain", "execution_time"]
+
+        to_print_data = [dict(), dict()]  # pylint: disable=use-dict-literal
+
+        if self.template_to_use not in ignore_header:
+            for key, value in self.HEADERS.items():
+                if key not in self.TEMPLATES[self.template_to_use].template:
+                    continue
+
+                to_print_data[0][key] = f"{value:<{self.STD_LENGTH[key]}}"
+
+            for key, value in to_print_data[0].items():
+                to_print_data[1][key] = "-" * len(value)
+
+            to_print = [
+                self.TEMPLATES[self.template_to_use].safe_substitute(
+                    **to_print_data[0]
+                ),
+                self.TEMPLATES[self.template_to_use].safe_substitute(
+                    **to_print_data[1]
+                ),
+            ]
+
+            return "\n".join(to_print)
+        return ""
+
+    @ensure_template_to_use_is_given
+    @ensure_dataset_is_given
+    def get_line_to_print(self) -> str:
+        """
+        Provides the line to print.
         """
 
-        if self.status.idna_subject.startswith(
-            "http:"
-        ) or self.status.idna_subject.startswith("https://"):
-            url = self.status.idna_subject
-        else:
-            url = f"https://{self.status.idna_subject}"
+        to_print = {}
+        ignore_length = ["simple", "hosts", "plain", "execution_time"]
 
-        req = PyFunceble.factory.Requester.get(url, allow_redirects=False)
-        username = self.status.netloc.replace(".imgur.com", "")
+        for key, value in self.dataset.items():
+            if key not in self.HEADERS:
+                continue
 
-        if "Location" in req.headers:
-            if req.headers["Location"].endswith(("/removed.png", f"/user/{username}")):
-                self.switch_to_down()
+            if not value and value != 0:
+                value = self.STD_UNKNOWN
 
-        return self
+            if self.template_to_use not in ignore_length:
+                to_print[key] = f"{value:<{self.STD_LENGTH[key]}}"
+            else:
+                to_print[key] = value
+
+        missings = [
+            x[1:]
+            for x in self.TEMPLATES[self.template_to_use].template.split()
+            if x.startswith("$") and x[1:] not in to_print
+        ]
+
+        for missing in missings:
+            try:
+                to_print[missing] = f"{self.STD_UNKNOWN:<{self.STD_LENGTH[missing]}}"
+            except KeyError:
+                # Example: execution time
+                pass
 
-    def __handle_active2inactive(self) -> "ExtraRulesHandler":
+        return self.TEMPLATES[self.template_to_use].safe_substitute(**to_print)
+
+    def print_header(self) -> None:
         """
-        Handles the status deescalation.
+        Prints the header.
         """
 
-        if self.status.http_status_code:
-            self.__regex_registry_handler(self.regex_active2inactive)
+        header = self.get_header_to_print()
 
-        return self
+        if header:
+            print(f"\n\n{header}")
 
-    @ExtraRuleHandlerBase.ensure_status_is_given
-    @ExtraRuleHandlerBase.setup_status_before
-    @ExtraRuleHandlerBase.setup_status_after
-    def start(self) -> "ExtraRulesHandler":
-        """
-        Starts the process.
-        """
-
-        PyFunceble.facility.Logger.info(
-            "Started to check %r against our own set of extra rules.",
-            self.status.idna_subject,
-        )
-
-        if self.status.status_before_extra_rules == PyFunceble.storage.STATUS.up:
-            self.__handle_active2inactive()
-
-        if (
-            not self.status.status_after_extra_rules
-            and self.status.status_before_extra_rules in PyFunceble.storage.STATUS.down
-        ):
-            if self.status.ipv4_range_syntax or self.status.ipv6_range_syntax:
-                self.switch_to_up()
-
-        PyFunceble.facility.Logger.info(
-            "Finished to check %r against our own set of extra rules.",
-            self.status.idna_subject,
-        )
+    def print_interpolated_line(self) -> None:
+        """
+        Prints the line where we are suppose to write it.
+        """
 
-        return self
+        raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/subject_switch.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/extras/subject_switch.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/ip.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/params.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/status.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/url.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/availability/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,28 +121,39 @@
         self.status.idna_subject = self.idna_subject
         self.status.netloc = self.url2netloc.set_data_to_convert(
             self.idna_subject
         ).get_converted()
 
         self.status.status = None
 
-        self.query_syntax_checker()
+        self.query_common_checker()
 
         return self
 
-    def try_to_query_status_from_http_status_code(self) -> "URLAvailabilityChecker":
+    def try_to_query_status_from_http_status_code(
+        self, *, from_domain_test: bool = False
+    ) -> "URLAvailabilityChecker":
         """
         Tries to query the status from the network information.
+
+        :param bool from_domain_test:
+            Whether we wanted to test a test - actually.
+
+            Setting this argument to :py:class:`True` will exit the http_status_code
+            test if the given subject is already a URL.
         """
 
         PyFunceble.facility.Logger.info(
             "Started to try to query the status of %r from: HTTP Status code Lookup",
             self.status.idna_subject,
         )
 
+        if from_domain_test and self.status.url_syntax:
+            return self
+
         lookup_result = self.http_status_code_query_tool.get_status_code()
 
         if (
             lookup_result
             and lookup_result
             != self.http_status_code_query_tool.STD_UNKNOWN_STATUS_CODE
         ):
@@ -247,25 +258,28 @@
         """
 
         ## Test Methods are more important.
 
         status_post_syntax_checker = None
 
         if not self.status.status and self.do_syntax_check_first:
-            self.try_to_query_status_from_syntax_lookup()
+            self.try_to_query_status_from_syntax_lookup(from_url_test=True)
 
             if self.status.status:
                 status_post_syntax_checker = self.status.status
 
         if self.use_reputation_lookup and self.should_we_continue_test(
             status_post_syntax_checker
         ):
             self.try_to_query_status_from_reputation()
 
-        if self.should_we_continue_test(status_post_syntax_checker):
+        if (
+            self.should_we_continue_test(status_post_syntax_checker)
+            and self.status.url_syntax
+        ):
             self.try_to_query_status_from_dns()
 
         if self.should_we_continue_test(status_post_syntax_checker):
             self.try_to_query_status_from_http_status_code()
 
         if not self.status.status:
             self.status.status = PyFunceble.storage.STATUS.down
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -370,19 +370,50 @@
             self.use_collection = self.STD_USE_COLLECTION
 
     def subject_propagator(self) -> "CheckerBase":
         """
         Propagate the currently set subject.
 
         .. warning::
-            You are not invited to run this method directly.
+            Be sure to use setup your status first.
+        """
+
+        self.status.subject = self.subject
+        self.status.idna_subject = self.idna_subject
+        self.status.netloc = self.url2netloc.set_data_to_convert(
+            self.idna_subject
+        ).get_converted()
+        self.status.status = None
 
-            Only the :code:`propagate_subject` decorator should call this
-            method.
+        return self.query_common_checker()
+
+    def query_common_checker(self) -> "CheckerBase":
         """
+        Queries the common checkers.
+
+        .. warning::
+            Be sure to use setup your status first.
+        """
+
+        if not self.status.subject_kind:
+            cls_name = self.__class__.__name__.lower()
+            if (
+                hasattr(self.status, "ip_syntax") and self.status.ip_syntax
+            ) or "ip" in cls_name:
+                self.status.subject_kind = "ip"
+            elif (
+                hasattr(self.status, "url_syntax") and self.status.url_syntax
+            ) or "url" in cls_name:
+                self.status.subject_kind = "url"
+            elif (
+                hasattr(self.status, "domain_syntax") and self.status.domain_syntax
+            ) or "domain" in cls_name:
+                self.status.subject_kind = "domain"
+            else:
+                self.status.subject_kind = "unknown"
 
         return self
 
     @ensure_subject_is_given
     def is_valid(self) -> bool:
         """
         Provides the result of the validation.
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/complex_json_encoder.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/complex_json_encoder.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/params_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/params_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,55 +132,47 @@
         self.ip_syntax_checker.subject = self.idna_subject
         self.url_syntax_checker.subject = self.idna_subject
 
         self.status = ReputationCheckerStatus()
         self.status.params = self.params
         self.status.dns_lookup_record = self.dns_query_tool.lookup_record
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-        self.status.netloc = self.url2netloc.set_data_to_convert(
-            self.idna_subject
-        ).get_converted()
-
-        self.query_syntax_checker()
-
-        return self
+        return super().subject_propagator()
 
     def should_we_continue_test(self, status_post_syntax_checker: str) -> bool:
         """
         Checks if we are allowed to continue a standard testing.
         """
 
         return bool(
             not self.status.status
             or status_post_syntax_checker == PyFunceble.storage.STATUS.invalid
         )
 
-    def query_syntax_checker(self) -> "ReputationCheckerBase":
+    def query_common_checker(self) -> "ReputationCheckerBase":
         """
-        Queries the syntax checker.
+        Queries the common checkers.
         """
 
         self.status.second_level_domain_syntax = (
             self.domain_syntax_checker.is_valid_second_level()
         )
         self.status.subdomain_syntax = self.domain_syntax_checker.is_valid_subdomain()
-        self.status.domain_syntax = bool(
-            self.status.subdomain_syntax or self.status.second_level_domain_syntax
+        self.status.domain_syntax = bool(self.status.subdomain_syntax) or bool(
+            self.status.second_level_domain_syntax
         )
 
         self.status.ipv4_syntax = self.ip_syntax_checker.is_valid_v4()
         self.status.ipv6_syntax = self.ip_syntax_checker.is_valid_v6()
         self.status.ipv4_range_syntax = self.ip_syntax_checker.is_valid_v4_range()
         self.status.ipv6_range_syntax = self.ip_syntax_checker.is_valid_v6_range()
         self.status.ip_syntax = bool(self.status.ipv4_syntax or self.status.ipv6_syntax)
         self.status.url_syntax = self.url_syntax_checker.is_valid()
 
-        return self
+        return super().query_common_checker()
 
     def query_a_record(self) -> Optional[List[str]]:
         """
         Queries all the A record.
         """
 
         raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain_and_ip.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/domain_and_ip.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the domains and IP reputation checker.
+Provides the domains and IP syntax checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,42 +46,47 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from PyFunceble.checker.reputation.base import ReputationCheckerBase
-from PyFunceble.checker.reputation.domain import DomainReputationChecker
-from PyFunceble.checker.reputation.ip import IPReputationChecker
+from typing import Union
 
+from PyFunceble.checker.syntax.base import SyntaxCheckerBase
+from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 
-class DomainAndIPReputationChecker(ReputationCheckerBase):
+
+class DomainAndIPSyntaxChecker(SyntaxCheckerBase):
     """
-    Provides the interface for checking the reputation of an IP or domain.
+    Provides the interface for checking the syntax of an IP or domain.
 
     :param str subject:
         Optional, The subject to work with.
-    :param bool do_syntax_check_first:
-        Optional, Activates/Disables the check of the status before the actual
-        status gathering.
     """
 
-    @ReputationCheckerBase.ensure_subject_is_given
-    @ReputationCheckerBase.update_status_date_after_query
-    def query_status(self) -> "DomainAndIPReputationChecker":
+    @SyntaxCheckerBase.ensure_subject_is_given
+    @SyntaxCheckerBase.update_status_date_after_query
+    def query_status(
+        self,
+    ) -> "DomainAndIPSyntaxChecker":  # pragma: no cover ## Just a switch.
         """
         Queries the result without anything more.
         """
 
-        if self.status.ip_syntax:
-            query_object = IPReputationChecker()
+        query_object: Union[IPSyntaxChecker, DomainSyntaxChecker] = None
+
+        ip_checker = IPSyntaxChecker(self.subject)
+
+        if ip_checker.is_valid():
+            query_object = ip_checker
         else:
-            query_object = DomainReputationChecker()
+            query_object = DomainSyntaxChecker(self.subject, db_session=self.db_session)
 
-        query_object.__dict__ = self.__dict__
+        query_object.collection_query_tool = self.collection_query_tool
 
         result = query_object.query_status()
 
         self.__dict__.update(query_object.__dict__)
 
         return result
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/ip.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/params.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/status.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/url.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/status_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/status_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
 @dataclasses.dataclass
 class CheckerStatusBase:
     """
     Provides the base of all status classes.
     """
 
+    subject_kind: Optional[str] = None
+
     subject: Optional[str] = None
     idna_subject: Optional[str] = None
     netloc: Optional[str] = None
 
     status: Optional[str] = None
     status_source: Optional[str] = None
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,21 +92,15 @@
 
         .. warning::
             You are not invited to run this method directly.
         """
 
         self.status = SyntaxCheckerStatus()
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-        self.status.netloc = self.url2netloc.set_data_to_convert(
-            self.idna_subject
-        ).get_converted()
-
-        return self
+        return super().subject_propagator()
 
     @CheckerBase.ensure_subject_is_given
     @CheckerBase.update_status_date_after_query
     def query_status(self) -> "SyntaxCheckerBase":
         """
         Queries the status.
         """
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/domain.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,22 +91,17 @@
             You are not invited to run this method directly.
         """
 
         self.second_level_checker.subject = self.idna_subject
         self.subdomain_checker.subject = self.idna_subject
 
         self.status = SyntaxCheckerStatus()
+        self.status.subject_kind = "domain"
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-        self.status.netloc = self.url2netloc.set_data_to_convert(
-            self.idna_subject
-        ).get_converted()
-
-        return self
+        return super().subject_propagator()
 
     @DomainSyntaxCheckerBase.ensure_subject_is_given
     def is_valid(self) -> bool:
         """
         Validate the given subject if exists.
         """
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/domain_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ip.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/ip.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,22 +84,17 @@
             You are not invited to run this method directly.
         """
 
         self.ipv4_checker.subject = self.idna_subject
         self.ipv6_checker.subject = self.idna_subject
 
         self.status = SyntaxCheckerStatus()
+        self.status.subject_kind = "ip"
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-        self.status.netloc = self.url2netloc.set_data_to_convert(
-            self.idna_subject
-        ).get_converted()
-
-        return self
+        return super().subject_propagator()
 
     @CheckerBase.ensure_subject_is_given
     def is_valid(self) -> bool:
         """
         Validate the given subject.
         """
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv4.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/ipv4.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv6.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/ipv6.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/params.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/second_lvl_domain.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/second_lvl_domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/status.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/subdomain.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/subdomain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/url.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/syntax/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,19 @@
     """
     Provides an interface to check the syntax of a URL.
 
     :param str subject:
         Optional, The subject to work with.
     """
 
+    def subject_propagator(self) -> CheckerBase:
+        self.status.subject_kind = "url"
+
+        return super().subject_propagator()
+
     @staticmethod
     def get_hostname_from_url(url: str) -> Optional[str]:
         """
         Extract the hostname part of the given URL.
 
         .. versionadded:: 4.1.0b7
         """
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/whois.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/utils/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/exceptions.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/github_actions.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/github_actions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/gitlab_ci.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/jenkins.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/jenkins.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/travis_ci.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/travis_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/utils.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/continuous_integration/utils.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/credential_loader.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/credential_loader.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/clean.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/clean.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/iana.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/production.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/public_suffix.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/argsparser.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/argsparser.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/cli.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/entry_points/pyfunceble/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
             },
         ),
         (
             [
                 "--aggressive",
             ],
             {
-                "dest": "cli_decoding.adblock_aggressive",
+                "dest": "cli_decoding.aggressive",
                 "action": "store_true",
                 "help": argparse.SUPPRESS,
             },
         ),
         (
             ["--cidr"],
             {
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/execution_time.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/execution_time.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/facility.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/factory.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/file_preloader.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/file_preloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,15 @@
 
                         if self.rpz_policy2subject and "SOA" in line:
                             self.rpz_policy2subject.set_soa(line.split()[0])
 
                         for subject in get_subjects_from_line(
                             line,
                             self.checker_type,
+                            subject_type=self.protocol["subject_type"],
                             adblock_inputline2subject=self.adblock_inputline2subject,
                             wildcard2subject=self.wildcard2subject,
                             rpz_policy2subject=self.rpz_policy2subject,
                             rpz_inputline2subject=self.rpz_inputline2subject,
                             inputline2subject=self.inputline2subject,
                             subject2complements=self.subject2complements,
                             url2netloc=self.url2netloc,
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/cleanup.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/cleanup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/counter.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/counter.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,21 +47,22 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import copy
-from typing import Dict, List, Union
+from typing import Dict, List, Tuple, Union
 
 import PyFunceble.cli.storage
 import PyFunceble.cli.utils.testing
 import PyFunceble.storage
 from PyFunceble.checker.status_base import CheckerStatusBase
 from PyFunceble.cli.filesystem.json_base import FilesystemJSONBase
+from PyFunceble.helpers.list import ListHelper
 
 
 class FilesystemCounter(FilesystemJSONBase):
     """
     Provides our counter.
     """
 
@@ -101,14 +102,28 @@
             PyFunceble.storage.STATUS.invalid,
         ],
     }
 
     SOURCE_FILE: str = PyFunceble.cli.storage.COUNTER_FILE
 
     @FilesystemJSONBase.fetch_dataset_beforehand
+    def get_sorted_dataset(self) -> List[Tuple[str, float]]:
+        """
+        Provides the datasets in a sorted manner.
+        """
+
+        return (
+            ListHelper(
+                [(x, y) for x, y in self.dataset["percentage"].items() if x != "total"]
+            )
+            .custom_sort(key_method=lambda x: x[-1], reverse=True)
+            .subject
+        )
+
+    @FilesystemJSONBase.fetch_dataset_beforehand
     def get_dataset_for_printer(self) -> List[Dict[str, Union[str, int]]]:
         """
         Provides the dataset that the printer may understand.
 
         :raise ValueError:
             When the current testing mode is not supported (yet?).
         """
@@ -158,16 +173,20 @@
 
         if "counter" not in self.dataset:
             self.dataset = copy.deepcopy(self.STD_DATASET)
 
         self.dataset["counter"][status.status] += 1
         self.dataset["counter"]["total"] += 1
 
-        self.dataset["percentage"][status.status] = (
-            self.dataset["counter"][status.status] * 100
-        ) / self.dataset["counter"]["total"]
+        for key in self.dataset["percentage"]:
+            if key == "total":
+                continue
+
+            self.dataset["percentage"][key] = (
+                self.dataset["counter"][key] * 100
+            ) / self.dataset["counter"]["total"]
 
         self.dataset["percentage"]["total"] = sum(
             y for x, y in self.dataset["percentage"].items() if x != "total"
         )
 
         return self
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a common base to the manipulation of the output directory.
+Provides our WHOIS record migrator.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,92 +46,75 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import os
-from typing import Optional
+import domain2idna
 
-import PyFunceble.cli.storage
-from PyFunceble.database.session import DBSession
+import PyFunceble.cli.factory
+import PyFunceble.facility
+import PyFunceble.sessions
+from PyFunceble.cli.migrators.mariadb.base import MariaDBMigratorBase
+from PyFunceble.cli.utils.stdout import print_single_line
+from PyFunceble.database.sqlalchemy.all_schemas import WhoisRecord
 
 
-class FilesystemDirBase:
+class WhoisRecordIDNASubjectMigrator(MariaDBMigratorBase):
     """
-    Provides a common base for the manipulation of our output directory.
+    Provides the interface which provides the completion of the missing
+    IDNA subject column.
     """
 
-    _parent_dirname: Optional[str] = None
-    db_session: Optional[DBSession] = None
-
-    def __init__(
-        self,
-        parent_dirname: Optional[str] = None,
-        *,
-        db_session: Optional[DBSession] = None,
-    ) -> None:
-        if parent_dirname is not None:
-            self.parent_dirname = parent_dirname
-        else:
-            self.parent_dirname = PyFunceble.cli.storage.STD_PARENT_DIRNAME
-
-        self.db_session = db_session
-
     @property
-    def parent_dirname(self) -> Optional[str]:
+    def authorized(self) -> bool:
         """
-        Provides the current state of the :code:`_parent_dirname` attribute.
+        Provides the authorization to process.
         """
 
-        return self._parent_dirname
-
-    @parent_dirname.setter
-    def parent_dirname(self, value: str) -> None:
-        """
-        Sets the parent dirname. The parent dirname is a directory which
-        acts a parent into the output directory.
-
-        :parm value:
-            The value to set.
+        if PyFunceble.cli.facility.CredentialLoader.is_already_loaded():
+            # pylint: disable=singleton-comparison
+            return (
+                self.db_session.query(WhoisRecord)
+                .filter(WhoisRecord.idna_subject == None)
+                .first()
+                is not None
+            )
+        return False
 
-        :raise TypeError:
-            When the given :code:`value` is not a :py:class:`str`.
-        :raise ValueError:
-            When the given :code:`value` is empty.
-        """
+    @MariaDBMigratorBase.execute_if_authorized(None)
+    def migrate(self) -> "WhoisRecordIDNASubjectMigrator":
+        # pylint: disable=singleton-comparison
+
+        broken = False
+
+        for row in self.db_session.query(WhoisRecord).filter(
+            WhoisRecord.idna_subject == None
+        ):
+            if (
+                self.continuous_integration
+                and self.continuous_integration.is_time_exceeded()
+            ):
+                broken = True
+                break
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+            PyFunceble.facility.Logger.info(
+                "Started to fix idna_subject field of %r", row.subject
+            )
+            row.idna_subject = domain2idna.domain2idna(row.subject)
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
+            self.db_session.add(row)
 
-        self._parent_dirname = value
+            if self.print_action_to_stdout:
+                print_single_line()
 
-    def set_parent_dirname(self, value: str) -> "FilesystemDirBase":
-        """
-        Sets the parent dirname. The parent dirname is a directory which
-        acts a parent into the output directory.
+            PyFunceble.facility.Logger.info(
+                "Finished to fix idna_subject field of %r", row.subject
+            )
 
-        :parm value:
-            The value to set.
-        """
+        self.db_session.commit()
 
-        self.parent_dirname = value
+        if not broken:
+            self.done = True
 
         return self
-
-    def get_output_basedir(self) -> str:
-        """
-        Provides the output base directory.
-
-        :param create_if_missing:
-            Authorizes the creation of the directory if it's missing.
-        """
-
-        if self.parent_dirname:
-            return os.path.join(
-                PyFunceble.cli.storage.OUTPUT_DIRECTORY, self.parent_dirname
-            )
-        return PyFunceble.cli.storage.OUTPUT_DIRECTORY
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/backup.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/backup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/restore.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/dir_structure/restore.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/json_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/json_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/db_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all our printers.
+Provides the base of all datasets which acts as database interface.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,296 +46,267 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import copy
 import functools
-import string
-from typing import Dict, Optional
+from typing import Any, Generator, List, Optional
 
+from PyFunceble.dataset.base import DatasetBase
 
-class PrinterBase:
-    """
-    Provides the base of all printer class.
 
-    Printer classes are classes which derivate from this class. their objectives
-    should be the same: Unify and simplify the way to print something to a given
-    destination.
+class DBDatasetBase(DatasetBase):
+    """
+    Provides the base of all datasets which acts as database interface.
     """
 
-    STD_UNKNOWN: str = "Unknown"
+    STD_REMOVE_UNNEEDED_FIELDS: bool = True
+    STD_AUTHORIZED: bool = False
 
-    STD_LENGTH: Dict[str, int] = {
-        "idna_subject": 100,
-        "status": 11,
-        "status_source": 10,
-        "http_status_code": 10,
-        "percentage": 12,
-        "expiration_date": 17,
-        "amount": 12,
-        "checker_type": 13,
-        "days": 2,
-        "hours": 2,
-        "minutes": 2,
-        "seconds": 6,
-        "registrar": 30,
-    }
-
-    TEMPLATES: Dict[str, string.Template] = {
-        "all": string.Template(
-            "$idna_subject $status $status_source $expiration_date $registrar "
-            "$http_status_code $checker_type"
-        ),
-        "less": string.Template("$idna_subject $status $status_source"),
-        "simple": string.Template("$idna_subject $status"),
-        "percentage": string.Template("$status $percentage $amount"),
-        "hosts": string.Template("$ip $idna_subject"),
-        "plain": string.Template("$idna_subject"),
-        "execution_time": string.Template(
-            "\nExecution Time: $days:$hours:$minutes:$seconds\n"
-        ),
-        "registrar": string.Template("$registrar $percentage $amount"),
-    }
-
-    HEADERS: Dict[str, str] = {
-        "idna_subject": "Subject",
-        "status": "Status",
-        "status_source": "Source",
-        "http_status_code": "HTTP Code",
-        "expiration_date": "Expiration Date",
-        "percentage": "Percentage",
-        "amount": "Amount",
-        "ip": "IP",
-        "checker_type": "Checker",
-        "days": "Days",
-        "hours": "Hours",
-        "minutes": "Minutes",
-        "seconds": "Seconds",
-        "registrar": "Registrar",
-    }
+    FIELDS: List[str] = []
+    COMPARISON_FIELDS: List[str] = []
 
-    _template_to_use: Optional[str] = None
-    _dataset: Optional[Dict[str, str]] = None
+    source_file: Optional[str] = None
+
+    _remove_unneeded_fields: Optional[bool] = True
+    _authorized: Optional[bool] = False
 
     def __init__(
         self,
-        template_to_use: Optional[str] = None,
         *,
-        dataset: Optional[Dict[str, str]] = None,
+        authorized: Optional[bool] = None,
+        remove_unneeded_fields: Optional[bool] = None,
     ) -> None:
-        if template_to_use is not None:
-            self.template_to_use = template_to_use
+        if authorized is not None:
+            self.set_authorized(authorized)
 
-        if dataset is not None:
-            self.dataset = dataset
+        if remove_unneeded_fields is not None:
+            self.set_remove_unneeded_fields(remove_unneeded_fields)
 
-    def ensure_template_to_use_is_given(func):  # pylint: disable=no-self-argument
-        """
-        Ensures that the template to use is given before launching the
-        decorated method.
+        self.__post_init__()
 
-        :raise TypeError:
-            When the current :code:`self.template_to_use` is not set.
+    def __post_init__(self) -> None:
         """
-
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(self.template_to_use, str):
-                raise TypeError("<self.template_to_use> is not given.")
-
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
-
-        return wrapper
-
-    def ensure_dataset_is_given(func):  # pylint: disable=no-self-argument
+        A method to be called (automatically) after __init__.
         """
-        Ensures that the dataset to write is given before launching the
-        decorated method.
 
-        :raise TypeError:
-            When the current :code:`self.template_to_use` is not set.
+    def execute_if_authorized(default: Any = None):  # pylint: disable=no-self-argument
+        """
+        Executes the decorated method only if we are authorized to process.
+        Otherwise, apply the given :code:`default`.
         """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(self.dataset, dict):
-                raise TypeError("<self.dataset> is not given.")
+        def inner_metdhod(func):
+            @functools.wraps(func)
+            def wrapper(self, *args, **kwargs):
+                if self.authorized:
+                    return func(self, *args, **kwargs)  # pylint: disable=not-callable
+                return default
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+            return wrapper
 
-        return wrapper
+        return inner_metdhod
 
     @property
-    def template_to_use(self) -> Optional[str]:
+    def authorized(self) -> Optional[bool]:
         """
-        Provides the current state of the :code:`_template_to_use` attribute.
+        Provides the current state of the :code:`_authorized` attribute.
         """
 
-        return self._template_to_use
+        return self._authorized
 
-    @template_to_use.setter
-    def template_to_use(self, value: str) -> None:
+    @authorized.setter
+    def authorized(self, value: bool) -> None:
         """
-        Sets the template to use.
+        Sets the value of the :code:`_authorized` attribute.
 
         :param value:
             The value to set.
 
         :raise TypeError:
-            When the given :code:`value` is not a :py:class:`str`.
-        :raise ValueError:
-            When the given :code:`value` is not supported.
+            When the given :code:`value` is not a :py:class:`bool`
         """
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
-
-        if value not in self.TEMPLATES:
-            raise ValueError(
-                f"<value> ({value!r}) is not supported "
-                f"({list(self.TEMPLATES.keys())!r})."
-            )
+        if not isinstance(value, bool):
+            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
 
-        self._template_to_use = value
+        self._authorized = value
 
-    def set_template_to_use(self, value: str) -> "PrinterBase":
+    def set_authorized(self, value: bool) -> "DBDatasetBase":
         """
-        Sets the template to use.
+        Sets the value of the :code:`_authorized` attribute.
 
         :param value:
             The value to set.
         """
 
-        self.template_to_use = value
+        self.authorized = value
 
         return self
 
     @property
-    def dataset(self) -> Optional[Dict[str, str]]:
+    def remove_unneeded_fields(self) -> Optional[bool]:
         """
-        Provides the current state of the :code:`_dataset` attribute.
+        Provides the current state of the :code:`_remove_unneeded_fields`.
         """
 
-        return self._dataset
+        return self._remove_unneeded_fields
 
-    @dataset.setter
-    def dataset(self, value: Dict[str, str]) -> None:
+    @remove_unneeded_fields.setter
+    def remove_unneeded_fields(self, value: bool) -> None:
         """
-        Sets the dataset to apply to the template.
+        Sets the value of the :code:`_remove_unneeded_fields` attribute.
 
         :param value:
             The value to set.
 
         :raise TypeError:
-            When the given :code:`value` is not a :py:class:`dict`
-        :raise ValueError:
-            When the given :code:`value` is empty.
+            When the given :code:`value` is not a :py:class:`bool`
         """
 
-        if not isinstance(value, dict):
-            raise TypeError(f"<value> should be {dict}, {type(value)} given.")
-
-        if not value:
-            raise ValueError("<value> should not be empty.")
+        if not isinstance(value, bool):
+            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
 
-        self._dataset = copy.deepcopy(value)
+        self._remove_unneeded_fields = value
 
-    def set_dataset(self, value: Dict[str, str]) -> "PrinterBase":
+    def set_remove_unneeded_fields(self, value: bool) -> "DBDatasetBase":
         """
-        Sets the dataset to apply to the template.
+        Sets the value of the :code:`_remove_unneeded_fields` attribute.
 
         :param value:
             The value to set.
         """
 
-        self.dataset = value
+        self.remove_unneeded_fields = value
 
         return self
 
-    @ensure_template_to_use_is_given
-    def get_header_to_print(self) -> str:
+    @execute_if_authorized(dict())  # pylint: disable=use-dict-literal
+    def get_filtered_row(self, row: dict) -> dict:
         """
-        Provides the template header to print.
+        Removes all unkowns fields (not declared) from the given row.
+
+        :param row:
+            The row to work with.
         """
 
-        ignore_header = ["simple", "hosts", "plain", "execution_time"]
+        result = {}
 
-        to_print_data = [dict(), dict()]  # pylint: disable=use-dict-literal
+        for key, value in row.items():
+            if value is None:
+                value = ""
 
-        if self.template_to_use not in ignore_header:
-            for key, value in self.HEADERS.items():
-                if key not in self.TEMPLATES[self.template_to_use].template:
-                    continue
+            if key in self.FIELDS:
+                result[key] = value
 
-                to_print_data[0][key] = f"{value:<{self.STD_LENGTH[key]}}"
+        for field in self.COMPARISON_FIELDS:
+            if field not in result:
+                result[field] = ""
 
-            for key, value in to_print_data[0].items():
-                to_print_data[1][key] = "-" * len(value)
+        return result
 
-            to_print = [
-                self.TEMPLATES[self.template_to_use].safe_substitute(
-                    **to_print_data[0]
-                ),
-                self.TEMPLATES[self.template_to_use].safe_substitute(
-                    **to_print_data[1]
-                ),
-            ]
+    def add(self, row: dict) -> "DBDatasetBase":
+        """
+        Adds the given dataset into the database.
 
-            return "\n".join(to_print)
-        return ""
+        :param row:
+            The row or dataset to add.
 
-    @ensure_template_to_use_is_given
-    @ensure_dataset_is_given
-    def get_line_to_print(self) -> str:
+        :raise TypeError:
+            When the given :code:`row` is not a :py:class`dict`.
         """
-        Provides the line to print.
+
+        raise NotImplementedError()
+
+    def remove(self, row: dict) -> "DBDatasetBase":
         """
+        Removes the given dataset from the database.
 
-        to_print = {}
-        ignore_length = ["simple", "hosts", "plain", "execution_time"]
+        :param row:
+            The row or dataset to remove.
 
-        for key, value in self.dataset.items():
-            if key not in self.HEADERS:
-                continue
+        :raise TypeError:
+            When the given :code:`row` is not a :py:class`dict`.
+        """
 
-            if not value and value != 0:
-                value = self.STD_UNKNOWN
+        raise NotImplementedError()
 
-            if self.template_to_use not in ignore_length:
-                to_print[key] = f"{value:<{self.STD_LENGTH[key]}}"
-            else:
-                to_print[key] = value
+    def update(self, row: dict, *, ignore_if_exist: bool = False) -> "DBDatasetBase":
+        """
+        Adds the given dataset into the database if it does not exists.
+        Update otherwise.
 
-        missings = [
-            x[1:]
-            for x in self.TEMPLATES[self.template_to_use].template.split()
-            if x.startswith("$") and x[1:] not in to_print
-        ]
+        :param row:
+            The row or dataset to manipulate.
 
-        for missing in missings:
-            try:
-                to_print[missing] = f"{self.STD_UNKNOWN:<{self.STD_LENGTH[missing]}}"
-            except KeyError:
-                # Example: execution time
-                pass
+        :param ignore_if_exist:
+            Ignores the insertion/update if the row already exists.
 
-        return self.TEMPLATES[self.template_to_use].safe_substitute(**to_print)
 
-    def print_header(self) -> None:
+        :raise TypeError:
+            When the given :code:`row` is not a :py:class`dict`.
         """
-        Prints the header.
+
+        raise NotImplementedError()
+
+    def get_content(self) -> Generator[Optional[dict], None, None]:
+        """
+        Provides a generator which provides the next line to read.
         """
 
-        header = self.get_header_to_print()
+        raise NotImplementedError()
 
-        if header:
-            print(f"\n\n{header}")
+    def cleanup(self) -> "DBDatasetBase":
+        """
+        Cleanups the dataset.
+        """
 
-    def print_interpolated_line(self) -> None:
+        raise NotImplementedError()
+
+    @execute_if_authorized(None)
+    def get_filtered_content(
+        self, filter_map: dict
+    ) -> Generator[Optional[dict], None, None]:
+        """
+        Provides a generator which provides the next dataset. to read.
+
+        :param filter_map:
+            A dictionary representing what we need to filter.
+
+        :raise TypeError:
+            When the given :code:`filter_map` is not a :py:class:`dict`.
         """
-        Prints the line where we are suppose to write it.
+
+        if not isinstance(filter_map, dict):
+            raise TypeError(f"<filter_map> should be {dict}, {type(filter_map)} given.")
+
+        for row in self.get_content():
+            for key, value in filter_map.items():
+                if key not in row:
+                    continue
+
+                if row[key] == value:
+                    yield row
+
+    def exists(self, row: dict) -> bool:
+        """
+        Checks if the given dataset exists in our dataset.
+
+        :param row:
+            The row or dataset to add.
+        """
+
+        raise NotImplementedError()
+
+    def are_equal(self, read_row: dict, row: dict) -> bool:
+        """
+        Compares the given :code:`read_row` to the `row`.
+
+        :param read_row:
+            The row read from the dataset infrastructure.
+        :param row:
+            The row given by the testing infrastructure.
         """
 
         raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/file.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/stdout.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/printer/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/registrar_counter.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/registrar_counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/status_file.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/filesystem/status_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,27 +572,42 @@
 
     @ensure_status_is_given
     def generate_plain_file(self) -> "StatusFileGenerator":
         """
         Generates the plain file.
         """
 
+        location = None
+
         if not hasattr(self.status, "ip_syntax") or not self.status.ip_syntax:
             location = os.path.join(
                 self.get_output_basedir(),
                 PyFunceble.cli.storage.OUTPUTS.domains.directory,
                 self.status.status.upper(),
                 PyFunceble.cli.storage.OUTPUTS.domains.filename,
             )
 
             self.file_printer.destination = location
             self.file_printer.dataset = self.status.to_dict()
             self.file_printer.template_to_use = "plain"
             self.file_printer.print_interpolated_line()
 
+        if not hasattr(self.status, "ip_syntax") or self.status.subject_kind == "ip":
+            location = os.path.join(
+                self.get_output_basedir(),
+                PyFunceble.cli.storage.OUTPUTS.ips.directory,
+                self.status.status.upper(),
+                PyFunceble.cli.storage.OUTPUTS.ips.filename,
+            )
+
+            self.file_printer.destination = location
+            self.file_printer.dataset = self.status.to_dict()
+            self.file_printer.template_to_use = "plain"
+            self.file_printer.print_interpolated_line()
+
         return self
 
     @ensure_status_is_given
     def generate_analytic_file(self) -> "StatusFileGenerator":
         """
         Generates the analytic files.
         """
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/alembic.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/alembic.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/db_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/hashes_file.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/hashes_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/mining_file.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/mining_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/production_config_file.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/file_cleanup/production_config_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/inactive.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/whois.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/json2csv/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/file_and_status.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/migrators/mariadb/file_and_status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/rpz_input_line2subject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint:disable=line-too-long
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides our WHOIS record migrator.
+Provides the conversion of the an RPZ input line into testable subjects.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -45,76 +46,59 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+# pylint: enable=line-too-long
 
-import domain2idna
+from typing import Any, List
 
-import PyFunceble.cli.factory
-import PyFunceble.facility
-import PyFunceble.sessions
-from PyFunceble.cli.migrators.mariadb.base import MariaDBMigratorBase
-from PyFunceble.cli.utils.stdout import print_single_line
-from PyFunceble.database.sqlalchemy.all_schemas import WhoisRecord
+from PyFunceble.converter.input_line2subject import InputLine2Subject
 
 
-class WhoisRecordIDNASubjectMigrator(MariaDBMigratorBase):
+class RPZInputLine2Subject(InputLine2Subject):
     """
-    Provides the interface which provides the completion of the missing
-    IDNA subject column.
+    Converts/Extracts the subject from the given RPZ inputline.
     """
 
-    @property
-    def authorized(self) -> bool:
+    COMMENT: list = [";", "//", "#"]
+    SPECIAL: list = ["$", "@"]
+
+    def get_converted(self) -> List[str]:
         """
-        Provides the authorization to process.
+        Provides the converted data.
         """
 
-        if PyFunceble.cli.facility.CredentialLoader.is_already_loaded():
-            # pylint: disable=singleton-comparison
-            return (
-                self.db_session.query(WhoisRecord)
-                .filter(WhoisRecord.idna_subject == None)
-                .first()
-                is not None
-            )
-        return False
-
-    @MariaDBMigratorBase.execute_if_authorized(None)
-    def migrate(self) -> "WhoisRecordIDNASubjectMigrator":
-        # pylint: disable=singleton-comparison
-
-        broken = False
-
-        for row in self.db_session.query(WhoisRecord).filter(
-            WhoisRecord.idna_subject == None
-        ):
-            if (
-                self.continuous_integration
-                and self.continuous_integration.is_time_exceeded()
-            ):
-                broken = True
-                break
-
-            PyFunceble.facility.Logger.info(
-                "Started to fix idna_subject field of %r", row.subject
-            )
-            row.idna_subject = domain2idna.domain2idna(row.subject)
+        return self.convert(self.data_to_convert)
 
-            self.db_session.add(row)
-
-            if self.print_action_to_stdout:
-                print_single_line()
-
-            PyFunceble.facility.Logger.info(
-                "Finished to fix idna_subject field of %r", row.subject
-            )
+    def convert(self, data: Any, *, aggressive: bool = False) -> List[str]:
+        """
+        Converts the given dataset.
 
-        self.db_session.commit()
+        :param data:
+            The data to convert.
+        """
 
-        if not broken:
-            self.done = True
+        _ = aggressive
+        result = []
+        subject = data.strip()
+
+        if (
+            subject
+            and not any(subject.startswith(x) for x in self.COMMENT)
+            and not any(subject.startswith(x) for x in self.SPECIAL)
+        ):
+            for comment_sign in self.COMMENT:
+                if comment_sign in subject:
+                    subject = subject[: subject.find(comment_sign)].strip()
+
+            if self.SPACE in subject or self.TAB in subject:
+                subject = subject.split()[0]
+
+                if not subject.isdigit():
+                    result.append(subject)
+            elif not subject.isdigit():
+                result.append(subject)
 
-        return self
+        return result
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_producer.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_tester.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/dir_files_sorter.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/file_sorter.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/migrator.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/miner.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/producer.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/tester.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_producer.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_tester.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/dir_files_sorter.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/file_sorter_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/migrator.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/miner.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/producer.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/producer.py`

 * *Files 6% similar despite different names*

```diff
@@ -342,23 +342,31 @@
             self.status_file_generator.allow_plain_files = previous_allow_plain_file
 
     def run_counter(self, test_dataset: dict, test_result: CheckerStatusBase) -> None:
         """
         Runs the counter of the current file.
         """
 
-        if (
-            test_dataset["destination"]
-            and not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file
-        ):
+        if not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file:
             # Note: We don't want hidden data to be counted.
 
-            self.counter.set_parent_dirname(test_dataset["destination"]).count(
-                test_result
+            self.counter.set_differ_to_inline(True).set_parent_dirname(
+                test_dataset["destination"]
             )
+            self.registrar_counter.set_differ_to_inline(True).set_parent_dirname(
+                test_dataset["destination"]
+            )
+
+            self.counter.count(test_result)
+
+            if hasattr(test_result, "registrar") and test_result.registrar:
+                self.registrar_counter.count(test_result.registrar)
+
+            self.counter.set_differ_to_inline(False)
+            self.registrar_counter.set_differ_to_inline(False)
 
             if hasattr(test_result, "registrar") and test_result.registrar:
                 self.registrar_counter.set_parent_dirname(
                     test_dataset["destination"]
                 ).count(test_result.registrar)
 
     def target(self, consumed: Any) -> Optional[Tuple[Any, ...]]:
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/tester.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/processes/workers/tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 import PyFunceble.facility
 import PyFunceble.factory
 from PyFunceble.checker.availability.domain_and_ip import DomainAndIPAvailabilityChecker
 from PyFunceble.checker.availability.url import URLAvailabilityChecker
 from PyFunceble.checker.base import CheckerBase
 from PyFunceble.checker.reputation.domain_and_ip import DomainAndIPReputationChecker
 from PyFunceble.checker.reputation.url import URLReputationChecker
-from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.domain_and_ip import DomainAndIPSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
 from PyFunceble.cli.processes.workers.base import WorkerBase
 from PyFunceble.cli.utils.stdout import print_single_line
 from PyFunceble.dataset.autocontinue.base import ContinueDatasetBase
 from PyFunceble.dataset.autocontinue.csv import CSVContinueDataset
 from PyFunceble.dataset.inactive.base import InactiveDatasetBase
@@ -97,15 +97,15 @@
         self.inactive_dataset = (
             PyFunceble.cli.utils.testing.get_inactive_dataset_object(
                 db_session=self.db_session
             )
         )
 
         self.known_testing_objects = {
-            "SYNTAX": {"domain": DomainSyntaxChecker, "url": URLSyntaxChecker},
+            "SYNTAX": {"domain": DomainAndIPSyntaxChecker, "url": URLSyntaxChecker},
             "AVAILABILITY": {
                 "domain": DomainAndIPAvailabilityChecker,
                 "url": URLAvailabilityChecker,
             },
             "REPUTATION": {
                 "domain": DomainAndIPReputationChecker,
                 "url": URLReputationChecker,
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/iana.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/production.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/public_suffix.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/scripts/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,48 +63,90 @@
 
 if PlatformUtility.is_unix() and sys.stdin.encoding == "utf-8":
     STD_EPILOG: str = (
         f"Crafted with {colorama.Fore.RED}♥{colorama.Fore.RESET} by "
         f"{colorama.Style.BRIGHT}{colorama.Fore.CYAN}Nissar Chababy (@funilrys)"
         f"{colorama.Style.RESET_ALL} "
         f"with the help of\n{colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPS{colorama.Style.RESET_ALL} "
+        f"https://pyfunceble.github.io/#/contributors{colorama.Style.RESET_ALL} "
         f"&& {colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPF{colorama.Style.RESET_ALL}"
+        f"https://pyfunceble.github.io/#/special-thanks{colorama.Style.RESET_ALL}"
     )
 
     ASCII_PYFUNCEBLE = """
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
     """
+
+    ASCII_PYUNCEBLE_RESULT = """
+                          █
+                        ████    ██
+                     ███ ██   █████   ███
+               ███ █████    █████   █████
+             ██████████   █████   █████
+           ██████████   █████   ██████   ██
+         ██████████   █████   ██████   ████
+       ███████████████████████████   █████
+      ██████████████████████████   ████
+     ████████ █████ ██████████   █████
+     ███████   ███   ███████   █████
+     █████████████████████   █████
+     ████████████████████  █████
+     ███████         █████████
+      ████████     █████████
+        ██████████████████
+          ██████████████
+               ████
+
+    """
     DONE: str = f"{colorama.Fore.GREEN}✔"
     ERROR: str = f"{colorama.Fore.RED}✘"
 else:
     STD_EPILOG: str = (
         f"Crafted with {colorama.Fore.RED}HEART{colorama.Fore.RESET} by "
         f"{colorama.Style.BRIGHT}{colorama.Fore.CYAN}Nissar Chababy (@funilrys)"
         f"{colorama.Style.RESET_ALL} "
         f"with the help of\n{colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPS{colorama.Style.RESET_ALL} "
+        f"https://pyfunceble.github.io/#/contributors{colorama.Style.RESET_ALL} "
         f"&& {colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPF{colorama.Style.RESET_ALL}"
+        f"https://pyfunceble.github.io/#/special-thanks{colorama.Style.RESET_ALL}"
     )
     ASCII_PYFUNCEBLE = """
     ########  ##    ## ######## ##     ## ##    ##  ######  ######## ########  ##       ########
     ##     ##  ##  ##  ##       ##     ## ###   ## ##    ## ##       ##     ## ##       ##
     ##     ##   ####   ##       ##     ## ####  ## ##       ##       ##     ## ##       ##
     ########     ##    ######   ##     ## ## ## ## ##       ######   ########  ##       ######
     ##           ##    ##       ##     ## ##  #### ##       ##       ##     ## ##       ##
     ##           ##    ##       ##     ## ##   ### ##    ## ##       ##     ## ##       ##
     ##           ##    ##        #######  ##    ##  ######  ######## ########  ######## ########
-"""
+    """
+    ASCII_PYUNCEBLE_RESULT = """
+                          .
+                        :==:    ::
+                     .:. ..   :-=-.   .:.
+               .:. .-==-    :-=-:   .-==:
+             .-==--==-.   :-=-:   .-==:
+           .-===-==-.   :-=-:   .-==:.   ..
+         .-==-====:   :-==.   .-==:.   :==-
+       .-==--=====-::-==-=:..-==:.   ..--.
+      :===============-=======:.   :-=:
+     :=-===:  .-=-. .-======:.   :==-.
+     -=====.   --:   -====-.   :==-.
+     =======--=====-====:.   :==-.
+     -=====---:::::---==.  :==-.
+     .==--=.         -===-==-.
+      .-==--:      .-=-===-.
+        :-====-----=====-.
+          .:-=======--:.
+               ....
+    """
     DONE: str = f"{colorama.Fore.GREEN}DONE"
     ERROR: str = f"{colorama.Fore.RED}ERROR"
 
 VERSION_DUMP_LINK: str = (
     "https://raw.githubusercontent.com/funilrys/PyFunceble/dev/version.yaml"
 )
 
@@ -130,14 +172,15 @@
 PRE_LOADER_FILE = "preload.json"
 
 STD_PARENT_DIRNAME: str = "__pyfunceble_origin__"
 STD_LOGGING_DIRNAME: str = "__pyfunceble_loggging__"
 
 UNIX_OUTPUTS: dict = {
     "domains": {"filename": "list"},
+    "ips": {"filename": "list"},
     "hosts": {"filename": "hosts", "ip_filename": "ips"},
     "analytic": {
         "filenames": {
             "potentially_down": "down_or_potentially_down",
             "potentially_up": "potentially_up",
             "up": "active_and_merged_in_results",
             "suspicious": "suspicious_and_merged_in_results",
@@ -148,14 +191,15 @@
             "inactive_not_retested": "inactive_not_retested",
         },
     },
 }
 
 WIN_OUTPUTS: dict = {
     "domains": {"filename": "list.txt"},
+    "ips": {"filename": "list.txt"},
     "hosts": {"filename": "hosts.txt", "ip_filename": "ips.txt"},
     "analytic": {
         "filenames": {
             "potentially_down": "down_or_potentially_down.txt",
             "potentially_up": "potentially_up.txt",
             "up": "active_and_merged_in_results.txt",
             "suspicious": "suspicious_and_merged_in_results.txt",
@@ -166,14 +210,15 @@
             "inactive_not_retested": "inactive_not_retested.txt",
         },
     },
 }
 
 UNIVERSAL_OUTPUTS: dict = {
     "domains": {"directory": "domains", "filename": "list"},
+    "ips": {"directory": "ips", "filename": "list"},
     "hosts": {"directory": "hosts", "filename": "hosts", "ip_filename": "ips"},
     "analytic": {
         "directories": {
             "parent": "Analytic",
             "potentially_down": "POTENTIALLY_INACTIVE",
             "potentially_up": "POTENTIALLY_ACTIVE",
             "up": "ACTIVE",
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage_facility.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/system/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/system/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/integrator.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/system/integrator.py`

 * *Files 7% similar despite different names*

```diff
@@ -187,14 +187,36 @@
                 f"{colorama.Style.BRIGHT}{colorama.Fore.MAGENTA}Your setup won't "
                 "generate any output! "
                 "Reason: file_generation.hosts and file_generation.plain are "
                 "both disabled."
             )
 
     @SystemBase.ensure_args_is_given
+    def check_deprecated(self) -> "SystemIntegrator":
+        """
+        Checks or do some deprecation checks.
+
+        This method will basically check if deprecated keys are still given and
+        provide guidance for end-users.
+
+        !!! warning
+
+            The messages are not directly printed, but rather stored in the
+            PyFunceble.cli.storage.EXTRA_MESSAGES list.
+        """
+
+        if "adblock_aggressive" in PyFunceble.storage.CONFIGURATION.cli_decoding:
+            PyFunceble.cli.storage.EXTRA_MESSAGES.append(
+                f"{colorama.Style.BRIGHT}{colorama.Fore.MAGENTA}The "
+                "'cli_decoding.adblock_aggressive' configuration key has been "
+                "replaced by the 'cli_decoding.aggressive' key but you are "
+                "still setting it."
+            )
+
+    @SystemBase.ensure_args_is_given
     def start(self) -> "SystemIntegrator":
         """
         Starts a group of actions provided by this interface.
         """
 
         if hasattr(self.args, "output_location") and self.args.output_location:
             PyFunceble.cli.storage.OUTPUT_DIRECTORY = os.path.realpath(
@@ -206,12 +228,13 @@
 
         self.init_logger()
 
         PyFunceble.facility.Logger.debug("Given arguments:\n%r", self.args)
 
         self.inject_into_config()
         self.check_config()
+        self.check_deprecated()
 
         PyFunceble.cli.facility.CredentialLoader.start()
         PyFunceble.cli.factory.DBSession.init_db_sessions()
 
         return self
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/launcher.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/system/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 from PyFunceble.converter.rpz_policy2subject import RPZPolicy2Subject
 from PyFunceble.converter.subject2complements import Subject2Complements
 from PyFunceble.converter.url2netloc import Url2Netloc
 from PyFunceble.converter.wildcard2subject import Wildcard2Subject
 from PyFunceble.dataset.autocontinue.base import ContinueDatasetBase
 from PyFunceble.dataset.autocontinue.csv import CSVContinueDataset
 from PyFunceble.dataset.inactive.base import InactiveDatasetBase
+from PyFunceble.helpers.directory import DirectoryHelper
 from PyFunceble.helpers.download import DownloadHelper
 from PyFunceble.helpers.file import FileHelper
 
 
 class SystemLauncher(SystemBase):
     """
     Provides the system tests launcher.
@@ -571,14 +572,15 @@
 
                         if "SOA" in line:
                             self.rpz_policy2subject.set_soa(line.split()[0])
 
                         for subject in get_subjects_from_line(
                             line,
                             self.checker_type,
+                            subject_type=protocol["subject_type"],
                             adblock_inputline2subject=self.adblock_inputline2subject,
                             wildcard2subject=self.wildcard2subject,
                             rpz_policy2subject=self.rpz_policy2subject,
                             rpz_inputline2subject=self.rpz_inputline2subject,
                             inputline2subject=self.inputline2subject,
                             subject2complements=self.subject2complements,
                             url2netloc=self.url2netloc,
@@ -621,14 +623,15 @@
         for protocol in self.testing_protocol:
             self.ci_stop_in_the_middle_if_time_exceeded()
 
             if protocol["type"] == "single":
                 for subject in get_subjects_from_line(
                     protocol["idna_subject"],
                     self.checker_type,
+                    subject_type=protocol["subject_type"],
                     adblock_inputline2subject=self.adblock_inputline2subject,
                     wildcard2subject=self.wildcard2subject,
                     rpz_policy2subject=self.rpz_policy2subject,
                     rpz_inputline2subject=self.rpz_inputline2subject,
                     inputline2subject=self.inputline2subject,
                     subject2complements=self.subject2complements,
                     url2netloc=self.url2netloc,
@@ -650,21 +653,23 @@
 
     def generate_waiting_files(self) -> "SystemLauncher":
         """
         Generates all the files that needs to be generated when all status
         are proceeses.
         """
 
-        def generate_percentage_file(parent_dirname: str) -> None:
+        def generate_percentage_file(parent_dirname: Union[str, None]) -> None:
             """
             Generates the percentage file.
             """
 
             if not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file:
-                self.counter.set_parent_dirname(parent_dirname)
+                self.counter.set_differ_to_inline(True).set_parent_dirname(
+                    parent_dirname
+                )
 
                 destination = os.path.join(
                     self.counter.get_output_basedir(),
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.parent,
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.percentage,
                     PyFunceble.cli.storage.OUTPUTS.logs.filenames.percentage,
                 )
@@ -687,21 +692,23 @@
 
                         if not stdout_header_printed:
                             self.stdout_printer.print_header()
                             stdout_header_printed = True
 
                         self.stdout_printer.print_interpolated_line()
 
-        def generate_registrar_file(parent_dirname: str) -> None:
+        def generate_registrar_file(parent_dirname: Union[str, None]) -> None:
             """
             Generates the registrar file.
             """
 
             if not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file:
-                self.registrar_counter.set_parent_dirname(parent_dirname)
+                self.registrar_counter.set_differ_to_inline(True).set_parent_dirname(
+                    parent_dirname
+                )
 
                 destination = os.path.join(
                     self.counter.get_output_basedir(),
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.parent,
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.percentage,
                     PyFunceble.cli.storage.OUTPUTS.logs.filenames.registrar,
                 )
@@ -728,19 +735,57 @@
                         if not stdout_header_printed:
                             self.stdout_printer.print_header()
                             stdout_header_printed = True
 
                         self.stdout_printer.print_interpolated_line()
                         registrar_limit += 1
 
+        def print_result_ascii(parent_dirname: Union[str, None]) -> None:
+            """
+            Generates the result repr.
+            """
+
+            # pylint: disable=line-too-long
+            if (
+                not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file
+                and not PyFunceble.storage.CONFIGURATION.cli_testing.display_mode.quiet
+                and PyFunceble.cli.utils.stdout.get_template_to_use() != "simple"
+            ):
+                self.counter.set_differ_to_inline(True).set_parent_dirname(
+                    parent_dirname
+                )
+
+                print(
+                    PyFunceble.cli.utils.ascii_logo.get_result_representation(
+                        self.counter.get_sorted_dataset()[0][0]
+                    )
+                )
+
+        no_destination_found = []
+        amount_protocol_without_dest = len(
+            [x["destination"] for x in self.testing_protocol if not x["destination"]]
+        )
+
         for protocol in self.testing_protocol:
             if not protocol["destination"]:
-                continue
+                if any(no_destination_found):
+                    continue
 
-            generate_percentage_file(protocol["destination"])
+                if amount_protocol_without_dest >= 2:
+                    # Show percentage, only if the amount of subjects is > 2.
+                    generate_percentage_file(protocol["destination"])
+            else:
+                generate_percentage_file(protocol["destination"])
+
+            if protocol["checker_type"] in self.registrar_counter.SUPPORTED_TEST_MODES:
+                generate_registrar_file(protocol["destination"])
+
+            print_result_ascii(protocol["destination"])
+
+            no_destination_found.append(not protocol["destination"])
 
             if protocol["checker_type"] in self.registrar_counter.SUPPORTED_TEST_MODES:
                 generate_registrar_file(protocol["destination"])
 
             # pylint: disable=line-too-long
             if (
                 PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.merge_output_dirs
@@ -827,23 +872,39 @@
                     os.path.join(
                         protocol["output_dir"],
                         PyFunceble.cli.storage.PRE_LOADER_FILE,
                     )
                 ).delete()
                 PyFunceble.facility.Logger.debug("Deleted: %r.", file_helper.path)
 
+        def remove_inline_dest(protocol: dict) -> None:
+            """
+            Remove the inline destination - when necessary.
+
+            :param protocl:
+                The protocol to work with.
+            """
+
+            if not protocol["destination"]:
+                DirectoryHelper(
+                    self.counter.set_differ_to_inline(True)
+                    .set_parent_dirname(protocol["destination"])
+                    .get_output_basedir()
+                ).delete()
+
         file_helper = FileHelper()
 
         for protocol in self.testing_protocol:
             if "destination" in protocol or "output_dir" in protocol:
                 remove_running_file(protocol)
                 remove_trigger_file(protocol)
 
                 remove_continue_dataset(protocol)
                 remove_preload_dataset(protocol)
+                remove_inline_dest(protocol)
 
         return self
 
     def run_standard_end_instructions(self) -> "SystemLauncher":
         """
         Runns our standard "end" instructions.
 
@@ -993,14 +1054,15 @@
                 # Reason: We have to continue.
                 self.run_ci_saving_instructions()
             elif self.continuous_integration.authorized:
                 # Includes the run_standard_end_instructions call.
                 self.run_ci_end_saving_instructions()
             else:
                 self.run_standard_end_instructions()
+
         except (KeyboardInterrupt, StopExecution):
             pass
         except Exception as exception:  # pylint: disable=broad-except
             PyFunceble.facility.Logger.critical(
                 "Fatal error.",
                 exc_info=True,
             )
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/ascii_logo.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/record/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some utilities related to the ascii logo.
+Provides the base of all our record classes.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,56 +46,46 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import colorama
+import dataclasses
+import json
+from typing import Any
 
-import PyFunceble.cli.storage
-import PyFunceble.facility
-import PyFunceble.storage
 
-
-def colorify(color: str) -> str:
+@dataclasses.dataclass
+class RecordBase:
     """
-    Colorify the logo with the given color.
-
-    :param color:
-        The name of the color to apply.
-
-        .. warning::
-            The given color name must be one of the supported
-            by colorama.
-
-    :raise ValueError:
-        When the given :code:`color` is unsupported.
+    Provides the base of all query record classes.
     """
 
-    color = color.upper()
-
-    if not hasattr(colorama.Fore, color):
-        raise ValueError(f"<color> ({color!r}) is not supported.")
-
-    color_to_apply = getattr(colorama.Fore, color)
-    result = []
-
-    to_color = PyFunceble.cli.storage.ASCII_PYFUNCEBLE
-
-    if (
-        PyFunceble.facility.ConfigLoader.is_already_loaded()
-        and PyFunceble.storage.CONFIGURATION.cli_testing.display_mode.colour
-    ):
-        for line in to_color.split("\n"):
-            result.append(f"{color_to_apply}{line}{colorama.Fore.RESET}")
-
-        return "\n".join(result)
-    return to_color
-
-
-def get_home_representation() -> str:
-    """
-    Provides our home ASCII logo representation.
-    """
+    def __getitem__(self, key: str) -> Any:
+        return getattr(self, key)
 
-    return colorify("yellow")
+    def to_dict(self) -> dict:
+        """
+        Provides the dict representation of the current object.
+        """
+
+        return {
+            x: y if not hasattr(y, "to_dict") else y.to_dict()
+            for x, y in self.__dict__.items()
+            if not x.startswith("__")
+        }
+
+    def to_json(self, *, pretty_print: bool = False) -> str:
+        """
+        Provides the JSON representation of the current object.
+
+        :param pretty_print:
+            If True, the JSON will be formatted.
+        """
+
+        return json.dumps(
+            self.to_dict(),
+            indent=4 if pretty_print else None,
+            ensure_ascii=False,
+            sort_keys=True if pretty_print else None,
+        )
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/sort.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/utils/sort.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/stdout.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/testing.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/utils/testing.py`

 * *Files 13% similar despite different names*

```diff
@@ -178,14 +178,15 @@
     return RegexHelper("[^a-zA-Z0-9._-]").replace_match(origin, "_")
 
 
 def get_subjects_from_line(
     line: str,
     checker_type: str,
     *,
+    subject_type: str = "domain",
     adblock_inputline2subject: Optional[AdblockInputLine2Subject] = None,
     wildcard2subject: Optional[Wildcard2Subject] = None,
     rpz_policy2subject: Optional[RPZPolicy2Subject] = None,
     rpz_inputline2subject: Optional[RPZInputLine2Subject] = None,
     inputline2subject: Optional[InputLine2Subject] = None,
     subject2complements: Optional[Subject2Complements] = None,
     url2netloc: Optional[Url2Netloc] = None,
@@ -194,45 +195,64 @@
     """
     Provides the list of subject to test.
     """
 
     result = []
 
     if adblock_inputline2subject is None:
-        adblock_inputline2subject = AdblockInputLine2Subject()
+        adblock_inputline2subject = AdblockInputLine2Subject(
+            aggressive=bool(PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive)
+        )
 
     if wildcard2subject is None:
-        wildcard2subject = Wildcard2Subject()
+        wildcard2subject = Wildcard2Subject(
+            aggressive=bool(PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive)
+        )
 
     if rpz_policy2subject is None:
         rpz_policy2subject = RPZPolicy2Subject()
 
     if rpz_inputline2subject is None:
-        rpz_inputline2subject = RPZInputLine2Subject()
+        rpz_inputline2subject = RPZInputLine2Subject(
+            aggressive=bool(PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive)
+        )
 
     if inputline2subject is None:
-        inputline2subject = InputLine2Subject()
+        inputline2subject = InputLine2Subject(
+            aggressive=bool(PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive)
+        )
 
     if subject2complements is None:
         subject2complements = Subject2Complements()
 
     if url2netloc is None:
-        url2netloc = Url2Netloc()
+        url2netloc = Url2Netloc(
+            aggressive=bool(PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive)
+        )
 
     if cidr2subject is None:
         cidr2subject = CIDR2Subject()
 
+    adblock_inputline2subject.aggressive = (
+        wildcard2subject.aggressive
+    ) = (
+        rpz_inputline2subject.aggressive
+    ) = inputline2subject.aggressive = url2netloc.aggressive = bool(
+        PyFunceble.storage.CONFIGURATION.cli_decoding.aggressive
+    )
+
+    if inputline2subject.aggressive and subject_type == "url":
+        # URL Decoder doesn't have an aggressive mode.
+        # Therefore, we fix the "misconfiguration"
+        inputline2subject.aggressive = not inputline2subject.aggressive
+
     if PyFunceble.storage.CONFIGURATION.cli_decoding.adblock:
         result.extend(
             # pylint: disable=line-too-long
-            adblock_inputline2subject.set_aggressive(
-                bool(PyFunceble.storage.CONFIGURATION.cli_decoding.adblock_aggressive)
-            )
-            .set_data_to_convert(line)
-            .get_converted()
+            adblock_inputline2subject.set_data_to_convert(line).get_converted()
         )
     elif PyFunceble.storage.CONFIGURATION.cli_decoding.wildcard:
         result.append(wildcard2subject.set_data_to_convert(line).get_converted())
     elif PyFunceble.storage.CONFIGURATION.cli_decoding.rpz:
         result.extend(
             [
                 rpz_policy2subject.set_data_to_convert(x).get_converted()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/version.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/config/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/config/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/config/compare.py` & `PyFunceble-dev-4.2.1/PyFunceble/config/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         "ci_autosave_commit": "cli_testing.ci.commit_message",
         "ci_autosave_final_commit": "cli_testing.ci.end_commit_message",
         "ci_autosave_minutes": "cli_testing.ci.max_exec_minutes",
         "ci_branch": "cli_testing.ci.branch",
         "ci_distribution_branch": "cli_testing.ci.distribution_branch",
         "whois_database": "cli_testing.whois_db",
         "wildcard": "cli_decoding.wildcard",
+        "cli_decoding.adblock_aggressive": "cli_decoding.aggressive",
     }
 
     OLD_TO_NEW_NEGATE: dict = {
         "no_special": "lookup.special",
         "no_whois": "lookup.whois",
         "split": "cli_testing.file_generation.unified_results",
     }
@@ -274,14 +275,17 @@
         for index in self.local_config["links"]:
             if index in self.DELETED_LINKS:
                 return False
 
         if "self_managed" in self.local_config["http_codes"] and not bool(
             self.local_config["http_codes"]["self_managed"]
         ):
+            if "http_codes" not in self.upstream_config:
+                return False
+
             for index, values in self.local_config["http_codes"]["list"].items():
                 if set(self.upstream_config["http_codes"]["list"][index]) != set(
                     values
                 ):
                     return False
 
         return True
@@ -308,26 +312,32 @@
         for key, value in self.OLD_TO_NEW.items():
             if key not in flatten_original:
                 continue
 
             if value not in flatten_upstream:  # pragma: no cover ## Safety.
                 raise RuntimeError(f"<value> ({value!r}) not found.")
 
-            flatten_original[value] = original_local[key]
+            if "." not in key:
+                flatten_original[value] = original_local[key]
+            else:
+                flatten_original[value] = flatten_original[key]
 
             del flatten_original[key]
 
         for key, value in self.OLD_TO_NEW_NEGATE.items():
             if key not in flatten_original:
                 continue
 
             if value not in flatten_upstream:  # pragma: no cover ## Safety.0
                 raise RuntimeError(f"<value> ({value!r}) not found.")
 
-            flatten_original[value] = not original_local[key]
+            if "." not in key:
+                flatten_original[value] = not original_local[key]
+            else:
+                flatten_original[value] = not flatten_original[key]
 
             del flatten_original[key]
 
         original_local = self.dict_helper.set_subject(flatten_original).unflatten()
         del flatten_original
 
         merged = Merge(original_local).into(original_upstream)
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/config/loader.py` & `PyFunceble-dev-4.2.1/PyFunceble/config/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,26 +337,29 @@
             config = self.dict_helper.from_yaml_file(self.path_to_config)
         except MarkedYAMLError:
             self.file_helper.set_path(self.path_to_default_config).copy(
                 self.path_to_config
             )
             config = self.dict_helper.from_yaml_file(self.path_to_config)
 
+        config_comparer = ConfigComparison(
+            local_config=config,
+            upstream_config=self.dict_helper.from_yaml_file(
+                self.path_to_default_config
+            ),
+        )
+
         if (
             not config
             or not isinstance(config, dict)
             or self.merge_upstream
             or is_3_x_version(config)
+            or not config_comparer.is_local_identical()
         ):  # pragma: no cover ## Testing the underlying comparison method is sufficent
-            config = ConfigComparison(
-                local_config=config,
-                upstream_config=self.dict_helper.from_yaml_file(
-                    self.path_to_default_config
-                ),
-            ).get_merged()
+            config = config_comparer.get_merged()
 
             self.dict_helper.set_subject(config).to_yaml_file(self.path_to_config)
 
         if self.file_helper.set_path(self.path_to_overwrite_config).exists():
             overwrite_data = self.dict_helper.from_yaml_file(
                 self.path_to_overwrite_config
             )
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/adblock_input_line2subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/adblock_input_line2subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,27 +68,24 @@
     _aggressive: bool = False
 
     _regex_helper: Optional[RegexHelper] = None
 
     def __init__(
         self,
         data_to_convert: Optional[Any] = None,
-        aggressive: bool = False,
         *,
+        aggressive: bool = False,
         regex_helper: Optional[RegexHelper] = None,
     ) -> None:
-        if aggressive is not None:
-            self.aggressive = aggressive
-
         if regex_helper is None:
             self._regex_helper = RegexHelper()
         else:
             self._regex_helper = regex_helper
 
-        super().__init__(data_to_convert=data_to_convert)
+        super().__init__(data_to_convert=data_to_convert, aggressive=aggressive)
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
         :raise TypeError:
@@ -99,45 +96,14 @@
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         # pylint: disable=no-member
         super(AdblockInputLine2Subject, self.__class__).data_to_convert.fset(
             self, value
         )
 
-    @property
-    def aggressive(self) -> bool:
-        """
-        Provides the state of the :code:`_aggressive` attribute.
-        """
-
-        return self._aggressive
-
-    @aggressive.setter
-    def aggressive(self, value: bool) -> None:
-        """
-        Provides a way to activate/deactivate the aggressive decoding.
-
-        :raise TypeError:
-            When the given data to convert is not :py:class:`str`
-        """
-
-        if not isinstance(value, bool):
-            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
-
-        self._aggressive = value
-
-    def set_aggressive(self, value: bool) -> "AdblockInputLine2Subject":
-        """
-        Provides a way to activate/deactivate the aggressive decoding.
-        """
-
-        self.aggressive = value
-
-        return self
-
     @staticmethod
     def should_be_ignored(line: str) -> bool:
         """
         Checks if we should ignore the given line.
         """
 
         starting_chars = ["!", "@@", "/", "[", ".", "-", "_", "?", "&"]
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all our converter class.
+Provides the base of all WHOIS converter/extracter class.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,65 +46,80 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
+import functools
 from typing import Any, Optional
 
 
 class ConverterBase:
     """
     Provides the base of all converter class.
     """
 
     _data_to_convert: Optional[Any] = None
 
     def __init__(self, data_to_convert: Optional[Any] = None) -> None:
         if data_to_convert is not None:
             self.data_to_convert = data_to_convert
 
+    def ensure_data_to_convert_is_given(func):  # pylint: disable=no-self-argument
+        """
+        Ensures that the data to convert is given before running the decorated method.
+
+        :raise TypeError:
+            If the subject is not a string.
+        """
+
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if not isinstance(self.data_to_convert, str):
+                raise TypeError(
+                    f"<self.subject> should be {str}, "
+                    f"{type(self.data_to_convert)} given."
+                )
+
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+
+        return wrapper
+
     @property
     def data_to_convert(self) -> Optional[Any]:
         """
         Provides the current state of the :code:`_data_to_convert` attribute.
         """
 
         return self._data_to_convert
 
     @data_to_convert.setter
-    def data_to_convert(self, value: Any) -> None:
+    def data_to_convert(self, value: Any) -> Any:
         """
         Sets the data to convert / to work with.
 
         :param value:
-            The value to set.
+            The data to convert
         """
 
         self._data_to_convert = value
 
     def set_data_to_convert(self, value: Any) -> "ConverterBase":
         """
         Sets the data to convert / to work with.
 
         :param value:
-            The value to set.
+            The data to convert
         """
 
         self.data_to_convert = value
 
         return self
 
+    @ensure_data_to_convert_is_given
     def get_converted(self) -> Optional[Any]:
         """
         Provides the converted data.
         """
 
         raise NotImplementedError()
-
-    def convert(self, data: Any) -> Optional[Any]:
-        """
-        Converts the given dataset.
-        """
-
-        raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/cidr2subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/cidr2subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,22 +96,23 @@
     def get_converted(self) -> List[str]:
         """
         Provides the subject-s to test.
         """
 
         return self.convert(self.data_to_convert)
 
-    def convert(self, data: Any) -> List[str]:
+    def convert(self, data: Any, *, aggressive: bool = False) -> List[str]:
         """
         Converts the given dataset.
 
         :param data:
             The data to convert.
         """
 
+        _ = aggressive
         result = set()
 
         subject = data.strip()
 
         if subject:
             try:
                 self.ip_syntax_checker.set_subject(subject)
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/input_line2subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/subject2complements.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the default input line converter.
+Provides an easy way to convert and get the complements of a subject.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,86 +46,111 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+# pylint: enable=line-too-long
 
-from typing import Any, List
+from typing import Any, List, Optional
 
-from PyFunceble.checker.syntax.ip import IPSyntaxChecker
+from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
 from PyFunceble.converter.base import ConverterBase
 
 
-class InputLine2Subject(ConverterBase):
+class Subject2Complements(ConverterBase):
     """
-    Converts/Extract the subjcts to test from an inputed line.
+    Converts a given wildcard into a testable subject.
     """
 
-    COMMENT: str = "#"
-    PARTICULAR_COMMENT: List[str] = ["!"]
-    SPACE: str = " "
-    NSLOOKUP_SPACE: str = "\\032"
-    TAB: str = "\t"
+    _include_given: bool = False
+
+    def __init__(
+        self,
+        data_to_convert: Optional[Any] = None,
+        *,
+        include_given: Optional[bool] = False,
+    ) -> None:
+        if include_given is not None:
+            self.include_given = include_given
+
+        super().__init__(data_to_convert=data_to_convert)
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
         :raise TypeError:
-            When the given data to convert is not :py:class:`str`
+            When the given data to convert is not :py:class:`str` or a
+            :py:class:`list`.
         """
 
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         # pylint: disable=no-member
-        super(InputLine2Subject, self.__class__).data_to_convert.fset(self, value)
+        super(Subject2Complements, self.__class__).data_to_convert.fset(self, value)
+
+    @property
+    def include_given(self) -> bool:
+        """
+        Provides the state of the :code:`_include_given` attribute.
+        """
+
+        return self._include_given
+
+    @include_given.setter
+    def include_given(self, value: bool) -> None:
+        """
+        Provides a way to activate/deactivate the inclusion of the given
+        subject into the result.
+
+        :raise TypeError:
+            When the given data to convert is not :py:class:`str`
+        """
+
+        if not isinstance(value, bool):
+            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
+
+        self._include_given = value
+
+    def set_include_given(self, value: bool) -> "Subject2Complements":
+        """
+        Provides a way to activate/deactivate the inclusion of the given
+        subject into the result.
+        """
+
+        self.include_given = value
+
+        return self
 
     def get_converted(self) -> List[str]:
         """
-        Provides the subject to test.
+        Provides the converted data.
         """
 
         return self.convert(self.data_to_convert)
 
-    def convert(self, data: Any) -> List[str]:
+    def convert(self, data: Any, *, aggressive: bool = False) -> List[str]:
         """
         Converts the given dataset.
 
         :param data:
             The data to convert.
         """
 
+        _ = aggressive
         result = []
 
-        subject = data.strip()
+        checker = DomainSyntaxChecker(data)
+
+        if self.include_given and data not in result:
+            result.append(data)
+
+        if data.startswith("www."):
+            result.append(data[4:])
+        elif checker.is_valid_second_level():
+            result.append(f"www.{data}")
 
-        if subject and (
-            not subject.startswith(self.COMMENT)
-            and any(not subject.startswith(x) for x in self.PARTICULAR_COMMENT)
-        ):
-            if self.COMMENT in subject:
-                subject = subject[: subject.find(self.COMMENT)].strip()
-
-            if self.NSLOOKUP_SPACE in subject:
-                # Comply with RFC 6367:
-                #    Note that nslookup escapes spaces as "\032" for display
-                #    purposes, but a graphical DNS-SD browser should not.
-                subject = subject.replace(self.NSLOOKUP_SPACE, self.SPACE)
-
-            if self.SPACE in subject or self.TAB in subject:
-                splitted = subject.split()
-
-                if IPSyntaxChecker(splitted[0]).is_valid():
-                    # This is for the hosts format.
-                    # If the first entry is an IP, we will only extract
-                    # the entries after the first one.
-                    result.extend(splitted[1:])
-                else:
-                    # All other cases, we extract every entries.
-                    result.extend(splitted)
-            else:
-                result.append(subject)
         return result
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/internal_url.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/internal_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,20 @@
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
         """
 
         return self.convert(self.data_to_convert)
 
-    def convert(self, data: Any) -> str:
+    def convert(self, data: Any, *, aggressive: bool = False) -> str:
         """
         Converts the given dataset.
 
         :param data:
             The data to convert.
         """
 
+        _ = aggressive
+
         if VersionUtility(PyFunceble.storage.PROJECT_VERSION).is_dev():
             return data.replace("master", "dev")
         return data.replace("dev", "master")
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_input_line2subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# pylint:disable=line-too-long
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the conversion of the an RPZ input line into testable subjects.
+Provides the base of all checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,58 +45,92 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-# pylint: enable=line-too-long
 
-from typing import Any, List
+import functools
+from typing import Any, Optional
 
-from PyFunceble.converter.input_line2subject import InputLine2Subject
 
-
-class RPZInputLine2Subject(InputLine2Subject):
+class NetInfoBase:
     """
-    Converts/Extracts the subject from the given RPZ inputline.
+    Provides the base of network information classes.
     """
 
-    COMMENT: list = [";", "//", "#"]
-    SPECIAL: list = ["$", "@"]
+    _subject: Optional[str] = None
+    base: Optional[str] = None
+
+    def __init__(self, subject: Optional[str] = None) -> None:
+        if subject is not None:
+            self.subject = subject
+
+    def ensure_subject_is_given(func):  # pylint: disable=no-self-argument
+        """
+        Ensures that the subject is given before running the decorated method.
+
+        :raise TypeError:
+            If the subject is not a string.
+        """
+
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if not isinstance(self.subject, str):
+                raise TypeError(
+                    f"<self.subject> should be {str}, {type(self.subject)} given."
+                )
+
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+
+        return wrapper
 
-    def get_converted(self) -> List[str]:
+    @property
+    def subject(self) -> Optional[str]:
         """
-        Provides the converted data.
+        Provides the current state of the :code:`_subject` attribute.
         """
 
-        return self.convert(self.data_to_convert)
+        return self._subject
 
-    def convert(self, data: Any) -> List[str]:
+    @subject.setter
+    def subject(self, value: str) -> None:
         """
-        Converts the given dataset.
+        Sets the subject to work with.
 
-        :param data:
-            The data to convert.
+        :param value:
+            The subject to set.
+
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
-        result = []
-        subject = data.strip()
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-        if (
-            subject
-            and not any(subject.startswith(x) for x in self.COMMENT)
-            and not any(subject.startswith(x) for x in self.SPECIAL)
-        ):
-            for comment_sign in self.COMMENT:
-                if comment_sign in subject:
-                    subject = subject[: subject.find(comment_sign)].strip()
+        self._subject = value
 
-            if self.SPACE in subject or self.TAB in subject:
-                subject = subject.split()[0]
+    def set_subject(self, value: str) -> "NetInfoBase":
+        """
+        Sets the subject to work with.
+
+        :param value:
+            The subject to set.
+        """
 
-                if not subject.isdigit():
-                    result.append(subject)
-            elif not subject.isdigit():
-                result.append(subject)
+        self.subject = value
+
+        return self
+
+    @ensure_subject_is_given
+    def get_info(self) -> Any:
+        """
+        Provides the wanted network information.
+        """
 
-        return result
+        raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_policy2subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/rpz_policy2subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,22 +262,23 @@
     def get_converted(self) -> Optional[str]:
         """
         Provides the converted data.
         """
 
         return self.convert(self.data_to_convert)
 
-    def convert(self, data: Any) -> Optional[str]:
+    def convert(self, data: Any, *, aggressive: bool = False) -> Optional[str]:
         """
         Converts the given dataset.
 
         :param data:
             The data to convert.
         """
 
+        _ = aggressive
         subject = data.strip()
 
         if (
             subject
             and not any(subject.startswith(x) for x in self.COMMENT)
             and not any(subject.startswith(x) for x in self.SPECIAL)
         ):
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/subject2complements.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/registrar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# pylint:disable=line-too-long
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an easy way to convert and get the complements of a subject.
+Provides our registrar extrator.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,110 +45,85 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-# pylint: enable=line-too-long
 
 from typing import Any, List, Optional
 
-from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
-from PyFunceble.converter.base import ConverterBase
+from PyFunceble.helpers.regex import RegexHelper
+from PyFunceble.query.whois.converter.base import ConverterBase
 
 
-class Subject2Complements(ConverterBase):
+class RegistarExtractor(ConverterBase):
     """
-    Converts a given wildcard into a testable subject.
+    Provides an interface for the extration of the registrar.
     """
 
-    _include_given: bool = False
-
-    def __init__(
-        self,
-        data_to_convert: Optional[Any] = None,
-        *,
-        include_given: Optional[bool] = False,
-    ) -> None:
-        if include_given is not None:
-            self.include_given = include_given
-
-        super().__init__(data_to_convert=data_to_convert)
+    PATTERNS: List[str] = [
+        r"authorized\s+agency(\s+|):(.*)",
+        r"domain\s+support(\s+|):(.*)",
+        r"registrar\s+name(\s+|):(.*)",
+        r"registrar_name(\s+|):(.*)",
+        r"registrar(\s+|):(.*)",
+        r"registrar\.+(\s+|):(.*)",
+        r"registration\s+service\s+provider(\s+|):(.*)",
+        r"sponsoring\s+registrar(\s+|):(.*)",
+        r"sponsoring\s+registrar\s+organization(\s+|):(.*)",
+    ]
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
-        Overrites the default behavior.
+        Sets the data to convert and work with.
+
+        :param value:
+            The record to work with.
 
         :raise TypeError:
-            When the given data to convert is not :py:class:`str` or a
-            :py:class:`list`.
+            When the given data to convert is not :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        # pylint: disable=no-member
-        super(Subject2Complements, self.__class__).data_to_convert.fset(self, value)
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-    @property
-    def include_given(self) -> bool:
-        """
-        Provides the state of the :code:`_include_given` attribute.
-        """
-
-        return self._include_given
-
-    @include_given.setter
-    def include_given(self, value: bool) -> None:
-        """
-        Provides a way to activate/deactivate the inclusion of the given
-        subject into the result.
-
-        :raise TypeError:
-            When the given data to convert is not :py:class:`str`
-        """
-
-        if not isinstance(value, bool):
-            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
-
-        self._include_given = value
+        # pylint: disable=no-member
+        super(RegistarExtractor, self.__class__).data_to_convert.fset(self, value)
 
-    def set_include_given(self, value: bool) -> "Subject2Complements":
+    def __get_line(self) -> Optional[str]:
         """
-        Provides a way to activate/deactivate the inclusion of the given
-        subject into the result.
+        Tries to get the registrar line from the given record.
         """
 
-        self.include_given = value
-
-        return self
+        for regex in self.PATTERNS:
+            registrar_line = RegexHelper(r"(?i)" + regex).match(
+                self.data_to_convert, return_match=True, rematch=True, group=0
+            )
 
-    def get_converted(self) -> List[str]:
-        """
-        Provides the converted data.
-        """
+            if not registrar_line:
+                continue
 
-        return self.convert(self.data_to_convert)
+            return registrar_line
+        return None
 
-    def convert(self, data: Any) -> List[str]:
+    @ConverterBase.ensure_data_to_convert_is_given
+    def get_converted(self) -> Optional[str]:
         """
-        Converts the given dataset.
-
-        :param data:
-            The data to convert.
+        Provides the registrar of the record (if found).
         """
 
-        result = []
-
-        checker = DomainSyntaxChecker(data)
-
-        if self.include_given and data not in result:
-            result.append(data)
+        registrar_line = self.__get_line()
 
-        if data.startswith("www."):
-            result.append(data[4:])
-        elif checker.is_valid_second_level():
-            result.append(f"www.{data}")
+        if registrar_line:
+            try:
+                return [x.strip() for x in registrar_line if x.strip()][0]
+            except IndexError:
+                pass
 
-        return result
+        return None
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/url2netloc.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/url2netloc.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,14 +90,19 @@
     @staticmethod
     def parse_single_url(data) -> Optional[urllib.parse.ParseResult]:
         """
         Parses the URL.
         """
 
         if data:
+            if "[" in data and "]" not in data or "]" in data and "[" not in data:
+                # Own wrapper around "Invalid IPv6 URL" when
+                # http://example.org."] is given (for example.)
+                data = data.replace("[", "").replace("]", "")
+
             return urllib.parse.urlparse(data)
         return None
 
     def parse_url(self) -> "Url2Netloc":
         """
         Parses the URL.
         """
@@ -112,22 +117,23 @@
         """
 
         # Retrocompatibility.
         self.parse_url()
 
         return self.convert(self.data_to_convert)
 
-    def convert(self, data: Any) -> str:
+    def convert(self, data: Any, *, aggressive: bool = False) -> str:
         """
         Converts the given dataset.
 
         :param data:
             The data to convert.
         """
 
+        _ = aggressive
         parsed_url = self.parse_single_url(data)
 
         if not parsed_url.netloc and parsed_url.path:
             netloc = parsed_url.path
         elif parsed_url.netloc:
             netloc = parsed_url.netloc
         else:  # pragma: no cover ## Safety
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/converter/wildcard2subject.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/wildcard2subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,22 +82,23 @@
     def get_converted(self) -> str:
         """
         Provides the converted data.
         """
 
         return self.convert(self.data_to_convert)
 
-    def convert(self, data: Any) -> str:
+    def convert(self, data: Any, *, aggressive: bool = False) -> str:
         """
         Converts the given dataset.
 
         :param data:
             The data to convert.
         """
 
+        _ = aggressive
         subject = data.strip()
 
         if not subject:
             return None
 
         if subject.startswith(self.WILDCARD):
             return subject[2:]
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/env.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 # pylint: skip-file
 # flake8: noqa
 
 from alembic import context
 from sqlalchemy import engine_from_config, pool
 
 import PyFunceble.cli.facility
+import PyFunceble.database.sqlalchemy.all_schemas
 import PyFunceble.facility
-from PyFunceble.database.sqlalchemy.all_schemas import Continue, Inactive, WhoisRecord
 from PyFunceble.database.sqlalchemy.base_schema import SchemaBase
 
 config = context.config
 target_metadata = SchemaBase.metadata
 
 if not PyFunceble.facility.ConfigLoader.is_already_loaded():
     # We load the configuration because we don't want to manually give
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/env.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 # pylint: skip-file
 # flake8: noqa
 
 from alembic import context
 from sqlalchemy import engine_from_config, pool
 
 import PyFunceble.cli.facility
+import PyFunceble.database.sqlalchemy.all_schemas
 import PyFunceble.facility
-from PyFunceble.database.sqlalchemy.all_schemas import Continue, Inactive, WhoisRecord
 from PyFunceble.database.sqlalchemy.base_schema import SchemaBase
 
 config = context.config
 target_metadata = SchemaBase.metadata
 
 if not PyFunceble.facility.ConfigLoader.is_already_loaded():
     # We load the configuration because we don't want to manually give
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py` & `PyFunceble-dev-4.2.1/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/.PyFunceble_production.yaml` & `PyFunceble-dev-4.2.1/PyFunceble/data/infrastructure/.PyFunceble_production.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 debug:
   # Provides everything related to the debug mode.
 
   # Activates the debug/logging.
-  active: False
+  active: no
   # Sets the logging level.
   level: info
 
 cli_decoding:
   # Provides everything related to the decoding from the CLI.
 
   # Activates the aggressive decoding.
-  adblock_aggressive: False
+  aggressive: no
 
   # Activates the decoding using the adblock decoder.
-  adblock: False
+  adblock: no
 
   # Activates the decoding using the RPZ decoder.
-  rpz: False
+  rpz: no
 
   # Activated the decoding using the Wildcard decoder.
-  wildcard: False
+  wildcard: no
 
 cli_testing:
   # Provides everything directly related to the CLI testing.
 
   # Sets the Hosts IP to use while generation the hosts file(s)
   hosts_ip: "0.0.0.0"
 
   # Sets the number of maximal workers to use.
   # If set to null, the system use: CPU * Cores - 2
   max_workers: null
 
   # Activates the automatic continuation after a break or shortage.
-  autocontinue: False
+  autocontinue: no
 
   # Activates the storage and creation of a database of all INACTIVA and INVALID
   # subjects for continuous testing.
-  inactive_db: True
+  inactive_db: yes
 
   # Activates the storage of some WHOIS information in order to avoid having
   # to spam the WHOIS servers.
-  whois_db: True
+  whois_db: yes
 
   # Activates the generation of complements.
-  complements: False
+  complements: no
 
   # Activates the expansion of CIDR to single addresses.
-  cidr_expand: False
+  cidr_expand: no
 
   # Sets the cooldown time to apply between each tests.
   cooldown_time: 0.0
 
   # Sets the Database Connector type to use.
   # Available: csv | mariadb | mysql | postgresql
   db_type: csv
 
   # Sets the filter to apply while reading the given input.
   # For example, if you give `\.info`, we will only test the subjects who match
   # `\.info`.
   file_filter: null
 
   # Activates the mining of data.
-  mining: False
+  mining: no
 
   # Acknowledges that we may test for local network component.
   # NOTE: Activating this, will remove the syntax checker completely.
-  local_network: False
+  local_network: no
 
   # Activates or disable the preloading of the given input file(s).
   # When this is activated, we take the time to pre load and decode the content
   # of your file so that we can optimize some of our process regarding the
   # auto continue.
   #
   # Note: This has no effect if the auto-continue is deactivated.
-  preload_file: False
+  preload_file: no
 
   # Activates or disables a chancy tester mode that unleashes the safety
   # workflow in place.
   #
   # WARNING:
   #   You shouldn't have to use this unless you feel really lucky and trust your
   #   machine.
   #
   #   This mode makes things look 'fast', but it may produce some unexpected
   #   results if :code:`N` process simultaneously write the same output file.
   #
   #   This mode makes the graphical CLI output unparsable - either.
   #
   #   **MAY THE FORCE BE WITH YOU!**
-  chancy_tester: False
+  chancy_tester: no
 
   ci:
     # Provides everything related to the Continuous integration.
 
     # Activates the continuous integration mode.
     # WARNING: Do not activate without asking or knowing what you are doing.
-    active: False
+    active: no
 
     # Sets the commit message to apply everytime except for the last one.
     commit_message: "PyFunceble - AutoSave"
 
     # Sets the commit message to apply at the very end of the test.
     end_commit_message: "PyFunceble - Results"
 
@@ -121,39 +121,39 @@
     # Sets the command to execute before the last commit.
     end_command: null
 
   display_mode:
     # Provides everything related to the display mode.
 
     # Activates the printing of dots.
-    dots: False
+    dots: no
 
     # Activates the printing of the execution time.
-    execution_time: False
+    execution_time: no
 
     # Activates the output of the percentage information.
-    percentage: True
+    percentage: yes
 
     # Activates the output of the top registrar information.
-    registrar: False
+    registrar: no
 
     # Activates the quiet mode.
-    quiet: False
+    quiet: no
 
     # Activates the output of very few information.
-    less: True
+    less: yes
 
     # Activates the output of all information.
-    all: False
+    all: no
 
     # Activates the output of the status and it's status (only)
-    simple: False
+    simple: no
 
     # Activates the coloration of stdout.
-    colour: True
+    colour: yes
 
     # Sets the status do display to STDOUT.
     # NOTE: This does not have any effect with the generated files.
     # Available values: ALL | ACTIVE | INACTIVE | INVALID | SANE | MALICIOUS
     status: all
 
     # Sets the maximum number of registrar to display.
@@ -161,21 +161,21 @@
     max_registrar: 15
 
   testing_mode:
     # Provides all available testing modes.
     # WARNING: Only one can be used at a time.
 
     # Activates the availability test.
-    availability: True
+    availability: yes
 
     # Activates the syntax test.
-    syntax: False
+    syntax: no
 
     # Activates the reputation test.
-    reputation: False
+    reputation: no
 
   days_between:
     # Provides everything which is x days periodic.
 
     # NOT IMPLEMENTED (Anticipation for future usage).
     db_clean: 28
 
@@ -184,81 +184,81 @@
     db_retest: 1
 
   sorting_mode:
     # Provides all our sorting mode.
     # WARNING: The sorting mode is only applied to the files. NOT STDOUT.
 
     # Activates the hierarchical sorting.
-    hierarchical: False
+    hierarchical: no
 
     # Activates the standard sorting.
-    standard: True
+    standard: yes
 
   file_generation:
     # Provides everything related to the generation of file.
 
     # Deactivates the generation of any status file.
-    no_file: False
+    no_file: no
 
     # Activates the generation of the hosts file(s).
-    hosts: False
+    hosts: no
 
     # Activates the generation of the plain (or raw) file(s).
-    plain: True
+    plain: yes
 
     # Activates the generation of the analytic file(s).
-    analytic: True
+    analytic: yes
 
     # Activate the generation of an unified file for the copy of what is
     # outputted to STDOUT.
-    unified_results: False
+    unified_results: no
 
     # Activates or disables the merging of the results of all inputted files into
     # one single output subdirectory.
-    merge_output_dirs: False
+    merge_output_dirs: no
 
 lookup:
   # Provides everything related to the lookup.
 
   # Activates the usage of the DNS lookup.
-  dns: True
+  dns: yes
 
   # Activates the usage of the HTTP status code lookup.
-  http_status_code: True
+  http_status_code: yes
 
   # Activates the usage of the network information socket.
-  netinfo: True
+  netinfo: yes
 
   # Activates the usage of our special rules.
-  special: True
+  special: yes
 
   # Activates the usage of the WHOIS record.
-  whois: True
+  whois: yes
 
   # Activates the usage of the reputation data reputation.
-  reputation: False
+  reputation: no
 
   # Activate the usage of the collection.
-  collection: False
+  collection: no
 
   # Sets the timeout to apply to each of our lookup tools who support a timeout
   # option.
   timeout: 5
 
 dns:
   # Provides everything related to the DNS lookup.
 
   # Activates the follow-up of the given order.
-  follow_server_order: true
+  follow_server_order: yes
 
   # Activates the trust mode. Meaning that if one of the DNS give us a negative
   # response (without error), we take it as it is.
-  # When this mode is deactivated (false), when one of the DNS give us a negative
+  # When this mode is deactivated (no), when one of the DNS give us a negative
   # response (without error), we still ask all other servers.
-  trust_server: false
+  trust_server: no
 
   # Sets the list of server to communicate with.
   # It must be a list.
   #
   # WARNING:
   #   IPv6 should be given in this format if a port is explicitly given:
   #     [ip]:port
@@ -276,21 +276,18 @@
 
   # Sets the delay (seconds) to apply between each queries.
   # When a value > 0.00000 is given, we will wait for the given amount of
   # seconds between each queries.
   delay: 0.0
 
 # Not Implemented yet. Reserved for future usage and implementation.
-share_logs: False
+share_logs: no
 
 user_agent:
   # Provides everything related to the user agent choice.
-  # Note:
-  #   Please report to https://git.io/JLWe5 for more insight about the
-  #   browser and platform available..
 
   browser: chrome
   platform: linux
 
   # Sets the user agent to use.
   # WARNING: If given, this will be used systematically.
   custom: null
@@ -335,26 +332,26 @@
     # Global HTTPS proxy to use when no rule is given or matched.
     https: null
 
   rules: []
 
 
 # Activates the verification of the certificate.
-verify_ssl_certificate: False
+verify_ssl_certificate: no
 
 # Set the maximum number of retries to perform.
 # This should be an integer >= 0.
 max_http_retries: 3
 
 http_codes:
   # Provides everything related to the HTTP code lookup interpretation.
 
   # Informs PyFunceble that the end-user (not PyFunceble) is managing this list.
   # This means that you won't get any update in this section.
-  self_managed: False
+  self_managed: no
 
   list:
     up:
       - 100
       - 101
       - 102
       - 200
@@ -429,15 +426,15 @@
 
   # Provides the base of the URL to access to communicate with the collection.
   url_base: https://collection.dead-hosts.funilrys.com
 
   # Activates the push of dataset into the collection.
   # WARNING: This is useless, if you don't have an API Token set as the
   # COLLECTION_API_TOKEN environment variable.
-  push: False
+  push: no
 
   # Sets the preferred pull origin.
   #
   # When choosing, `frequent`, the system will pull the most frequent status
   # that is provided and calculated by the collection.
   #
   # When choosing, `latest`, the system will pull the latest status that is
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/dir_structure_production.json` & `PyFunceble-dev-4.2.1/PyFunceble/data/infrastructure/dir_structure_production.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7586206896551724%*

 * *Differences: {"'ips'": "OrderedDict([('.gitignore', OrderedDict([('content', "*

 * *          "'*\\n!.gitignore\\n!/ACTIVE/\\n!/INACTIVE/\\n!/INVALID/\\n!/MALICIOUS/\\n!/SANE/\\n!/VALID/\\n'), "*

 * *          "('hash', 'a273966a13322ad4da9fbad4bd7247ca046de503de543c6f909e5e2b')]))])",*

 * * "'ips/ACTIVE'": "OrderedDict([('.gitignore', OrderedDict([('content', '*\\n!.gitignore\\n'), "*

 * *                 "('hash', '0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b')]))])",*

 * * "'ips/INACTIVE'": "OrderedDict([('.gitignore', OrderedDic […]*

```diff
@@ -109,14 +109,56 @@
     },
     "hosts/VALID": {
         ".gitignore": {
             "content": "*\n!.gitignore\n",
             "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
         }
     },
+    "ips": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n!/ACTIVE/\n!/INACTIVE/\n!/INVALID/\n!/MALICIOUS/\n!/SANE/\n!/VALID/\n",
+            "hash": "a273966a13322ad4da9fbad4bd7247ca046de503de543c6f909e5e2b"
+        }
+    },
+    "ips/ACTIVE": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/INACTIVE": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/INVALID": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/MALICIOUS": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/SANE": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/VALID": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
     "logs": {
         ".gitignore": {
             "content": "*\n!.gitignore\n!/date_format/\n!/no_referrer/\n!/percentage/\n!/whois/\n",
             "hash": "7e533b26a45b8712a1ed4895b52b2cc798a03a632074800af98a52e7"
         }
     },
     "logs/percentage": {
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/credential/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mariadb.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/credential/mariadb.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mysql.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/credential/mysql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/postgresql.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/credential/postgresql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/autocontinue.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/schemas/autocontinue.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/inactive.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/schemas/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/status.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/schemas/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/whois_record.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/schemas/whois_record.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/session.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/session.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/all_schemas.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/all_schemas.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/base_schema.py` & `PyFunceble-dev-4.2.1/PyFunceble/database/sqlalchemy/base_schema.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/csv.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/sql.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/autocontinue/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     mariadb.
     """
 
     ORM_OBJ: Continue = Continue
 
     @SQLDBDatasetBase.execute_if_authorized(None)
     # pylint: disable=arguments-differ
-    def cleanup(self, *, session_id: str) -> "MariaDBContinueDataset":
+    def cleanup(self, *, session_id: str) -> "SQLDBContinueDataset":
         """
         Cleanups the dataset. Meaning that we delete every entries which are
         needed anymore.
 
         :param source:
             The source to delete.
         :param session_id:
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all datasets classes.
+Provides the interface for the WHOIS DB CSV management.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,100 +46,134 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
-from typing import Any, Optional
+import os
+from typing import Any, Generator, Optional
 
+import PyFunceble.cli.storage
 import PyFunceble.storage
-from PyFunceble.downloader.base import DownloaderBase
-from PyFunceble.helpers.dict import DictHelper
-from PyFunceble.helpers.file import FileHelper
+from PyFunceble.dataset.csv_base import CSVDatasetBase
+from PyFunceble.dataset.whois.base import WhoisDatasetBase
 
 
-class DatasetBase:
+class CSVWhoisDataset(CSVDatasetBase, WhoisDatasetBase):
     """
-    Provides the base of all dataset.
+    Provides the interface for the management of the WHOIS (db)
+    CSV file.
     """
 
-    STORAGE_INDEX: Optional[str] = None
-    DOWNLOADER: Optional[DownloaderBase] = None
+    def __post_init__(self) -> None:
+        self.source_file = os.path.join(
+            PyFunceble.storage.CONFIG_DIRECTORY, PyFunceble.cli.storage.WHOIS_DB_FILE
+        )
 
-    source_file: Optional[str] = None
+        return super().__post_init__()
 
-    def __contains__(self, value: Any):  # pragma: no cover
-        raise NotImplementedError()
+    def __contains__(self, value: str) -> bool:
+        for row in self.get_content():
+            try:
+                if value in (row["subject"], row["idna_subject"]):
+                    return True
+            except KeyError:
+                break
+
+        return False
+
+    def __getitem__(self, value: Any) -> Optional[dict]:
+        try:
+            for row in self.get_content():
+                if value in (row["subject"], row["idna_subject"]):
+                    return row
+        except TypeError:
+            pass
 
-    def __getattr__(self, value: Any):  # pragma: no cover
-        raise AttributeError(value)
+        return None
 
-    def __getitem__(self, value: Any):  # pragma: no cover
-        raise KeyError(value)
+    @CSVDatasetBase.execute_if_authorized(None)
+    def get_content(self) -> Generator[Optional[dict], None, None]:
+        """
+        Provides a generator which provides the next line to read.
+        """
 
-    def __getstate__(self):  # pragma: no cover
-        return vars(self)
+        for row in super().get_content():
+            try:
+                row["epoch"] = float(row["epoch"])
+            except (TypeError, ValueError):
+                continue
 
-    def __setstate__(self, state):  # pragma: no cover
-        vars(self).update(state)
+            yield row
 
-    def ensure_source_file_exists(func):  # pylint: disable=no-self-argument
+    @CSVDatasetBase.execute_if_authorized(None)
+    def update(self, row: dict, *, ignore_if_exist: bool = False) -> "CSVWhoisDataset":
         """
-        Ensures that the source file exists before running the decorated
-        method.
+        Adds the given dataset into the database if it does not exists.
+        Update otherwise.
+
+        ..note::
+            This should be the prefered method for introduction of new dataset.
+
+        ..warning::
+            This method do nothing if the row is expired.
+
+        :param row:
+            The row or dataset to manipulate.
+
+        :param ignore_if_exist:
+            Ignores the insertion/update if the row already exists.
 
         :raise TypeError:
-            When :code:`self.source_file` is not a :py:class:`str`.
-        :raise ValueError:
-            When :code:`self.source_file` is empty.
+            When the given :code:`row` is not a :py:class`dict`.
         """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(self.source_file, str):
-                raise TypeError(
-                    f"<self.source_file> should be {str}, "
-                    f"{type(self.source_file)} given."
-                )
+        if not isinstance(row, dict):
+            raise TypeError(f"<row> should be {dict}, {type(row)} given.")
 
-            if not self.source_file:
-                raise ValueError("<self.source_file> should not be empty.")
+        if not self.is_expired(row):
+            if self.exists(row):
+                if not ignore_if_exist and self[row["subject"]] != row:
+                    self.remove(row)
+                    self.add(row)
+            else:
+                self.add(row)
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+        return self
 
-        return wrapper
-
-    @ensure_source_file_exists
-    def get_content(self) -> Optional[dict]:
+    @CSVDatasetBase.execute_if_authorized(None)
+    def remove(self, row: dict) -> "CSVDatasetBase":
         """
-        Provides the cached or the real contend of the dataset (after caching)
+        Removes the given dataset from the CSV file.
+
+        :param row:
+            The row or dataset to add.
 
-        :raise FileNotFoundError:
-            When the declared file does not exists.
+        :raise TypeError:
+            When the given :code:`row` is not a :py:class`dict`.
         """
 
-        if (
-            bool(self.STORAGE_INDEX)
-            and hasattr(PyFunceble.storage, self.STORAGE_INDEX)
-            and bool(getattr(PyFunceble.storage, self.STORAGE_INDEX))
-        ):
-            return getattr(PyFunceble.storage, self.STORAGE_INDEX)
+        # If we don't do this, the comparison will fail. #
+        # We don't want to overwrite the whole (remove) method just for what
+        # we need.
+        previous_remove_uneeded_fields = self.remove_unneeded_fields
 
-        file_helper = FileHelper(self.source_file)
+        self.set_remove_unneeded_fields(False)
 
-        if not file_helper.exists() and bool(
-            self.DOWNLOADER
-        ):  # pragma: no cover ## This is just a safety endpoint.
-            self.DOWNLOADER.start()
+        super().remove(row)
 
-            if not file_helper.exists():
-                raise FileNotFoundError(file_helper.path)
+        self.set_remove_unneeded_fields(previous_remove_uneeded_fields)
 
-        content = DictHelper().from_json_file(
-            self.source_file, return_dict_on_error=False
-        )
+        return self
+
+    def cleanup(self) -> "CSVWhoisDataset":
+        """
+        Cleanups the dataset. Meaning that we delete every entries which are
+        in the past.
+        """
 
-        setattr(PyFunceble.storage, self.STORAGE_INDEX, content)
+        for row in self.get_content():
+            if self.is_expired(row):
+                self.remove(row)
 
-        return content
+        return self
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/csv_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/csv_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/db_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/command.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all datasets which acts as database interface.
+Provides the command helpers. This helpers let us run Shell commands.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,267 +46,201 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
-from typing import Any, Generator, List, Optional
+import os
+import subprocess
+import sys
+from typing import Generator, Optional, Union
 
-from PyFunceble.dataset.base import DatasetBase
 
-
-class DBDatasetBase(DatasetBase):
-    """
-    Provides the base of all datasets which acts as database interface.
+class CommandHelper:
     """
+    Shell command execution.
 
-    STD_REMOVE_UNNEEDED_FIELDS: bool = True
-    STD_AUTHORIZED: bool = False
-
-    FIELDS: List[str] = []
-    COMPARISON_FIELDS: List[str] = []
-
-    source_file: Optional[str] = None
+    :param str command: The command to execute.
+    :param str encoding: The encoding to use to decode the shell output.
+    """
 
-    _remove_unneeded_fields: Optional[bool] = True
-    _authorized: Optional[bool] = False
+    _command: Optional[str] = None
+    _encoding: str = "utf-8"
 
     def __init__(
         self,
+        command: Optional[Union[str, list]] = None,
         *,
-        authorized: Optional[bool] = None,
-        remove_unneeded_fields: Optional[bool] = None,
+        encoding: Optional[str] = None,
     ) -> None:
-        if authorized is not None:
-            self.set_authorized(authorized)
-
-        if remove_unneeded_fields is not None:
-            self.set_remove_unneeded_fields(remove_unneeded_fields)
-
-        self.__post_init__()
-
-    def __post_init__(self) -> None:
-        """
-        A method to be called (automatically) after __init__.
-        """
-
-    def execute_if_authorized(default: Any = None):  # pylint: disable=no-self-argument
-        """
-        Executes the decorated method only if we are authorized to process.
-        Otherwise, apply the given :code:`default`.
-        """
+        if command is not None:
+            self.command = command
 
-        def inner_metdhod(func):
-            @functools.wraps(func)
-            def wrapper(self, *args, **kwargs):
-                if self.authorized:
-                    return func(self, *args, **kwargs)  # pylint: disable=not-callable
-                return default
-
-            return wrapper
-
-        return inner_metdhod
+        if encoding is not None:
+            self.encoding = encoding
 
     @property
-    def authorized(self) -> Optional[bool]:
+    def command(self) -> Optional[str]:
         """
-        Provides the current state of the :code:`_authorized` attribute.
+        Provides the current state of the :code:`_command` attribute.
         """
 
-        return self._authorized
+        return self._command
 
-    @authorized.setter
-    def authorized(self, value: bool) -> None:
+    @command.setter
+    def command(self, value: Union[str, list]) -> None:
         """
-        Sets the value of the :code:`_authorized` attribute.
+        Sets the command to use.
 
         :param value:
-            The value to set.
+            The command to use/execute.
 
         :raise TypeError:
-            When the given :code:`value` is not a :py:class:`bool`
+            When the value is not a :py:class:`list` or :py:class:`str`
         """
 
-        if not isinstance(value, bool):
-            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
+        if not isinstance(value, (str, list)):
+            raise TypeError(
+                f"<value> should be {str} or {list}, " f"{type(value)} given."
+            )
 
-        self._authorized = value
+        if isinstance(value, list):
+            self._command = " ".join(value)
+        else:
+            self._command = value
 
-    def set_authorized(self, value: bool) -> "DBDatasetBase":
+    def set_command(self, value: Union[str, list]) -> "CommandHelper":
         """
-        Sets the value of the :code:`_authorized` attribute.
+        Sets the command to use.
 
         :param value:
-            The value to set.
+            The command to use/execute.
         """
 
-        self.authorized = value
+        self.command = value
 
         return self
 
     @property
-    def remove_unneeded_fields(self) -> Optional[bool]:
+    def encoding(self) -> Optional[str]:
         """
-        Provides the current state of the :code:`_remove_unneeded_fields`.
+        Provides the current state of the :code:`_encoding` attribute.
         """
 
-        return self._remove_unneeded_fields
+        return self._encoding
 
-    @remove_unneeded_fields.setter
-    def remove_unneeded_fields(self, value: bool) -> None:
+    @encoding.setter
+    def encoding(self, value: str) -> None:
         """
-        Sets the value of the :code:`_remove_unneeded_fields` attribute.
+        Sets the encoding to use.
 
         :param value:
             The value to set.
 
         :raise TypeError:
-            When the given :code:`value` is not a :py:class:`bool`
+            When the value is not a :py:class:`str`
         """
 
-        if not isinstance(value, bool):
-            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        self._remove_unneeded_fields = value
+        self._encoding = value
 
-    def set_remove_unneeded_fields(self, value: bool) -> "DBDatasetBase":
+    def set_encoding(self, value: str) -> "CommandHelper":
         """
-        Sets the value of the :code:`_remove_unneeded_fields` attribute.
+        Sets the encoding to use.
 
         :param value:
             The value to set.
         """
 
-        self.remove_unneeded_fields = value
+        self.encoding = value
 
         return self
 
-    @execute_if_authorized(dict())  # pylint: disable=use-dict-literal
-    def get_filtered_row(self, row: dict) -> dict:
-        """
-        Removes all unkowns fields (not declared) from the given row.
-
-        :param row:
-            The row to work with.
+    def _decode_output(self, to_decode: bytes) -> str:
         """
+        Decode the output of a shell command in order to be readable.
 
-        result = {}
+        :param bytes to_decode: Output of a command to decode.
 
-        for key, value in row.items():
-            if value is None:
-                value = ""
-
-            if key in self.FIELDS:
-                result[key] = value
-
-        for field in self.COMPARISON_FIELDS:
-            if field not in result:
-                result[field] = ""
-
-        return result
-
-    def add(self, row: dict) -> "DBDatasetBase":
+        :return: The decoded output.
+        :rtype: str
         """
-        Adds the given dataset into the database.
 
-        :param row:
-            The row or dataset to add.
+        if to_decode:
+            return to_decode.decode(self.encoding)
 
-        :raise TypeError:
-            When the given :code:`row` is not a :py:class`dict`.
-        """
+        return ""
 
-        raise NotImplementedError()
-
-    def remove(self, row: dict) -> "DBDatasetBase":
-        """
-        Removes the given dataset from the database.
-
-        :param row:
-            The row or dataset to remove.
-
-        :raise TypeError:
-            When the given :code:`row` is not a :py:class`dict`.
-        """
-
-        raise NotImplementedError()
-
-    def update(self, row: dict, *, ignore_if_exist: bool = False) -> "DBDatasetBase":
+    def execute(self, *, raise_on_error: bool = False) -> str:
         """
-        Adds the given dataset into the database if it does not exists.
-        Update otherwise.
-
-        :param row:
-            The row or dataset to manipulate.
+        Execute the given command.
 
-        :param ignore_if_exist:
-            Ignores the insertion/update if the row already exists.
-
-
-        :raise TypeError:
-            When the given :code:`row` is not a :py:class`dict`.
-        """
+        :parma raise_on_error:
+            Raises on error if set to :py:class:`True`.
 
-        raise NotImplementedError()
+        :return: The output of the command.
 
-    def get_content(self) -> Generator[Optional[dict], None, None]:
-        """
-        Provides a generator which provides the next line to read.
+        :raise RuntimeError:
+            When the exit code is not equal to 0.
         """
 
-        raise NotImplementedError()
-
-    def cleanup(self) -> "DBDatasetBase":
-        """
-        Cleanups the dataset.
-        """
+        # We initiate a process and parse the command to it.
+        with subprocess.Popen(
+            self.command,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            shell=True,
+            env=os.environ,
+        ) as process:
+            stdout, stderr = process.communicate()
 
-        raise NotImplementedError()
+            if process.returncode != 0:
+                if raise_on_error:
+                    raise RuntimeError(repr(self._decode_output(stderr)))
+                return self._decode_output(stderr)
+            return self._decode_output(stdout)
 
-    @execute_if_authorized(None)
-    def get_filtered_content(
-        self, filter_map: dict
-    ) -> Generator[Optional[dict], None, None]:
+    def run(self, rstrip: bool = True) -> Generator[str, None, None]:
         """
-        Provides a generator which provides the next dataset. to read.
+        Run the given command and yield each line(s) one by one.
 
-        :param filter_map:
-            A dictionary representing what we need to filter.
+        .. note::
+            The difference between this method and
+            :func:`~PyFunceble.helpers.Command.execute`
+            is that :func:`~PyFunceble.helpers.Command.execute` wait for the
+            process to end in order to return its output while this method
+            return each line one by one
+            - as they are outputed.
 
-        :raise TypeError:
-            When the given :code:`filter_map` is not a :py:class:`dict`.
+        :param bool rstrip:
+            Deactivates the rstrip of the output.
         """
 
-        if not isinstance(filter_map, dict):
-            raise TypeError(f"<filter_map> should be {dict}, {type(filter_map)} given.")
+        with subprocess.Popen(
+            self.command,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            shell=True,
+            env=os.environ,
+        ) as process:
+            while True:
+                # Note: we use rstrip() because we are paranoid :-)
+                current_line = process.stdout.readline()
 
-        for row in self.get_content():
-            for key, value in filter_map.items():
-                if key not in row:
-                    continue
+                if not current_line and process.poll() is not None:
+                    break
 
-                if row[key] == value:
-                    yield row
+                if rstrip:
+                    yield self._decode_output(current_line.rstrip())
+                else:
+                    yield self._decode_output(current_line)
 
-    def exists(self, row: dict) -> bool:
+    def run_to_stdout(self) -> None:
         """
-        Checks if the given dataset exists in our dataset.
-
-        :param row:
-            The row or dataset to add.
-        """
-
-        raise NotImplementedError()
-
-    def are_equal(self, read_row: dict, row: dict) -> bool:
-        """
-        Compares the given :code:`read_row` to the `row`.
-
-        :param read_row:
-            The row read from the dataset infrastructure.
-        :param row:
-            The row given by the testing infrastructure.
+        Run the given command and print each line(s) to stdout.
         """
 
-        raise NotImplementedError()
+        for line in self.run(rstrip=False):
+            sys.stdout.write(line)
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/iana.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/csv.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/sql.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/inactive/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/ipv4_reputation.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/public_suffix.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/sql_base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/sql_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         for row in self.db_session.query(self.ORM_OBJ):
             row = row.to_dict()
 
             yield row
 
     @DBDatasetBase.execute_if_authorized(None)
-    def update(self, row, *, ignore_if_exist: bool = False) -> "MariaDBDatasetBase":
+    def update(self, row, *, ignore_if_exist: bool = False) -> "SQLDBDatasetBase":
         """
         Adds the given dataset into the database if it does not exists.
         Update otherwise.
 
         .. note::
             This should be the preferred method for introduction of new dataset.
 
@@ -164,15 +164,15 @@
         PyFunceble.facility.Logger.debug("Updated row:\n%r", row)
         PyFunceble.facility.Logger.info("Finished to update row.")
 
         return self
 
     @DBDatasetBase.execute_if_authorized(None)
     @ensure_orm_obj_is_given
-    def remove(self, row) -> "MariaDBDatasetBase":
+    def remove(self, row) -> "SQLDBDatasetBase":
         """
         Removes the given dataset from the database.
 
         :param row:
             The row or dataset to check.
 
         :raise TypeError:
@@ -272,15 +272,15 @@
         for field in self.COMPARISON_FIELDS:
             result = result.filter(getattr(self.ORM_OBJ, field) == row[field])
 
         return result.first()
 
     @DBDatasetBase.execute_if_authorized(None)
     @ensure_orm_obj_is_given
-    def add(self, row) -> "MariaDBDatasetBase":
+    def add(self, row) -> "SQLDBDatasetBase":
         """
         Adds the given dataset into the database.
 
         :param row:
             The row or dataset to add.
 
         :raise TypeError:
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/user_agent.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/user_agent.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/csv.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/input_line2subject.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint:disable=line-too-long
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the interface for the WHOIS DB CSV management.
+Provides the default input line converter.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,134 +47,114 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import os
-from typing import Any, Generator, Optional
+from typing import Any, List
 
-import PyFunceble.cli.storage
-import PyFunceble.storage
-from PyFunceble.dataset.csv_base import CSVDatasetBase
-from PyFunceble.dataset.whois.base import WhoisDatasetBase
+from PyFunceble.checker.syntax.ip import IPSyntaxChecker
+from PyFunceble.converter.base import ConverterBase
+from PyFunceble.converter.url2netloc import Url2Netloc
 
 
-class CSVWhoisDataset(CSVDatasetBase, WhoisDatasetBase):
+class InputLine2Subject(ConverterBase):
     """
-    Provides the interface for the management of the WHOIS (db)
-    CSV file.
+    Converts/Extract the subjcts to test from an inputed line.
     """
 
-    def __post_init__(self) -> None:
-        self.source_file = os.path.join(
-            PyFunceble.storage.CONFIG_DIRECTORY, PyFunceble.cli.storage.WHOIS_DB_FILE
-        )
-
-        return super().__post_init__()
-
-    def __contains__(self, value: str) -> bool:
-        for row in self.get_content():
-            try:
-                if value in (row["subject"], row["idna_subject"]):
-                    return True
-            except KeyError:
-                break
+    COMMENT: str = "#"
+    PARTICULAR_COMMENT: List[str] = ["!"]
+    SPACE: str = " "
+    NSLOOKUP_SPACE: str = "\\032"
+    TAB: str = "\t"
 
-        return False
-
-    def __getitem__(self, value: Any) -> Optional[dict]:
-        try:
-            for row in self.get_content():
-                if value in (row["subject"], row["idna_subject"]):
-                    return row
-        except TypeError:
-            pass
-
-        return None
-
-    @CSVDatasetBase.execute_if_authorized(None)
-    def get_content(self) -> Generator[Optional[dict], None, None]:
-        """
-        Provides a generator which provides the next line to read.
+    @ConverterBase.data_to_convert.setter
+    def data_to_convert(self, value: Any) -> None:
         """
+        Overrites the default behavior.
 
-        for row in super().get_content():
-            try:
-                row["epoch"] = float(row["epoch"])
-            except (TypeError, ValueError):
-                continue
-
-            yield row
-
-    @CSVDatasetBase.execute_if_authorized(None)
-    def update(self, row: dict, *, ignore_if_exist: bool = False) -> "CSVWhoisDataset":
+        :raise TypeError:
+            When the given data to convert is not :py:class:`str`
         """
-        Adds the given dataset into the database if it does not exists.
-        Update otherwise.
 
-        ..note::
-            This should be the prefered method for introduction of new dataset.
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        ..warning::
-            This method do nothing if the row is expired.
+        # pylint: disable=no-member
+        super(InputLine2Subject, self.__class__).data_to_convert.fset(self, value)
 
-        :param row:
-            The row or dataset to manipulate.
+    def get_converted(self) -> List[str]:
+        """
+        Provides the subject to test.
+        """
 
-        :param ignore_if_exist:
-            Ignores the insertion/update if the row already exists.
+        return self.convert(self.data_to_convert, aggressive=self.aggressive)
 
-        :raise TypeError:
-            When the given :code:`row` is not a :py:class`dict`.
+    @staticmethod
+    def extract_base(subject: str) -> str:
         """
+        Extracts the base of the given subject - assuming that it may be a URL.
 
-        if not isinstance(row, dict):
-            raise TypeError(f"<row> should be {dict}, {type(row)} given.")
+        :param subject:
+            The subject to work with.
+        """
 
-        if not self.is_expired(row):
-            if self.exists(row):
-                if not ignore_if_exist and self[row["subject"]] != row:
-                    self.remove(row)
-                    self.add(row)
-            else:
-                self.add(row)
+        try:
+            return Url2Netloc(subject).get_converted()
+        except ValueError:
+            return subject
 
-        return self
+    def convert(self, data: Any, *, aggressive: bool = False) -> List[str]:
+        """
+        Converts the given dataset.
 
-    @CSVDatasetBase.execute_if_authorized(None)
-    def remove(self, row: dict) -> "CSVDatasetBase":
+        :param data:
+            The data to convert.
+        :param bool aggressive:
+            Whether we should aggressively decode subjects.
         """
-        Removes the given dataset from the CSV file.
 
-        :param row:
-            The row or dataset to add.
+        result = []
 
-        :raise TypeError:
-            When the given :code:`row` is not a :py:class`dict`.
-        """
+        subject = data.strip()
 
-        # If we don't do this, the comparison will fail. #
-        # We don't want to overwrite the whole (remove) method just for what
-        # we need.
-        previous_remove_uneeded_fields = self.remove_unneeded_fields
+        if subject and (
+            not subject.startswith(self.COMMENT)
+            and any(not subject.startswith(x) for x in self.PARTICULAR_COMMENT)
+        ):
+            if self.COMMENT in subject:
+                subject = subject[: subject.find(self.COMMENT)].strip()
 
-        self.set_remove_unneeded_fields(False)
+            if self.NSLOOKUP_SPACE in subject:
+                # Comply with RFC 6367:
+                #    Note that nslookup escapes spaces as "\032" for display
+                #    purposes, but a graphical DNS-SD browser should not.
+                subject = subject.replace(self.NSLOOKUP_SPACE, self.SPACE)
 
-        super().remove(row)
+            if self.SPACE in subject or self.TAB in subject:
+                splitted = subject.split()
 
-        self.set_remove_unneeded_fields(previous_remove_uneeded_fields)
+                if IPSyntaxChecker(splitted[0]).is_valid():
+                    # This is for the hosts format.
+                    # If the first entry is an IP, we will only extract
+                    # the entries after the first one.
 
-        return self
+                    datasets = splitted[1:]
 
-    def cleanup(self) -> "CSVWhoisDataset":
-        """
-        Cleanups the dataset. Meaning that we delete every entries which are
-        in the past.
-        """
+                    if aggressive:
+                        datasets = [self.extract_base(x) for x in datasets]
 
-        for row in self.get_content():
-            if self.is_expired(row):
-                self.remove(row)
+                    result.extend(datasets)
+                else:
+                    if aggressive:
+                        splitted = [self.extract_base(x) for x in splitted]
+
+                    # All other cases, we extract every entries.
+                    result.extend(splitted)
+            else:
+                if aggressive:
+                    subject = self.extract_base(subject)
 
-        return self
+                result.append(subject)
+        return result
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/sql.py` & `PyFunceble-dev-4.2.1/PyFunceble/dataset/whois/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             row["epoch"] = float(row["epoch"])
 
             yield row
 
     @SQLDBDatasetBase.execute_if_authorized(None)
     def update(
         self, row: Union[dict, WhoisRecord], *, ignore_if_exist: bool = False
-    ) -> "MariaDBWhoisDataset":
+    ) -> "SQLDBWhoisDataset":
         """
         Adds the given dataset into the database if it does not exists.
         Update otherwise.
 
         ..note::
             This should be the prefered method for introduction of new dataset.
 
@@ -151,15 +151,15 @@
                 pass
         else:
             PyFunceble.facility.Logger.debug("Expired dataset:\n%r", row)
 
         return self
 
     @SQLDBDatasetBase.execute_if_authorized(None)
-    def cleanup(self) -> "MariaDBWhoisDataset":
+    def cleanup(self) -> "SQLDBWhoisDataset":
         """
         Cleanups the dataset. Meaning that we delete every entries which are
         in the past.
         """
 
         current_timestamp = int(datetime.utcnow().timestamp())
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/exceptions.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/iana.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/ipv4_reputation.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/public_suffix.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/user_agents.py` & `PyFunceble-dev-4.2.1/PyFunceble/downloader/user_agents.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/exceptions.py` & `PyFunceble-dev-4.2.1/PyFunceble/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/facility.py` & `PyFunceble-dev-4.2.1/PyFunceble/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/factory.py` & `PyFunceble-dev-4.2.1/PyFunceble/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/command.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/dns/nameserver.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the command helpers. This helpers let us run Shell commands.
+Provides a way to get or guess the nameserver to use.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,201 +46,243 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import os
-import subprocess
-import sys
-from typing import Generator, Optional, Union
+from typing import List, Optional, Tuple
 
+import dns.exception
+import dns.resolver
+
+import PyFunceble.facility
+import PyFunceble.storage
+from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.url import URLSyntaxChecker
+from PyFunceble.converter.url2netloc import Url2Netloc
 
-class CommandHelper:
-    """
-    Shell command execution.
 
-    :param str command: The command to execute.
-    :param str encoding: The encoding to use to decode the shell output.
+class Nameservers:
+    """
+    Provides an interface to get the right nameserver to communicate with.
     """
 
-    _command: Optional[str] = None
-    _encoding: str = "utf-8"
+    DEFAULT_NAMESERVERS: List[str] = [
+        "9.9.9.10",
+        "149.112.112.10",
+        "2620:fe::10",
+        "2620:fe::fe:10",
+    ]
+
+    nameservers: Optional[List[str]] = None
+    nameserver_ports: Optional[dict] = None
+
+    protocol: Optional[str] = None
+
+    domain_syntax_checker: DomainSyntaxChecker = DomainSyntaxChecker()
+    url_syntax_checker: URLSyntaxChecker = URLSyntaxChecker()
+    url2netloc: Url2Netloc = Url2Netloc()
 
     def __init__(
-        self,
-        command: Optional[Union[str, list]] = None,
-        *,
-        encoding: Optional[str] = None,
+        self, nameserver: Optional[List[str]] = None, protocol: str = "TCP"
     ) -> None:
-        if command is not None:
-            self.command = command
+        self.protocol = protocol
 
-        if encoding is not None:
-            self.encoding = encoding
+        if nameserver is not None:
+            self.set_nameservers(nameserver)
 
-    @property
-    def command(self) -> Optional[str]:
+    @staticmethod
+    def split_nameserver_from_port(
+        nameserver: str,
+        *,
+        default_port: int = 53,
+    ) -> Tuple[str, int]:
         """
-        Provides the current state of the :code:`_command` attribute.
+        Splits the nameserver from its port.re
+
+        :param nameserver:
+            The nameserver to work with.
+        :param default_port:
+            The default port to apply, if none is found.
         """
 
-        return self._command
+        if ":" in nameserver:
+            if nameserver.count(":") > 1:
+                if "]" not in nameserver:
+                    return nameserver, default_port
 
-    @command.setter
-    def command(self, value: Union[str, list]) -> None:
-        """
-        Sets the command to use.
+                nameserver, port = nameserver.split("]:", 1)
 
-        :param value:
-            The command to use/execute.
+                if port.isdigit():
+                    return nameserver[1:], int(port)
+                return nameserver[1:], default_port
 
-        :raise TypeError:
-            When the value is not a :py:class:`list` or :py:class:`str`
-        """
+            splitted = nameserver.rsplit(":")
 
-        if not isinstance(value, (str, list)):
-            raise TypeError(
-                f"<value> should be {str} or {list}, " f"{type(value)} given."
-            )
+            if splitted[-1].isdigit():
+                return ":".join(splitted[:-1]), int(splitted[-1])
 
-        if isinstance(value, list):
-            self._command = " ".join(value)
-        else:
-            self._command = value
+            return ":".join(splitted[:-1]), default_port
+        return nameserver, default_port
 
-    def set_command(self, value: Union[str, list]) -> "CommandHelper":
+    @classmethod
+    def get_ip_from_nameserver(cls, nameserver: str) -> List[str]:
         """
-        Sets the command to use.
+        Given a nameserver, this method resolve it in order to get the
+        IP to contact.
 
-        :param value:
-            The command to use/execute.
+        :param nameserver:
+            The name to resolve.
         """
 
-        self.command = value
+        PyFunceble.facility.Logger.info(
+            "Started to get ip from nameserver (%r)", nameserver
+        )
 
-        return self
+        result = []
 
-    @property
-    def encoding(self) -> Optional[str]:
-        """
-        Provides the current state of the :code:`_encoding` attribute.
-        """
+        if cls.domain_syntax_checker.set_subject(nameserver).is_valid():
+            try:
+                result.extend(
+                    [
+                        x.address
+                        for x in dns.resolver.Resolver().resolve(nameserver, "A")
+                    ]
+                )
+            except dns.exception.DNSException:
+                pass
 
-        return self._encoding
+            try:
+                result.extend(
+                    [
+                        x.address
+                        for x in dns.resolver.Resolver().resolve(nameserver, "AAAA")
+                    ]
+                )
+            except dns.exception.DNSException:
+                pass
+        else:
+            result.append(nameserver)
 
-    @encoding.setter
-    def encoding(self, value: str) -> None:
-        """
-        Sets the encoding to use.
+        PyFunceble.facility.Logger.debug(
+            "IP from nameserver (%r):\n%r", nameserver, result
+        )
 
-        :param value:
-            The value to set.
+        PyFunceble.facility.Logger.info(
+            "Finished to get ip from nameserver (%r)", nameserver
+        )
 
-        :raise TypeError:
-            When the value is not a :py:class:`str`
+        return result
+
+    def set_nameservers(self, value: List[str]) -> "Nameservers":
         """
+        Sets the nameserver to use.
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+        Side Effect:
+            Also updates the :code:`nameserver_ports` variable.
 
-        self._encoding = value
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`list`.
+        :raise ValueError:
+            When the given :code:`value` is emtpy.
+        """
+
+        if not isinstance(value, list):
+            raise TypeError(f"<value> should be {list}, {type(value)} given.")
+
+        if not value:
+            raise ValueError("<value> should not be empty.")
+
+        self.nameserver_ports = {}
+        self.nameservers = []
+
+        for nameserver in value:
+            if self.protocol.lower() == "https":
+                if not nameserver.startswith("https://"):
+                    netloc = self.url2netloc.set_data_to_convert(
+                        nameserver
+                    ).get_converted()
+
+                    if "/" in nameserver:
+                        path = nameserver[nameserver.find("/") :]
+                    else:
+                        path = ""
+
+                    self.nameservers.append(
+                        "https://"
+                        # pylint: disable=line-too-long
+                        f"{netloc}{path}"
+                    )
+                else:
+                    self.nameservers.append(nameserver)
 
-    def set_encoding(self, value: str) -> "CommandHelper":
-        """
-        Sets the encoding to use.
+                # 443 is because it's more likely to be for DOH.
+                self.nameserver_ports.update({self.nameservers[-1]: 443})
+                continue
 
-        :param value:
-            The value to set.
-        """
+            server, port = self.split_nameserver_from_port(nameserver)
 
-        self.encoding = value
+            for dns_ip in self.get_ip_from_nameserver(server):
+                self.nameservers.append(dns_ip)
+                self.nameserver_ports.update({dns_ip: port})
 
         return self
 
-    def _decode_output(self, to_decode: bytes) -> str:
+    def get_nameservers(self) -> Optional[List[str]]:
         """
-        Decode the output of a shell command in order to be readable.
-
-        :param bytes to_decode: Output of a command to decode.
-
-        :return: The decoded output.
-        :rtype: str
+        Provides the currently set nameservers.
         """
 
-        if to_decode:
-            return to_decode.decode(self.encoding)
+        return self.nameservers
 
-        return ""
-
-    def execute(self, *, raise_on_error: bool = False) -> str:
+    def get_nameserver_ports(self) -> Optional[dict]:
+        """
+        Provides the currently set nameserver_ports.
         """
-        Execute the given command.
-
-        :parma raise_on_error:
-            Raises on error if set to :py:class:`True`.
 
-        :return: The output of the command.
+        return self.nameserver_ports
 
-        :raise RuntimeError:
-            When the exit code is not equal to 0.
+    def guess_and_set_nameservers(self) -> "Nameservers":
+        """
+        Try to guess and set the nameserver to use.
         """
 
-        # We initiate a process and parse the command to it.
-        with subprocess.Popen(
-            self.command,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT,
-            shell=True,
-            env=os.environ,
-        ) as process:
-            stdout, stderr = process.communicate()
+        if PyFunceble.facility.ConfigLoader.is_already_loaded():
+            if PyFunceble.storage.CONFIGURATION.dns.server:
+                if isinstance(PyFunceble.storage.CONFIGURATION.dns.server, list):
+                    self.set_nameservers(PyFunceble.storage.CONFIGURATION.dns.server)
+                else:
+                    self.set_nameservers([PyFunceble.storage.CONFIGURATION.dns.server])
+            else:  # pragma: no cover
+                try:
+                    ## Well, I don't like playing with the default resolver.
+                    self.set_nameservers(
+                        dns.resolver.get_default_resolver().nameservers
+                    )
+                except dns.resolver.NoResolverConfiguration:
+                    self.set_nameservers(self.DEFAULT_NAMESERVERS)
+        else:  # pragma: no cover
+            try:
+                ## Well, I don't like playing with the default resolver.
+                self.set_nameservers(dns.resolver.get_default_resolver().nameservers)
+            except dns.resolver.NoResolverConfiguration:
+                self.set_nameservers(self.DEFAULT_NAMESERVERS)
 
-            if process.returncode != 0:
-                if raise_on_error:
-                    raise RuntimeError(repr(self._decode_output(stderr)))
-                return self._decode_output(stderr)
-            return self._decode_output(stdout)
+        return self
 
-    def run(self, rstrip: bool = True) -> Generator[str, None, None]:
+    def guess_all_settings(
+        self,
+    ) -> "Nameservers":  # pragma: no cover ## Method themselves are more important
         """
-        Run the given command and yield each line(s) one by one.
-
-        .. note::
-            The difference between this method and
-            :func:`~PyFunceble.helpers.Command.execute`
-            is that :func:`~PyFunceble.helpers.Command.execute` wait for the
-            process to end in order to return its output while this method
-            return each line one by one
-            - as they are outputed.
-
-        :param bool rstrip:
-            Deactivates the rstrip of the output.
+        Try to guess all settings.
         """
 
-        with subprocess.Popen(
-            self.command,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.STDOUT,
-            shell=True,
-            env=os.environ,
-        ) as process:
-            while True:
-                # Note: we use rstrip() because we are paranoid :-)
-                current_line = process.stdout.readline()
+        to_ignore = ["guess_all_settings"]
 
-                if not current_line and process.poll() is not None:
-                    break
+        for method in dir(self):
+            if method in to_ignore or not method.startswith("guess_"):
+                continue
 
-                if rstrip:
-                    yield self._decode_output(current_line.rstrip())
-                else:
-                    yield self._decode_output(current_line)
+            getattr(self, method)()
 
-    def run_to_stdout(self) -> None:
-        """
-        Run the given command and print each line(s) to stdout.
-        """
-
-        for line in self.run(rstrip=False):
-            sys.stdout.write(line)
+        return self
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/dict.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/directory.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/directory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/download.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/download.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/environment_variable.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/environment_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
+import logging
 import os
 from typing import Any, Optional, Union
 
 import dotenv
 
 
 class EnvironmentVariableHelper:
@@ -70,14 +71,16 @@
     def __init__(self, name: Optional[str] = None, env_file_path: Optional[str] = None):
         if name is not None:
             self.name = name
 
         if env_file_path is not None:
             self.env_file_path = env_file_path
 
+        logging.getLogger("dotenv").setLevel(logging.CRITICAL)
+
     @property
     def name(self) -> Optional[str]:
         """
         Provides the current state of the :code:`_name` attribute.
         """
 
         return self._name
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/exceptions.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/file.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/hash.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/hash.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/list.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/list.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/merge.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/merge.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/regex.py` & `PyFunceble-dev-4.2.1/PyFunceble/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/logger.py` & `PyFunceble-dev-4.2.1/PyFunceble/logger.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/collection.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/collection.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/nameserver.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a way to get or guess the nameserver to use.
+Provides the base of all our adapter.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,243 +46,243 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import List, Optional, Tuple
+from typing import Optional
 
-import dns.exception
-import dns.resolver
+import requests.adapters
+import requests.models
 
-import PyFunceble.facility
 import PyFunceble.storage
-from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
-from PyFunceble.checker.syntax.url import URLSyntaxChecker
-from PyFunceble.converter.url2netloc import Url2Netloc
+from PyFunceble.checker.syntax.ip import IPSyntaxChecker
+from PyFunceble.query.dns.query_tool import DNSQueryTool
 
 
-class Nameservers:
+class RequestAdapterBase(requests.adapters.HTTPAdapter):
     """
-    Provides an interface to get the right nameserver to communicate with.
+    Extends the built-in HTTP adapater and acts as a base for all our own
+    adapter.
     """
 
-    DEFAULT_NAMESERVERS: List[str] = [
-        "9.9.9.10",
-        "149.112.112.10",
-        "2620:fe::10",
-        "2620:fe::fe:10",
-    ]
-
-    nameservers: Optional[List[str]] = None
-    nameserver_ports: Optional[dict] = None
-
-    protocol: Optional[str] = None
-
-    domain_syntax_checker: DomainSyntaxChecker = DomainSyntaxChecker()
-    url_syntax_checker: URLSyntaxChecker = URLSyntaxChecker()
-    url2netloc: Url2Netloc = Url2Netloc()
-
-    def __init__(
-        self, nameserver: Optional[List[str]] = None, protocol: str = "TCP"
-    ) -> None:
-        self.protocol = protocol
+    resolving_cache: dict = {}
+    resolving_use_cache: bool = False
+    timeout: float = 5.0
+    proxy_pattern: dict = {}
+
+    def __init__(self, *args, **kwargs):
+        if "timeout" in kwargs:
+            self.timeout = float(kwargs["timeout"])
+            del kwargs["timeout"]
+
+        if "max_retries" in kwargs:
+            kwargs["max_retries"] = requests.adapters.Retry(
+                total=kwargs["max_retries"], respect_retry_after_header=False
+            )
+
+        if "dns_query_tool" in kwargs:
+            self.dns_query_tool = kwargs["dns_query_tool"]
+            del kwargs["dns_query_tool"]
+        else:
+            self.dns_query_tool = DNSQueryTool()
+
+        if "proxy_pattern" in kwargs:
+            self.proxy_pattern = kwargs["proxy_pattern"]
+            del kwargs["proxy_pattern"]
+        else:
+            self.proxy_pattern = {}
 
-        if nameserver is not None:
-            self.set_nameservers(nameserver)
+        super().__init__(*args, **kwargs)
 
     @staticmethod
-    def split_nameserver_from_port(
-        nameserver: str,
-        *,
-        default_port: int = 53,
-    ) -> Tuple[str, int]:
+    def fake_response() -> requests.models.Response:
         """
-        Splits the nameserver from its port.re
+        Provides the fake response that is provided when we couldn't resolve the
+        given domain.
+        """
+
+        raise PyFunceble.factory.Requester.exceptions.ConnectionError(
+            "Could not resolve."
+        )
 
-        :param nameserver:
-            The nameserver to work with.
-        :param default_port:
-            The default port to apply, if none is found.
+    @staticmethod
+    def extract_extension(subject: str) -> Optional[str]:
         """
+        Provides the extension of the given subject.
 
-        if ":" in nameserver:
-            if nameserver.count(":") > 1:
-                if "]" not in nameserver:
-                    return nameserver, default_port
+        .. versionchanged:: 4.1.1.dev
+            Handle the case that the given subject does not have a `.` (point).
 
-                nameserver, port = nameserver.split("]:", 1)
+        :param str subject:
+            The subject to get extract the extension from.
 
-                if port.isdigit():
-                    return nameserver[1:], int(port)
-                return nameserver[1:], default_port
+        :raise TypeError:
+            When the given :code:`subject` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`subject` is an empty :py:class:`str`.
+        """
 
-            splitted = nameserver.rsplit(":")
+        if not subject or "." not in subject:
+            return None
 
-            if splitted[-1].isdigit():
-                return ":".join(splitted[:-1]), int(splitted[-1])
+        if subject.endswith("."):
+            # Absolute needs a little correction.
+            last_point = subject[:-1].rfind(".")
+        else:
+            last_point = subject.rindex(".")
 
-            return ":".join(splitted[:-1]), default_port
-        return nameserver, default_port
+        extension = subject[last_point + 1 :]
 
-    @classmethod
-    def get_ip_from_nameserver(cls, nameserver: str) -> List[str]:
-        """
-        Given a nameserver, this method resolve it in order to get the
-        IP to contact.
+        if extension.endswith("."):
+            return extension[:-1]
+        return extension
 
-        :param nameserver:
-            The name to resolve.
+    def fetch_proxy_from_pattern(self, subject: str) -> dict:
         """
+        Provides the proxy settings to use for the given subject.
 
-        PyFunceble.facility.Logger.info(
-            "Started to get ip from nameserver (%r)", nameserver
-        )
+        .. versionchanged:: 4.1.1.dev
+            Handle the case that the given subject has no extension/TLD.
 
-        result = []
+        :param str subject:
+            The subject to work with.
 
-        if cls.domain_syntax_checker.set_subject(nameserver).is_valid():
-            try:
-                result.extend(
-                    [
-                        x.address
-                        for x in dns.resolver.Resolver().resolve(nameserver, "A")
-                    ]
-                )
-            except dns.exception.DNSException:
-                pass
+        :raise TypeError:
+            When the given :code:`subject` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`subject` is an empty :py:class:`str`.
+        """
 
-            try:
-                result.extend(
-                    [
-                        x.address
-                        for x in dns.resolver.Resolver().resolve(nameserver, "AAAA")
-                    ]
-                )
-            except dns.exception.DNSException:
-                pass
-        else:
-            result.append(nameserver)
+        def correct_input(pattern_input: dict) -> dict:
+            result = {}
 
-        PyFunceble.facility.Logger.debug(
-            "IP from nameserver (%r):\n%r", nameserver, result
-        )
+            if "http" in pattern_input and pattern_input["http"]:
+                result["http"] = pattern_input["http"]
 
-        PyFunceble.facility.Logger.info(
-            "Finished to get ip from nameserver (%r)", nameserver
-        )
+            if "https" in pattern_input and pattern_input["https"]:
+                result["https"] = pattern_input["https"]
 
-        return result
+            if "http" in result and "https" not in result:
+                result["https"] = result["http"]
 
-    def set_nameservers(self, value: List[str]) -> "Nameservers":
-        """
-        Sets the nameserver to use.
+            if "https" in result and "http" not in result:
+                result["http"] = result["https"]
 
-        Side Effect:
-            Also updates the :code:`nameserver_ports` variable.
+            return result
 
-        :raise TypeError:
-            When the given :code:`value` is not a :py:class:`list`.
-        :raise ValueError:
-            When the given :code:`value` is emtpy.
-        """
+        extension = self.extract_extension(subject)
 
-        if not isinstance(value, list):
-            raise TypeError(f"<value> should be {list}, {type(value)} given.")
+        proxies = {}
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
+        if extension and "rules" in self.proxy_pattern:
+            for rule in self.proxy_pattern["rules"]:
+                local_proxy = {}
 
-        self.nameserver_ports = {}
-        self.nameservers = []
-
-        for nameserver in value:
-            if self.protocol.lower() == "https":
-                if not nameserver.startswith("https://"):
-                    netloc = self.url2netloc.set_data_to_convert(
-                        nameserver
-                    ).get_converted()
-
-                    if "/" in nameserver:
-                        path = nameserver[nameserver.find("/") :]
-                    else:
-                        path = ""
-
-                    self.nameservers.append(
-                        "https://"
-                        # pylint: disable=line-too-long
-                        f"{netloc}{path}"
-                    )
-                else:
-                    self.nameservers.append(nameserver)
+                if "http" in rule and rule["http"]:
+                    local_proxy["http"] = rule["http"]
+                if "https" in rule and rule["https"]:
+                    local_proxy["https"] = rule["https"]
 
-                # 443 is because it's more likely to be for DOH.
-                self.nameserver_ports.update({self.nameservers[-1]: 443})
-                continue
+                if not local_proxy:
+                    continue
 
-            server, port = self.split_nameserver_from_port(nameserver)
+                if "tld" in rule and extension in rule["tld"]:
+                    proxies = correct_input(local_proxy)
+                    break
 
-            for dns_ip in self.get_ip_from_nameserver(server):
-                self.nameservers.append(dns_ip)
-                self.nameserver_ports.update({dns_ip: port})
+        if not proxies and "global" in self.proxy_pattern:
+            proxies = correct_input(self.proxy_pattern["global"])
 
-        return self
+        return proxies
 
-    def get_nameservers(self) -> Optional[List[str]]:
+    def resolve_with_cache(self, hostname: str) -> Optional[str]:
         """
-        Provides the currently set nameservers.
+        Try to resolve using an internal cache.
         """
 
-        return self.nameservers
+        if hostname not in self.resolving_cache:
+            self.resolving_cache[hostname] = self.resolve_without_cache(hostname)
+
+        return self.resolving_cache[hostname]
 
-    def get_nameserver_ports(self) -> Optional[dict]:
+    def resolve_without_cache(self, hostname: str) -> Optional[str]:
         """
-        Provides the currently set nameserver_ports.
+        Resolves the IP of the given hostname.
+
+        :param hostname:
+            The hostname to get resolve.
         """
 
-        return self.nameserver_ports
+        def get_last_cname(subject: str, recursion_depth: int = 60) -> Optional[str]:
+            """
+            Given a subject, this function tries to query the CNAME until there
+            is none.
 
-    def guess_and_set_nameservers(self) -> "Nameservers":
-        """
-        Try to guess and set the nameserver to use.
-        """
+            :param subject:
+                The first subject.
+            """
 
-        if PyFunceble.facility.ConfigLoader.is_already_loaded():
-            if PyFunceble.storage.CONFIGURATION.dns.server:
-                if isinstance(PyFunceble.storage.CONFIGURATION.dns.server, list):
-                    self.set_nameservers(PyFunceble.storage.CONFIGURATION.dns.server)
+            last_cname_result = []
+            last_cname_new_subject = subject
+
+            depth = 0
+
+            while depth < recursion_depth:
+                local_last_cname_result = (
+                    self.dns_query_tool.set_query_record_type("CNAME")
+                    .set_subject(last_cname_new_subject)
+                    .query()
+                )
+
+                depth += 1
+
+                if any(x in last_cname_result for x in local_last_cname_result):
+                    break
+
+                last_cname_result.extend(local_last_cname_result)
+
+                if local_last_cname_result:
+                    last_cname_new_subject = local_last_cname_result[0]
                 else:
-                    self.set_nameservers([PyFunceble.storage.CONFIGURATION.dns.server])
-            else:  # pragma: no cover
-                try:
-                    ## Well, I don't like playing with the default resolver.
-                    self.set_nameservers(
-                        dns.resolver.get_default_resolver().nameservers
-                    )
-                except dns.resolver.NoResolverConfiguration:
-                    self.set_nameservers(self.DEFAULT_NAMESERVERS)
-        else:  # pragma: no cover
+                    break
+
             try:
-                ## Well, I don't like playing with the default resolver.
-                self.set_nameservers(dns.resolver.get_default_resolver().nameservers)
-            except dns.resolver.NoResolverConfiguration:
-                self.set_nameservers(self.DEFAULT_NAMESERVERS)
+                return last_cname_result[-1]
+            except IndexError:
+                return None
+
+        result = set()
+
+        if not IPSyntaxChecker(hostname).is_valid():
+            last_cname = get_last_cname(hostname)
+
+            if last_cname:
+                result.update(
+                    self.dns_query_tool.set_query_record_type("A")
+                    .set_subject(last_cname)
+                    .query()
+                )
+            else:
+                result.update(
+                    self.dns_query_tool.set_query_record_type("A")
+                    .set_subject(hostname)
+                    .query()
+                )
+        else:
+            result.add(hostname)
 
-        return self
+        if result:
+            return result.pop()
+        return None
 
-    def guess_all_settings(
-        self,
-    ) -> "Nameservers":  # pragma: no cover ## Method themselves are more important
+    def resolve(self, hostname: str) -> Optional[str]:
         """
-        Try to guess all settings.
+        Resolves with the prefered method.
         """
 
-        to_ignore = ["guess_all_settings"]
-
-        for method in dir(self):
-            if method in to_ignore or not method.startswith("guess_"):
-                continue
-
-            getattr(self, method)()
-
-        return self
+        if hostname:
+            if self.resolving_use_cache:
+                return self.resolve_with_cache(hostname)
+            return self.resolve_without_cache(hostname)
+        return None
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/query_tool.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/dns/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/resolver.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/dns/resolver.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/http_status_code.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/http_status_code.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/address.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/address.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/converter/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all checker.
+Provides the base of all our converter class.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,91 +46,110 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
 from typing import Any, Optional
 
 
-class NetInfoBase:
+class ConverterBase:
     """
-    Provides the base of network information classes.
+    Provides the base of all converter class.
     """
 
-    _subject: Optional[str] = None
-    base: Optional[str] = None
+    _aggressive: bool = False
+    _data_to_convert: Optional[Any] = None
 
-    def __init__(self, subject: Optional[str] = None) -> None:
-        if subject is not None:
-            self.subject = subject
+    def __init__(
+        self,
+        data_to_convert: Optional[Any] = None,
+        *,
+        aggressive: bool = None,
+    ) -> None:
+        if data_to_convert is not None:
+            self.data_to_convert = data_to_convert
 
-    def ensure_subject_is_given(func):  # pylint: disable=no-self-argument
+        if aggressive is not None:
+            self.aggressive = aggressive
+
+    @property
+    def data_to_convert(self) -> Optional[Any]:
+        """
+        Provides the current state of the :code:`_data_to_convert` attribute.
         """
-        Ensures that the subject is given before running the decorated method.
 
-        :raise TypeError:
-            If the subject is not a string.
+        return self._data_to_convert
+
+    @data_to_convert.setter
+    def data_to_convert(self, value: Any) -> None:
         """
+        Sets the data to convert / to work with.
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(self.subject, str):
-                raise TypeError(
-                    f"<self.subject> should be {str}, {type(self.subject)} given."
-                )
+        :param value:
+            The value to set.
+        """
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+        self._data_to_convert = value
 
-        return wrapper
+    def set_data_to_convert(self, value: Any) -> "ConverterBase":
+        """
+        Sets the data to convert / to work with.
+
+        :param value:
+            The value to set.
+        """
+
+        self.data_to_convert = value
+
+        return self
 
     @property
-    def subject(self) -> Optional[str]:
+    def aggressive(self) -> bool:
         """
-        Provides the current state of the :code:`_subject` attribute.
+        Provides the state of the :code:`_aggressive` attribute.
         """
 
-        return self._subject
+        return self._aggressive
 
-    @subject.setter
-    def subject(self, value: str) -> None:
+    @aggressive.setter
+    def aggressive(self, value: bool) -> None:
         """
-        Sets the subject to work with.
-
-        :param value:
-            The subject to set.
+        Provides a way to activate/deactivate the aggressive decoding.
 
         :raise TypeError:
-            When the given :code:`value` is not a :py:class:`str`.
-        :raise ValueError:
-            When the given :code:`value` is empty.
+            When the given data to convert is not :py:class:`str`
         """
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+        if not isinstance(value, bool):
+            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
+        self._aggressive = value
 
-        self._subject = value
-
-    def set_subject(self, value: str) -> "NetInfoBase":
+    def set_aggressive(self, value: bool) -> "ConverterBase":
         """
-        Sets the subject to work with.
-
-        :param value:
-            The subject to set.
+        Provides a way to activate/deactivate the aggressive decoding.
         """
 
-        self.subject = value
+        self.aggressive = value
 
         return self
 
-    @ensure_subject_is_given
-    def get_info(self) -> Any:
+    def get_converted(self) -> Optional[Any]:
         """
-        Provides the wanted network information.
+        Provides the converted data.
+        """
+
+        raise NotImplementedError()
+
+    def convert(self, data: Any, *, aggressive: bool = False) -> Optional[Any]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        :param aggressive.
+            Whether we should aggressively extract datasets.
         """
 
         raise NotImplementedError()
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/hostbyaddr.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/netinfo/hostbyaddr.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/record/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/digit2digits.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all our record classes.
+Provides an easy way to convert a digit string to 2 digits.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -45,47 +45,44 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+# pylint: enable=line-too-long
 
-import dataclasses
-import json
 from typing import Any
 
+from PyFunceble.query.whois.converter.base import ConverterBase
 
-@dataclasses.dataclass
-class RecordBase:
+
+class Digit2Digits(ConverterBase):
     """
-    Provides the base of all query record classes.
+    Converts a given digit to a 2 digits string.
     """
 
-    def __getitem__(self, key: str) -> Any:
-        return getattr(self, key)
-
-    def to_dict(self) -> dict:
-        """
-        Provides the dict representation of the current object.
+    @ConverterBase.data_to_convert.setter
+    def data_to_convert(self, value: Any) -> Any:
         """
+        Overrites the default behavior.
 
-        return {
-            x: y if not hasattr(y, "to_dict") else y.to_dict()
-            for x, y in self.__dict__.items()
-            if not x.startswith("__")
-        }
+        :param value:
+            The data to convert.
 
-    def to_json(self, *, pretty_print: bool = False) -> str:
+        :raise TypeError:
+            When the given data to convert is not :py:class:`str`
         """
-        Provides the JSON representation of the current object.
 
-        :param pretty_print:
-            If True, the JSON will be formatted.
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+
+        # pylint: disable=no-member
+        super(Digit2Digits, self.__class__).data_to_convert.fset(self, value)
+
+    @ConverterBase.ensure_data_to_convert_is_given
+    def get_converted(self) -> str:
+        """
+        Provides the converted data (after conversion)
         """
 
-        return json.dumps(
-            self.to_dict(),
-            indent=4 if pretty_print else None,
-            ensure_ascii=False,
-            sort_keys=True if pretty_print else None,
-        )
+        return str(self.data_to_convert).zfill(2)
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/dns.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/record/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/whois.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/record/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/http.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/http.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/https.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/requests/adapter/https.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/requester.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/requests/requester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/base.py` & `PyFunceble-dev-4.2.1/PyFunceble/utils/platform.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all WHOIS converter/extracter class.
+Provides a simple way to get the current platform.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,80 +46,76 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
-from typing import Any, Optional
+import platform
 
 
-class ConverterBase:
+class PlatformUtility:
     """
-    Provides the base of all converter class.
+    Provides an easy way to get the current platform.
     """
 
-    _data_to_convert: Optional[Any] = None
-
-    def __init__(self, data_to_convert: Optional[Any] = None) -> None:
-        if data_to_convert is not None:
-            self.data_to_convert = data_to_convert
+    WINDOWS: list = ["windows"]
+    """
+    Provides the list of supported windows platform.
+    """
 
-    def ensure_data_to_convert_is_given(func):  # pylint: disable=no-self-argument
-        """
-        Ensures that the data to convert is given before running the decorated method.
+    CYGWIN: list = ["cygwin", "cygwin_nt-10.0"]
+    """
+    Provides the list of supporter cygwin platform.
+    """
 
-        :raise TypeError:
-            If the subject is not a string.
-        """
+    UNIX: list = ["linux", "darwin"]
+    """
+    Provides the list of supported unix platform.
+    """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(self.data_to_convert, str):
-                raise TypeError(
-                    f"<self.subject> should be {str}, "
-                    f"{type(self.data_to_convert)} given."
-                )
+    MAC: list = ["darwin"]
+    """
+    Provides the list of supported MAC platform.
+    """
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+    @staticmethod
+    def get() -> str:
+        """
+        Returns the current platform.
+        """
 
-        return wrapper
+        return platform.system().lower()
 
-    @property
-    def data_to_convert(self) -> Optional[Any]:
+    @classmethod
+    def is_cygwin(cls) -> bool:
         """
-        Provides the current state of the :code:`_data_to_convert` attribute.
+        Checks if the current platform is in our cygwin list.
         """
 
-        return self._data_to_convert
+        current_platform = cls.get()
 
-    @data_to_convert.setter
-    def data_to_convert(self, value: Any) -> Any:
-        """
-        Sets the data to convert / to work with.
+        return any(x in current_platform for x in cls.CYGWIN)
 
-        :param value:
-            The data to convert
+    @classmethod
+    def is_windows(cls) -> bool:
+        """
+        Checks if the current platform is in our windows list.
         """
 
-        self._data_to_convert = value
+        return cls.get() in cls.WINDOWS or cls.is_cygwin()
 
-    def set_data_to_convert(self, value: Any) -> "ConverterBase":
+    @classmethod
+    def is_unix(cls) -> bool:
         """
-        Sets the data to convert / to work with.
-
-        :param value:
-            The data to convert
+        Checks if the current platform is in our unix list.
         """
 
-        self.data_to_convert = value
-
-        return self
+        return cls.get() in cls.UNIX
 
-    @ensure_data_to_convert_is_given
-    def get_converted(self) -> Optional[Any]:
+    @classmethod
+    def is_mac_os(cls) -> bool:
         """
-        Provides the converted data.
+        Checks if the current platform is in our OSX list.
         """
 
-        raise NotImplementedError()
+        return cls.get() in cls.MAC
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/digit2digits.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/month2unified.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an easy way to convert a digit string to 2 digits.
+Provides a way to convert a given month to our unified format.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -45,44 +45,62 @@
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-# pylint: enable=line-too-long
 
-from typing import Any
+from typing import Any, Dict, List
 
 from PyFunceble.query.whois.converter.base import ConverterBase
 
 
-class Digit2Digits(ConverterBase):
+class Month2Unified(ConverterBase):
     """
-    Converts a given digit to a 2 digits string.
+    Converts the given month into our unified format.
     """
 
+    MAP: Dict[str, List[str]] = {
+        "jan": [str(1), "01", "jan", "january", "jan."],
+        "feb": [str(2), "02", "feb", "february", "feb."],
+        "mar": [str(3), "03", "mar", "march", "mar."],
+        "apr": [str(4), "04", "apr", "april", "apr."],
+        "may": [str(5), "05", "may"],
+        "jun": [str(6), "06", "jun", "june", "jun."],
+        "jul": [str(7), "07", "jul", "july", "jul."],
+        "aug": [str(8), "08", "aug", "august", "aug."],
+        "sep": [str(9), "09", "sep", "september", "sep.", "sept", "sept."],
+        "oct": [str(10), "oct", "october", "oct."],
+        "nov": [str(11), "nov", "november", "nov."],
+        "dec": [str(12), "dec", "december", "dec."],
+    }
+
     @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> Any:
+    def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
-        :param value:
-            The data to convert.
-
         :raise TypeError:
             When the given data to convert is not :py:class:`str`
         """
 
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         # pylint: disable=no-member
-        super(Digit2Digits, self.__class__).data_to_convert.fset(self, value)
+        super(Month2Unified, self.__class__).data_to_convert.fset(self, value)
 
     @ConverterBase.ensure_data_to_convert_is_given
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
+
+        .. warning::
+            If no month is found, the given data is given as response.
         """
 
-        return str(self.data_to_convert).zfill(2)
+        for to_return, possibilities in self.MAP.items():
+            if self.data_to_convert.lower() in possibilities:
+                return to_return
+
+        return self.data_to_convert
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/expiration_date.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/converter/expiration_date.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/month2unified.py` & `PyFunceble-dev-4.2.1/PyFunceble/utils/profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint: disable=invalid-name
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a way to convert a given month to our unified format.
+Provides some global utilities.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,61 +47,87 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Any, Dict, List
+import contextlib
+import cProfile
+import io
+import linecache
+import pstats
+import tracemalloc
 
-from PyFunceble.query.whois.converter.base import ConverterBase
 
+@contextlib.contextmanager
+def profile_it(*, sort_stats: str = "cumulative", show_callers: bool = False):
+    """
+    Provides a context manager which will activates the profiling of our
+    source code.
+
+    :param sort_starts:
+        The column to sort.
+    :param show_callers:
+        Authorizes the output of the callers.
+    """
+
+    profiler = cProfile.Profile()
+    profiler.enable()
+
+    yield
+
+    profiler.disable()
+
+    our_stream = io.StringIO()
 
-class Month2Unified(ConverterBase):
+    profiler_starts = pstats.Stats(profiler, stream=our_stream)
+
+    if sort_stats:
+        profiler_starts.sort_stats(sort_stats)
+
+    profiler_starts.print_stats()
+
+    if show_callers:
+        profiler_starts.print_callees()
+
+    print(our_stream.getvalue())
+
+
+@contextlib.contextmanager
+def profile_memory(stats_mode: str = "lineno", top_limit: int = 10):
     """
-    Converts the given month into our unified format.
+    Provides a context manager which will activates memory profiling of our
+    source code.
     """
 
-    MAP: Dict[str, List[str]] = {
-        "jan": [str(1), "01", "jan", "january", "jan."],
-        "feb": [str(2), "02", "feb", "february", "feb."],
-        "mar": [str(3), "03", "mar", "march", "mar."],
-        "apr": [str(4), "04", "apr", "april", "apr."],
-        "may": [str(5), "05", "may"],
-        "jun": [str(6), "06", "jun", "june", "jun."],
-        "jul": [str(7), "07", "jul", "july", "jul."],
-        "aug": [str(8), "08", "aug", "august", "aug."],
-        "sep": [str(9), "09", "sep", "september", "sep.", "sept", "sept."],
-        "oct": [str(10), "oct", "october", "oct."],
-        "nov": [str(11), "nov", "november", "nov."],
-        "dec": [str(12), "dec", "december", "dec."],
-    }
-
-    @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> None:
-        """
-        Overrites the default behavior.
-
-        :raise TypeError:
-            When the given data to convert is not :py:class:`str`
-        """
-
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
-
-        # pylint: disable=no-member
-        super(Month2Unified, self.__class__).data_to_convert.fset(self, value)
-
-    @ConverterBase.ensure_data_to_convert_is_given
-    def get_converted(self) -> str:
-        """
-        Provides the converted data (after conversion)
-
-        .. warning::
-            If no month is found, the given data is given as response.
-        """
-
-        for to_return, possibilities in self.MAP.items():
-            if self.data_to_convert.lower() in possibilities:
-                return to_return
+    tracemalloc.start()
+
+    yield
 
-        return self.data_to_convert
+    snapshot = tracemalloc.take_snapshot()
+    snapshot = snapshot.filter_traces(
+        (
+            tracemalloc.Filter(False, "<frozen importlib._bootstrap>"),
+            tracemalloc.Filter(False, "<unknown>"),
+            tracemalloc.Filter(False, "<frozen importlib._bootstrap_external>"),
+        )
+    )
+    top_stats = snapshot.statistics(stats_mode)
+
+    print("Top %s lines" % top_limit)
+    for index, stat in enumerate(top_stats[:top_limit], 1):
+        frame = stat.traceback[0]
+        print(
+            "#%s: %s:%s: %.1f KiB"
+            % (index, frame.filename, frame.lineno, stat.size / 1024)
+        )
+        line = linecache.getline(frame.filename, frame.lineno).strip()
+        if line:
+            print("    %s" % line)
+
+    other = top_stats[top_limit:]
+    if other:
+        size = sum(stat.size for stat in other)
+        print("%s other: %.1f KiB" % (len(other), size / 1024))
+    total = sum(stat.size for stat in top_stats)
+    print("Total allocated size: %.1f KiB" % (total / 1024))
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/registrar.py` & `PyFunceble-dev-4.2.1/PyFunceble/cli/utils/ascii_logo.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides our registrar extrator.
+Provides some utilities related to the ascii logo.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,84 +46,81 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Any, List, Optional
+import colorama
 
-from PyFunceble.helpers.regex import RegexHelper
-from PyFunceble.query.whois.converter.base import ConverterBase
+import PyFunceble.cli.storage
+import PyFunceble.facility
+import PyFunceble.storage
 
 
-class RegistarExtractor(ConverterBase):
-    """
-    Provides an interface for the extration of the registrar.
+def colorify(color: str, *, text=None) -> str:
     """
+    Colorify the logo with the given color.
 
-    PATTERNS: List[str] = [
-        r"authorized\s+agency(\s+|):(.*)",
-        r"domain\s+support(\s+|):(.*)",
-        r"registrar\s+name(\s+|):(.*)",
-        r"registrar_name(\s+|):(.*)",
-        r"registrar(\s+|):(.*)",
-        r"registrar\.+(\s+|):(.*)",
-        r"registration\s+service\s+provider(\s+|):(.*)",
-        r"sponsoring\s+registrar(\s+|):(.*)",
-        r"sponsoring\s+registrar\s+organization(\s+|):(.*)",
-    ]
+    :param color:
+        The name of the color to apply.
 
-    @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> None:
-        """
-        Sets the data to convert and work with.
+        .. warning::
+            The given color name must be one of the supported
+            by colorama.
 
-        :param value:
-            The record to work with.
+    :raise ValueError:
+        When the given :code:`color` is unsupported.
+    """
 
-        :raise TypeError:
-            When the given data to convert is not :py:class:`str`.
-        :raise ValueError:
-            When the given :code:`value` is empty.
-        """
+    color = color.upper()
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+    if not text:
+        to_color = PyFunceble.cli.storage.ASCII_PYFUNCEBLE
+    else:
+        to_color = text
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
+    if not hasattr(colorama.Fore, color):
+        raise ValueError(f"<color> ({color!r}) is not supported.")
 
-        # pylint: disable=no-member
-        super(RegistarExtractor, self.__class__).data_to_convert.fset(self, value)
+    color_to_apply = getattr(colorama.Fore, color)
+    result = []
 
-    def __get_line(self) -> Optional[str]:
-        """
-        Tries to get the registrar line from the given record.
-        """
+    if (
+        PyFunceble.facility.ConfigLoader.is_already_loaded()
+        and PyFunceble.storage.CONFIGURATION.cli_testing.display_mode.colour
+    ):
+        for line in to_color.split("\n"):
+            result.append(f"{color_to_apply}{line}{colorama.Fore.RESET}")
 
-        for regex in self.PATTERNS:
-            registrar_line = RegexHelper(r"(?i)" + regex).match(
-                self.data_to_convert, return_match=True, rematch=True, group=0
-            )
+        return "\n".join(result)
+    return to_color
 
-            if not registrar_line:
-                continue
 
-            return registrar_line
-        return None
+def get_home_representation() -> str:
+    """
+    Provides our home ASCII logo representation.
+    """
 
-    @ConverterBase.ensure_data_to_convert_is_given
-    def get_converted(self) -> Optional[str]:
-        """
-        Provides the registrar of the record (if found).
-        """
+    return colorify("yellow")
 
-        registrar_line = self.__get_line()
 
-        if registrar_line:
-            try:
-                return [x.strip() for x in registrar_line if x.strip()][0]
-            except IndexError:
-                pass
+def get_result_representation(status: str) -> str:
+    """
+    Provides our result ASCII logo representation.
+    """
+
+    if status in (
+        PyFunceble.storage.STATUS.up,
+        PyFunceble.storage.STATUS.valid,
+        PyFunceble.storage.STATUS.sane,
+    ):
+        color = "green"
+    elif status in (
+        PyFunceble.storage.STATUS.down,
+        PyFunceble.storage.STATUS.malicious,
+    ):
+        color = "red"
+    else:
+        color = "cyan"
 
-        return None
+    return colorify(color, text=PyFunceble.cli.storage.ASCII_PYUNCEBLE_RESULT)
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/query_tool.py` & `PyFunceble-dev-4.2.1/PyFunceble/query/whois/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/sessions.py` & `PyFunceble-dev-4.2.1/PyFunceble/sessions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/storage.py` & `PyFunceble-dev-4.2.1/PyFunceble/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 from box import Box
 from dotenv import load_dotenv
 
 from PyFunceble.storage_facility import get_config_directory
 
 PROJECT_NAME: str = "PyFunceble"
-PROJECT_VERSION: str = "4.2.0a9.dev (Blue Duckling: Ixora)"
+PROJECT_VERSION: str = "4.2.1.dev (Blue Duckling: Ixora)"
 
 DISTRIBUTED_CONFIGURATION_FILENAME: str = ".PyFunceble_production.yaml"
 DISTRIBUTED_DIR_STRUCTURE_FILENAME: str = "dir_structure_production.json"
 
 IANA_DUMP_FILENAME: str = "iana-domains-db.json"
 PUBLIC_SUFFIX_DUMP_FILENAME: str = "public-suffix.json"
 CONFIGURATION_FILENAME: str = ".PyFunceble.yaml"
@@ -81,15 +81,15 @@
 )
 PUBLIC_SUFFIX_DUMP_LINK: str = "https://raw.githubusercontent.com/PyFunceble/public-suffix/master/public-suffix.json"
 USER_AGENT_DUMP_LINK: str = (
     "https://raw.githubusercontent.com/PyFunceble/user_agents/master/user_agents.json"
 )
 IPV4_REPUTATION_DUMP_LINK: str = "https://reputation.alienvault.com/reputation.data"
 
-SHORT_REPO_LINK: str = "https://git.io/vpZoI"
+SHORT_REPO_LINK: str = "https://pyfunceble.github.io"
 REPO_LINK: str = "https://github.com/funilrys/PyFunceble"
 
 NOT_RESOLVED_STD_HOSTNAME: str = f"pyfunceble-{secrets.token_hex(12)}.com"
 
 IANA: Optional[dict] = {}
 PUBLIC_SUFFIX: Optional[dict] = {}
 USER_AGENTS: Optional[dict] = {}
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/storage_facility.py` & `PyFunceble-dev-4.2.1/PyFunceble/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/utils/__init__.py` & `PyFunceble-dev-4.2.1/PyFunceble/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/utils/platform.py` & `PyFunceble-dev-4.2.1/PyFunceble/checker/reputation/domain_and_ip.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a simple way to get the current platform.
+Provides the domains and IP reputation checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -46,76 +46,54 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import platform
+from PyFunceble.checker.reputation.base import ReputationCheckerBase
+from PyFunceble.checker.reputation.domain import DomainReputationChecker
+from PyFunceble.checker.reputation.ip import IPReputationChecker
 
 
-class PlatformUtility:
-    """
-    Provides an easy way to get the current platform.
-    """
-
-    WINDOWS: list = ["windows"]
-    """
-    Provides the list of supported windows platform.
-    """
-
-    CYGWIN: list = ["cygwin", "cygwin_nt-10.0"]
-    """
-    Provides the list of supporter cygwin platform.
-    """
-
-    UNIX: list = ["linux", "darwin"]
-    """
-    Provides the list of supported unix platform.
+class DomainAndIPReputationChecker(ReputationCheckerBase):
     """
+    Provides the interface for checking the reputation of an IP or domain.
 
-    MAC: list = ["darwin"]
-    """
-    Provides the list of supported MAC platform.
+    :param str subject:
+        Optional, The subject to work with.
+    :param bool do_syntax_check_first:
+        Optional, Activates/Disables the check of the status before the actual
+        status gathering.
     """
 
-    @staticmethod
-    def get() -> str:
-        """
-        Returns the current platform.
-        """
-
-        return platform.system().lower()
-
-    @classmethod
-    def is_cygwin(cls) -> bool:
-        """
-        Checks if the current platform is in our cygwin list.
-        """
-
-        current_platform = cls.get()
-
-        return any(x in current_platform for x in cls.CYGWIN)
-
-    @classmethod
-    def is_windows(cls) -> bool:
+    @ReputationCheckerBase.ensure_subject_is_given
+    @ReputationCheckerBase.update_status_date_after_query
+    def query_status(self) -> "DomainAndIPReputationChecker":
         """
-        Checks if the current platform is in our windows list.
+        Queries the result without anything more.
         """
 
-        return cls.get() in cls.WINDOWS or cls.is_cygwin()
+        if self.status.ip_syntax:
+            query_object = IPReputationChecker(
+                self.subject,
+                do_syntax_check_first=self.do_syntax_check_first,
+                db_session=self.db_session,
+                use_collection=self.use_collection,
+            )
+        else:
+            query_object = DomainReputationChecker(
+                self.subject,
+                do_syntax_check_first=self.do_syntax_check_first,
+                db_session=self.db_session,
+                use_collection=self.use_collection,
+            )
 
-    @classmethod
-    def is_unix(cls) -> bool:
-        """
-        Checks if the current platform is in our unix list.
-        """
+        query_object.ipv4_reputation_query_tool = self.ipv4_reputation_query_tool
+        query_object.collection_query_tool = self.collection_query_tool
+        query_object.dns_query_tool = self.dns_query_tool
 
-        return cls.get() in cls.UNIX
+        result = query_object.query_status()
 
-    @classmethod
-    def is_mac_os(cls) -> bool:
-        """
-        Checks if the current platform is in our OSX list.
-        """
+        self.__dict__.update(query_object.__dict__)
 
-        return cls.get() in cls.MAC
+        return result
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble/utils/version.py` & `PyFunceble-dev-4.2.1/PyFunceble/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/PKG-INFO` & `PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.0a9
+Version: 4.2.1
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -15,15 +15,15 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: psql
 Provides-Extra: full
 License-File: LICENSE
 
@@ -86,24 +86,24 @@
 ------------
 
 :code:`pip`
 ^^^^^^^^^^^
 
 ::
 
-    $ pip install --upgrade --pre pyfunceble-dev
+    $ pip install --upgrade pyfunceble
     $ pyfunceble --version
 
 :code:`docker`
 ^^^^^^^^^^^^^^
 
 ::
 
-    $ docker pull pyfunceble/pyfunceble-dev
-    $ docker run -it pyfunceble/pyfunceble-dev --version
+    $ docker pull pyfunceble/pyfunceble
+    $ docker run -it pyfunceble/pyfunceble --version
 
 ___________________________________________
 
 Documentation as the place to be!
 ---------------------------------
 
 Want to know more about details **PyFunceble**?
```

### Comparing `PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/SOURCES.txt` & `PyFunceble-dev-4.2.1/PyFunceble_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,28 +31,30 @@
 PyFunceble/checker/availability/ip.py
 PyFunceble/checker/availability/params.py
 PyFunceble/checker/availability/status.py
 PyFunceble/checker/availability/url.py
 PyFunceble/checker/availability/extras/__init__.py
 PyFunceble/checker/availability/extras/base.py
 PyFunceble/checker/availability/extras/dns.py
+PyFunceble/checker/availability/extras/etoxic.py
 PyFunceble/checker/availability/extras/parked.py
 PyFunceble/checker/availability/extras/rules.py
 PyFunceble/checker/availability/extras/subject_switch.py
 PyFunceble/checker/reputation/__init__.py
 PyFunceble/checker/reputation/base.py
 PyFunceble/checker/reputation/domain.py
 PyFunceble/checker/reputation/domain_and_ip.py
 PyFunceble/checker/reputation/ip.py
 PyFunceble/checker/reputation/params.py
 PyFunceble/checker/reputation/status.py
 PyFunceble/checker/reputation/url.py
 PyFunceble/checker/syntax/__init__.py
 PyFunceble/checker/syntax/base.py
 PyFunceble/checker/syntax/domain.py
+PyFunceble/checker/syntax/domain_and_ip.py
 PyFunceble/checker/syntax/domain_base.py
 PyFunceble/checker/syntax/ip.py
 PyFunceble/checker/syntax/ipv4.py
 PyFunceble/checker/syntax/ipv6.py
 PyFunceble/checker/syntax/params.py
 PyFunceble/checker/syntax/second_lvl_domain.py
 PyFunceble/checker/syntax/status.py
```

### Comparing `PyFunceble-dev-4.2.0a9/README.rst` & `PyFunceble-dev-4.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 ------------
 
 :code:`pip`
 ^^^^^^^^^^^
 
 ::
 
-    $ pip install --upgrade --pre pyfunceble-dev
+    $ pip install --upgrade pyfunceble
     $ pyfunceble --version
 
 :code:`docker`
 ^^^^^^^^^^^^^^
 
 ::
 
-    $ docker pull pyfunceble/pyfunceble-dev
-    $ docker run -it pyfunceble/pyfunceble-dev --version
+    $ docker pull pyfunceble/pyfunceble
+    $ docker run -it pyfunceble/pyfunceble --version
 
 ___________________________________________
 
 Documentation as the place to be!
 ---------------------------------
 
 Want to know more about details **PyFunceble**?
```

### Comparing `PyFunceble-dev-4.2.0a9/setup.py` & `PyFunceble-dev-4.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     return open("README.rst", encoding="utf-8").read()
 
 
 if __name__ == "__main__":
     setuptools.setup(
         name="PyFunceble-dev",
         version=get_version(),
-        python_requires=">=3.6, <4",
+        python_requires=">=3.8, <4",
         install_requires=get_requirements(mode="standard"),
         extras_require={
             "docs": get_requirements(mode="docs"),
             "dev": get_requirements(mode="dev"),
             "test": get_requirements(mode="test"),
             "psql": get_requirements(mode="psql"),
             "full": get_requirements(mode="full"),
```

