# Comparing `tmp/litie-0.0.4.tar.gz` & `tmp/litie-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litie-0.0.4.tar", last modified: Sun Jun 18 15:57:51 2023, max compression
+gzip compressed data, was "litie-1.0.1.tar", last modified: Sun Jun 18 16:05:16 2023, max compression
```

## Comparing `litie-0.0.4.tar` & `litie-1.0.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:51.036101 litie-0.0.4/
--rw-rw-rw-   0        0        0    10854 2023-06-12 13:46:58.000000 litie-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    22798 2023-06-18 15:57:51.035101 litie-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    22501 2023-06-15 12:21:55.000000 litie-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.846607 litie-0.0.4/litie/
--rw-rw-rw-   0        0        0       23 2023-06-13 13:33:13.000000 litie-0.0.4/litie/__about__.py
--rw-rw-rw-   0        0        0        0 2023-06-13 13:33:13.000000 litie-0.0.4/litie/__init__.py
--rw-rw-rw-   0        0        0     8729 2023-06-15 12:21:27.000000 litie-0.0.4/litie/arguments.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.854587 litie-0.0.4/litie/callbacks/
--rw-rw-rw-   0        0        0       82 2023-06-15 12:21:27.000000 litie-0.0.4/litie/callbacks/__init__.py
--rw-rw-rw-   0        0        0     2926 2023-06-15 12:21:27.000000 litie-0.0.4/litie/callbacks/adversarial.py
--rw-rw-rw-   0        0        0     1085 2023-06-15 11:34:55.000000 litie-0.0.4/litie/callbacks/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.861570 litie-0.0.4/litie/datasets/
--rw-rw-rw-   0        0        0      149 2023-06-16 14:35:08.000000 litie-0.0.4/litie/datasets/__init__.py
--rw-rw-rw-   0        0        0     8016 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.867558 litie-0.0.4/litie/datasets/ee/
--rw-rw-rw-   0        0        0      271 2023-06-16 11:00:22.000000 litie-0.0.4/litie/datasets/ee/__init__.py
--rw-rw-rw-   0        0        0     8622 2023-06-18 12:01:23.000000 litie-0.0.4/litie/datasets/ee/base.py
--rw-rw-rw-   0        0        0     3057 2023-06-18 05:00:47.000000 litie-0.0.4/litie/datasets/ee/gplinker.py
--rw-rw-rw-   0        0        0      566 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/iterable.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.888493 litie-0.0.4/litie/datasets/ner/
--rw-rw-rw-   0        0        0     1400 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/__init__.py
--rw-rw-rw-   0        0        0     7503 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/base.py
--rw-rw-rw-   0        0        0     4975 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/cnn.py
--rw-rw-rw-   0        0        0     4637 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/crf.py
--rw-rw-rw-   0        0        0     2913 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/global_pointer.py
--rw-rw-rw-   0        0        0     3189 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/lear.py
--rw-rw-rw-   0        0        0     6845 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/mrc.py
--rw-rw-rw-   0        0        0     1998 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/span.py
--rw-rw-rw-   0        0        0     2165 2023-06-13 13:33:13.000000 litie-0.0.4/litie/datasets/ner/tplinker.py
--rw-rw-rw-   0        0        0     9529 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/ner/w2ner.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.903454 litie-0.0.4/litie/datasets/re/
--rw-rw-rw-   0        0        0     1206 2023-06-15 14:25:21.000000 litie-0.0.4/litie/datasets/re/__init__.py
--rw-rw-rw-   0        0        0     8646 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/base.py
--rw-rw-rw-   0        0        0     2976 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/casrel.py
--rw-rw-rw-   0        0        0     2661 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/gplinker.py
--rw-rw-rw-   0        0        0     3215 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/grte.py
--rw-rw-rw-   0        0        0     2240 2023-06-15 14:24:51.000000 litie-0.0.4/litie/datasets/re/onerel.py
--rw-rw-rw-   0        0        0     2482 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/pfn.py
--rw-rw-rw-   0        0        0     4444 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/prgc.py
--rw-rw-rw-   0        0        0     2332 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/spn.py
--rw-rw-rw-   0        0        0     2690 2023-06-13 13:33:14.000000 litie-0.0.4/litie/datasets/re/tplinker.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.909442 litie-0.0.4/litie/datasets/uie/
--rw-rw-rw-   0        0        0       92 2023-06-13 16:27:09.000000 litie-0.0.4/litie/datasets/uie/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-13 16:26:56.000000 litie-0.0.4/litie/datasets/uie/data.py
--rw-rw-rw-   0        0        0     7871 2023-06-13 16:21:18.000000 litie-0.0.4/litie/datasets/uie/doccano.py
--rw-rw-rw-   0        0        0    21781 2023-06-13 16:23:51.000000 litie-0.0.4/litie/datasets/uie/utils.py
--rw-rw-rw-   0        0        0     7575 2023-06-18 15:55:39.000000 litie-0.0.4/litie/datasets/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.919412 litie-0.0.4/litie/engines/
--rw-rw-rw-   0        0        0      151 2023-06-16 14:33:25.000000 litie-0.0.4/litie/engines/__init__.py
--rw-rw-rw-   0        0        0    14877 2023-06-17 12:04:10.000000 litie-0.0.4/litie/engines/base.py
--rw-rw-rw-   0        0        0     4351 2023-06-16 14:32:54.000000 litie-0.0.4/litie/engines/ee.py
--rw-rw-rw-   0        0        0     4084 2023-06-15 12:21:27.000000 litie-0.0.4/litie/engines/ner.py
--rw-rw-rw-   0        0        0     4108 2023-06-15 12:21:27.000000 litie-0.0.4/litie/engines/re.py
--rw-rw-rw-   0        0        0     1837 2023-06-15 12:21:27.000000 litie-0.0.4/litie/engines/uie.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.941352 litie-0.0.4/litie/layers/
--rw-rw-rw-   0        0        0      771 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/__init__.py
--rw-rw-rw-   0        0        0     2930 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/conv.py
--rw-rw-rw-   0        0        0    20163 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/crf.py
--rw-rw-rw-   0        0        0     1719 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/dropouts.py
--rw-rw-rw-   0        0        0    13250 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/global_pointer.py
--rw-rw-rw-   0        0        0     3605 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/layer_norm.py
--rw-rw-rw-   0        0        0     2462 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/lear.py
--rw-rw-rw-   0        0        0     6918 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/pfn.py
--rw-rw-rw-   0        0        0     6790 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/pooling.py
--rw-rw-rw-   0        0        0     7142 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/position.py
--rw-rw-rw-   0        0        0     4364 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/set_decoder.py
--rw-rw-rw-   0        0        0     3209 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/transformer.py
--rw-rw-rw-   0        0        0      146 2023-06-13 13:33:14.000000 litie-0.0.4/litie/layers/utils.py
--rw-rw-rw-   0        0        0    23626 2023-06-13 14:50:53.000000 litie-0.0.4/litie/losses.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.944346 litie-0.0.4/litie/metrics/
--rw-rw-rw-   0        0        0       95 2023-06-16 14:28:24.000000 litie-0.0.4/litie/metrics/__init__.py
--rw-rw-rw-   0        0        0      319 2023-06-13 13:33:14.000000 litie-0.0.4/litie/metrics/base.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.948333 litie-0.0.4/litie/metrics/extraction/
--rw-rw-rw-   0        0        0       33 2023-06-13 13:33:14.000000 litie-0.0.4/litie/metrics/extraction/__init__.py
--rw-rw-rw-   0        0        0     2138 2023-06-18 04:21:44.000000 litie-0.0.4/litie/metrics/extraction/precision_recall_fscore.py
--rw-rw-rw-   0        0        0     1865 2023-06-16 13:04:36.000000 litie-0.0.4/litie/metrics/extraction/score.py
--rw-rw-rw-   0        0        0     6352 2023-06-13 13:33:14.000000 litie-0.0.4/litie/metrics/extraction/span.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.955315 litie-0.0.4/litie/models/
--rw-rw-rw-   0        0        0      151 2023-06-16 14:38:13.000000 litie-0.0.4/litie/models/__init__.py
--rw-rw-rw-   0        0        0     4580 2023-06-18 11:38:24.000000 litie-0.0.4/litie/models/base.py
--rw-rw-rw-   0        0        0     2224 2023-06-17 05:41:59.000000 litie-0.0.4/litie/models/ee.py
--rw-rw-rw-   0        0        0     2172 2023-06-15 12:21:27.000000 litie-0.0.4/litie/models/ner.py
--rw-rw-rw-   0        0        0     2178 2023-06-15 12:21:27.000000 litie-0.0.4/litie/models/re.py
--rw-rw-rw-   0        0        0     1868 2023-06-13 16:45:34.000000 litie-0.0.4/litie/models/uie.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.959308 litie-0.0.4/litie/nn/
--rw-rw-rw-   0        0        0      224 2023-06-15 15:46:07.000000 litie-0.0.4/litie/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.965290 litie-0.0.4/litie/nn/chinese_bert/
--rw-rw-rw-   0        0        0      342 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/chinese_bert/__init__.py
--rw-rw-rw-   0        0        0     5399 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/chinese_bert/configuration_chinese_bert.py
--rw-rw-rw-   0        0        0    29685 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/chinese_bert/modeling_chinese_bert.py
--rw-rw-rw-   0        0        0     1710 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/chinese_bert/tokenization_chinesebert_fast.py
--rw-rw-rw-   0        0        0     3155 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/decode_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.968312 litie-0.0.4/litie/nn/ee/
--rw-rw-rw-   0        0        0      729 2023-06-15 15:46:07.000000 litie-0.0.4/litie/nn/ee/__init__.py
--rw-rw-rw-   0        0        0     8896 2023-06-18 04:20:43.000000 litie-0.0.4/litie/nn/ee/gplinker.py
--rw-rw-rw-   0        0        0     2839 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.979251 litie-0.0.4/litie/nn/ner/
--rw-rw-rw-   0        0        0     2703 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/__init__.py
--rw-rw-rw-   0        0        0    12856 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/cnn.py
--rw-rw-rw-   0        0        0    15930 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/crf.py
--rw-rw-rw-   0        0        0     7318 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/global_pointer.py
--rw-rw-rw-   0        0        0     9715 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/lear.py
--rw-rw-rw-   0        0        0     7262 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/mrc.py
--rw-rw-rw-   0        0        0     5440 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/span.py
--rw-rw-rw-   0        0        0     6612 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/tplinker.py
--rw-rw-rw-   0        0        0    11773 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/ner/w2ner.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.994212 litie-0.0.4/litie/nn/re/
--rw-rw-rw-   0        0        0     2161 2023-06-15 13:57:04.000000 litie-0.0.4/litie/nn/re/__init__.py
--rw-rw-rw-   0        0        0    11034 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/casrel.py
--rw-rw-rw-   0        0        0     7837 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/gplinker.py
--rw-rw-rw-   0        0        0     9001 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/grte.py
--rw-rw-rw-   0        0        0     6994 2023-06-15 13:54:49.000000 litie-0.0.4/litie/nn/re/onerel.py
--rw-rw-rw-   0        0        0     7342 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/pfn.py
--rw-rw-rw-   0        0        0    14301 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/prgc.py
--rw-rw-rw-   0        0        0     9936 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/spn.py
--rw-rw-rw-   0        0        0     9637 2023-06-15 12:21:27.000000 litie-0.0.4/litie/nn/re/tplinker.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.999199 litie-0.0.4/litie/nn/roformer/
--rw-rw-rw-   0        0        0      434 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/roformer/__init__.py
--rw-rw-rw-   0        0        0     8143 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/roformer/configuration_roformer.py
--rw-rw-rw-   0        0        0    79700 2023-06-13 13:33:14.000000 litie-0.0.4/litie/nn/roformer/modeling_roformer.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:51.006186 litie-0.0.4/litie/nn/uie/
--rw-rw-rw-   0        0        0       74 2023-06-13 16:31:51.000000 litie-0.0.4/litie/nn/uie/__init__.py
--rw-rw-rw-   0        0        0    15989 2023-06-13 16:31:51.000000 litie-0.0.4/litie/nn/uie/convert.py
--rw-rw-rw-   0        0        0     9031 2023-06-13 16:31:51.000000 litie-0.0.4/litie/nn/uie/model.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:51.018147 litie-0.0.4/litie/pipelines/
--rw-rw-rw-   0        0        0      145 2023-06-16 14:29:12.000000 litie-0.0.4/litie/pipelines/__init__.py
--rw-rw-rw-   0        0        0     3234 2023-06-13 13:33:14.000000 litie-0.0.4/litie/pipelines/base.py
--rw-rw-rw-   0        0        0     5163 2023-06-18 15:44:54.000000 litie-0.0.4/litie/pipelines/ee.py
--rw-rw-rw-   0        0        0    16323 2023-06-13 13:33:14.000000 litie-0.0.4/litie/pipelines/ner.py
--rw-rw-rw-   0        0        0     6337 2023-06-13 13:33:14.000000 litie-0.0.4/litie/pipelines/re.py
--rw-rw-rw-   0        0        0    19411 2023-06-14 14:13:28.000000 litie-0.0.4/litie/pipelines/uie.py
--rw-rw-rw-   0        0        0     2862 2023-06-13 13:33:14.000000 litie-0.0.4/litie/pipelines/utils.py
--rw-rw-rw-   0        0        0      659 2023-06-13 13:33:14.000000 litie-0.0.4/litie/registry.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:51.024133 litie-0.0.4/litie/ui/
--rw-rw-rw-   0        0        0       78 2023-06-13 13:33:14.000000 litie-0.0.4/litie/ui/__init__.py
--rw-rw-rw-   0        0        0     3334 2023-06-14 14:13:28.000000 litie-0.0.4/litie/ui/ner.py
--rw-rw-rw-   0        0        0     3246 2023-06-13 13:33:14.000000 litie-0.0.4/litie/ui/re.py
--rw-rw-rw-   0        0        0     1294 2023-06-13 13:33:14.000000 litie-0.0.4/litie/ui/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:51.033108 litie-0.0.4/litie/utils/
--rw-rw-rw-   0        0        0        0 2023-06-13 13:33:14.000000 litie-0.0.4/litie/utils/__init__.py
--rw-rw-rw-   0        0        0     4654 2023-06-13 13:33:14.000000 litie-0.0.4/litie/utils/common.py
--rw-rw-rw-   0        0        0      609 2023-06-13 13:33:14.000000 litie-0.0.4/litie/utils/deepspeed.py
--rw-rw-rw-   0        0        0     7558 2023-06-13 13:33:14.000000 litie-0.0.4/litie/utils/download.py
--rw-rw-rw-   0        0        0      476 2023-06-13 13:33:14.000000 litie-0.0.4/litie/utils/imports.py
--rw-rw-rw-   0        0        0     3899 2023-06-13 13:33:14.000000 litie-0.0.4/litie/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-18 15:57:50.851594 litie-0.0.4/litie.egg-info/
--rw-rw-rw-   0        0        0    22798 2023-06-18 15:57:50.000000 litie-0.0.4/litie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3249 2023-06-18 15:57:50.000000 litie-0.0.4/litie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 15:57:50.000000 litie-0.0.4/litie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2023-06-18 15:57:50.000000 litie-0.0.4/litie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 15:57:50.000000 litie-0.0.4/litie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 15:57:51.036101 litie-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-06-18 15:56:29.000000 litie-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.866268 litie-1.0.1/
+-rw-rw-rw-   0        0        0    10854 2023-06-12 13:46:58.000000 litie-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    22798 2023-06-18 16:05:16.865271 litie-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    22501 2023-06-15 12:21:55.000000 litie-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.685937 litie-1.0.1/litie/
+-rw-rw-rw-   0        0        0       23 2023-06-13 13:33:13.000000 litie-1.0.1/litie/__about__.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:33:13.000000 litie-1.0.1/litie/__init__.py
+-rw-rw-rw-   0        0        0     8729 2023-06-15 12:21:27.000000 litie-1.0.1/litie/arguments.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.695911 litie-1.0.1/litie/callbacks/
+-rw-rw-rw-   0        0        0       82 2023-06-15 12:21:27.000000 litie-1.0.1/litie/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     2926 2023-06-15 12:21:27.000000 litie-1.0.1/litie/callbacks/adversarial.py
+-rw-rw-rw-   0        0        0     1085 2023-06-15 11:34:55.000000 litie-1.0.1/litie/callbacks/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.704894 litie-1.0.1/litie/datasets/
+-rw-rw-rw-   0        0        0      149 2023-06-16 14:35:08.000000 litie-1.0.1/litie/datasets/__init__.py
+-rw-rw-rw-   0        0        0     8016 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.709876 litie-1.0.1/litie/datasets/ee/
+-rw-rw-rw-   0        0        0      271 2023-06-16 11:00:22.000000 litie-1.0.1/litie/datasets/ee/__init__.py
+-rw-rw-rw-   0        0        0     8622 2023-06-18 12:01:23.000000 litie-1.0.1/litie/datasets/ee/base.py
+-rw-rw-rw-   0        0        0     3057 2023-06-18 05:00:47.000000 litie-1.0.1/litie/datasets/ee/gplinker.py
+-rw-rw-rw-   0        0        0      566 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/iterable.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.723836 litie-1.0.1/litie/datasets/ner/
+-rw-rw-rw-   0        0        0     1400 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/__init__.py
+-rw-rw-rw-   0        0        0     7503 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/base.py
+-rw-rw-rw-   0        0        0     4975 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/cnn.py
+-rw-rw-rw-   0        0        0     4637 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/crf.py
+-rw-rw-rw-   0        0        0     2913 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/global_pointer.py
+-rw-rw-rw-   0        0        0     3189 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/lear.py
+-rw-rw-rw-   0        0        0     6845 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/mrc.py
+-rw-rw-rw-   0        0        0     1998 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/span.py
+-rw-rw-rw-   0        0        0     2165 2023-06-13 13:33:13.000000 litie-1.0.1/litie/datasets/ner/tplinker.py
+-rw-rw-rw-   0        0        0     9529 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/ner/w2ner.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.741792 litie-1.0.1/litie/datasets/re/
+-rw-rw-rw-   0        0        0     1206 2023-06-15 14:25:21.000000 litie-1.0.1/litie/datasets/re/__init__.py
+-rw-rw-rw-   0        0        0     8646 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/base.py
+-rw-rw-rw-   0        0        0     2976 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/casrel.py
+-rw-rw-rw-   0        0        0     2661 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/gplinker.py
+-rw-rw-rw-   0        0        0     3215 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/grte.py
+-rw-rw-rw-   0        0        0     2240 2023-06-15 14:24:51.000000 litie-1.0.1/litie/datasets/re/onerel.py
+-rw-rw-rw-   0        0        0     2482 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/pfn.py
+-rw-rw-rw-   0        0        0     4444 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/prgc.py
+-rw-rw-rw-   0        0        0     2332 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/spn.py
+-rw-rw-rw-   0        0        0     2690 2023-06-13 13:33:14.000000 litie-1.0.1/litie/datasets/re/tplinker.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.748770 litie-1.0.1/litie/datasets/uie/
+-rw-rw-rw-   0        0        0       92 2023-06-13 16:27:09.000000 litie-1.0.1/litie/datasets/uie/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-13 16:26:56.000000 litie-1.0.1/litie/datasets/uie/data.py
+-rw-rw-rw-   0        0        0     7871 2023-06-13 16:21:18.000000 litie-1.0.1/litie/datasets/uie/doccano.py
+-rw-rw-rw-   0        0        0    21781 2023-06-13 16:23:51.000000 litie-1.0.1/litie/datasets/uie/utils.py
+-rw-rw-rw-   0        0        0     7580 2023-06-18 16:02:48.000000 litie-1.0.1/litie/datasets/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.756753 litie-1.0.1/litie/engines/
+-rw-rw-rw-   0        0        0      151 2023-06-16 14:33:25.000000 litie-1.0.1/litie/engines/__init__.py
+-rw-rw-rw-   0        0        0    14877 2023-06-17 12:04:10.000000 litie-1.0.1/litie/engines/base.py
+-rw-rw-rw-   0        0        0     4351 2023-06-16 14:32:54.000000 litie-1.0.1/litie/engines/ee.py
+-rw-rw-rw-   0        0        0     4084 2023-06-15 12:21:27.000000 litie-1.0.1/litie/engines/ner.py
+-rw-rw-rw-   0        0        0     4108 2023-06-15 12:21:27.000000 litie-1.0.1/litie/engines/re.py
+-rw-rw-rw-   0        0        0     1837 2023-06-15 12:21:27.000000 litie-1.0.1/litie/engines/uie.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.778402 litie-1.0.1/litie/layers/
+-rw-rw-rw-   0        0        0      771 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/__init__.py
+-rw-rw-rw-   0        0        0     2930 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/conv.py
+-rw-rw-rw-   0        0        0    20163 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/crf.py
+-rw-rw-rw-   0        0        0     1719 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/dropouts.py
+-rw-rw-rw-   0        0        0    13250 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/global_pointer.py
+-rw-rw-rw-   0        0        0     3605 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/layer_norm.py
+-rw-rw-rw-   0        0        0     2462 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/lear.py
+-rw-rw-rw-   0        0        0     6918 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/pfn.py
+-rw-rw-rw-   0        0        0     6790 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/pooling.py
+-rw-rw-rw-   0        0        0     7142 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/position.py
+-rw-rw-rw-   0        0        0     4364 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/set_decoder.py
+-rw-rw-rw-   0        0        0     3209 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/transformer.py
+-rw-rw-rw-   0        0        0      146 2023-06-13 13:33:14.000000 litie-1.0.1/litie/layers/utils.py
+-rw-rw-rw-   0        0        0    23626 2023-06-13 14:50:53.000000 litie-1.0.1/litie/losses.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.781392 litie-1.0.1/litie/metrics/
+-rw-rw-rw-   0        0        0       95 2023-06-16 14:28:24.000000 litie-1.0.1/litie/metrics/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-06-13 13:33:14.000000 litie-1.0.1/litie/metrics/base.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.786378 litie-1.0.1/litie/metrics/extraction/
+-rw-rw-rw-   0        0        0       33 2023-06-13 13:33:14.000000 litie-1.0.1/litie/metrics/extraction/__init__.py
+-rw-rw-rw-   0        0        0     2138 2023-06-18 04:21:44.000000 litie-1.0.1/litie/metrics/extraction/precision_recall_fscore.py
+-rw-rw-rw-   0        0        0     1865 2023-06-16 13:04:36.000000 litie-1.0.1/litie/metrics/extraction/score.py
+-rw-rw-rw-   0        0        0     6352 2023-06-13 13:33:14.000000 litie-1.0.1/litie/metrics/extraction/span.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.793358 litie-1.0.1/litie/models/
+-rw-rw-rw-   0        0        0      151 2023-06-16 14:38:13.000000 litie-1.0.1/litie/models/__init__.py
+-rw-rw-rw-   0        0        0     4580 2023-06-18 11:38:24.000000 litie-1.0.1/litie/models/base.py
+-rw-rw-rw-   0        0        0     2224 2023-06-17 05:41:59.000000 litie-1.0.1/litie/models/ee.py
+-rw-rw-rw-   0        0        0     2172 2023-06-15 12:21:27.000000 litie-1.0.1/litie/models/ner.py
+-rw-rw-rw-   0        0        0     2178 2023-06-15 12:21:27.000000 litie-1.0.1/litie/models/re.py
+-rw-rw-rw-   0        0        0     1868 2023-06-13 16:45:34.000000 litie-1.0.1/litie/models/uie.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.797349 litie-1.0.1/litie/nn/
+-rw-rw-rw-   0        0        0      224 2023-06-15 15:46:07.000000 litie-1.0.1/litie/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.801337 litie-1.0.1/litie/nn/chinese_bert/
+-rw-rw-rw-   0        0        0      342 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/chinese_bert/__init__.py
+-rw-rw-rw-   0        0        0     5399 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/chinese_bert/configuration_chinese_bert.py
+-rw-rw-rw-   0        0        0    29685 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/chinese_bert/modeling_chinese_bert.py
+-rw-rw-rw-   0        0        0     1710 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/chinese_bert/tokenization_chinesebert_fast.py
+-rw-rw-rw-   0        0        0     3155 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/decode_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.804331 litie-1.0.1/litie/nn/ee/
+-rw-rw-rw-   0        0        0      729 2023-06-15 15:46:07.000000 litie-1.0.1/litie/nn/ee/__init__.py
+-rw-rw-rw-   0        0        0     8896 2023-06-18 04:20:43.000000 litie-1.0.1/litie/nn/ee/gplinker.py
+-rw-rw-rw-   0        0        0     2839 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/model_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.818366 litie-1.0.1/litie/nn/ner/
+-rw-rw-rw-   0        0        0     2703 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/__init__.py
+-rw-rw-rw-   0        0        0    12856 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/cnn.py
+-rw-rw-rw-   0        0        0    15930 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/crf.py
+-rw-rw-rw-   0        0        0     7318 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/global_pointer.py
+-rw-rw-rw-   0        0        0     9715 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/lear.py
+-rw-rw-rw-   0        0        0     7262 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/mrc.py
+-rw-rw-rw-   0        0        0     5440 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/span.py
+-rw-rw-rw-   0        0        0     6612 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/tplinker.py
+-rw-rw-rw-   0        0        0    11773 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/ner/w2ner.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.836319 litie-1.0.1/litie/nn/re/
+-rw-rw-rw-   0        0        0     2161 2023-06-15 13:57:04.000000 litie-1.0.1/litie/nn/re/__init__.py
+-rw-rw-rw-   0        0        0    11034 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/casrel.py
+-rw-rw-rw-   0        0        0     7837 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/gplinker.py
+-rw-rw-rw-   0        0        0     9001 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/grte.py
+-rw-rw-rw-   0        0        0     6994 2023-06-15 13:54:49.000000 litie-1.0.1/litie/nn/re/onerel.py
+-rw-rw-rw-   0        0        0     7342 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/pfn.py
+-rw-rw-rw-   0        0        0    14301 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/prgc.py
+-rw-rw-rw-   0        0        0     9936 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/spn.py
+-rw-rw-rw-   0        0        0     9637 2023-06-15 12:21:27.000000 litie-1.0.1/litie/nn/re/tplinker.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.840338 litie-1.0.1/litie/nn/roformer/
+-rw-rw-rw-   0        0        0      434 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/roformer/__init__.py
+-rw-rw-rw-   0        0        0     8143 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/roformer/configuration_roformer.py
+-rw-rw-rw-   0        0        0    79700 2023-06-13 13:33:14.000000 litie-1.0.1/litie/nn/roformer/modeling_roformer.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.843329 litie-1.0.1/litie/nn/uie/
+-rw-rw-rw-   0        0        0       74 2023-06-13 16:31:51.000000 litie-1.0.1/litie/nn/uie/__init__.py
+-rw-rw-rw-   0        0        0    15989 2023-06-13 16:31:51.000000 litie-1.0.1/litie/nn/uie/convert.py
+-rw-rw-rw-   0        0        0     9031 2023-06-13 16:31:51.000000 litie-1.0.1/litie/nn/uie/model.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.852307 litie-1.0.1/litie/pipelines/
+-rw-rw-rw-   0        0        0      145 2023-06-16 14:29:12.000000 litie-1.0.1/litie/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     3234 2023-06-13 13:33:14.000000 litie-1.0.1/litie/pipelines/base.py
+-rw-rw-rw-   0        0        0     5163 2023-06-18 15:44:54.000000 litie-1.0.1/litie/pipelines/ee.py
+-rw-rw-rw-   0        0        0    16323 2023-06-13 13:33:14.000000 litie-1.0.1/litie/pipelines/ner.py
+-rw-rw-rw-   0        0        0     6337 2023-06-13 13:33:14.000000 litie-1.0.1/litie/pipelines/re.py
+-rw-rw-rw-   0        0        0    19411 2023-06-14 14:13:28.000000 litie-1.0.1/litie/pipelines/uie.py
+-rw-rw-rw-   0        0        0     2862 2023-06-13 13:33:14.000000 litie-1.0.1/litie/pipelines/utils.py
+-rw-rw-rw-   0        0        0      659 2023-06-13 13:33:14.000000 litie-1.0.1/litie/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.857293 litie-1.0.1/litie/ui/
+-rw-rw-rw-   0        0        0       78 2023-06-13 13:33:14.000000 litie-1.0.1/litie/ui/__init__.py
+-rw-rw-rw-   0        0        0     3334 2023-06-14 14:13:28.000000 litie-1.0.1/litie/ui/ner.py
+-rw-rw-rw-   0        0        0     3246 2023-06-13 13:33:14.000000 litie-1.0.1/litie/ui/re.py
+-rw-rw-rw-   0        0        0     1294 2023-06-13 13:33:14.000000 litie-1.0.1/litie/ui/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.864274 litie-1.0.1/litie/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:33:14.000000 litie-1.0.1/litie/utils/__init__.py
+-rw-rw-rw-   0        0        0     4654 2023-06-13 13:33:14.000000 litie-1.0.1/litie/utils/common.py
+-rw-rw-rw-   0        0        0      609 2023-06-13 13:33:14.000000 litie-1.0.1/litie/utils/deepspeed.py
+-rw-rw-rw-   0        0        0     7558 2023-06-13 13:33:14.000000 litie-1.0.1/litie/utils/download.py
+-rw-rw-rw-   0        0        0      476 2023-06-13 13:33:14.000000 litie-1.0.1/litie/utils/imports.py
+-rw-rw-rw-   0        0        0     3899 2023-06-13 13:33:14.000000 litie-1.0.1/litie/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:16.691921 litie-1.0.1/litie.egg-info/
+-rw-rw-rw-   0        0        0    22798 2023-06-18 16:05:16.000000 litie-1.0.1/litie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3249 2023-06-18 16:05:16.000000 litie-1.0.1/litie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:05:16.000000 litie-1.0.1/litie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      151 2023-06-18 16:05:16.000000 litie-1.0.1/litie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 16:05:16.000000 litie-1.0.1/litie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:05:16.866268 litie-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-06-18 16:03:43.000000 litie-1.0.1/setup.py
```

### Comparing `litie-0.0.4/LICENSE` & `litie-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/PKG-INFO` & `litie-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litie
-Version: 0.0.4
+Version: 1.0.1
 Summary: Pytorch-lightning Code Blocks for NER and RE
 Home-page: https://github.com/xusenlinzy/lit-ie
 Author: xusenlin
 Author-email: 1659821119@qq.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: litie Version: 0.0.4 Summary: Pytorch-lightning
+Metadata-Version: 2.1 Name: litie Version: 1.0.1 Summary: Pytorch-lightning
 Code Blocks for NER and RE Home-page: https://github.com/xusenlinzy/lit-ie
 Author: xusenlin Author-email: 1659821119@qq.com Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # Lit-IE
      [https://img.shields.io/github/license/xusenlinzy/lit-ner] [https://
    img.shields.io/badge/python-3.8+-aff.svg] [https://img.shields.io/badge/
 pytorch-%3E=1.12-red?logo=pytorch] [https://img.shields.io/github/last-commit/
    xusenlinzy/lit-ner] [https://img.shields.io/github/issues/xusenlinzy/lit-
```

### Comparing `litie-0.0.4/README.md` & `litie-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/arguments.py` & `litie-1.0.1/litie/arguments.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/callbacks/adversarial.py` & `litie-1.0.1/litie/callbacks/adversarial.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/callbacks/logger.py` & `litie-1.0.1/litie/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/base.py` & `litie-1.0.1/litie/datasets/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ee/base.py` & `litie-1.0.1/litie/datasets/ee/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ee/gplinker.py` & `litie-1.0.1/litie/datasets/ee/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/iterable.py` & `litie-1.0.1/litie/datasets/iterable.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/__init__.py` & `litie-1.0.1/litie/datasets/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/base.py` & `litie-1.0.1/litie/datasets/ner/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/cnn.py` & `litie-1.0.1/litie/datasets/ner/cnn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/crf.py` & `litie-1.0.1/litie/datasets/ner/crf.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/global_pointer.py` & `litie-1.0.1/litie/datasets/ner/global_pointer.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/lear.py` & `litie-1.0.1/litie/datasets/ner/lear.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/mrc.py` & `litie-1.0.1/litie/datasets/ner/mrc.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/span.py` & `litie-1.0.1/litie/datasets/ner/span.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/tplinker.py` & `litie-1.0.1/litie/datasets/ner/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/ner/w2ner.py` & `litie-1.0.1/litie/datasets/ner/w2ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/__init__.py` & `litie-1.0.1/litie/datasets/re/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/base.py` & `litie-1.0.1/litie/datasets/re/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/casrel.py` & `litie-1.0.1/litie/datasets/re/casrel.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/gplinker.py` & `litie-1.0.1/litie/datasets/re/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/grte.py` & `litie-1.0.1/litie/datasets/re/grte.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/onerel.py` & `litie-1.0.1/litie/datasets/re/onerel.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/pfn.py` & `litie-1.0.1/litie/datasets/re/pfn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/prgc.py` & `litie-1.0.1/litie/datasets/re/prgc.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/spn.py` & `litie-1.0.1/litie/datasets/re/spn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/re/tplinker.py` & `litie-1.0.1/litie/datasets/re/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/uie/data.py` & `litie-1.0.1/litie/datasets/uie/data.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/uie/doccano.py` & `litie-1.0.1/litie/datasets/uie/doccano.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/uie/utils.py` & `litie-1.0.1/litie/datasets/uie/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/datasets/utils.py` & `litie-1.0.1/litie/datasets/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,12 +201,12 @@
 
 
 def batchify_ee_labels(batch, features, return_offset_mapping=False):
     """ 事件抽取验证集标签处理 """
     if "text" in features[0].keys():
         batch["texts"] = [feature.pop("text") for feature in features]
     if "target" in features[0].keys():
-        batch['target'] = [[[tuple([a[0], a[1], a[2], int(a[3]), a[4]]) for a in e] for e in feature.pop("target")] for feature in features]
+        batch['target'] = [[[tuple([a[0], a[1], a[2], int(a[3]), int(a[4])]) for a in e] for e in feature.pop("target")] for feature in features]
     if return_offset_mapping and "offset_mapping" in features[0].keys():
         batch["offset_mapping"] = [feature.pop("offset_mapping") for feature in features]
 
     return batch
```

### Comparing `litie-0.0.4/litie/engines/base.py` & `litie-1.0.1/litie/engines/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/engines/ee.py` & `litie-1.0.1/litie/engines/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/engines/ner.py` & `litie-1.0.1/litie/engines/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/engines/re.py` & `litie-1.0.1/litie/engines/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/engines/uie.py` & `litie-1.0.1/litie/engines/uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/__init__.py` & `litie-1.0.1/litie/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/conv.py` & `litie-1.0.1/litie/layers/conv.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/crf.py` & `litie-1.0.1/litie/layers/crf.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/dropouts.py` & `litie-1.0.1/litie/layers/dropouts.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/global_pointer.py` & `litie-1.0.1/litie/layers/global_pointer.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/layer_norm.py` & `litie-1.0.1/litie/layers/layer_norm.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/lear.py` & `litie-1.0.1/litie/layers/lear.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/pfn.py` & `litie-1.0.1/litie/layers/pfn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/pooling.py` & `litie-1.0.1/litie/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/position.py` & `litie-1.0.1/litie/layers/position.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/set_decoder.py` & `litie-1.0.1/litie/layers/set_decoder.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/layers/transformer.py` & `litie-1.0.1/litie/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/losses.py` & `litie-1.0.1/litie/losses.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/metrics/extraction/precision_recall_fscore.py` & `litie-1.0.1/litie/metrics/extraction/precision_recall_fscore.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/metrics/extraction/score.py` & `litie-1.0.1/litie/metrics/extraction/score.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/metrics/extraction/span.py` & `litie-1.0.1/litie/metrics/extraction/span.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/models/base.py` & `litie-1.0.1/litie/models/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/models/ee.py` & `litie-1.0.1/litie/models/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/models/ner.py` & `litie-1.0.1/litie/models/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/models/re.py` & `litie-1.0.1/litie/models/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/models/uie.py` & `litie-1.0.1/litie/models/uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/chinese_bert/configuration_chinese_bert.py` & `litie-1.0.1/litie/nn/chinese_bert/configuration_chinese_bert.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/chinese_bert/modeling_chinese_bert.py` & `litie-1.0.1/litie/nn/chinese_bert/modeling_chinese_bert.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/chinese_bert/tokenization_chinesebert_fast.py` & `litie-1.0.1/litie/nn/chinese_bert/tokenization_chinesebert_fast.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/decode_utils.py` & `litie-1.0.1/litie/nn/decode_utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ee/__init__.py` & `litie-1.0.1/litie/nn/ee/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ee/gplinker.py` & `litie-1.0.1/litie/nn/ee/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/model_utils.py` & `litie-1.0.1/litie/nn/model_utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/__init__.py` & `litie-1.0.1/litie/nn/ner/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/cnn.py` & `litie-1.0.1/litie/nn/ner/cnn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/crf.py` & `litie-1.0.1/litie/nn/ner/crf.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/global_pointer.py` & `litie-1.0.1/litie/nn/ner/global_pointer.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/lear.py` & `litie-1.0.1/litie/nn/ner/lear.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/mrc.py` & `litie-1.0.1/litie/nn/ner/mrc.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/span.py` & `litie-1.0.1/litie/nn/ner/span.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/tplinker.py` & `litie-1.0.1/litie/nn/ner/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/ner/w2ner.py` & `litie-1.0.1/litie/nn/ner/w2ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/__init__.py` & `litie-1.0.1/litie/nn/re/__init__.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/casrel.py` & `litie-1.0.1/litie/nn/re/casrel.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/gplinker.py` & `litie-1.0.1/litie/nn/re/gplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/grte.py` & `litie-1.0.1/litie/nn/re/grte.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/onerel.py` & `litie-1.0.1/litie/nn/re/onerel.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/pfn.py` & `litie-1.0.1/litie/nn/re/pfn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/prgc.py` & `litie-1.0.1/litie/nn/re/prgc.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/spn.py` & `litie-1.0.1/litie/nn/re/spn.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/re/tplinker.py` & `litie-1.0.1/litie/nn/re/tplinker.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/roformer/configuration_roformer.py` & `litie-1.0.1/litie/nn/roformer/configuration_roformer.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/roformer/modeling_roformer.py` & `litie-1.0.1/litie/nn/roformer/modeling_roformer.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/uie/convert.py` & `litie-1.0.1/litie/nn/uie/convert.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/nn/uie/model.py` & `litie-1.0.1/litie/nn/uie/model.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/pipelines/base.py` & `litie-1.0.1/litie/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/pipelines/ee.py` & `litie-1.0.1/litie/pipelines/ee.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/pipelines/ner.py` & `litie-1.0.1/litie/pipelines/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/pipelines/re.py` & `litie-1.0.1/litie/pipelines/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/pipelines/uie.py` & `litie-1.0.1/litie/pipelines/uie.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/pipelines/utils.py` & `litie-1.0.1/litie/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/registry.py` & `litie-1.0.1/litie/registry.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/ui/ner.py` & `litie-1.0.1/litie/ui/ner.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/ui/re.py` & `litie-1.0.1/litie/ui/re.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/ui/utils.py` & `litie-1.0.1/litie/ui/utils.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/utils/common.py` & `litie-1.0.1/litie/utils/common.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/utils/deepspeed.py` & `litie-1.0.1/litie/utils/deepspeed.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/utils/download.py` & `litie-1.0.1/litie/utils/download.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie/utils/logger.py` & `litie-1.0.1/litie/utils/logger.py`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/litie.egg-info/PKG-INFO` & `litie-1.0.1/litie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litie
-Version: 0.0.4
+Version: 1.0.1
 Summary: Pytorch-lightning Code Blocks for NER and RE
 Home-page: https://github.com/xusenlinzy/lit-ie
 Author: xusenlin
 Author-email: 1659821119@qq.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: litie Version: 0.0.4 Summary: Pytorch-lightning
+Metadata-Version: 2.1 Name: litie Version: 1.0.1 Summary: Pytorch-lightning
 Code Blocks for NER and RE Home-page: https://github.com/xusenlinzy/lit-ie
 Author: xusenlin Author-email: 1659821119@qq.com Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # Lit-IE
      [https://img.shields.io/github/license/xusenlinzy/lit-ner] [https://
    img.shields.io/badge/python-3.8+-aff.svg] [https://img.shields.io/badge/
 pytorch-%3E=1.12-red?logo=pytorch] [https://img.shields.io/github/last-commit/
    xusenlinzy/lit-ner] [https://img.shields.io/github/issues/xusenlinzy/lit-
```

### Comparing `litie-0.0.4/litie.egg-info/SOURCES.txt` & `litie-1.0.1/litie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litie-0.0.4/setup.py` & `litie-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "torchmetrics",
     "transformers",
 ]
 
 
 setup(
     name="litie",
-    version="0.0.4",
+    version="1.0.1",
     description="Pytorch-lightning Code Blocks for NER and RE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xusenlinzy/lit-ie",
     author="xusenlin",
     author_email="1659821119@qq.com",
     ikeywords=["deep learning", "pytorch", "AI"],
```

