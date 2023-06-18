# Comparing `tmp/netbox-contract-2.0.3.tar.gz` & `tmp/netbox-contract-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.3.tar", last modified: Wed Jun  7 19:32:38 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.4.tar", last modified: Sun Jun 18 16:14:40 2023, max compression
```

## Comparing `netbox-contract-2.0.3.tar` & `netbox-contract-2.0.4.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.865804 netbox-contract-2.0.3/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.3/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.3/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3156 2023-06-07 19:32:38.861803 netbox-contract-2.0.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2617 2023-06-07 19:30:34.000000 netbox-contract-2.0.3/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-07 19:31:19.000000 netbox-contract-2.0.3/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-07 19:32:38.865804 netbox-contract-2.0.3/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.3/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.765802 netbox-contract-2.0.3/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.809802 netbox-contract-2.0.3/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-07 19:31:06.000000 netbox-contract-2.0.3/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.829803 netbox-contract-2.0.3/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1435 2023-06-04 09:17:47.000000 netbox-contract-2.0.3/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5650 2023-06-04 08:54:12.000000 netbox-contract-2.0.3/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.853803 netbox-contract-2.0.3/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1982 2023-06-07 19:20:38.000000 netbox-contract-2.0.3/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3712 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.857803 netbox-contract-2.0.3/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-07 19:05:00.000000 netbox-contract-2.0.3/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-07 19:03:26.000000 netbox-contract-2.0.3/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.861803 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4390 2023-06-07 19:24:12.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8388 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.825803 netbox-contract-2.0.3/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3156 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.482623 netbox-contract-2.0.4/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.4/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.4/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3733 2023-06-18 16:14:40.478623 netbox-contract-2.0.4/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3194 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-18 16:12:50.000000 netbox-contract-2.0.4/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-18 16:14:40.482623 netbox-contract-2.0.4/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.4/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.454622 netbox-contract-2.0.4/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.462622 netbox-contract-2.0.4/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-18 16:13:17.000000 netbox-contract-2.0.4/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.470622 netbox-contract-2.0.4/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4090 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      983 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1444 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7013 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.474623 netbox-contract-2.0.4/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      630 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0016_contract_parent.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5692 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2240 2023-06-18 13:35:02.000000 netbox-contract-2.0.4/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3785 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.474623 netbox-contract-2.0.4/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-18 13:30:49.000000 netbox-contract-2.0.4/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-18 13:30:49.000000 netbox-contract-2.0.4/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.478623 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3871 2023-06-18 13:35:02.000000 netbox-contract-2.0.4/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8622 2023-06-18 13:35:02.000000 netbox-contract-2.0.4/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.466622 netbox-contract-2.0.4/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3733 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2276 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.3/LICENSE` & `netbox-contract-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/PKG-INFO` & `netbox-contract-2.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: netbox-contract
-Version: 2.0.3
-Summary: Contract management plugin for Netbox
-Author-email: Marc Lebreuil <marc@famillelebreuil.net>
-Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
-Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
 ## Installation
@@ -93,7 +79,16 @@
 
 Add support for Netbox 3.5 which become the minimum version supported to accomodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
 
 #### version 2.0.3
 
 * [#60](https://github.com/mlebreuil/netbox-contract/issues/60) Update contract quick search to also filter on fields "External reference" and "Comments".
 * [#49](https://github.com/mlebreuil/netbox-contract/issues/49) Manage permissions.
+
+#### version 2.0.4
+
+* Add bulk update capability for contract assignement
+* [#63](https://github.com/mlebreuil/netbox-contract/issues/63) Correct an API issue on the invoice object.
+* [#64](https://github.com/mlebreuil/netbox-contract/issues/64) Add hierarchy to contract; New parent field created.
+* [#65](https://github.com/mlebreuil/netbox-contract/issues/65) Add end date to contact import form.
+* Removed the possibility of add or modify circuits to contracts. The field becomes read only and will be removed in next major release.
+* Make accounting dimensions optional.
```

### Comparing `netbox-contract-2.0.3/README.md` & `netbox-contract-2.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: netbox-contract
+Version: 2.0.4
+Summary: Contract management plugin for Netbox
+Author-email: Marc Lebreuil <marc@famillelebreuil.net>
+Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
+Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
 ## Installation
@@ -79,7 +93,16 @@
 
 Add support for Netbox 3.5 which become the minimum version supported to accomodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
 
 #### version 2.0.3
 
 * [#60](https://github.com/mlebreuil/netbox-contract/issues/60) Update contract quick search to also filter on fields "External reference" and "Comments".
 * [#49](https://github.com/mlebreuil/netbox-contract/issues/49) Manage permissions.
+
+#### version 2.0.4
+
+* Add bulk update capability for contract assignement
+* [#63](https://github.com/mlebreuil/netbox-contract/issues/63) Correct an API issue on the invoice object.
+* [#64](https://github.com/mlebreuil/netbox-contract/issues/64) Add hierarchy to contract; New parent field created.
+* [#65](https://github.com/mlebreuil/netbox-contract/issues/65) Add end date to contact import form.
+* Removed the possibility of add or modify circuits to contracts. The field becomes read only and will be removed in next major release.
+* Make accounting dimensions optional.
```

### Comparing `netbox-contract-2.0.3/pyproject.toml` & `netbox-contract-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-contract"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/api/serializers.py` & `netbox-contract-2.0.4/src/netbox_contract/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,20 @@
 
 class ContractSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:contract-detail'
     )
     circuit= NestedCircuitSerializer(many=True, required=False)
     external_partie = NestedServiceProviderSerializer(many=False)
+    parent = NestedContracSerializer(many=False, required=False)
 
     class Meta:
         model = Contract
         fields = (
-            'id', 'url','display', 'name', 'status', 'external_partie','internal_partie','circuit','comments',
+            'id', 'url','display', 'name', 'status', 'external_partie','internal_partie','parent','circuit','comments',
             'tags', 'custom_fields', 'created', 'last_updated',
         )
 
 class InvoiceSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_contract-api:invoice-detail'
     )
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/api/views.py` & `netbox-contract-2.0.4/src/netbox_contract/api/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import filtersets, models
 from .serializers import ContractSerializer, InvoiceSerializer, ServiceProviderSerializer, ContractAssignementSerializer
 
 class ContractViewSet(NetBoxModelViewSet):
-    queryset = models.Contract.objects.prefetch_related('circuit','tags')
+    queryset = models.Contract.objects.prefetch_related(
+        'parent','circuit','tags'
+        )
     serializer_class = ContractSerializer
 
 class InvoiceViewSet(NetBoxModelViewSet):
     queryset = models.Invoice.objects.prefetch_related(
-        'contract', 'tags'
+        'contracts', 'tags'
     )
     serializer_class = InvoiceSerializer
     filterset_class = filtersets.InvoiceFilterSet
 
 class ServiceProviderViewSet(NetBoxModelViewSet):
     queryset = models.ServiceProvider.objects.prefetch_related('tags')
     serializer_class = ServiceProviderSerializer
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.4/src/netbox_contract/filtersets.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from netbox.filtersets import NetBoxModelFilterSet
 from .models import Contract,Invoice,ServiceProvider,ContractAssignement
 
 class ContractFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = Contract
-        fields = ('id', 'external_partie', 'internal_partie', 'status','circuit')
+        fields = ('id', 'external_partie', 'internal_partie', 'status','parent','circuit')
 
     def search(self, queryset, name, value):
         return queryset.filter( Q(name__icontains=value)
                                | Q(external_partie__name__icontains=value)
                                | Q(external_reference__icontains=value)
                                | Q(comments__icontains=value))
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/forms.py` & `netbox-contract-2.0.4/src/netbox_contract/forms.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from django import forms
+from django.contrib.contenttypes.models import ContentType
 import django_filters
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
-from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField, CSVModelChoiceField, SlugField
+from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField, CSVModelChoiceField, SlugField, CSVContentTypeField
 from utilities.forms.widgets import DatePicker
 from extras.filters import TagFilter
 from circuits.models import Circuit
+from tenancy.models import Tenant
 from .models import Contract, Invoice, ServiceProvider, StatusChoices, ContractAssignement
 
 class ContractForm(NetBoxModelForm):
     comments = CommentField()
-    circuit=DynamicModelMultipleChoiceField(
-        queryset=Circuit.objects.all(),
-        required=False
-    )
+
     external_partie=DynamicModelChoiceField(
         queryset=ServiceProvider.objects.all()
     )
+    tenant=DynamicModelChoiceField(
+        queryset=Tenant.objects.all()
+    )
+    parent=DynamicModelChoiceField(
+        queryset=Contract.objects.all(),
+        required=False
+    )
 
     class Meta:
         model = Contract
         fields = ('name', 'external_partie', 'external_reference', 'internal_partie','tenant', 'status',
           'start_date', 'end_date','initial_term', 'renewal_term', 'currency','accounting_dimensions',
-          'mrc', 'nrc','invoice_frequency','circuit', 'documents', 'comments', 'tags')
+          'mrc', 'nrc','invoice_frequency','parent','documents', 'comments', 'tags')
 
         widgets = {
             'start_date': DatePicker(),
             'end_date': DatePicker(),
         }
 
 class InvoiceForm(NetBoxModelForm):
@@ -42,75 +48,100 @@
             'date': DatePicker(),
             'period_start': DatePicker(),
             'period_end': DatePicker(),
         }
 
 class ContractFilterSetForm(NetBoxModelFilterSetForm):
     model = Contract
-    external_partie=DynamicModelMultipleChoiceField(
+    external_partie=DynamicModelChoiceField(
         queryset=ServiceProvider.objects.all(),
         required=False
     )
+    tenant=DynamicModelChoiceField(
+        queryset=Tenant.objects.all(),
+        required=False
+    )
     external_reference=forms.CharField(
         required=False
     )
     internal_partie= forms.CharField(
         required=False
     )
     status = MultipleChoiceField(
         choices=StatusChoices,
         required= False
     )
     circuit = DynamicModelMultipleChoiceField(
         queryset=Circuit.objects.all(),
         required=False
     )
+    parent=DynamicModelChoiceField(
+        queryset=Contract.objects.all(),
+        required=False
+    )
 
 class InvoiceFilterSetForm(NetBoxModelFilterSetForm):
     model = Invoice
     contracts=DynamicModelMultipleChoiceField(
         queryset=Contract.objects.all(),
         required=False
     )
 
 class ContractCSVForm(NetBoxModelImportForm):
-    circuit = CSVModelChoiceField(
-        queryset=Circuit.objects.all(),
+    external_partie = CSVModelChoiceField(
+        queryset=ServiceProvider.objects.all(),
+        to_field_name='name',
+        help_text='Service provider name'
+    )
+    tenant = CSVModelChoiceField(
+        queryset=Tenant.objects.all(),
+        to_field_name='name',
+        help_text='Tenant name',
+        required=False
+    )
+    parent = CSVModelChoiceField(
+        queryset=Contract.objects.all(),
         to_field_name='name',
-        help_text='Related Circuit'
+        help_text='Contract name',
+        required=False
     )
 
     class Meta:
         model = Contract
         fields = [
             'name', 'external_partie', 'internal_partie','tenant', 'status',
-            'start_date', 'initial_term', 'renewal_term', 'mrc', 'nrc',
-            'invoice_frequency', 'circuit'
+            'start_date', 'end_date','initial_term', 'renewal_term', 'mrc', 'nrc',
+            'invoice_frequency', 'parent'
         ]
 
 class ContractBulkEditForm(NetBoxModelBulkEditForm):
     name = forms.CharField(
         max_length=100,
         required=True
     )
-    external_partie = forms.CharField(
-        max_length=30,
-        required=True
+    external_partie = DynamicModelChoiceField(
+        queryset=ServiceProvider.objects.all(),
+        required=False
     )
     external_reference=forms.CharField(
         max_length=100,
         required=False
     )
     internal_partie = forms.CharField(
         max_length=30,
         required=True
     )
     comments = CommentField()
     circuit=DynamicModelChoiceField(
-        queryset=Circuit.objects.all()
+        queryset=Circuit.objects.all(),
+        required=False
+    )
+    parent = DynamicModelChoiceField(
+        queryset=Contract.objects.all(),
+        required=False
     )
 
     nullable_fields = (
         'comments',
     )
     model = Contract
 
@@ -177,20 +208,34 @@
 
 # ContractAssignement
 
 class ContractAssignementForm(NetBoxModelForm):
     contract=DynamicModelChoiceField(
         queryset=Contract.objects.all()
     )
+
     class Meta:
         model = ContractAssignement
         fields = ['content_type', 'object_id', 'contract','tags']
         widgets = {
             'content_type': forms.HiddenInput(),
             'object_id': forms.HiddenInput(),
         }
 
 class ContractAssignementFilterSetForm(NetBoxModelFilterSetForm):
     model = ContractAssignement
     contract=DynamicModelChoiceField(
         queryset=Contract.objects.all()
     )
+
+class ContractAssignementImportForm(NetBoxModelImportForm):
+    content_type = CSVContentTypeField(
+        queryset=ContentType.objects.all(),
+        help_text="Content Type in the form <app>.<model>"
+    )
+    contract = CSVModelChoiceField(
+        queryset=Contract.objects.all(),
+        help_text="Contract id"
+    )
+    class Meta:
+        model = ContractAssignement
+        fields = ['content_type', 'object_id', 'contract','tags']
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox-contract-2.0.4/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/models.py` & `netbox-contract-2.0.4/src/netbox_contract/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,16 @@
     )
     currency = models.CharField(
         max_length=3,
         choices=CurrencyChoices,
         default=CurrencyChoices.CURRENCY_USD
     )
     accounting_dimensions = models.JSONField(
-        null=True
+        null=True,
+        blank=True
     )
     mrc = models.DecimalField(
         verbose_name = "Monthly recuring cost",
         max_digits = 10,
         decimal_places= 2
     )
     nrc = models.DecimalField(
@@ -160,22 +161,29 @@
     )
     invoice_frequency = models.IntegerField(
         help_text = "The frequency of invoices in month",
         default = 1
     )
     circuit = models.ManyToManyField(Circuit,
         related_name='contracts',
-        blank=True,
+        blank=True
     )
     documents = models.URLField(
         blank=True
     )
     comments = models.TextField(
         blank=True
     )
+    parent = models.ForeignKey(
+        'self',
+        on_delete=models.CASCADE,
+        related_name='child',
+        null=True,
+        blank=True
+    )
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_contract:contract', args=[self.pk])
 
     class Meta:
         ordering = ('name',)
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/navigation.py` & `netbox-contract-2.0.4/src/netbox_contract/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,16 +50,21 @@
 
 service_provider_menu_item = PluginMenuItem(
         link='plugins:netbox_contract:serviceprovider_list',
         link_text='Service Providers',
         buttons=serviceprovider_buttons,
         permissions=['netbox_contract.view_serviceprovider']
     )
+contract_assignemnt_menu_item = PluginMenuItem(
+        link='plugins:netbox_contract:contractassignement_list',
+        link_text='Contract assignements',
+        permissions=['netbox_contract.view_contractassignement']
+    )
 
-items = (contract_menu_item,invoices_menu_item,service_provider_menu_item)
+items = (contract_menu_item,invoices_menu_item,service_provider_menu_item, contract_assignemnt_menu_item)
 
 if plugin_settings.get("top_level_menu"):
     menu = PluginMenu(
         label="Contracts",
         groups=(("Contracts", items),),
         icon_class="mdi mdi-file-sign",
     )
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/search.py` & `netbox-contract-2.0.4/src/netbox_contract/search.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/tables.py` & `netbox-contract-2.0.4/src/netbox_contract/tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,21 +59,24 @@
     name = tables.Column(
         linkify=True
     )
     external_partie = tables.Column(
         linkify=True
     )
     circuit = tables.ManyToManyColumn()
+    parent = tables.Column(
+        linkify=True
+    )
 
     class Meta(NetBoxTable.Meta):
         model = Contract
         fields = ('pk', 'id', 'name', 'circuit', 'external_partie',
          'external_reference','internal_partie', 'status', 'mrc',
-         'comments', 'actions')
-        default_columns = ('name', 'status', 'circuit')
+         'parent','comments', 'actions')
+        default_columns = ('name', 'status', 'parent','circuit')
 
 class ContractListBottomTable(NetBoxTable):
     name = tables.Column(
         linkify=True
     )
     class Meta(NetBoxTable.Meta):
         model = Contract
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/template_content.py` & `netbox-contract-2.0.4/src/netbox_contract/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox-contract-2.0.4/src/netbox_contract/templates/contract_assignements_bottom.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,20 @@
               <th scope="row">Non recuring costs</th>
               <td>{{ object.nrc }}</td>
             </tr>
             <tr>
               <th scope="row">Invoice frequency</th>
               <td>{{ object.invoice_frequency }}</td>
             </tr>
+            <tr>
+              <th scope="row">Parent</th>
+              <td>
+                <a href="{{ object.parent.get_absolute_url }}">{{ object.parent.name }}</a>
+              </td>
+            </tr>
             {% if object.documents %}
             <tr>
               <th scope="row">Documents</th>
                 <td>
                   <a href="{{ object.documents }}" target="_blank">Documents</a>
                 </td>
             </tr>
```

#### html2text {}

```diff
@@ -14,14 +14,15 @@
 Initial term           {{ object.initial_term }}
 Renewal term           {{ object.renewal_term }}
 Currency               {{ object.currency }}
 Accounting dimensions  {{ object.accounting_dimensions }}
 Monthly recuring costs {{ object.mrc }}
 Non recuring costs     {{ object.nrc }}
 Invoice frequency      {{ object.invoice_frequency }}
+Parent                 {{_object.parent.name_}}
 Documents              Documents
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 ** Circuits **
 {% render_table circuit_table %}
 ** Assignements **
 {% render_table assignements_table %}
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract_assignement.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.3/src/netbox_contract/urls.py` & `netbox-contract-2.0.4/src/netbox_contract/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     path('invoices/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='invoice_changelog', kwargs={
         'model': models.Invoice
     }),
 
     # Contract assignements
     path('assignements/', views.ContractAssignementListView.as_view(), name='contractassignement_list'),
     path('assignements/add/', views.ContractAssignementEditView.as_view(), name='contractassignement_add'),
+    path('assignements/import/', views.ContractAssignementBulkImportView.as_view(), name='contractassignement_import'),
     path('assignements/<int:pk>/', views.ContractAssignementView.as_view(), name='contractassignement'),
     path('assignements/<int:pk>/edit/', views.ContractAssignementEditView.as_view(), name='contractassignement_edit'),
     path('assignements/<int:pk>/delete/', views.ContractAssignementDeleteView.as_view(), name='contractassignement_delete'),
     path('assignements/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='contractassignement_changelog', kwargs={
         'model': models.ContractAssignement
     }),
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract/views.py` & `netbox-contract-2.0.4/src/netbox_contract/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,29 +56,34 @@
     filterset_form = forms.ContractAssignementFilterSetForm
 
 class ContractAssignementEditView(generic.ObjectEditView):
     queryset = models.ContractAssignement.objects.all()
     form = forms.ContractAssignementForm
 
     def alter_object(self, instance, request, args, kwargs):
-        if not instance.pk:
+        if not instance.pk and kwargs:
             # Assign the object based on URL kwargs
             content_type = get_object_or_404(ContentType, pk=request.GET.get('content_type'))
             instance.object = get_object_or_404(content_type.model_class(), pk=request.GET.get('object_id'))
         return instance
 
     def get_extra_addanother_params(self, request):
         return {
             'content_type': request.GET.get('content_type'),
             'object_id': request.GET.get('object_id'),
         }
 
 class ContractAssignementDeleteView(generic.ObjectDeleteView):
     queryset = models.ContractAssignement.objects.all()
 
+class ContractAssignementBulkImportView(generic.BulkImportView):
+    queryset = models.ContractAssignement.objects.all()
+    model_form = forms.ContractAssignementImportForm
+    table = tables.ContractAssignementListTable
+
 # Contract views
 
 class ContractView(generic.ObjectView):
     queryset = models.Contract.objects.all()
 
     def get_extra_context(self, request, instance):
         invoices_table = tables.InvoiceListTable(instance.invoices.all())
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.4/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.3
+Version: 2.0.4
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -93,7 +93,16 @@
 
 Add support for Netbox 3.5 which become the minimum version supported to accomodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
 
 #### version 2.0.3
 
 * [#60](https://github.com/mlebreuil/netbox-contract/issues/60) Update contract quick search to also filter on fields "External reference" and "Comments".
 * [#49](https://github.com/mlebreuil/netbox-contract/issues/49) Manage permissions.
+
+#### version 2.0.4
+
+* Add bulk update capability for contract assignement
+* [#63](https://github.com/mlebreuil/netbox-contract/issues/63) Correct an API issue on the invoice object.
+* [#64](https://github.com/mlebreuil/netbox-contract/issues/64) Add hierarchy to contract; New parent field created.
+* [#65](https://github.com/mlebreuil/netbox-contract/issues/65) Add end date to contact import form.
+* Removed the possibility of add or modify circuits to contracts. The field becomes read only and will be removed in next major release.
+* Make accounting dimensions optional.
```

### Comparing `netbox-contract-2.0.3/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.4/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 src/netbox_contract/migrations/0009_contract_external_reference.py
 src/netbox_contract/migrations/0010_invoice_contracts.py
 src/netbox_contract/migrations/0011_auto_20230122_2112.py
 src/netbox_contract/migrations/0012_remove_invoice_contract.py
 src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
 src/netbox_contract/migrations/0014_contract_end_date.py
 src/netbox_contract/migrations/0015_contractassignement.py
+src/netbox_contract/migrations/0016_contract_parent.py
+src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
 src/netbox_contract/migrations/__init__.py
 src/netbox_contract/templates/contract_assignements_bottom.html
 src/netbox_contract/templates/contract_list_bottom.html
 src/netbox_contract/templates/netbox_contract/contract.html
 src/netbox_contract/templates/netbox_contract/contract_assignement.html
 src/netbox_contract/templates/netbox_contract/invoice.html
 src/netbox_contract/templates/netbox_contract/serviceprovider.html
```

