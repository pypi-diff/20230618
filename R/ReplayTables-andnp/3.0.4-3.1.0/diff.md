# Comparing `tmp/ReplayTables-andnp-3.0.4.tar.gz` & `tmp/ReplayTables-andnp-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-3.0.4.tar", last modified: Thu May 25 16:59:24 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-3.1.0.tar", last modified: Sun Jun 18 00:12:00 2023, max compression
```

## Comparing `ReplayTables-andnp-3.0.4.tar` & `ReplayTables-andnp-3.1.0.tar`

### file list

```diff
@@ -1,27 +1,483 @@
--rw-r--r--   0        0        0        0 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/README.md
--rw-r--r--   0        0        0     5167 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     2392 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/PER.py
--rw-r--r--   0        0        0     2964 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/PrioritizedHeap.py
--rw-r--r--   0        0        0     3692 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8237 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/__init__.py
--rw-r--r--   0        0        0     3418 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     5811 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/MinMaxHeap.py
--rw-r--r--   0        0        0     1772 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3822 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1356 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0       58 2023-05-25 16:58:31.587096 ReplayTables-andnp-3.0.4/ReplayTables/_utils/logger.py
--rw-r--r--   0        0        0      886 2023-05-25 16:59:21.063285 ReplayTables-andnp-3.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     2449 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_PER.py
--rw-r--r--   0        0        0     1384 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_PrioritizedHeap.py
--rw-r--r--   0        0        0     3252 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1537 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_Table.py
--rw-r--r--   0        0        0     5619 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/test_View.py
--rw-r--r--   0        0        0        0 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/utils/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/utils/test_MinMaxHeap.py
--rw-r--r--   0        0        0     2998 2023-05-25 16:58:31.591096 ReplayTables-andnp-3.0.4/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2350 2023-06-13 21:33:00.349875 ReplayTables-andnp-3.1.0/README.md
+-rw-r--r--   0        0        0     5167 2023-05-08 23:10:54.125615 ReplayTables-andnp-3.1.0/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-03-16 20:40:38.037236 ReplayTables-andnp-3.1.0/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     2574 2023-06-18 00:11:46.374786 ReplayTables-andnp-3.1.0/ReplayTables/PER.py
+-rw-r--r--   0        0        0     2964 2023-06-17 22:20:09.953421 ReplayTables-andnp-3.1.0/ReplayTables/PrioritizedHeap.py
+-rw-r--r--   0        0        0     3692 2023-06-17 22:20:09.953421 ReplayTables-andnp-3.1.0/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8237 2023-05-08 23:10:48.125581 ReplayTables-andnp-3.1.0/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2022-04-06 23:02:12.927133 ReplayTables-andnp-3.1.0/ReplayTables/__init__.py
+-rw-r--r--   0        0        0    23934 2021-10-21 15:57:57.105439 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/NStepView.rotatedSequence-108.py38.1.nbc
+-rw-r--r--   0        0        0     1152 2021-10-21 15:57:57.105439 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/NStepView.rotatedSequence-108.py38.nbi
+-rw-r--r--   0        0        0    34988 2021-09-09 21:30:40.586019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-114.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 21:30:40.586019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-114.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 21:33:15.666019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-118.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 21:33:15.666019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-118.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 21:35:03.136019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-121.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 21:35:03.136019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-121.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 22:01:42.396021 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-122.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 22:01:42.396021 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-122.py38.nbi
+-rw-r--r--   0        0        0    40387 2021-10-21 15:57:57.425439 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-130.py38.1.nbc
+-rw-r--r--   0        0        0    41339 2021-10-21 15:57:57.735439 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-130.py38.2.nbc
+-rw-r--r--   0        0        0    36061 2021-10-21 15:57:58.005439 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-130.py38.3.nbc
+-rw-r--r--   0        0        0     3283 2021-10-21 15:57:58.005439 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-130.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 22:28:02.456023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-131.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 22:28:02.456023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-131.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 22:35:59.286023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-138.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 22:35:59.286023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-138.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 22:33:21.596023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-143.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 22:33:21.596023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-143.py38.nbi
+-rw-r--r--   0        0        0    35009 2021-09-09 22:38:16.046023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-145.py38.1.nbc
+-rw-r--r--   0        0        0     1300 2021-09-09 22:38:16.046023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-145.py38.nbi
+-rw-r--r--   0        0        0    32527 2021-09-09 22:49:21.606024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-146.py38.1.nbc
+-rw-r--r--   0        0        0    32442 2021-09-09 22:49:58.236024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-146.py38.2.nbc
+-rw-r--r--   0        0        0    31072 2021-09-09 22:48:45.416024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-146.py38.3.nbc
+-rw-r--r--   0        0        0     2274 2021-09-09 22:49:58.236024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-146.py38.nbi
+-rw-r--r--   0        0        0    33190 2021-09-09 22:57:51.936025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-159.py38.1.nbc
+-rw-r--r--   0        0        0     1291 2021-09-09 22:57:51.936025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-159.py38.nbi
+-rw-r--r--   0        0        0    32153 2021-09-09 23:07:21.686025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-174.py38.1.nbc
+-rw-r--r--   0        0        0    32218 2021-09-09 23:07:30.656026 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-174.py38.2.nbc
+-rw-r--r--   0        0        0     2191 2021-09-09 23:07:30.656026 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-174.py38.nbi
+-rw-r--r--   0        0        0    33190 2021-09-09 23:05:17.906025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-175.py38.1.nbc
+-rw-r--r--   0        0        0     1291 2021-09-09 23:05:17.906025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-175.py38.nbi
+-rw-r--r--   0        0        0    43421 2022-06-25 16:47:42.208691 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-232.py310.1.nbc
+-rw-r--r--   0        0        0    44369 2022-06-25 16:47:42.548691 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-232.py310.2.nbc
+-rw-r--r--   0        0        0    39017 2022-06-25 16:47:42.878691 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-232.py310.3.nbc
+-rw-r--r--   0        0        0     3286 2022-06-25 16:47:42.878691 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-232.py310.nbi
+-rw-r--r--   0        0        0    43421 2022-04-17 17:55:01.574104 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py310.1.nbc
+-rw-r--r--   0        0        0    44369 2022-04-17 17:55:01.984104 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py310.2.nbc
+-rw-r--r--   0        0        0    39017 2022-04-17 17:55:02.304104 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py310.3.nbc
+-rw-r--r--   0        0        0     3286 2022-04-17 17:55:02.304104 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py310.nbi
+-rw-r--r--   0        0        0    40387 2021-10-21 15:11:51.095436 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py38.1.nbc
+-rw-r--r--   0        0        0    41339 2021-10-21 15:11:51.405436 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py38.2.nbc
+-rw-r--r--   0        0        0    36061 2021-10-21 15:11:51.665436 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py38.3.nbc
+-rw-r--r--   0        0        0     3283 2021-10-21 15:11:51.665436 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-233.py38.nbi
+-rw-r--r--   0        0        0    49424 2023-05-08 23:39:02.304737 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py310.1.nbc
+-rw-r--r--   0        0        0    49234 2023-05-08 23:39:02.744740 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py310.2.nbc
+-rw-r--r--   0        0        0    44651 2023-05-08 23:39:03.094741 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py310.3.nbc
+-rw-r--r--   0        0        0     3451 2023-05-08 23:39:03.094741 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py310.nbi
+-rw-r--r--   0        0        0    49383 2023-06-12 19:46:30.678380 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py311.1.nbc
+-rw-r--r--   0        0        0    49193 2023-06-12 19:46:31.058380 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py311.2.nbc
+-rw-r--r--   0        0        0    44606 2023-06-12 19:46:31.478381 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py311.3.nbc
+-rw-r--r--   0        0        0     3451 2023-06-12 19:46:31.478381 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py311.nbi
+-rw-r--r--   0        0        0    38060 2022-11-20 17:54:59.496681 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py38.1.nbc
+-rw-r--r--   0        0        0    38237 2022-11-20 17:54:59.726681 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py38.2.nbc
+-rw-r--r--   0        0        0    32995 2022-11-20 17:54:59.976681 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py38.3.nbc
+-rw-r--r--   0        0        0     3055 2022-11-20 17:54:59.976681 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.padded-234.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 21:33:15.136019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-113.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 21:33:15.136019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-113.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 21:35:02.536019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-116.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 21:35:02.536019 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-116.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:01:41.886021 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-117.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:01:41.886021 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-117.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:28:01.826023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-126.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:28:01.826023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-126.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:35:58.706023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-133.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:35:58.706023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-133.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:33:21.016023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-138.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:33:21.006023 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-138.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:38:15.476024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-140.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:38:15.476024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-140.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:49:21.056024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-141.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:49:21.056024 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-141.py38.nbi
+-rw-r--r--   0        0        0    23448 2021-09-09 22:57:51.446025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-154.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 22:57:51.446025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-154.py38.nbi
+-rw-r--r--   0        0        0    23858 2021-09-09 23:07:21.196025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-169.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 23:07:21.196025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-169.py38.nbi
+-rw-r--r--   0        0        0    23858 2021-09-09 23:05:17.366025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-170.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-09-09 23:05:17.356025 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-170.py38.nbi
+-rw-r--r--   0        0        0    26742 2022-06-25 16:47:41.858691 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-227.py310.1.nbc
+-rw-r--r--   0        0        0     1149 2022-06-25 16:47:41.858691 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-227.py310.nbi
+-rw-r--r--   0        0        0    26742 2022-04-17 17:55:01.184104 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-228.py310.1.nbc
+-rw-r--r--   0        0        0     1149 2022-04-17 17:55:01.184104 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-228.py310.nbi
+-rw-r--r--   0        0        0    23858 2021-10-21 15:11:50.785436 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-228.py38.1.nbc
+-rw-r--r--   0        0        0     1148 2021-10-21 15:11:50.785436 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-228.py38.nbi
+-rw-r--r--   0        0        0    33105 2023-05-08 23:39:01.924735 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-229.py310.1.nbc
+-rw-r--r--   0        0        0     1204 2023-05-08 23:39:01.924735 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-229.py310.nbi
+-rw-r--r--   0        0        0    33105 2023-06-12 19:46:30.288380 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-229.py311.1.nbc
+-rw-r--r--   0        0        0     1204 2023-06-12 19:46:30.288380 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-229.py311.nbi
+-rw-r--r--   0        0        0    24112 2022-11-20 17:54:59.266681 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-229.py38.1.nbc
+-rw-r--r--   0        0        0     1072 2022-11-20 17:54:59.266681 ReplayTables-andnp-3.1.0/ReplayTables/__pycache__/Table.rotatedSequence-229.py38.nbi
+-rw-r--r--   0        0        0     3418 2023-04-23 17:25:03.164905 ReplayTables-andnp-3.1.0/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     5811 2023-04-24 20:55:35.833368 ReplayTables-andnp-3.1.0/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0        0        0     1772 2022-11-09 01:40:22.813901 ReplayTables-andnp-3.1.0/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     3822 2023-05-08 23:11:03.755669 ReplayTables-andnp-3.1.0/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2022-04-17 17:53:22.394104 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0    39294 2023-05-08 23:38:54.394697 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py310.1.nbc
+-rw-r--r--   0        0        0    39215 2023-05-08 23:38:56.814709 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py310.2.nbc
+-rw-r--r--   0        0        0    36947 2023-03-17 23:40:33.508733 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py310.3.nbc
+-rw-r--r--   0        0        0     2556 2023-05-08 23:38:56.814709 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py310.nbi
+-rw-r--r--   0        0        0    39254 2023-06-12 19:46:22.408373 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py311.1.nbc
+-rw-r--r--   0        0        0    39183 2023-06-12 19:46:24.848375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py311.2.nbc
+-rw-r--r--   0        0        0     2556 2023-06-12 19:46:24.848375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MemoryWriter._update-7.py311.nbi
+-rw-r--r--   0        0        0    55508 2023-04-24 18:52:48.562698 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-138.py310.1.nbc
+-rw-r--r--   0        0        0     1606 2023-04-24 18:52:48.562698 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-138.py310.nbi
+-rw-r--r--   0        0        0    55508 2023-04-24 19:06:12.015121 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-140.py310.1.nbc
+-rw-r--r--   0        0        0     1606 2023-04-24 19:06:12.015121 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-140.py310.nbi
+-rw-r--r--   0        0        0    55508 2023-04-24 19:09:04.187782 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-141.py310.1.nbc
+-rw-r--r--   0        0        0     1606 2023-04-24 19:09:04.187782 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-141.py310.nbi
+-rw-r--r--   0        0        0    72838 2023-05-08 23:39:01.014731 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-143.py310.1.nbc
+-rw-r--r--   0        0        0     1703 2023-05-08 23:39:01.014731 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-143.py310.nbi
+-rw-r--r--   0        0        0    71183 2023-06-12 19:46:29.438379 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-143.py311.1.nbc
+-rw-r--r--   0        0        0     1703 2023-06-12 19:46:29.438379 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._delete-143.py311.nbi
+-rw-r--r--   0        0        0    52087 2023-04-24 02:18:58.288894 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-100.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-24 02:18:58.288894 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-100.py310.nbi
+-rw-r--r--   0        0        0    52087 2023-04-24 18:42:20.202981 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-102.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-24 18:42:20.202981 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-102.py310.nbi
+-rw-r--r--   0        0        0    52067 2023-04-23 21:13:55.116946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-42.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-23 21:13:55.116946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-42.py310.nbi
+-rw-r--r--   0        0        0    52067 2023-04-23 22:55:59.545924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-59.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-23 22:55:59.545924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-59.py310.nbi
+-rw-r--r--   0        0        0    52067 2023-04-24 01:09:32.434123 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-78.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-24 01:09:32.434123 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-78.py310.nbi
+-rw-r--r--   0        0        0    52067 2023-04-24 01:46:41.764605 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-80.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-24 01:46:41.764605 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-80.py310.nbi
+-rw-r--r--   0        0        0    52068 2023-04-24 18:52:49.132707 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-91.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-24 18:52:49.132707 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-91.py310.nbi
+-rw-r--r--   0        0        0    52074 2023-04-24 19:06:12.625130 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-93.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-24 19:06:12.625130 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-93.py310.nbi
+-rw-r--r--   0        0        0    52075 2023-04-24 19:09:04.807792 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-94.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-24 19:09:04.807792 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-94.py310.nbi
+-rw-r--r--   0        0        0    59179 2023-05-08 23:39:01.604734 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-96.py310.1.nbc
+-rw-r--r--   0        0        0     1660 2023-05-08 23:39:01.604734 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-96.py310.nbi
+-rw-r--r--   0        0        0    59139 2023-06-12 19:46:29.968380 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-96.py311.1.nbc
+-rw-r--r--   0        0        0     1660 2023-06-12 19:46:29.968380 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-96.py311.nbi
+-rw-r--r--   0        0        0    52086 2023-04-24 02:54:23.842540 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-99.py310.1.nbc
+-rw-r--r--   0        0        0     1601 2023-04-24 02:54:23.842540 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._extend-99.py310.nbi
+-rw-r--r--   0        0        0    15771 2023-04-23 23:12:28.025690 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._has_children-116.py310.1.nbc
+-rw-r--r--   0        0        0     1610 2023-04-23 23:12:28.025690 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._has_children-116.py310.nbi
+-rw-r--r--   0        0        0    10987 2023-04-24 02:54:22.622528 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-110.py310.1.nbc
+-rw-r--r--   0        0        0     1148 2023-04-24 02:54:22.622528 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-110.py310.nbi
+-rw-r--r--   0        0        0    11192 2023-04-24 02:18:57.088877 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-111.py310.1.nbc
+-rw-r--r--   0        0        0     1148 2023-04-24 02:18:57.088877 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-111.py310.nbi
+-rw-r--r--   0        0        0    11018 2023-04-24 18:42:16.822929 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-113.py310.1.nbc
+-rw-r--r--   0        0        0     1148 2023-04-24 18:42:16.822929 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-113.py310.nbi
+-rw-r--r--   0        0        0    11159 2023-04-23 21:10:46.456972 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-46.py310.1.nbc
+-rw-r--r--   0        0        0     1147 2023-04-23 21:10:46.456972 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-46.py310.nbi
+-rw-r--r--   0        0        0    11159 2023-04-23 21:13:53.976946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-53.py310.1.nbc
+-rw-r--r--   0        0        0     1147 2023-04-23 21:13:53.976946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-53.py310.nbi
+-rw-r--r--   0        0        0    11159 2023-04-23 22:55:58.375924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-70.py310.1.nbc
+-rw-r--r--   0        0        0     1147 2023-04-23 22:55:58.375924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-70.py310.nbi
+-rw-r--r--   0        0        0    11159 2023-04-24 01:09:31.194069 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-89.py310.1.nbc
+-rw-r--r--   0        0        0     1147 2023-04-24 01:09:31.194069 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-89.py310.nbi
+-rw-r--r--   0        0        0    11159 2023-04-24 01:46:40.554576 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-91.py310.1.nbc
+-rw-r--r--   0        0        0     1147 2023-04-24 01:46:40.554576 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._is_min_level-91.py310.nbi
+-rw-r--r--   0        0        0    35150 2023-04-24 01:27:11.763121 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-225.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 01:27:11.763121 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-225.py310.nbi
+-rw-r--r--   0        0        0    35146 2023-04-24 01:33:23.265111 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-226.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 01:33:23.265111 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-226.py310.nbi
+-rw-r--r--   0        0        0    35146 2023-04-24 01:37:03.000618 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-227.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 01:37:03.000618 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-227.py310.nbi
+-rw-r--r--   0        0        0    35023 2023-04-24 01:45:58.703565 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-235.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 01:45:58.703565 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-235.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 01:46:42.934633 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-236.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 01:46:42.934633 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-236.py310.nbi
+-rw-r--r--   0        0        0    35051 2023-04-23 23:03:54.005813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-242.py310.1.nbc
+-rw-r--r--   0        0        0     1625 2023-04-23 23:03:54.005813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-242.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 02:54:25.062551 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-251.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 02:54:25.062551 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-251.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 02:46:34.748196 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-253.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 02:46:34.748196 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-253.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 18:42:19.142964 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-254.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 18:42:19.142964 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-254.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 18:52:48.042690 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-256.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 18:52:48.042690 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-256.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 19:06:11.515113 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-258.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 19:06:11.515113 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-258.py310.nbi
+-rw-r--r--   0        0        0    35391 2023-04-24 19:09:03.677774 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-259.py310.1.nbc
+-rw-r--r--   0        0        0     1627 2023-04-24 19:09:03.677774 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-259.py310.nbi
+-rw-r--r--   0        0        0    38368 2023-05-08 23:39:00.314727 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-261.py310.1.nbc
+-rw-r--r--   0        0        0     1724 2023-05-08 23:39:00.314727 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-261.py310.nbi
+-rw-r--r--   0        0        0    38383 2023-06-12 19:46:28.698378 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-261.py311.1.nbc
+-rw-r--r--   0        0        0     1724 2023-06-12 19:46:28.698378 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-261.py311.nbi
+-rw-r--r--   0        0        0    35051 2023-04-24 01:09:33.544171 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-271.py310.1.nbc
+-rw-r--r--   0        0        0     1625 2023-04-24 01:09:33.544171 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-271.py310.nbi
+-rw-r--r--   0        0        0    35051 2023-04-24 01:10:55.157718 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-273.py310.1.nbc
+-rw-r--r--   0        0        0     1625 2023-04-24 01:10:55.157718 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._largest_child_or_grandchild-273.py310.nbi
+-rw-r--r--   0        0        0    68001 2023-04-24 01:09:33.864185 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-175.py310.1.nbc
+-rw-r--r--   0        0        0     1607 2023-04-24 01:09:33.864185 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-175.py310.nbi
+-rw-r--r--   0        0        0    71963 2023-04-24 01:37:03.320626 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-177.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:37:03.320626 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-177.py310.nbi
+-rw-r--r--   0        0        0    71883 2023-04-24 01:46:43.324643 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-185.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:46:43.324643 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-185.py310.nbi
+-rw-r--r--   0        0        0    69395 2023-04-24 02:54:25.452555 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-202.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 02:54:25.452555 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-202.py310.nbi
+-rw-r--r--   0        0        0    68717 2023-04-24 02:46:35.078199 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-204.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 02:46:35.078199 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-204.py310.nbi
+-rw-r--r--   0        0        0    69401 2023-04-24 18:42:19.502970 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-205.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 18:42:19.502970 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-205.py310.nbi
+-rw-r--r--   0        0        0    68412 2023-04-24 18:52:48.382695 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-207.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 18:52:48.382695 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-207.py310.nbi
+-rw-r--r--   0        0        0    68412 2023-04-24 19:06:11.835118 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-209.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 19:06:11.835118 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-209.py310.nbi
+-rw-r--r--   0        0        0    68416 2023-04-24 19:09:04.007779 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-210.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 19:09:04.007779 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-210.py310.nbi
+-rw-r--r--   0        0        0    85580 2023-05-08 23:39:00.754729 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-212.py310.1.nbc
+-rw-r--r--   0        0        0     1706 2023-05-08 23:39:00.744729 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-212.py310.nbi
+-rw-r--r--   0        0        0    84027 2023-06-12 19:46:29.178379 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-212.py311.1.nbc
+-rw-r--r--   0        0        0     1706 2023-06-12 19:46:29.178379 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_down-212.py311.nbi
+-rw-r--r--   0        0        0    38987 2023-04-23 23:03:52.275813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-118.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-23 23:03:52.275813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-118.py310.nbi
+-rw-r--r--   0        0        0    38987 2023-04-24 01:09:31.874098 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-123.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 01:09:31.874098 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-123.py310.nbi
+-rw-r--r--   0        0        0    38987 2023-04-24 01:37:01.320577 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-125.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 01:37:01.320577 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-125.py310.nbi
+-rw-r--r--   0        0        0    38987 2023-04-24 01:46:41.214592 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-133.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 01:46:41.214592 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-133.py310.nbi
+-rw-r--r--   0        0        0    39851 2023-04-24 02:54:23.262534 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-150.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 02:54:23.262534 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-150.py310.nbi
+-rw-r--r--   0        0        0    39038 2023-04-24 02:46:27.838133 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-152.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 02:46:27.838133 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-152.py310.nbi
+-rw-r--r--   0        0        0    39886 2023-04-24 18:42:17.662942 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-153.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 18:42:17.662942 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-153.py310.nbi
+-rw-r--r--   0        0        0    38897 2023-04-24 18:52:46.762670 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-155.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 18:52:46.762670 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-155.py310.nbi
+-rw-r--r--   0        0        0    38897 2023-04-24 19:06:10.225093 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-157.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 19:06:10.225093 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-157.py310.nbi
+-rw-r--r--   0        0        0    38897 2023-04-24 19:09:02.337753 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-158.py310.1.nbc
+-rw-r--r--   0        0        0     1605 2023-04-24 19:09:02.337753 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-158.py310.nbi
+-rw-r--r--   0        0        0    37743 2023-05-08 23:38:57.544713 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-160.py310.1.nbc
+-rw-r--r--   0        0        0     1702 2023-05-08 23:38:57.544713 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-160.py310.nbi
+-rw-r--r--   0        0        0    37857 2023-06-12 19:46:25.688376 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-160.py311.1.nbc
+-rw-r--r--   0        0        0     1702 2023-06-12 19:46:25.688376 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-160.py311.nbi
+-rw-r--r--   0        0        0    38950 2023-04-23 21:13:54.586946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-82.py310.1.nbc
+-rw-r--r--   0        0        0     1604 2023-04-23 21:13:54.586946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-82.py310.nbi
+-rw-r--r--   0        0        0    38984 2023-04-23 22:55:58.985924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-99.py310.1.nbc
+-rw-r--r--   0        0        0     1604 2023-04-23 22:55:58.985924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up-99.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-23 21:13:54.236946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-117.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-23 21:13:54.236946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-117.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-23 22:55:58.635924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-134.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-23 22:55:58.635924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-134.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-23 23:03:51.875813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-153.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-23 23:03:51.875813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-153.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 01:09:31.504082 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-158.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:09:31.504082 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-158.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 01:37:00.940568 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-160.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:37:00.940568 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-160.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 01:46:40.834583 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-168.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:46:40.834583 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-168.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 02:54:22.892531 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-185.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 02:54:22.892531 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-185.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 02:46:27.468130 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-187.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 02:46:27.468130 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-187.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 18:42:17.162934 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-188.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 18:42:17.162934 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-188.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 18:52:46.372664 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-190.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 18:52:46.362664 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-190.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 19:06:09.855087 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-192.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 19:06:09.855087 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-192.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 19:09:01.947747 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-193.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 19:09:01.947747 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-193.py310.nbi
+-rw-r--r--   0        0        0    26394 2023-05-08 23:38:57.174711 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-195.py310.1.nbc
+-rw-r--r--   0        0        0     1706 2023-05-08 23:38:57.174711 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-195.py310.nbi
+-rw-r--r--   0        0        0    26431 2023-06-12 19:46:25.308375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-195.py311.1.nbc
+-rw-r--r--   0        0        0     1706 2023-06-12 19:46:25.308375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_max-195.py311.nbi
+-rw-r--r--   0        0        0    26135 2023-04-23 21:13:54.406946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-105.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-23 21:13:54.406946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-105.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-23 22:55:58.805924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-122.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-23 22:55:58.805924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-122.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-23 23:03:52.055813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-141.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-23 23:03:52.055813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-141.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 01:09:31.694090 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-146.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:09:31.694090 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-146.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 01:37:01.130572 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-148.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:37:01.130572 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-148.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 01:46:41.034587 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-156.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 01:46:41.034587 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-156.py310.nbi
+-rw-r--r--   0        0        0    26135 2023-04-24 02:54:23.072533 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-173.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 02:54:23.072533 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-173.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 02:46:27.608131 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-175.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 02:46:27.608131 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-175.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 18:42:17.352937 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-176.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 18:42:17.352937 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-176.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 18:52:46.512666 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-178.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 18:52:46.512666 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-178.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 19:06:09.995089 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-180.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 19:06:09.995089 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-180.py310.nbi
+-rw-r--r--   0        0        0    26171 2023-04-24 19:09:02.097750 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-181.py310.1.nbc
+-rw-r--r--   0        0        0     1609 2023-04-24 19:09:02.097750 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-181.py310.nbi
+-rw-r--r--   0        0        0    26394 2023-05-08 23:38:57.344712 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-183.py310.1.nbc
+-rw-r--r--   0        0        0     1706 2023-05-08 23:38:57.344712 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-183.py310.nbi
+-rw-r--r--   0        0        0    26431 2023-06-12 19:46:25.488376 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-183.py311.1.nbc
+-rw-r--r--   0        0        0     1706 2023-06-12 19:46:25.488376 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._push_up_min-183.py311.nbi
+-rw-r--r--   0        0        0    35190 2023-04-24 01:27:11.063098 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-208.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 01:27:11.063098 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-208.py310.nbi
+-rw-r--r--   0        0        0    35190 2023-04-24 01:33:22.625090 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-209.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 01:33:22.625090 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-209.py310.nbi
+-rw-r--r--   0        0        0    35190 2023-04-24 01:37:02.330602 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-210.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 01:37:02.330602 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-210.py310.nbi
+-rw-r--r--   0        0        0    35423 2023-04-24 01:46:42.284618 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-218.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 01:46:42.284618 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-218.py310.nbi
+-rw-r--r--   0        0        0    35087 2023-04-23 23:03:53.305813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-223.py310.1.nbc
+-rw-r--r--   0        0        0     1626 2023-04-23 23:03:53.305813 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-223.py310.nbi
+-rw-r--r--   0        0        0    35423 2023-04-24 02:54:24.362545 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-233.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 02:54:24.362545 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-233.py310.nbi
+-rw-r--r--   0        0        0    35416 2023-04-24 02:46:34.038190 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-235.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 02:46:34.038190 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-235.py310.nbi
+-rw-r--r--   0        0        0    35423 2023-04-24 18:42:18.222950 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-236.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 18:42:18.222950 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-236.py310.nbi
+-rw-r--r--   0        0        0    35423 2023-04-24 18:52:47.282678 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-238.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 18:52:47.282678 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-238.py310.nbi
+-rw-r--r--   0        0        0    35423 2023-04-24 19:06:10.735101 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-240.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 19:06:10.735101 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-240.py310.nbi
+-rw-r--r--   0        0        0    35435 2023-04-24 19:09:02.867761 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-241.py310.1.nbc
+-rw-r--r--   0        0        0     1628 2023-04-24 19:09:02.867761 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-241.py310.nbi
+-rw-r--r--   0        0        0    38402 2023-05-08 23:38:58.164716 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-243.py310.1.nbc
+-rw-r--r--   0        0        0     1725 2023-05-08 23:38:58.164716 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-243.py310.nbi
+-rw-r--r--   0        0        0    38417 2023-06-12 19:46:26.378376 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-243.py311.1.nbc
+-rw-r--r--   0        0        0     1725 2023-06-12 19:46:26.378376 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-243.py311.nbi
+-rw-r--r--   0        0        0    35087 2023-04-24 01:09:32.894143 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-252.py310.1.nbc
+-rw-r--r--   0        0        0     1626 2023-04-24 01:09:32.894143 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-252.py310.nbi
+-rw-r--r--   0        0        0    35091 2023-04-24 01:10:54.517690 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-254.py310.1.nbc
+-rw-r--r--   0        0        0     1626 2023-04-24 01:10:54.517690 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap._smallest_child_or_grandchild-254.py310.nbi
+-rw-r--r--   0        0        0     9346 2023-04-23 20:52:29.587122 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.grandparent-68.py310.1.nbc
+-rw-r--r--   0        0        0     1145 2023-04-23 20:52:29.587122 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.grandparent-68.py310.nbi
+-rw-r--r--   0        0        0     9239 2023-04-23 21:10:46.496972 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.parent-63.py310.1.nbc
+-rw-r--r--   0        0        0     1140 2023-04-23 21:10:46.496972 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.parent-63.py310.nbi
+-rw-r--r--   0        0        0     9239 2023-04-23 20:52:29.427122 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.parent-64.py310.1.nbc
+-rw-r--r--   0        0        0     1140 2023-04-23 20:52:29.427122 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.parent-64.py310.nbi
+-rw-r--r--   0        0        0     9239 2023-04-23 21:12:20.836958 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.parent-70.py310.1.nbc
+-rw-r--r--   0        0        0     1140 2023-04-23 21:12:20.836958 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.parent-70.py310.nbi
+-rw-r--r--   0        0        0    23548 2023-04-24 18:52:46.212662 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-102.py310.1.nbc
+-rw-r--r--   0        0        0     1603 2023-04-24 18:52:46.212662 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-102.py310.nbi
+-rw-r--r--   0        0        0    23548 2023-04-24 19:06:09.705085 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-104.py310.1.nbc
+-rw-r--r--   0        0        0     1603 2023-04-24 19:06:09.705085 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-104.py310.nbi
+-rw-r--r--   0        0        0    23548 2023-04-24 19:09:01.807745 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-105.py310.1.nbc
+-rw-r--r--   0        0        0     1603 2023-04-24 19:09:01.807745 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-105.py310.nbi
+-rw-r--r--   0        0        0    24406 2023-05-08 23:38:57.024710 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-107.py310.1.nbc
+-rw-r--r--   0        0        0     1700 2023-05-08 23:38:57.024710 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-107.py310.nbi
+-rw-r--r--   0        0        0    24435 2023-06-12 19:46:25.088375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-107.py311.1.nbc
+-rw-r--r--   0        0        0     1700 2023-06-12 19:46:25.088375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-107.py311.nbi
+-rw-r--r--   0        0        0    23513 2023-04-24 02:54:22.752530 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-115.py310.1.nbc
+-rw-r--r--   0        0        0     1603 2023-04-24 02:54:22.752530 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-115.py310.nbi
+-rw-r--r--   0        0        0    23548 2023-04-24 02:46:27.318129 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-117.py310.1.nbc
+-rw-r--r--   0        0        0     1603 2023-04-24 02:46:27.318129 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-117.py310.nbi
+-rw-r--r--   0        0        0    23548 2023-04-24 18:42:16.982931 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-118.py310.1.nbc
+-rw-r--r--   0        0        0     1603 2023-04-24 18:42:16.982931 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-118.py310.nbi
+-rw-r--r--   0        0        0    23504 2023-04-23 21:10:46.616972 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-53.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-23 21:10:46.616972 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-53.py310.nbi
+-rw-r--r--   0        0        0    23727 2023-04-23 20:52:29.547122 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-54.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-23 20:52:29.547122 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-54.py310.nbi
+-rw-r--r--   0        0        0    23504 2023-04-23 21:13:54.096946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-60.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-23 21:13:54.096946 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-60.py310.nbi
+-rw-r--r--   0        0        0    23504 2023-04-23 22:55:58.495924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-77.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-23 22:55:58.495924 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-77.py310.nbi
+-rw-r--r--   0        0        0    23509 2023-04-24 01:09:31.324074 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-96.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-24 01:09:31.324074 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-96.py310.nbi
+-rw-r--r--   0        0        0    23511 2023-04-24 01:46:40.684579 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-98.py310.1.nbc
+-rw-r--r--   0        0        0     1602 2023-04-24 01:46:40.684579 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/MinMaxHeap.swap-98.py310.nbi
+-rw-r--r--   0        0        0     5186 2022-11-16 00:41:37.633216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-25.py310.1.nbc
+-rw-r--r--   0        0        0     1139 2022-11-16 00:41:37.633216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-25.py310.nbi
+-rw-r--r--   0        0        0     5186 2022-11-20 04:15:08.346262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-25.py39.1.nbc
+-rw-r--r--   0        0        0     1138 2022-11-20 04:15:08.346262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-25.py39.nbi
+-rw-r--r--   0        0        0     5166 2023-05-08 23:38:55.864704 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py310.1.nbc
+-rw-r--r--   0        0        0     1194 2023-05-08 23:38:55.864704 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py310.nbi
+-rw-r--r--   0        0        0     5142 2023-06-12 19:46:23.938374 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py311.1.nbc
+-rw-r--r--   0        0        0     1194 2023-06-12 19:46:23.938374 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py311.nbi
+-rw-r--r--   0        0        0     4393 2022-11-20 17:54:58.506681 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py38.1.nbc
+-rw-r--r--   0        0        0     1062 2022-11-20 17:54:58.506681 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py38.nbi
+-rw-r--r--   0        0        0     5186 2022-11-20 05:08:12.366289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py39.1.nbc
+-rw-r--r--   0        0        0     1138 2022-11-20 05:08:12.366289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-26.py39.nbi
+-rw-r--r--   0        0        0     5186 2023-01-20 23:31:41.287769 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-27.py310.1.nbc
+-rw-r--r--   0        0        0     1139 2023-01-20 23:31:41.287769 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._bound-27.py310.nbi
+-rw-r--r--   0        0        0    10603 2023-05-08 23:38:53.714693 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py310.1.nbc
+-rw-r--r--   0        0        0     1202 2023-05-08 23:38:53.714693 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py310.nbi
+-rw-r--r--   0        0        0    10568 2023-06-12 19:46:21.708372 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py311.1.nbc
+-rw-r--r--   0        0        0     1202 2023-06-12 19:46:21.708372 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py311.nbi
+-rw-r--r--   0        0        0     9458 2022-11-20 17:54:57.596680 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py38.1.nbc
+-rw-r--r--   0        0        0     1070 2022-11-20 17:54:57.596680 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py38.nbi
+-rw-r--r--   0        0        0    10617 2022-11-20 05:08:10.156289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py39.1.nbc
+-rw-r--r--   0        0        0     1146 2022-11-20 05:08:10.156289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-10.py39.nbi
+-rw-r--r--   0        0        0    10601 2023-01-20 23:31:39.237766 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-11.py310.1.nbc
+-rw-r--r--   0        0        0     1147 2023-01-20 23:31:39.237766 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-11.py310.nbi
+-rw-r--r--   0        0        0    10636 2022-11-07 01:40:28.942482 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-7.py310.1.nbc
+-rw-r--r--   0        0        0     1146 2022-11-07 01:40:28.942482 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-7.py310.nbi
+-rw-r--r--   0        0        0    10636 2022-11-16 00:41:33.143216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-9.py310.1.nbc
+-rw-r--r--   0        0        0     1146 2022-11-16 00:41:33.143216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-9.py310.nbi
+-rw-r--r--   0        0        0    10616 2022-11-20 04:15:06.396263 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-9.py39.1.nbc
+-rw-r--r--   0        0        0     1145 2022-11-20 04:15:06.396263 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._nearestPowerOf2-9.py39.nbi
+-rw-r--r--   0        0        0   124060 2022-11-07 01:41:54.772482 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-27.py310.1.nbc
+-rw-r--r--   0        0        0     1484 2022-11-07 01:41:54.772482 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-27.py310.nbi
+-rw-r--r--   0        0        0   101900 2022-11-16 00:41:38.243216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-29.py310.1.nbc
+-rw-r--r--   0        0        0     1513 2022-11-16 00:41:38.243216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-29.py310.nbi
+-rw-r--r--   0        0        0   101838 2022-11-20 04:15:09.056262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-29.py39.1.nbc
+-rw-r--r--   0        0        0     1483 2022-11-20 04:15:09.056262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-29.py39.nbi
+-rw-r--r--   0        0        0   108404 2023-05-08 23:38:56.574708 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py310.1.nbc
+-rw-r--r--   0        0        0     1539 2023-05-08 23:38:56.574708 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py310.nbi
+-rw-r--r--   0        0        0   108331 2023-06-12 19:46:24.658375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py311.1.nbc
+-rw-r--r--   0        0        0     1539 2023-06-12 19:46:24.658375 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py311.nbi
+-rw-r--r--   0        0        0    70215 2022-11-20 17:54:59.046681 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py38.1.nbc
+-rw-r--r--   0        0        0     1407 2022-11-20 17:54:59.046681 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py38.nbi
+-rw-r--r--   0        0        0   101838 2022-11-20 05:08:13.436289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py39.1.nbc
+-rw-r--r--   0        0        0     1483 2022-11-20 05:08:13.436289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-30.py39.nbi
+-rw-r--r--   0        0        0   101843 2023-01-20 23:31:41.977770 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-31.py310.1.nbc
+-rw-r--r--   0        0        0     1484 2023-01-20 23:31:41.977770 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._query-31.py310.nbi
+-rw-r--r--   0        0        0    27213 2022-11-09 01:37:40.483900 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-110.py310.1.nbc
+-rw-r--r--   0        0        0     1250 2022-11-09 01:37:40.483900 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-110.py310.nbi
+-rw-r--r--   0        0        0    27212 2022-11-15 18:06:25.773014 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-124.py310.1.nbc
+-rw-r--r--   0        0        0     1261 2022-11-15 18:06:25.773014 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-124.py310.nbi
+-rw-r--r--   0        0        0    27193 2023-01-20 16:54:53.398669 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-126.py310.1.nbc
+-rw-r--r--   0        0        0     1250 2023-01-20 16:54:53.398669 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-126.py310.nbi
+-rw-r--r--   0        0        0    27217 2022-11-20 04:15:07.586262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-126.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 04:15:07.576262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-126.py39.nbi
+-rw-r--r--   0        0        0    27193 2023-01-20 23:24:35.048947 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-127.py310.1.nbc
+-rw-r--r--   0        0        0     1250 2023-01-20 23:24:35.048947 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-127.py310.nbi
+-rw-r--r--   0        0        0    29957 2023-05-08 23:38:54.944699 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-129.py310.1.nbc
+-rw-r--r--   0        0        0     1305 2023-05-08 23:38:54.944699 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-129.py310.nbi
+-rw-r--r--   0        0        0    29963 2023-06-12 19:46:22.988373 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-129.py311.1.nbc
+-rw-r--r--   0        0        0     1305 2023-06-12 19:46:22.978373 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-129.py311.nbi
+-rw-r--r--   0        0        0    27193 2023-01-20 23:31:40.407768 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-130.py310.1.nbc
+-rw-r--r--   0        0        0     1250 2023-01-20 23:31:40.407768 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-130.py310.nbi
+-rw-r--r--   0        0        0    27201 2022-11-20 04:27:01.436268 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-145.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 04:27:01.436268 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-145.py39.nbi
+-rw-r--r--   0        0        0    27201 2022-11-20 04:30:05.426270 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-146.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 04:30:05.426270 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-146.py39.nbi
+-rw-r--r--   0        0        0    27201 2022-11-20 04:54:25.016282 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-148.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 04:54:25.016282 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-148.py39.nbi
+-rw-r--r--   0        0        0    27201 2022-11-20 04:53:31.896282 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-149.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 04:53:31.896282 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-149.py39.nbi
+-rw-r--r--   0        0        0    27201 2022-11-20 05:08:11.316290 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-151.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 05:08:11.316290 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-151.py39.nbi
+-rw-r--r--   0        0        0    27193 2022-11-20 20:26:54.156758 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-152.py310.1.nbc
+-rw-r--r--   0        0        0     1250 2022-11-20 20:26:54.156758 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-152.py310.nbi
+-rw-r--r--   0        0        0    21516 2022-11-20 17:54:58.296681 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-152.py38.1.nbc
+-rw-r--r--   0        0        0     1173 2022-11-20 17:54:58.296681 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-152.py38.nbi
+-rw-r--r--   0        0        0    27217 2022-11-20 05:01:50.826286 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-152.py39.1.nbc
+-rw-r--r--   0        0        0     1249 2022-11-20 05:01:50.826286 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._safe_invert-152.py39.nbi
+-rw-r--r--   0        0        0    36744 2022-11-07 01:41:05.052482 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-13.py310.1.nbc
+-rw-r--r--   0        0        0     1543 2022-11-07 01:41:05.052482 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-13.py310.nbi
+-rw-r--r--   0        0        0    36794 2022-11-16 00:41:33.773216 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-15.py310.1.nbc
+-rw-r--r--   0        0        0    36841 2022-11-17 23:03:26.284635 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-15.py310.2.nbc
+-rw-r--r--   0        0        0     2564 2022-11-17 23:03:26.284635 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-15.py310.nbi
+-rw-r--r--   0        0        0    36848 2022-11-20 04:15:07.146263 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-15.py39.1.nbc
+-rw-r--r--   0        0        0    36936 2022-11-20 04:15:09.746262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-15.py39.2.nbc
+-rw-r--r--   0        0        0     2533 2022-11-20 04:15:09.746262 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-15.py39.nbi
+-rw-r--r--   0        0        0    36733 2022-11-20 20:26:53.626758 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py310.1.nbc
+-rw-r--r--   0        0        0    36681 2022-11-20 20:26:57.566758 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py310.2.nbc
+-rw-r--r--   0        0        0    36842 2022-11-24 20:59:44.747305 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py310.3.nbc
+-rw-r--r--   0        0        0     3458 2022-11-24 20:59:44.747305 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py310.nbi
+-rw-r--r--   0        0        0    33165 2022-11-20 17:54:58.116680 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py38.1.nbc
+-rw-r--r--   0        0        0    33086 2022-11-20 17:55:00.126680 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py38.2.nbc
+-rw-r--r--   0        0        0     2284 2022-11-20 17:55:00.126680 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py38.nbi
+-rw-r--r--   0        0        0    36848 2022-11-20 05:08:10.886289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py39.1.nbc
+-rw-r--r--   0        0        0    36936 2022-11-20 05:08:14.426289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py39.2.nbc
+-rw-r--r--   0        0        0     2533 2022-11-20 05:08:14.426289 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/SumTree._update-16.py39.nbi
+-rw-r--r--   0        0        0    40460 2021-10-23 22:26:52.435667 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/numpy.padded-24.py38.1.nbc
+-rw-r--r--   0        0        0    41416 2021-10-23 22:26:52.755667 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/numpy.padded-24.py38.2.nbc
+-rw-r--r--   0        0        0    36134 2021-10-23 22:26:53.035667 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/numpy.padded-24.py38.3.nbc
+-rw-r--r--   0        0        0     3280 2021-10-23 22:26:53.035667 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/numpy.padded-24.py38.nbi
+-rw-r--r--   0        0        0    23945 2021-10-23 22:26:52.115667 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/numpy.rotatedSequence-7.py38.1.nbc
+-rw-r--r--   0        0        0     1146 2021-10-23 22:26:52.115667 ReplayTables-andnp-3.1.0/ReplayTables/_utils/__pycache__/numpy.rotatedSequence-7.py38.nbi
+-rw-r--r--   0        0        0     1356 2023-04-23 21:10:14.486976 ReplayTables-andnp-3.1.0/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0       58 2023-04-24 03:51:20.156164 ReplayTables-andnp-3.1.0/ReplayTables/_utils/logger.py
+-rw-r--r--   0        0        0      938 2023-06-18 00:11:46.374786 ReplayTables-andnp-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-06 23:02:12.927133 ReplayTables-andnp-3.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2932 2023-06-13 20:42:17.010244 ReplayTables-andnp-3.1.0/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     3565 2023-06-18 00:11:46.374786 ReplayTables-andnp-3.1.0/tests/test_PER.py
+-rw-r--r--   0        0        0     2095 2023-06-13 20:42:17.010244 ReplayTables-andnp-3.1.0/tests/test_PrioritizedHeap.py
+-rw-r--r--   0        0        0     3707 2023-06-17 22:20:09.963421 ReplayTables-andnp-3.1.0/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1422 2023-06-13 20:42:17.010244 ReplayTables-andnp-3.1.0/tests/test_Table.py
+-rw-r--r--   0        0        0     5453 2023-06-13 20:42:17.010244 ReplayTables-andnp-3.1.0/tests/test_View.py
+-rw-r--r--   0        0        0        0 2022-11-07 18:27:48.972978 ReplayTables-andnp-3.1.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-13 20:42:17.010244 ReplayTables-andnp-3.1.0/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0        0        0     3635 2023-06-13 20:42:17.010244 ReplayTables-andnp-3.1.0/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 ReplayTables-andnp-3.1.0/PKG-INFO
```

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/Distributions.py` & `ReplayTables-andnp-3.1.0/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-3.1.0/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/PER.py` & `ReplayTables-andnp-3.1.0/ReplayTables/PER.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from dataclasses import dataclass
 from typing import cast, Any, Optional, Type
-from ReplayTables.ReplayBuffer import ReplayBufferInterface, EIDS, T
+from ReplayTables.ReplayBuffer import ReplayBufferInterface, EID, EIDS, T
 from ReplayTables.Distributions import MixinUniformDistribution, MixtureDistribution, PrioritizedDistribution, SubDistribution, UniformDistribution
 
 @dataclass
 class PERConfig:
     new_priority_mode: str = 'max'
     uniform_probability: float = 1e-3
     priority_exponent: float = 0.5
@@ -58,7 +58,14 @@
         priorities = priorities ** self._c.priority_exponent
         self._p_dist.update(idxs, priorities)
 
         self._max_priority = max(
             self._c.max_decay * self._max_priority,
             priorities.max(),
         )
+
+    def delete_sample(self, eid: EID):
+        idx = np.array([eid])
+        zero = np.zeros(1)
+
+        self._p_dist.update(idx, zero)
+        self._uniform.update(idx, zero)
```

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/PrioritizedHeap.py` & `ReplayTables-andnp-3.1.0/ReplayTables/PrioritizedHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/ReplayBuffer.py` & `ReplayTables-andnp-3.1.0/ReplayTables/ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/Table.py` & `ReplayTables-andnp-3.1.0/ReplayTables/Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-3.1.0/ReplayTables/_utils/MemoryWriter.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/_utils/MinMaxHeap.py` & `ReplayTables-andnp-3.1.0/ReplayTables/_utils/MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-3.1.0/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-3.1.0/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-3.1.0/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.4/pyproject.toml` & `ReplayTables-andnp-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.4"
+version = "3.1.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -15,22 +15,24 @@
 dev = [
     "mypy",
     "flake8",
     "commitizen",
     "pre-commit",
     "matplotlib",
     "twine",
+    "pytest>=7.3.2",
+    "pytest-benchmark>=4.0.0",
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "3.0.4"
+version = "3.1.0"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.57",
     "numpy>=1.23.5",
```

### Comparing `ReplayTables-andnp-3.0.4/tests/test_LagBuffer.py` & `ReplayTables-andnp-3.1.0/tests/test_LagBuffer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import unittest
 from typing import Any, Optional
 from dataclasses import dataclass
 
 from ReplayTables.LagBuffer import LagBuffer, LaggedExperience
 
 @dataclass
 class Experience:
     s: Any
     a: int
     r: Optional[float]
     gamma: float
     terminal: bool
 
 
-class TestLagBuffer(unittest.TestCase):
+class TestLagBuffer:
     def test_1_step(self):
         buffer = LagBuffer(1)
 
         exp1 = Experience(
             s=3,
             a=0,
             r=None,
@@ -30,113 +29,112 @@
             a=2,
             r=2.0,
             gamma=0,
             terminal=True,
         )
 
         out = list(buffer.add(exp1))
-        self.assertEqual(out, [])
+        assert out == []
 
         out = list(buffer.add(exp2))
-        self.assertEqual(len(out), 1)
-
-        self.assertEqual(out[0], LaggedExperience(
+        assert len(out) == 1
+        assert out[0] == LaggedExperience(
             s=3,
             a=0,
             r=2.,
             gamma=0,
             terminal=True,
             sp=4,
             raw=exp1,
-        ))
+        )
 
     def test_3_step(self):
         buffer = LagBuffer(3)
 
         experiences = []
         for i in range(3):
             exp = Experience(
                 s=1 + i,
                 a=i,
                 r=2.0 * (i + 1),
                 gamma=0.9,
                 terminal=False,
             )
             out = list(buffer.add(exp))
-            self.assertEqual(out, [])
+            assert out == []
 
             experiences.append(exp)
 
         exp = Experience(
             s=4,
             a=22,
             r=8.0,
             gamma=0.9,
             terminal=False,
         )
         out = list(buffer.add(exp))
-        self.assertEqual(len(out), 1)
-        self.assertEqual(out[0], LaggedExperience(
+        assert len(out) == 1
+        assert out[0] == LaggedExperience(
             s=1,
             a=0,
             r=4 + (0.9 * 6) + (0.9 ** 2 * 8),
             gamma=0.9 ** 3,
             terminal=False,
             sp=4,
             raw=experiences[0],
-        ))
+        )
 
         term = Experience(
             s=5,
             a=33,
             r=10.0,
             gamma=0,
             terminal=True,
         )
 
         out = list(buffer.add(term))
-        self.assertEqual(len(out), 3)
+        assert len(out) == 3
 
-        self.assertEqual(out[0], LaggedExperience(
+        assert out[0] == LaggedExperience(
             s=2,
             a=1,
             r=6 + (0.9 * 8) + (0.9 ** 2 * 10),
             gamma=0.,
             terminal=True,
             sp=5,
             raw=experiences[1],
-        ))
+        )
 
-        self.assertEqual(out[1], LaggedExperience(
+        assert out[1] == LaggedExperience(
             s=3,
             a=2,
             r=8 + (0.9 * 10),
             gamma=0,
             terminal=True,
             sp=5,
             raw=experiences[2],
-        ))
+        )
 
-        self.assertEqual(out[2], LaggedExperience(
+        assert out[2] == LaggedExperience(
             s=4,
             a=22,
             r=10,
             gamma=0,
             terminal=True,
             sp=5,
             raw=exp,
-        ))
+        )
 
     def test_flush(self):
         buffer = LagBuffer(lag=1)
 
         buffer.add(Experience(
             s=0,
             a=0,
             r=0,
             gamma=0,
             terminal=True,
         ))
 
-        self.assertEqual(len(buffer._buffer), 1)
+        assert len(buffer._buffer) == 1
         buffer.flush()
-        self.assertEqual(len(buffer._buffer), 0)
+        assert len(buffer._buffer) == 0
```

### Comparing `ReplayTables-andnp-3.0.4/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-3.1.0/tests/test_PER.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,111 +1,130 @@
-import unittest
-import numpy as np
 import pickle
-from dataclasses import dataclass, fields
-from typing import NamedTuple
+import numpy as np
+from typing import cast, NamedTuple
 
-from ReplayTables.ReplayBuffer import ReplayBuffer
+from ReplayTables.ReplayBuffer import EID, EIDS
+from ReplayTables.PER import PrioritizedReplay
 
 class Data(NamedTuple):
-    a: float | np.ndarray
-    b: int | np.ndarray
-
-@dataclass
-class Data2:
-    b: float | np.ndarray
-    c: float | np.ndarray
+    a: float
+    b: int
 
-    def __iter__(self):
-        return (getattr(self, field.name) for field in fields(self))
 
-class TestReplayBuffer(unittest.TestCase):
+class TestPER:
     def test_simple_buffer(self):
         rng = np.random.default_rng(0)
-        buffer = ReplayBuffer(5, Data, rng)
+        buffer = PrioritizedReplay(5, Data, rng)
 
         # on creation, the buffer should have no size
-        self.assertEqual(buffer.size(), 0)
+        assert buffer.size() == 0
 
         # should be able to simply add and sample a single data point
         d = Data(a=0.1, b=1)
         buffer.add(d)
-        self.assertEqual(buffer.size(), 1)
+        assert buffer.size() == 1
         samples, idxs, weights = buffer.sample(10)
-        self.assertTrue(np.all(samples.b == 1))
-        self.assertTrue(np.all(idxs == 0))
-        self.assertTrue(np.all(weights == 1))
+        assert np.all(samples.b == 1)
+        assert np.all(idxs == 0)
+        assert np.all(weights == 0.2)
 
         # should be able to add a few more points
         for i in range(4):
             x = i + 2
             buffer.add(Data(a=x / 10, b=x))
 
-        self.assertEqual(buffer.size(), 5)
+        assert buffer.size() == 5
         samples, idxs, weights = buffer.sample(1000)
 
         unique = np.unique(samples.b)
         unique.sort()
 
-        self.assertTrue(np.all(unique == np.array([1, 2, 3, 4, 5])))
+        assert np.all(unique == np.array([1, 2, 3, 4, 5]))
 
         # buffer drops the oldest element when over max size
         buffer.add(Data(a=0.6, b=6))
-        self.assertEqual(buffer.size(), 5)
+        assert buffer.size() == 5
 
         samples, _, _ = buffer.sample(1000)
         unique = np.unique(samples.b)
         unique.sort()
-        self.assertTrue(np.all(unique == np.array([2, 3, 4, 5, 6])))
-
-        # -------------------------------
-        # Can also handle other iterables
+        assert np.all(unique == np.array([2, 3, 4, 5, 6]))
 
+    def test_priority_on_add(self):
         rng = np.random.default_rng(0)
-        buffer = ReplayBuffer(5, Data2, rng)
-        buffer.add(Data2(1, 2))
-        buffer.add(Data2(2, 3))
+        buffer = PrioritizedReplay(5, Data, rng)
+
+        d = Data(a=0.1, b=1)
+        buffer.add(d, priority=1)
+        d = Data(a=0.2, b=2)
+        buffer.add(d, priority=2)
 
-        samples, _, _ = buffer.sample(2)
-        self.assertTrue(
-            np.all(samples.b == np.array([2, 2]))
-        )
+        batch, _, _ = buffer.sample(128)
 
-    def test_getitem(self):
+        b = np.sum(batch.b == 2)
+        a = np.sum(batch.b == 1)
+
+        assert b == 91
+        assert a == 37
+
+    def test_pickeable(self):
         rng = np.random.default_rng(0)
-        buffer = ReplayBuffer(10, Data, rng)
+        buffer = PrioritizedReplay(5, Data, rng)
+
+        for i in range(5):
+            buffer.add(Data(i, 2 * i))
 
-        for i in range(15):
-            buffer.add(Data(a=i, b=2 * i))
+        ids = cast(EIDS, np.arange(5))
+        buffer.update_priorities(ids, np.arange(5) + 1)
 
-        # should be the most recently added item
-        got, _, _ = buffer[0]
-        expect = Data(a=np.array([14]), b=np.array([28]))
-        self.assertEqual(got, expect)
+        byt = pickle.dumps(buffer)
+        buffer2 = pickle.loads(byt)
 
-        # should be oldest item in buffer
-        got, _, _ = buffer[-1]
-        expect = Data(a=np.array([5]), b=np.array([10]))
-        self.assertEqual(got, expect)
+        s, _, _ = buffer.sample(20)
+        s2, _, _ = buffer2.sample(20)
 
-        got, _, _ = buffer[2:7:2]
-        expect = Data(
-            a=np.array([12, 10, 8]),
-            b=np.array([24, 20, 16]),
-        )
-        self.assertTrue(np.all(got.a == expect.a))
-        self.assertTrue(np.all(got.b == expect.b))
+        assert np.all(s.a == s2.a) and np.all(s.b == s2.b)
 
-    def test_pickleable(self):
+    def test_delete_sample(self):
         rng = np.random.default_rng(0)
-        buffer = ReplayBuffer(5, Data, rng)
+        buffer = PrioritizedReplay(5, Data, rng)
 
-        for i in range(8):
-            buffer.add(Data(a=i, b=i))
+        for i in range(5):
+            buffer.add(Data(i, 2 * i))
 
-        byt = pickle.dumps(buffer)
-        buffer2 = pickle.loads(byt)
+        batch, _, _, = buffer.sample(512)
+        assert np.unique(batch.a).shape == (5,)
+
+        buffer.delete_sample(cast(EID, 2))
+        batch, _, _ = buffer.sample(512)
+        assert np.unique(batch.a).shape == (4,)
+        assert 2 not in batch.a
+
+# ----------------
+# -- Benchmarks --
+# ----------------
+class TestBenchmarks:
+    def test_per_add(self, benchmark):
+        rng = np.random.default_rng(0)
+        buffer = PrioritizedReplay(100_000, Data, rng)
+        d = Data(a=0.1, b=1)
+
+        for i in range(100_000):
+            buffer.add(d, priority=2 * i + 1)
+
+        def _inner(buffer: PrioritizedReplay, d: Data):
+            buffer.add(d, priority=1)
+
+        benchmark(_inner, buffer, d)
+
+    def test_per_sample(self, benchmark):
+        rng = np.random.default_rng(0)
+        buffer = PrioritizedReplay(100_000, Data, rng)
+        d = Data(a=0.1, b=1)
+
+        for i in range(100_000):
+            buffer.add(d, priority=2 * i + 1)
 
-        s, _, _ = buffer.sample(3)
-        s2, _, _ = buffer2.sample(3)
+        def _inner(buffer: PrioritizedReplay):
+            buffer.sample(32)
 
-        self.assertTrue(np.all(s.a == s2.a) and np.all(s.b == s2.b))
+        benchmark(_inner, buffer)
```

### Comparing `ReplayTables-andnp-3.0.4/tests/test_Table.py` & `ReplayTables-andnp-3.1.0/tests/test_Table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import unittest
 import numpy as np
 
 from ReplayTables.Table import Table
 
-class TestTable(unittest.TestCase):
+class TestTable:
     def test_canAddMultipleColumns(self):
         table = Table(3, seed=0, columns=[
             { 'name': 'A', 'shape': 3 },
             { 'name': 'B', 'shape': 1, 'dtype': bool },
             { 'name': 'C', 'shape': tuple(), 'dtype': 'int32' },
         ])
 
@@ -15,37 +14,37 @@
         table.addTuple((np.arange(3) * 2.2, False, 2))
         table.addTuple((np.arange(3) * 3.3, True, 3))
         table.addTuple((np.arange(3) * 4.4, True, 4))
         table.addTuple((np.arange(3) * 5.5, False, 5))
 
         A, B, C = table.getAll()
 
-        self.assertTrue(np.allclose(A, np.array([
+        assert np.allclose(A, [
             [0, 3.3, 6.6],
             [0, 4.4, 8.8],
             [0, 5.5, 11],
-        ])))
+        ])
 
-        self.assertTrue(np.all(B == [[True], [True], [False]]))
+        assert np.all(B == [[True], [True], [False]])
 
-        self.assertTrue(np.allclose(C, [3, 4, 5]))
+        assert np.allclose(C, [3, 4, 5])
 
     def test_canSampleTable(self):
         table = Table(3, seed=1, columns=[
             { 'name': 'A', 'shape': 3 },
             { 'name': 'B', 'shape': tuple()},
         ])
 
         for i in range(8):
             table.addTuple((np.arange(3) * i, i**2))
 
         A, B = table.sample()
-        self.assertTrue(np.allclose(A, [[0, 6, 12]]))
-        self.assertTrue(np.allclose(B, [36]))
+        assert np.allclose(A, [[0, 6, 12]])
+        assert np.allclose(B, [36])
 
         A, B = table.sample(3)
-        self.assertTrue(np.allclose(A, [
+        assert np.allclose(A, [
             [0, 5, 10],
             [0, 6, 12],
             [0, 7, 14],
-        ]))
-        self.assertTrue(np.allclose(B, [25, 36, 49]))
+        ])
+        assert np.allclose(B, [25, 36, 49])
```

### Comparing `ReplayTables-andnp-3.0.4/tests/test_View.py` & `ReplayTables-andnp-3.1.0/tests/test_View.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import unittest
+import pytest
 import numpy as np
 
 from ReplayTables.Table import Table, View
 
-class TestView(unittest.TestCase):
+class TestView:
     def test_getAllSequences(self):
         table = Table(7, seed=0, columns=[
             { 'name': 'A', 'shape': 3 },
             { 'name': 'B', 'shape': 1, 'dtype': bool },
             { 'name': 'C', 'shape': tuple(), 'dtype': 'int32' },
         ])
 
@@ -15,34 +15,35 @@
         view = View(table, 3)
 
         for i in range(20):
             table.addTuple((np.arange(3) * i, i % 3 == 0, i))
 
         A, B, C = view.getAll()
 
-        self.assertEqual(A.shape, (7, 3, 3))
-        self.assertEqual(B.shape, (7, 3, 1))
-        self.assertEqual(C.shape, (7, 3))
+        assert A.shape == (7, 3, 3)
+        assert B.shape == (7, 3, 1)
+        assert C.shape == (7, 3)
 
-        self.assertTrue(np.allclose(C, [
+        assert np.allclose(C, [
             # n_t, n_{t+1}, n_{t+2}
             [13, 14, 15],
             [14, 15, 16],
             [15, 16, 17],
             [16, 17, 18],
             [17, 18, 19],
             # importantly, the last bits of the sequence will be incomplete
             # these are padded with np.nan for floats and 0 for ints (by default, configurable)
             [18, 19, 0 ],
             [19, 0, 0 ],
-        ]))
+        ])
 
         # if we try to add a view to a table that already has data
         # that is undefined behavior and so through an error
-        self.assertRaises(Exception, lambda: View(table, 4))
+        with pytest.raises(Exception):
+            View(table, 4)
 
     def test_customPad(self):
         table = Table(7, seed=0, columns=[
             { 'name': 'A', 'shape': 3 },
             { 'name': 'B', 'shape': 1, 'dtype': bool },
             { 'name': 'C', 'shape': tuple(), 'dtype': 'int32', 'pad': -22 },
         ])
@@ -51,27 +52,27 @@
         view = View(table, 3)
 
         for i in range(20):
             table.addTuple((np.arange(3) * i, i % 3 == 0, i))
 
         A, B, C = view.getAll()
 
-        self.assertEqual(A.shape, (7, 3, 3))
-        self.assertEqual(B.shape, (7, 3, 1))
-        self.assertEqual(C.shape, (7, 3))
+        assert A.shape, (7, 3, 3)
+        assert B.shape, (7, 3, 1)
+        assert C.shape, (7, 3)
 
-        self.assertTrue(np.allclose(C, [
+        assert np.allclose(C, [
             [13, 14, 15],
             [14, 15, 16],
             [15, 16, 17],
             [16, 17, 18],
             [17, 18, 19],
             [18, 19, -22],
             [19, -22, -22],
-        ]))
+        ])
 
     def test_endSequence(self):
         # if a sequence terminates during the stream
         # e.g. if an episode terminates during an RL stream of experience
         # then the view should also treat this as sequence termination
 
         table = Table(7, seed=0, columns=[
@@ -88,34 +89,34 @@
             table.addTuple((np.arange(3) * i, i % 3 == 0, i))
 
             # each sequence is of length 4
             if i % 4 == 3:
                 table.endTrajectory()
 
         A, B, C = view3.getAll()
-        self.assertTrue(np.allclose(C, [
+        assert np.allclose(C, [
             [13, 14, 15],
             [14, 15, 0],
             [15, 0, 0],
             [16, 17, 18],
             [17, 18, 19],
             [18, 19, 0],
             [19, 0, 0],
-        ]))
+        ])
 
         A, B, C = view5.getAll()
-        self.assertTrue(np.allclose(C, [
+        assert np.allclose(C, [
             [13, 14, 15, 0, 0],
             [14, 15, 0, 0, 0],
             [15, 0, 0, 0, 0],
             [16, 17, 18, 19, 0],
             [17, 18, 19, 0, 0],
             [18, 19, 0, 0, 0],
             [19, 0, 0, 0, 0],
-        ]))
+        ])
 
     def test_sample(self):
         table = Table(7, seed=0, columns=[
             { 'name': 'A', 'shape': 3 },
             { 'name': 'B', 'shape': 1, 'dtype': bool },
             { 'name': 'C', 'shape': tuple(), 'dtype': 'int32' },
         ])
@@ -133,25 +134,25 @@
 
         # lots of numbers, here's what happened
         # an ER buffer with the 7 most recent elements
         # a stream of length 20 was observed, there were terminations every 4 samples
         # we collected trajectories of length 3 (i.e. 3-step trajectories)
         # now I want 2 of those trajectories sampled at random
         A, B, C = view3.sample(2)
-        self.assertTrue(np.allclose(C, [
+        assert np.allclose(C, [
             [17, 18, 19],
             [15, 0, 0],
-        ]))
+        ])
 
         A, B, C = view5.sample(3)
-        self.assertTrue(np.allclose(C, [
+        assert np.allclose(C, [
             [15, 0, 0, 0, 0],
             [16, 17, 18, 19, 0],
             [15, 0, 0, 0, 0],
-        ]))
+        ])
 
     def test_getLastComplete(self):
         table = Table(7, seed=0, columns=[
             { 'name': 'A', 'shape': 3 },
             { 'name': 'B', 'shape': 1, 'dtype': bool },
             { 'name': 'C', 'shape': tuple(), 'dtype': 'int32' },
         ])
@@ -165,14 +166,14 @@
 
             # each sequence is of length 4
             if i % 4 == 3:
                 table.endTrajectory()
 
         # this should be the last *complete* trajectory
         A, B, C = view3.getLastComplete()
-        self.assertTrue(np.allclose(C, [17, 18, 19]))
+        assert np.allclose(C, [17, 18, 19])
 
         A, B, C = view5.getLastComplete()
-        self.assertTrue(np.allclose(C, [16, 17, 18, 19, 0]))
+        assert np.allclose(C, [16, 17, 18, 19, 0])
 
         A, B, C = view5.getLastComplete(offset=1)
-        self.assertTrue(np.allclose(C, [17, 18, 19, 0, 0]))
+        assert np.allclose(C, [17, 18, 19, 0, 0])
```

