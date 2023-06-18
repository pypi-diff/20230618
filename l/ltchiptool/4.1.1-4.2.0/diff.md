# Comparing `tmp/ltchiptool-4.1.1.tar.gz` & `tmp/ltchiptool-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool-4.1.1.tar", max compression
+gzip compressed data, was "ltchiptool-4.2.0.tar", max compression
```

## Comparing `ltchiptool-4.1.1.tar` & `ltchiptool-4.2.0.tar`

### file list

```diff
@@ -1,101 +1,119 @@
--rw-r--r--   0        0        0     1076 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/LICENSE
--rw-r--r--   0        0        0     2384 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/README.md
--rw-r--r--   0        0        0      376 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/ltchiptool/__init__.py
--rw-r--r--   0        0        0     2339 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/ltchiptool/__main__.py
--rw-r--r--   0        0        0     2517 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/dumptool.py
--rw-r--r--   0        0        0      908 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/elf2bin.py
--rw-r--r--   0        0        0      451 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/__main__.py
--rw-r--r--   0        0        0     1724 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/_utils.py
--rw-r--r--   0        0        0     1610 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/file.py
--rw-r--r--   0        0        0     3157 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/read.py
--rw-r--r--   0        0        0     7153 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/write.py
--rw-r--r--   0        0        0      881 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/link2bin.py
--rw-r--r--   0        0        0     2331 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/list.py
--rw-r--r--   0        0        0      423 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/soc.py
--rw-r--r--   0        0        0     2288 2023-05-15 18:28:43.810202 ltchiptool-4.1.1/ltchiptool/families.json
--rw-r--r--   0        0        0      127 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/__init__.py
--rw-r--r--   0        0        0     1459 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/__main__.py
--rw-r--r--   0        0        0     9477 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool-192x192.png
--rw-r--r--   0        0        0    15406 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.ico
--rw-r--r--   0        0        0    26033 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.wxui
--rw-r--r--   0        0        0    32878 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.xrc
--rw-r--r--   0        0        0     6613 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/main.py
--rw-r--r--   0        0        0       48 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/__init__.py
--rw-r--r--   0        0        0     2017 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/about.py
--rw-r--r--   0        0        0     4453 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/base.py
--rw-r--r--   0        0        0    17255 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/flash.py
--rw-r--r--   0        0        0     6995 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/log.py
--rw-r--r--   0        0        0    11834 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/upk.py
--rw-r--r--   0        0        0      789 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/utils.py
--rw-r--r--   0        0        0       47 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/__init__.py
--rw-r--r--   0        0        0      950 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/base.py
--rw-r--r--   0        0        0     6027 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/flash.py
--rw-r--r--   0        0        0     2528 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/ports.py
--rw-r--r--   0        0        0     4824 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/upk.py
--rw-r--r--   0        0        0      263 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/board.py
--rw-r--r--   0        0        0      155 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/enums.py
--rw-r--r--   0        0        0     5966 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/family.py
--rw-r--r--   0        0        0     3199 2023-05-15 18:28:43.810202 ltchiptool-4.1.1/ltchiptool/platform.json
--rw-r--r--   0        0        0      185 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/__init__.py
--rw-r--r--   0        0        0      111 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/__init__.py
--rw-r--r--   0        0        0     6198 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/binary.py
--rw-r--r--   0        0        0     6871 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/flash.py
--rw-r--r--   0        0        0      721 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/main.py
--rw-r--r--   0        0        0       48 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/util/__init__.py
--rw-r--r--   0        0        0    18071 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/util/rtltool.py
--rw-r--r--   0        0        0      114 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/flash.py
--rw-r--r--   0        0        0      595 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/main.py
--rw-r--r--   0        0        0       49 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/util/__init__.py
--rw-r--r--   0        0        0    13040 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/util/ambz2tool.py
--rw-r--r--   0        0        0      111 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/__init__.py
--rw-r--r--   0        0        0     9025 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/binary.py
--rw-r--r--   0        0        0     8305 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/bkpackager.py
--rw-r--r--   0        0        0     6820 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/flash.py
--rw-r--r--   0        0        0      723 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/main.py
--rw-r--r--   0        0        0      317 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/binary.py
--rw-r--r--   0        0        0     6175 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/crypto.py
--rw-r--r--   0        0        0      515 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/models.py
--rw-r--r--   0        0        0     2940 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/rbl.py
--rw-r--r--   0        0        0     2827 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/common.py
--rw-r--r--   0        0        0     6478 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/interface.py
--rw-r--r--   0        0        0       48 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/__init__.py
--rw-r--r--   0        0        0     2408 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/bitint.py
--rw-r--r--   0        0        0     2727 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/cli.py
--rw-r--r--   0        0        0     5642 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/crc16.py
--rw-r--r--   0        0        0     2277 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/crypto.py
--rw-r--r--   0        0        0     6631 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/detection.py
--rw-r--r--   0        0        0     1987 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/dict.py
--rw-r--r--   0        0        0      252 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/env.py
--rw-r--r--   0        0        0     2420 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/fileio.py
--rw-r--r--   0        0        0     3591 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/flash.py
--rw-r--r--   0        0        0     3296 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/fwbinary.py
--rw-r--r--   0        0        0     6105 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/intbin.py
--rw-r--r--   0        0        0     4845 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/logging.py
--rw-r--r--   0        0        0     7308 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/lvm.py
--rw-r--r--   0        0        0     1401 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/misc.py
--rw-r--r--   0        0        0     1878 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/obj.py
--rw-r--r--   0        0        0      866 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/slice.py
--rw-r--r--   0        0        0     1612 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/toolchain.py
--rw-r--r--   0        0        0      772 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/version.py
--rw-r--r--   0        0        0     1322 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/__init__.py
--rw-r--r--   0        0        0      251 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/__init__.py
--rw-r--r--   0        0        0      471 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/apply.py
--rw-r--r--   0        0        0     1027 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/bindiff.py
--rw-r--r--   0        0        0     1666 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/diff32.py
--rw-r--r--   0        0        0     4306 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/cli.py
--rw-r--r--   0        0        0      360 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/block.py
--rw-r--r--   0        0        0     5803 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/context.py
--rw-r--r--   0        0        0     2210 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/enums.py
--rw-r--r--   0        0        0     1256 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/flags.py
--rw-r--r--   0        0        0     3311 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/image.py
--rw-r--r--   0        0        0      778 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/partition.py
--rw-r--r--   0        0        0     4552 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/uf2.py
--rw-r--r--   0        0        0      124 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/upload/__init__.py
--rw-r--r--   0        0        0     4846 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/upload/esphome.py
--rw-r--r--   0        0        0     7219 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/writer.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 ltchiptool-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/LICENSE
+-rw-r--r--   0        0        0     2384 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/README.md
+-rw-r--r--   0        0        0      376 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/__init__.py
+-rw-r--r--   0        0        0     2769 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/__main__.py
+-rw-r--r--   0        0        0      908 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/compile/elf2bin.py
+-rw-r--r--   0        0        0      881 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/compile/link2bin.py
+-rw-r--r--   0        0        0      502 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/__main__.py
+-rw-r--r--   0        0        0     1724 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/_utils.py
+-rw-r--r--   0        0        0     1610 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/file.py
+-rw-r--r--   0        0        0     3192 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/read.py
+-rw-r--r--   0        0        0     2442 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/split.py
+-rw-r--r--   0        0        0     7188 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/write.py
+-rw-r--r--   0        0        0     2331 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/list.py
+-rw-r--r--   0        0        0     3833 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/plugin/manage.py
+-rw-r--r--   0        0        0     1022 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/plugin/run.py
+-rw-r--r--   0        0        0      423 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/soc.py
+-rw-r--r--   0        0        0     2022 2023-06-18 15:43:28.866084 ltchiptool-4.2.0/ltchiptool/families.json
+-rw-r--r--   0        0        0      127 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/__main__.py
+-rw-r--r--   0        0        0     5990 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/colors.json
+-rw-r--r--   0        0        0     3964 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/colors.py
+-rw-r--r--   0        0        0     9477 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool-192x192.png
+-rw-r--r--   0        0        0    15406 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.ico
+-rw-r--r--   0        0        0    17134 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.wxui
+-rw-r--r--   0        0        0    21898 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.xrc
+-rw-r--r--   0        0        0    10596 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/main.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/about.py
+-rw-r--r--   0        0        0     5807 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/base.py
+-rw-r--r--   0        0        0    17297 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/flash.py
+-rw-r--r--   0        0        0     6885 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/log.py
+-rw-r--r--   0        0        0    12398 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/plugins.py
+-rw-r--r--   0        0        0     1405 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/utils.py
+-rw-r--r--   0        0        0       47 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/base.py
+-rw-r--r--   0        0        0     6041 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/flash.py
+-rw-r--r--   0        0        0      798 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/plugins.py
+-rw-r--r--   0        0        0     2528 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/ports.py
+-rw-r--r--   0        0        0      263 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/models/__init__.py
+-rw-r--r--   0        0        0     3144 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/models/board.py
+-rw-r--r--   0        0        0      155 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/models/enums.py
+-rw-r--r--   0        0        0     5966 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/models/family.py
+-rw-r--r--   0        0        0     3199 2023-06-18 15:43:28.866084 ltchiptool-4.2.0/ltchiptool/platform.json
+-rw-r--r--   0        0        0      185 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/__init__.py
+-rw-r--r--   0        0        0     6198 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/binary.py
+-rw-r--r--   0        0        0     6959 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/flash.py
+-rw-r--r--   0        0        0      721 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/main.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/util/__init__.py
+-rw-r--r--   0        0        0    18071 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/util/rtltool.py
+-rw-r--r--   0        0        0      114 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/__init__.py
+-rw-r--r--   0        0        0     7749 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/binary.py
+-rw-r--r--   0        0        0     4791 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/flash.py
+-rw-r--r--   0        0        0      648 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/main.py
+-rw-r--r--   0        0        0     7691 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/parse_partition.py
+-rw-r--r--   0        0        0       49 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/__init__.py
+-rw-r--r--   0        0        0    17029 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/ambz2tool.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/__init__.py
+-rw-r--r--   0        0        0     1993 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/config.py
+-rw-r--r--   0        0        0     1036 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/enums.py
+-rw-r--r--   0        0        0     3188 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/headers.py
+-rw-r--r--   0        0        0     5129 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/images.py
+-rw-r--r--   0        0        0     4642 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/partitions.py
+-rw-r--r--   0        0        0      619 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/utils.py
+-rw-r--r--   0        0        0      111 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/__init__.py
+-rw-r--r--   0        0        0     9025 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/binary.py
+-rw-r--r--   0        0        0     8305 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/bkpackager.py
+-rw-r--r--   0        0        0     6855 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/flash.py
+-rw-r--r--   0        0        0      723 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/main.py
+-rw-r--r--   0        0        0      317 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/__init__.py
+-rw-r--r--   0        0        0     7069 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/binary.py
+-rw-r--r--   0        0        0     6175 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/crypto.py
+-rw-r--r--   0        0        0      515 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/models.py
+-rw-r--r--   0        0        0     2940 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/rbl.py
+-rw-r--r--   0        0        0     2843 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/common.py
+-rw-r--r--   0        0        0     6513 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/interface.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/bitint.py
+-rw-r--r--   0        0        0     3393 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/cli.py
+-rw-r--r--   0        0        0     5642 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/crc16.py
+-rw-r--r--   0        0        0     2277 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/crypto.py
+-rw-r--r--   0        0        0     4441 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/curve25519.py
+-rw-r--r--   0        0        0     6631 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/detection.py
+-rw-r--r--   0        0        0     1987 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/dict.py
+-rw-r--r--   0        0        0      252 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/env.py
+-rw-r--r--   0        0        0     2661 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/fileio.py
+-rw-r--r--   0        0        0     1746 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/flash.py
+-rw-r--r--   0        0        0     3296 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/fwbinary.py
+-rw-r--r--   0        0        0     6105 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/intbin.py
+-rw-r--r--   0        0        0     5164 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/logging.py
+-rw-r--r--   0        0        0     6332 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/lpm.py
+-rw-r--r--   0        0        0     7308 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/lvm.py
+-rw-r--r--   0        0        0     2670 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/misc.py
+-rw-r--r--   0        0        0     1878 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/obj.py
+-rw-r--r--   0        0        0      866 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/slice.py
+-rw-r--r--   0        0        0     5747 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/streams.py
+-rw-r--r--   0        0        0     1612 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/toolchain.py
+-rw-r--r--   0        0        0      772 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/version.py
+-rw-r--r--   0        0        0      154 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltctplugin/base/__init__.py
+-rw-r--r--   0        0        0     4431 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltctplugin/base/base.py
+-rw-r--r--   0        0        0     1338 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/__init__.py
+-rw-r--r--   0        0        0      251 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/__init__.py
+-rw-r--r--   0        0        0      471 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/apply.py
+-rw-r--r--   0        0        0     1027 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/bindiff.py
+-rw-r--r--   0        0        0     1666 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/diff32.py
+-rw-r--r--   0        0        0     4306 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/cli.py
+-rw-r--r--   0        0        0      360 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/block.py
+-rw-r--r--   0        0        0     5803 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/context.py
+-rw-r--r--   0        0        0     2210 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/enums.py
+-rw-r--r--   0        0        0     1256 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/flags.py
+-rw-r--r--   0        0        0     3311 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/image.py
+-rw-r--r--   0        0        0      772 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/partition.py
+-rw-r--r--   0        0        0     4552 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/uf2.py
+-rw-r--r--   0        0        0      124 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/upload/__init__.py
+-rw-r--r--   0        0        0     4846 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/upload/esphome.py
+-rw-r--r--   0        0        0     7219 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/writer.py
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 ltchiptool-4.2.0/PKG-INFO
```

### Comparing `ltchiptool-4.1.1/LICENSE` & `ltchiptool-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/README.md` & `ltchiptool-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/__main__.py` & `ltchiptool-4.2.0/ltchiptool/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # Copyright (c) Kuba Szczodrzyński 2022-07-29.
 
 import os
 from logging import DEBUG, INFO
 
 import click
 from click import Context
+from serial import Serial
 
 from ltchiptool.util.cli import get_multi_command_class
 from ltchiptool.util.logging import VERBOSE, LoggingHandler, log_setup_click_bars
+from ltchiptool.util.streams import LoggingStreamHook
 
 from .version import get_version
 
 COMMANDS = {
-    "dump": "ltchiptool/commands/dumptool.py",
-    "elf2bin": "ltchiptool/commands/elf2bin.py",
+    # compile commands
+    "elf2bin": "ltchiptool/commands/compile/elf2bin.py",
+    "link2bin": "ltchiptool/commands/compile/link2bin.py",
+    "uf2": "uf2tool/cli.py",
+    # flash commands
     "flash": "ltchiptool/commands/flash/__main__.py",
+    # plugin commands
+    "plugin": "ltchiptool/commands/plugin/run.py",
+    "plugins": "ltchiptool/commands/plugin/manage.py",
+    # other commands
     "gui": "ltchiptool/gui/__main__.py",
-    "link2bin": "ltchiptool/commands/link2bin.py",
     "list": "ltchiptool/commands/list.py",
     "soc": "ltchiptool/commands/soc.py",
-    "uf2": "uf2tool/cli.py",
 }
 
 VERBOSITY_LEVEL = {
     0: INFO,
     1: DEBUG,
     2: VERBOSE,
 }
@@ -61,39 +68,47 @@
 @click.option(
     "-i",
     "--indent",
     help="Indent log messages using graph lines",
     type=int,
     default=0,
 )
+@click.option(
+    "-s",
+    "--dump-serial",
+    help="Dump transmitted Serial data",
+    is_flag=True,
+)
 @click.version_option(
     get_version(),
     "-V",
     "--version",
     message="ltchiptool v%(version)s",
 )
 @click.pass_context
 def cli_entrypoint(
     ctx: Context,
     verbose: int,
     traceback: bool,
     timed: bool,
     raw_log: bool,
     indent: int,
+    dump_serial: bool,
 ):
     ctx.ensure_object(dict)
     if verbose == 0 and "LTCHIPTOOL_VERBOSE" in os.environ:
         verbose = int(os.environ["LTCHIPTOOL_VERBOSE"])
     logger = LoggingHandler.get()
     logger.level = VERBOSITY_LEVEL[min(verbose, 2)]
     logger.timed = timed
     logger.raw = raw_log
     logger.indent = indent
     logger.full_traceback = traceback
     log_setup_click_bars()
+    LoggingStreamHook.set_registered(Serial, dump_serial)
 
 
 def cli():
     try:
         cli_entrypoint()
     except Exception as e:
         LoggingHandler.get().emit_exception(e)
```

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/dumptool.py` & `ltchiptool-4.2.0/ltchiptool/commands/flash/split.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 import click
 
 from ltchiptool import Board
 from ltchiptool.models import BoardParamType
 from ltchiptool.util.crc16 import CRC16
 
 
-@click.group(help="Capture or process device dumps")
-def cli():
-    pass
-
-
-@cli.command()
+@click.command()
 @click.argument("board", type=BoardParamType())
 @click.argument("input", type=click.File("rb"))
 @click.option(
     "-o",
     "--output",
     type=click.Path(file_okay=False),
     default=None,
@@ -36,15 +31,15 @@
 )
 @click.option(
     "-c/-C",
     "--checksum/--no-checksum",
     default=True,
     help="Append checksum to file names (default)",
 )
-def split(board: Board, input: IO[bytes], output: str, trim: bool, checksum: bool):
+def cli(board: Board, input: IO[bytes], output: str, trim: bool, checksum: bool):
     """
     Split raw dump file based on board partitions.
 
     \b
     Arguments:
       BOARD    Name of the board of this dump
       INPUT    Raw input file
```

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/elf2bin.py` & `ltchiptool-4.2.0/ltchiptool/commands/compile/elf2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/flash/_utils.py` & `ltchiptool-4.2.0/ltchiptool/commands/flash/_utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/flash/file.py` & `ltchiptool-4.2.0/ltchiptool/commands/flash/file.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/flash/read.py` & `ltchiptool-4.2.0/ltchiptool/commands/flash/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 import click
 from click import File
 
 from ltchiptool import Family, SocInterface
 from ltchiptool.models import FamilyParamType
 from ltchiptool.util.cli import AutoIntParamType, DevicePortParamType
-from ltchiptool.util.flash import ClickProgressCallback, FlashConnection
+from ltchiptool.util.flash import FlashConnection
 from ltchiptool.util.logging import graph
 from ltchiptool.util.misc import sizeof
+from ltchiptool.util.streams import ClickProgressCallback
 
 from ._utils import flash_link_interactive
 
 
 @click.command(short_help="Read flash contents")
 @click.argument("family", type=FamilyParamType())
 @click.argument("file", type=File("wb"))
```

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/flash/write.py` & `ltchiptool-4.2.0/ltchiptool/commands/flash/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 import click
 from click import File
 
 from ltchiptool import Family, SocInterface
 from ltchiptool.models import FamilyParamType
 from ltchiptool.util.cli import AutoIntParamType, DevicePortParamType
 from ltchiptool.util.detection import Detection
-from ltchiptool.util.flash import ClickProgressCallback, FlashConnection
+from ltchiptool.util.flash import FlashConnection
 from ltchiptool.util.logging import graph
 from ltchiptool.util.misc import sizeof
+from ltchiptool.util.streams import ClickProgressCallback
 from uf2tool import UploadContext
 
 from ._utils import flash_link_interactive
 
 
 @click.command(short_help="Write flash contents")
 @click.argument("file", type=File("rb"))
```

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/link2bin.py` & `ltchiptool-4.2.0/ltchiptool/commands/compile/link2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/commands/list.py` & `ltchiptool-4.2.0/ltchiptool/commands/list.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/families.json` & `ltchiptool-4.2.0/ltchiptool/families.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9571428571428571%*

 * *Differences: {"'beken-7231n'": "{delete: ['mcus']}",*

 * * "'beken-7231u'": "{delete: ['mcus']}",*

 * * "'beken-7251'": "{delete: ['mcus']}",*

 * * "'boufallo-bl60x'": "{delete: ['mcus']}",*

 * * "'realtek-amb1'": "{delete: ['mcus']}",*

 * * "'realtek-ambd'": "{delete: ['mcus']}",*

 * * "'realtek-ambz'": "{delete: ['mcus']}",*

 * * "'realtek-ambz2'": "{delete: ['mcus']}"}*

```diff
@@ -1,40 +1,27 @@
 {
     "$schema": "./families.schema.json",
     "beken-7231n": {
         "code": "bk7231n",
         "description": "Beken 7231N",
         "id": "0x7B3EF230",
-        "mcus": [
-            "BK7231N",
-            "BL2028N"
-        ],
         "parent": "beken-72xx-gen1",
         "short_name": "BK7231N"
     },
     "beken-7231u": {
         "code": "bk7231u",
         "description": "Beken 7231U/7231T",
         "id": "0x675A40B0",
-        "mcus": [
-            "BK7231T",
-            "BK7231S",
-            "BK7231U"
-        ],
         "parent": "beken-72xx-gen1",
         "short_name": "BK7231U"
     },
     "beken-7251": {
         "code": "bk7251",
         "description": "Beken 7251/7252",
         "id": "0x6A82CC42",
-        "mcus": [
-            "BK7251",
-            "BK7252"
-        ],
         "parent": "beken-72xx-gen1",
         "short_name": "BK7251"
     },
     "beken-72xx": {
         "code": "bk72xx",
         "description": "Beken 72xx",
         "parent": null
@@ -50,15 +37,14 @@
         "description": "Beken 72xx (RISC-V & ARM)",
         "parent": "beken-72xx"
     },
     "boufallo-bl60x": {
         "code": "bl60x",
         "description": "Boufallo BL602/BL604",
         "id": "0xDE1270B7",
-        "mcus": [],
         "parent": "boufallo-bl678",
         "short_name": "BL60X"
     },
     "boufallo-bl678": {
         "code": "bl678",
         "description": "Boufallo BL6xx/BL7xx/BL8xx",
         "parent": null
@@ -68,45 +54,36 @@
         "description": "Realtek Ameba",
         "parent": null
     },
     "realtek-amb1": {
         "code": "amb1",
         "description": "Realtek Ameba1",
         "id": "0x9FFFD543",
-        "mcus": [],
         "parent": "realtek-amb",
         "short_name": "RTL8710A"
     },
     "realtek-ambd": {
         "code": "ambd",
         "description": "Realtek AmebaD",
         "id": "0x3379CFE2",
-        "mcus": [],
         "parent": "realtek-amb",
         "short_name": "RTL8720D"
     },
     "realtek-ambz": {
         "code": "ambz",
         "description": "Realtek AmebaZ",
         "id": "0x22E0D6FC",
-        "mcus": [
-            "RTL8710BN",
-            "RTL8710BX"
-        ],
         "package": "framework-realtek-amb1",
         "parent": "realtek-amb",
         "short_name": "RTL8710B"
     },
     "realtek-ambz2": {
         "code": "ambz2",
         "description": "Realtek AmebaZ2",
         "id": "0xE08F7564",
-        "mcus": [
-            "RTL8720CF"
-        ],
         "package": "framework-realtek-ambz2",
         "parent": "realtek-amb",
         "short_name": "RTL8720C"
     },
     "winnermicro-iot": {
         "code": "wmiot",
         "description": "WinnerMicro W60x/W800x",
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/__main__.py` & `ltchiptool-4.2.0/ltchiptool/gui/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #  Copyright (c) Kuba Szczodrzyński 2023-1-2.
 
 import sys
-from logging import error
+from logging import INFO, NOTSET, error
 
 import click
 
 from ltchiptool import get_version
-from ltchiptool.util.logging import VERBOSE, LoggingHandler
+from ltchiptool.util.logging import LoggingHandler
 
 
 def gui_entrypoint(*args, **kwargs):
     try:
         import wx
     except ImportError:
         error("Cannot find wxPython or one of its dependencies")
@@ -19,15 +19,16 @@
 
     app = wx.App()
     try:
         if sys.version_info < (3, 10, 0):
             raise RuntimeError("ltchiptool GUI requires Python 3.10 or newer")
         from .main import MainFrame
 
-        LoggingHandler.get().level = VERBOSE
+        if LoggingHandler.get().level == NOTSET:
+            LoggingHandler.get().level = INFO
         frm = MainFrame(None, title=f"ltchiptool v{get_version()}")
         frm.init_params = kwargs
         frm.Show()
         app.MainLoop()
     except Exception as e:
         LoggingHandler.get().exception_hook = None
         LoggingHandler.get().emit_exception(e)
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool-192x192.png` & `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool-192x192.png`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.ico` & `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.ico`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.xrc` & `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.xrc`

 * *Files 14% similar despite different names*

#### Comparing `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.xrc` & `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.xrc`

```diff
@@ -22,14 +22,18 @@
         <checkable>1</checkable>
       </object>
       <object class="wxMenuItem" name="menu_item_13">
         <label>Colors</label>
         <checked>1</checked>
         <checkable>1</checkable>
       </object>
+      <object class="wxMenuItem" name="menu_item">
+        <label>Dump serial data</label>
+        <checkable>1</checkable>
+      </object>
       <object class="separator" name="separator_3"/>
       <object class="wxMenuItem" name="menu_item_10">
         <label>Log level</label>
         <enabled>0</enabled>
       </object>
       <object class="wxMenuItem" name="menu_item_5">
         <label>Verbose</label>
@@ -48,14 +52,17 @@
         <radio>1</radio>
       </object>
       <object class="wxMenuItem" name="menu_item_9">
         <label>Error</label>
         <radio>1</radio>
       </object>
     </object>
+    <object class="wxMenu" name="m_menu_4">
+      <label>Colors</label>
+    </object>
     <object class="wxMenu" name="m_menu_3">
       <label>Debug</label>
       <object class="wxMenuItem" name="menu_item_14">
         <label>Print settings</label>
       </object>
     </object>
   </object>
@@ -151,15 +158,15 @@
       <hgap>0</hgap>
       <growablecols>1</growablecols>
       <flexibledirection>wxBOTH</flexibledirection>
       <nonflexiblegrowmode>wxFLEX_GROWMODE_SPECIFIED</nonflexiblegrowmode>
       <object class="sizeritem">
         <cellpos>0,0</cellpos>
         <cellspan>1,1</cellspan>
-        <flag>wxALL</flag>
+        <flag>wxALL|wxALIGN_CENTER_VERTICAL</flag>
         <border>5</border>
         <object class="wxStaticText" name="text_port">
           <label>Device port</label>
           <wrap>-1</wrap>
         </object>
       </object>
       <object class="sizeritem">
@@ -179,15 +186,15 @@
         <object class="wxButton" name="button_rescan">
           <label>Rescan</label>
         </object>
       </object>
       <object class="sizeritem">
         <cellpos>1,0</cellpos>
         <cellspan>1,1</cellspan>
-        <flag>wxALL</flag>
+        <flag>wxALL|wxALIGN_CENTER_VERTICAL</flag>
         <border>5</border>
         <object class="wxStaticText" name="text_baudrate">
           <label>Baud rate</label>
           <wrap>-1</wrap>
         </object>
       </object>
       <object class="sizeritem">
@@ -267,15 +274,15 @@
             </object>
           </object>
         </object>
       </object>
       <object class="sizeritem">
         <cellpos>3,0</cellpos>
         <cellspan>1,1</cellspan>
-        <flag>wxALL</flag>
+        <flag>wxALL|wxALIGN_CENTER_VERTICAL</flag>
         <border>5</border>
         <object class="wxStaticText" name="text_file">
           <label>Input file</label>
           <wrap>-1</wrap>
         </object>
       </object>
       <object class="sizeritem">
@@ -659,373 +666,69 @@
               <style>wxHL_ALIGN_LEFT</style>
             </object>
           </object>
         </object>
       </object>
     </object>
   </object>
-  <object class="wxPanel" name="UpkPanel">
+  <object class="wxPanel" name="PluginsPanel">
     <style>wxTAB_TRAVERSAL</style>
-    <object class="wxBoxSizer" name="sizer_upk_main">
-      <orient>wxHORIZONTAL</orient>
+    <object class="wxBoxSizer" name="sizer_main_plugins">
+      <orient>wxVERTICAL</orient>
       <object class="sizeritem">
         <flag>wxALL|wxEXPAND</flag>
         <border>5</border>
         <option>1</option>
-        <object class="wxNotebook" name="notebook_upk">
-          <object>
-            <label>Start page</label>
-            <style>wxTAB_TRAVERSAL</style>
-            <bg>#F0F0F0</bg>
-            <object class="wxPanel" name="page_start">
-              <style>wxTAB_TRAVERSAL</style>
-              <object class="wxBoxSizer" name="sizer_start">
-                <orient>wxVERTICAL</orient>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxStaticText" name="text_start">
-                    <label>This tool allows to easily generate ESPHome YAML configuration, having either:
-- ESPHome-Kickstart running
-- Cloudcutter device profile
-- full firmware dump
-
-Choose a mode of operation to begin:</label>
-                    <wrap>-1</wrap>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxCommandLinkButton" name="button_kickstart">
-                    <label>Grab from ESPHome-Kickstart</label>
-                    <note>If you have flashed Kickstart to a device</note>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxCommandLinkButton" name="button_cloudcutter">
-                    <label>Build from Cloudcutter device profile</label>
-                    <note>If your device has a matching manufacturer/model profile</note>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxCommandLinkButton" name="button_dump">
-                    <label>Analyze firmware dump</label>
-                    <note>If you read a firmware .BIN with ltchiptool or bk7231tools</note>
-                  </object>
-                </object>
-              </object>
-            </object>
-          </object>
-          <object>
-            <label>Options</label>
-            <style>wxTAB_TRAVERSAL</style>
-            <bg>#F0F0F0</bg>
-            <object class="wxPanel" name="page_opts">
-              <style>wxTAB_TRAVERSAL</style>
-              <object class="wxBoxSizer" name="sizer_opts_main">
-                <orient>wxVERTICAL</orient>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxStaticText" name="text_opts">
-                    <label>You can set various options related to the generated YAML.
-The default choices are usually fine in most cases.</label>
-                    <wrap>-1</wrap>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxBoxSizer" name="sizer_opts_horz">
-                    <orient>wxHORIZONTAL</orient>
-                    <object class="sizeritem">
-                      <flag>wxALL|wxEXPAND</flag>
-                      <border>5</border>
-                      <option>1</option>
-                      <object class="wxBoxSizer" name="sizer_opts_vert1">
-                        <orient>wxVERTICAL</orient>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_esphome_block">
-                            <label>Include esphome: block</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_name_mac">
-                            <label>Add MAC to device name</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_common">
-                            <label>Add common components</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_web_server">
-                            <label>Add Web Server &amp;&amp; Captive Portal</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_restart">
-                            <label>Add restart button &amp;&amp; sensor</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_uptime">
-                            <label>Add uptime sensor</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxCheckBox" name="opts_lt_version">
-                            <label>Add LT version sensor</label>
-                            <checked>1</checked>
-                          </object>
-                        </object>
-                      </object>
-                    </object>
-                    <object class="sizeritem">
-                      <flag>wxALL|wxEXPAND</flag>
-                      <border>5</border>
-                      <option>1</option>
-                      <object class="wxBoxSizer" name="sizer_opts_vert2">
-                        <orient>wxVERTICAL</orient>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxStaticText" name="text_wifi_ssid">
-                            <label>Wi-Fi SSID</label>
-                            <wrap>-1</wrap>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxTextCtrl" name="opts_wifi_ssid">
-                            <value>!secret wifi__ssid</value>
-                            <value>!secret wifi__ssid</value>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxStaticText" name="text_wifi_password">
-                            <label>Wi-Fi password</label>
-                            <wrap>-1</wrap>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxTextCtrl" name="opts_wifi_password">
-                            <value>!secret wifi__password</value>
-                            <value>!secret wifi__password</value>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxStaticText" name="text_ota_password">
-                            <label>OTA password</label>
-                            <wrap>-1</wrap>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxTextCtrl" name="opts_ota_password">
-                            <value>!secret ota__password</value>
-                            <value>!secret ota__password</value>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxStaticText" name="text_api_password">
-                            <label>API password</label>
-                            <wrap>-1</wrap>
-                          </object>
-                        </object>
-                        <object class="sizeritem">
-                          <flag>wxALL|wxEXPAND</flag>
-                          <border>5</border>
-                          <object class="wxTextCtrl" name="opts_api_password">
-                            <value>!secret api__password</value>
-                            <value>!secret api__password</value>
-                          </object>
-                        </object>
-                      </object>
-                    </object>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxALIGN_CENTER_HORIZONTAL</flag>
-                  <border>5</border>
-                  <object class="wxButton" name="button_generate">
-                    <label>Generate</label>
-                  </object>
-                </object>
-              </object>
-            </object>
-          </object>
-          <object>
-            <label>ESPHome YAML</label>
-            <style>wxTAB_TRAVERSAL</style>
-            <bg>#F0F0F0</bg>
-            <object class="wxPanel" name="page_esphome">
-              <style>wxTAB_TRAVERSAL</style>
-              <object class="wxGridBagSizer" name="sizer_esphome">
-                <vgap>0</vgap>
-                <hgap>0</hgap>
-                <growablerows>2</growablerows>
-                <growablecols>0</growablecols>
-                <flexibledirection>wxBOTH</flexibledirection>
-                <nonflexiblegrowmode>wxFLEX_GROWMODE_SPECIFIED</nonflexiblegrowmode>
-                <object class="sizeritem">
-                  <cellpos>0,0</cellpos>
-                  <cellspan>1,1</cellspan>
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxStaticText" name="text_esphome_1">
-                    <label>This page shows a suggested YAML config for your device.</label>
-                    <wrap>500</wrap>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <cellpos>1,0</cellpos>
-                  <cellspan>1,1</cellspan>
-                  <flag>wxALL</flag>
-                  <border>5</border>
-                  <object class="wxStaticText" name="text_esphome_2">
-                    <label>We do not take responsibility for using this tool and the generated configs.</label>
-                    <wrap>500</wrap>
-                    <font>
-                      <size>9</size>
-                      <weight>bold</weight>
-                    </font>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <cellpos>0,1</cellpos>
-                  <cellspan>2,1</cellspan>
-                  <flag>wxALL</flag>
-                  <border>5</border>
-                  <object class="wxButton" name="button_esphome_copy">
-                    <label>Copy</label>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <cellpos>2,0</cellpos>
-                  <cellspan>1,2</cellspan>
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <option>1</option>
-                  <object class="wxTextCtrl" name="input_esphome">
-                    <style>wxTE_MULTILINE|wxTE_READONLY</style>
-                    <font>
-                      <size>11</size>
-                      <face>Consolas</face>
-                    </font>
-                  </object>
-                </object>
-              </object>
+        <object class="wxDataViewCtrl" name="plugins_tree">
+          <style>wxDV_HORIZ_RULES</style>
+        </object>
+      </object>
+      <object class="sizeritem">
+        <flag>wxALL|wxEXPAND</flag>
+        <border>0</border>
+        <object class="wxBoxSizer" name="sizer_download">
+          <orient>wxHORIZONTAL</orient>
+          <object class="sizeritem">
+            <flag>wxALL|wxEXPAND</flag>
+            <border>5</border>
+            <object class="wxButton" name="button_download">
+              <label>Download plugins...</label>
             </object>
           </object>
-          <object>
-            <label>Device configuration</label>
-            <style>wxTAB_TRAVERSAL</style>
-            <bg>#F0F0F0</bg>
-            <object class="wxPanel" name="page_upk">
-              <style>wxTAB_TRAVERSAL</style>
-              <object class="wxBoxSizer" name="sizer_upk">
-                <orient>wxVERTICAL</orient>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxStaticText" name="text_upk">
-                    <label>This page shows the raw user__param__key (UPK) structure.
-
-Based on this, ESPHome config is generated.</label>
-                    <wrap>500</wrap>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <option>1</option>
-                  <object class="wxTextCtrl" name="input_upk">
-                    <style>wxTE_MULTILINE|wxTE_READONLY</style>
-                    <font>
-                      <size>11</size>
-                      <face>Consolas</face>
-                    </font>
-                  </object>
+          <object class="sizeritem">
+            <flag>wxALL|wxEXPAND</flag>
+            <border>0</border>
+            <option>1</option>
+            <object class="wxBoxSizer" name="sizer_install">
+              <orient>wxVERTICAL</orient>
+              <object class="sizeritem">
+                <flag>wxLEFT</flag>
+                <border>5</border>
+                <object class="wxStaticText" name="text_install">
+                  <label>Install/update a plugin</label>
+                  <wrap>-1</wrap>
                 </object>
               </object>
-            </object>
-          </object>
-          <object>
-            <label>Storage data</label>
-            <style>wxTAB_TRAVERSAL</style>
-            <bg>#F0F0F0</bg>
-            <object class="wxPanel" name="page_storage">
-              <style>wxTAB_TRAVERSAL</style>
-              <object class="wxBoxSizer" name="sizer_storage">
-                <orient>wxVERTICAL</orient>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <object class="wxStaticText" name="text_storage_1">
-                    <label>This page shows the extracted Storage Area JSON. It contains a device schema and some other information that are useful for building Cloudcutter profiles.
-
-If Cloudcutter doesn't support your device yet, consider submitting the JSON to the issues page:</label>
-                    <wrap>500</wrap>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL</flag>
-                  <border>5</border>
-                  <object class="wxHyperlinkCtrl" name="link_storage">
-                    <label>https://github.com/tuya-cloudcutter/tuya-cloudcutter/issues</label>
-                    <style>wxHL_DEFAULT_STYLE</style>
-                  </object>
-                </object>
-                <object class="sizeritem">
-                  <flag>wxALL|wxEXPAND</flag>
-                  <border>5</border>
-                  <option>1</option>
-                  <object class="wxTextCtrl" name="input_storage">
-                    <style>wxTE_MULTILINE|wxTE_READONLY</style>
-                    <font>
-                      <size>11</size>
-                      <face>Consolas</face>
-                    </font>
+              <object class="sizeritem">
+                <flag>wxALL|wxEXPAND</flag>
+                <border>0</border>
+                <object class="wxBoxSizer" name="sizer_distribution">
+                  <orient>wxHORIZONTAL</orient>
+                  <object class="sizeritem">
+                    <flag>wxALL</flag>
+                    <border>5</border>
+                    <option>1</option>
+                    <object class="wxTextCtrl" name="input_install"/>
+                  </object>
+                  <object class="sizeritem">
+                    <flag>wxALL</flag>
+                    <border>5</border>
+                    <object class="wxButton" name="button_install">
+                      <label>Install</label>
+                    </object>
                   </object>
                 </object>
               </object>
             </object>
           </object>
         </object>
       </object>
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/panels/about.py` & `ltchiptool-4.2.0/ltchiptool/gui/panels/about.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from ltchiptool import get_version
 from ltchiptool.util.lvm import LVM, LVMPlatform
 
 from .base import BasePanel
 
 
 class AboutPanel(BasePanel):
-    def __init__(self, res: wx.xrc.XmlResource, *args, **kw):
-        super().__init__(*args, **kw)
-        self.LoadXRC(res, "AboutPanel")
+    def __init__(self, parent: wx.Window, frame):
+        super().__init__(parent, frame)
+        self.LoadXRC("AboutPanel")
+        self.AddToNotebook("About")
 
         platform = LVM.default()
         lt_path = platform.path
         lt_version = f"v{platform.version}"
         if platform.type == LVMPlatform.Type.SNAPSHOT:
             lt_path_title = "Local data snapshot path"
             lt_version = None
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/panels/base.py` & `ltchiptool-4.2.0/ltchiptool/gui/panels/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 #  Copyright (c) Kuba Szczodrzyński 2023-1-3.
 
-from typing import Callable
+import sys
+from os.path import dirname, isfile, join
+from typing import Any, Callable, Tuple
 
 import wx
 import wx.xrc
 
+from ltchiptool.gui.colors import ColorPalette
+from ltchiptool.gui.utils import load_xrc_file
 from ltchiptool.gui.work.base import BaseThread
 
 
 # noinspection PyPep8Naming
 class BasePanel(wx.Panel):
     _components: list[wx.Window]
     _threads: list[BaseThread]
     _in_update: bool = False
     is_closing: bool = False
 
-    def __init__(self, *args, **kw):
-        super().__init__(*args, **kw)
+    def __init__(self, parent: wx.Window, frame):
+        super().__init__(parent)
+        self.Frame = frame
+        self.Xrc: wx.xrc.XmlResource = frame.Xrc
         self._components = []
         self._threads = []
 
-    def start_work(self, thread: BaseThread, freeze_ui: bool = False):
+    def StartWork(self, thread: BaseThread, freeze_ui: bool = True):
         self._threads.append(thread)
 
         def on_stop(t: BaseThread):
-            self.on_work_stopped(t)
+            self.OnWorkStopped(t)
             if freeze_ui:
                 self.EnableAll()
 
         thread.on_stop = on_stop
         if freeze_ui:
             self.DisableAll()
         thread.start()
 
-    def stop_work(self, cls: type[BaseThread]):
+    def StopWork(self, cls: type[BaseThread]):
         for t in list(self._threads):
             if isinstance(t, cls):
                 t.stop()
 
-    def on_work_stopped(self, t: BaseThread):
+    def OnWorkStopped(self, t: BaseThread):
         self._threads.remove(t)
 
     def SetInitParams(self, **kwargs):
         pass
 
     def GetSettings(self) -> dict:
         pass
@@ -55,20 +61,29 @@
 
     def OnClose(self):
         self.is_closing = True
         for t in list(self._threads):
             t.stop()
             t.join()
 
+    def OnActivate(self):
+        pass
+
+    def OnDeactivate(self):
+        pass
+
     def OnMenu(self, title: str, label: str, checked: bool):
         pass
 
     def OnFileDrop(self, *files):
         pass
 
+    def OnPaletteChanged(self, old: ColorPalette, new: ColorPalette):
+        pass
+
     def _OnUpdate(self, event: wx.Event | None):
         if self._in_update:
             event.Skip()
             return
         self._in_update = True
         event.Skip()
         self.OnUpdate(event.GetEventObject() if event else None)
@@ -80,59 +95,85 @@
         self._in_update = True
         self.OnUpdate(target)
         self._in_update = False
 
     def OnUpdate(self, target: wx.Window = None):
         pass
 
-    def LoadXRC(self, res: wx.xrc.XmlResource, name: str):
-        panel = res.LoadPanel(self, name)
+    def LoadXRCFile(self, *path: str):
+        xrc = join(*path)
+        if isfile(xrc):
+            self.Xrc = load_xrc_file(xrc)
+        else:
+            root = dirname(sys.modules[self.__module__].__file__)
+            self.Xrc = load_xrc_file(root, *path)
+
+    def LoadXRC(self, name: str):
+        panel = self.Xrc.LoadPanel(self, name)
+        if not panel:
+            raise ValueError(f"Panel not found: {name}")
         sizer = wx.BoxSizer(wx.VERTICAL)
         sizer.Add(panel, 1, wx.EXPAND)
         self.SetSizer(sizer)
 
+    def AddToNotebook(self, title: str):
+        self.Frame.Notebook.AddPage(self, title)
+
     def BindByName(self, event: int, name: str, handler: Callable[[wx.Event], None]):
-        self.FindWindowByName(name).Bind(event, handler)
+        self.FindWindowByName(name, self).Bind(event, handler)
 
     def BindComboBox(self, name: str):
-        window: wx.ComboBox = self.FindWindowByName(name)
+        window: wx.ComboBox = self.FindWindowByName(name, self)
         self._components.append(window)
         window.Bind(wx.EVT_COMBOBOX, self._OnUpdate)
         return window
 
+    def BindListBox(self, name: str):
+        window: wx.ListBox = self.FindWindowByName(name, self)
+        self._components.append(window)
+        window.Bind(wx.EVT_LISTBOX, self._OnUpdate)
+        return window
+
     def BindRadioButton(self, name: str):
-        window: wx.RadioButton = self.FindWindowByName(name)
+        window: wx.RadioButton = self.FindWindowByName(name, self)
         self._components.append(window)
         window.Bind(wx.EVT_RADIOBUTTON, self._OnUpdate)
         return window
 
     def BindCheckBox(self, name: str):
-        window: wx.CheckBox = self.FindWindowByName(name)
+        window: wx.CheckBox = self.FindWindowByName(name, self)
         self._components.append(window)
         window.Bind(wx.EVT_CHECKBOX, self._OnUpdate)
         return window
 
     def BindTextCtrl(self, name: str):
-        window: wx.TextCtrl = self.FindWindowByName(name)
+        window: wx.TextCtrl = self.FindWindowByName(name, self)
         self._components.append(window)
         window.Bind(wx.EVT_TEXT, self._OnUpdate)
         return window
 
     def BindButton(self, name: str, func: Callable[[wx.Event], None]):
-        window: wx.Button = self.FindWindowByName(name)
+        window: wx.Button = self.FindWindowByName(name, self)
         self._components.append(window)
         window.Bind(wx.EVT_BUTTON, func)
         return window
 
+    def BindWindow(self, name: str, *handlers: Tuple[Any, Callable[[wx.Event], None]]):
+        window = self.FindWindowByName(name, self)
+        self._components.append(window)
+        for event, func in handlers:
+            window.Bind(event, func)
+        return window
+
     def FindStaticText(self, name: str):
-        window: wx.StaticText = self.FindWindowByName(name)
+        window: wx.StaticText = self.FindWindowByName(name, self)
         return window
 
     def FindStaticBitmap(self, name: str):
-        window: wx.StaticBitmap = self.FindWindowByName(name)
+        window: wx.StaticBitmap = self.FindWindowByName(name, self)
         return window
 
     def EnableAll(self):
         if self.is_closing:
             return
         for window in self._components:
             window.Enable()
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/panels/flash.py` & `ltchiptool-4.2.0/ltchiptool/gui/panels/flash.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from os.path import dirname, isfile, realpath
 
 import wx
 import wx.adv
 import wx.xrc
 
 from ltchiptool import Family, SocInterface
+from ltchiptool.gui.main import MainFrame
 from ltchiptool.gui.utils import int_or_zero, on_event, only_target, with_target
 from ltchiptool.gui.work.flash import FlashThread
 from ltchiptool.gui.work.ports import PortWatcher
 from ltchiptool.util.cli import list_serial_ports
 from ltchiptool.util.detection import Detection
 from ltchiptool.util.fileio import chname
 from ltchiptool.util.flash import FlashOp
@@ -26,35 +27,36 @@
     detection: Detection | None = None
     ports: list[tuple[str, bool, str]]
     prev_read_full: bool = None
     prev_file: str | None = None
     auto_file: str | None = None
     delayed_port: str | None = None
 
-    def __init__(self, res: wx.xrc.XmlResource, *args, **kw):
-        super().__init__(*args, **kw)
-        self.LoadXRC(res, "FlashPanel")
+    def __init__(self, parent: wx.Window, frame):
+        super().__init__(parent, frame)
+        self.LoadXRC("FlashPanel")
+        self.AddToNotebook("Flashing")
 
         self.ports = []
 
         self.Port = self.BindComboBox("combo_port")
-        self.Rescan = self.BindButton("button_rescan", self.on_rescan_click)
+        self.Rescan = self.BindButton("button_rescan", self.OnRescanClick)
         self.Write = self.BindRadioButton("radio_write")
         self.Read = self.BindRadioButton("radio_read")
         self.ReadROM = self.BindRadioButton("radio_read_rom")
         self.AutoDetect = self.BindCheckBox("checkbox_auto_detect")
         self.FileText = self.FindStaticText("text_file")
         self.File = self.BindTextCtrl("input_file")
         self.Family = self.BindComboBox("combo_family")
-        self.BindButton("button_browse", self.on_browse_click)
+        self.BindButton("button_browse", self.OnBrowseClick)
         self.Start: wx.adv.CommandLinkButton = self.BindButton(
-            "button_start", self.on_start_click
+            "button_start", self.OnStartClick
         )
         self.Cancel: wx.adv.CommandLinkButton = self.BindButton(
-            "button_cancel", self.on_cancel_click
+            "button_cancel", self.OnCancelClick
         )
 
         self.Baudrate = {
             None: self.BindRadioButton("radio_baudrate_auto"),
             115200: self.BindRadioButton("radio_baudrate_115200"),
             230400: self.BindRadioButton("radio_baudrate_230400"),
             460800: self.BindRadioButton("radio_baudrate_460800"),
@@ -129,15 +131,15 @@
         self.skip = skip
         self.length = length
         self.prev_file = prev_file
         self.auto_file = auto_file
 
     def OnShow(self):
         super().OnShow()
-        self.start_work(PortWatcher(self.on_ports_updated))
+        self.StartWork(PortWatcher(self.OnPortsUpdated), freeze_ui=False)
 
     def OnUpdate(self, target: wx.Window = None):
         writing = self.operation == FlashOp.WRITE
         reading = not writing
         auto = self.auto_detect
         manual = not auto
         is_uf2 = self.detection is not None and self.detection.is_uf2
@@ -416,15 +418,15 @@
             filename = f"ltchiptool_{self.family.code}_{date}{rom}.bin"
         else:
             filename = f"ltchiptool_dump_{date}{rom}.bin"
         self.auto_file = chname(self.file, filename)
         verbose(f"Generated dump filename: {self.auto_file}")
         return self.auto_file
 
-    def on_ports_updated(self, ports: list[tuple[str, bool, str]]):
+    def OnPortsUpdated(self, ports: list[tuple[str, bool, str]]):
         self.Port.Enable(not not ports)
         if not ports:
             self.ports = []
             self.Port.Set(["No serial ports found"])
             self.Port.SetSelection(0)
             return
         user_port = self.port or self.delayed_port
@@ -436,19 +438,19 @@
             info(f"Device unplugged: {description}")
         self.Port.Set([port[2] for port in ports])
         self.ports = ports
         self.port = user_port
         self.delayed_port = None
 
     @on_event
-    def on_rescan_click(self):
-        self.on_ports_updated(list_serial_ports())
+    def OnRescanClick(self):
+        self.OnPortsUpdated(list_serial_ports())
 
     @on_event
-    def on_browse_click(self):
+    def OnBrowseClick(self):
         if self.operation == FlashOp.WRITE:
             title = "Open file"
             flags = wx.FD_OPEN | wx.FD_FILE_MUST_EXIST
         else:
             title = "Save file"
             flags = wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT
         init_dir = dirname(self.file) if self.file else os.getcwd()
@@ -458,15 +460,15 @@
                 return
             self.file = dialog.GetPath()
             if self.operation != FlashOp.WRITE:
                 # clear previous writing filename
                 self.prev_file = None
 
     @on_event
-    def on_start_click(self):
+    def OnStartClick(self):
         if self.operation == FlashOp.WRITE and self.auto_detect and self.detection:
             soc = self.detection.soc or SocInterface.get(self.family)
         else:
             soc = SocInterface.get(self.family)
 
         if self.operation != FlashOp.WRITE:
             if self.file == self.auto_file:
@@ -489,14 +491,14 @@
             offset=self.offset,
             skip=self.skip,
             length=self.length,
             verify=True,
             ctx=self.detection and self.detection.get_uf2_ctx(),
             on_chip_info=self.Start.SetNote,
         )
-        self.start_work(work, freeze_ui=True)
+        self.StartWork(work)
         self.Start.SetNote("")
         self.Cancel.Enable()
 
     @on_event
-    def on_cancel_click(self):
-        self.stop_work(FlashThread)
+    def OnCancelClick(self):
+        self.StopWork(FlashThread)
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/panels/log.py` & `ltchiptool-4.2.0/ltchiptool/gui/panels/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 import time
 from logging import INFO, info, log, warning
 
 import wx
 import wx.xrc
 from click import _termui_impl
 from click._termui_impl import ProgressBar
+from serial import Serial
 
+from ltchiptool.gui.colors import ColorPalette
 from ltchiptool.util.logging import LoggingHandler
 from ltchiptool.util.misc import sizeof
+from ltchiptool.util.streams import LoggingStreamHook
 
 from .base import BasePanel
 
 
 class GUIProgressBar(ProgressBar):
     parent: BasePanel
     elapsed: wx.StaticText
@@ -81,107 +84,94 @@
         self.time_elapsed.Hide()
         self.time_left.Hide()
         self.bar.Hide()
         self.parent.Layout()
 
 
 class LogPanel(BasePanel):
-    COLOR_MAP = {
-        "black": wx.Colour(12, 12, 12),
-        "red": wx.Colour(197, 15, 31),
-        "green": wx.Colour(19, 161, 14),
-        "yellow": wx.Colour(193, 156, 0),
-        "blue": wx.Colour(0, 55, 218),
-        "magenta": wx.Colour(136, 23, 152),
-        "cyan": wx.Colour(58, 150, 221),
-        "white": wx.Colour(204, 204, 204),
-        "bright_black": wx.Colour(118, 118, 118),
-        "bright_red": wx.Colour(231, 72, 86),
-        "bright_green": wx.Colour(22, 198, 12),
-        "bright_yellow": wx.Colour(249, 241, 165),
-        "bright_blue": wx.Colour(59, 120, 255),
-        "bright_magenta": wx.Colour(180, 0, 158),
-        "bright_cyan": wx.Colour(97, 214, 214),
-        "bright_white": wx.Colour(242, 242, 242),
-    }
-
     delayed_lines: list[tuple[str, str, str]] | None
 
-    def __init__(self, res: wx.xrc.XmlResource, *args, **kw):
-        super().__init__(*args, **kw)
-        self.LoadXRC(res, "LogPanel")
+    def __init__(self, parent: wx.Window, frame):
+        super().__init__(parent, frame)
+        self.LoadXRC("LogPanel")
 
         self.delayed_lines = []
 
-        self.Log: wx.TextCtrl = self.FindWindowByName("text_log")
+        self.Log: wx.TextCtrl = self.FindWindowByName("text_log", self)
         LoggingHandler.get().add_emitter(self.emit_raw)
 
         GUIProgressBar.parent = self
-        GUIProgressBar.elapsed = self.FindWindowByName("text_elapsed")
-        GUIProgressBar.progress = self.FindWindowByName("text_progress")
-        GUIProgressBar.left = self.FindWindowByName("text_left")
-        GUIProgressBar.time_elapsed = self.FindWindowByName("text_time_elapsed")
-        GUIProgressBar.time_left = self.FindWindowByName("text_time_left")
-        GUIProgressBar.bar = self.FindWindowByName("progress_bar")
+        GUIProgressBar.elapsed = self.FindWindowByName("text_elapsed", self)
+        GUIProgressBar.progress = self.FindWindowByName("text_progress", self)
+        GUIProgressBar.left = self.FindWindowByName("text_left", self)
+        GUIProgressBar.time_elapsed = self.FindWindowByName("text_time_elapsed", self)
+        GUIProgressBar.time_left = self.FindWindowByName("text_time_left", self)
+        GUIProgressBar.bar = self.FindWindowByName("progress_bar", self)
         GUIProgressBar.log = self.Log
         # noinspection PyTypeChecker
         GUIProgressBar.render_finish(GUIProgressBar)
         setattr(_termui_impl, "ProgressBar", GUIProgressBar)
 
     def emit_raw(self, log_prefix: str, message: str, color: str):
         # delay non-main-thread logging until the app finishes initializing
         is_main_thread = threading.current_thread() is threading.main_thread()
         if not is_main_thread and self.delayed_lines is not None:
             self.delayed_lines.append((log_prefix, message, color))
             return
         if self.is_closing:
             return
 
-        wx_color = self.COLOR_MAP[color]
+        wx_color = ColorPalette.get()[color]
         if LoggingHandler.get().raw:
             self.Log.SetDefaultStyle(wx.TextAttr(wx.WHITE))
         else:
             self.Log.SetDefaultStyle(wx.TextAttr(wx_color))
         self.Log.AppendText(f"{message}\n")
 
     def GetSettings(self) -> dict:
         handler = LoggingHandler.get()
         return dict(
             level=handler.level,
             timed=handler.timed,
             raw=handler.raw,
             full_traceback=handler.full_traceback,
+            dump_serial=LoggingStreamHook.is_registered(Serial),
         )
 
     def SetSettings(
         self,
         level: int = INFO,
         timed: bool = False,
         raw: bool = False,
         full_traceback: bool = True,
+        dump_serial: bool = False,
         **_,
     ):
         handler = LoggingHandler.get()
         handler.level = level
         handler.timed = timed
         handler.raw = raw
         handler.full_traceback = full_traceback
+        LoggingStreamHook.set_registered(Serial, registered=dump_serial)
+
         menu_bar: wx.MenuBar = self.TopLevelParent.MenuBar
         menu: wx.Menu = menu_bar.GetMenu(menu_bar.FindMenu("Logging"))
         if not menu:
             warning(f"Couldn't find Logging menu")
             return
         level_name = logging.getLevelName(level).title()
         for item in menu.GetMenuItems():
             item: wx.MenuItem
             match item.GetItemLabel():
                 case "Timed":
                     item.Check(timed)
                 case "Colors":
                     item.Check(not raw)
+                case "Dump serial data":
+                    item.Check(dump_serial)
                 case _ if item.GetItemLabel() == level_name:
                     item.Check()
 
     def OnShow(self):
         super().OnShow()
         if self.delayed_lines is None:
             return
@@ -201,11 +191,16 @@
                 self.Log.Clear()
             case "Timed":
                 LoggingHandler.get().timed = checked
                 info("Logging options changed")
             case "Colors":
                 LoggingHandler.get().raw = not checked
                 info("Logging options changed")
+            case "Dump serial data":
+                LoggingStreamHook.set_registered(Serial, registered=checked)
             case ("Verbose" | "Debug" | "Info" | "Warning" | "Error") as l:
                 level = logging.getLevelName(l.upper())
                 LoggingHandler.get().level = level
                 log(level, "Log level changed")
+
+    def OnPaletteChanged(self, old: ColorPalette, new: ColorPalette):
+        new.apply(self.Log, old)
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/work/base.py` & `ltchiptool-4.2.0/ltchiptool/gui/work/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/work/flash.py` & `ltchiptool-4.2.0/ltchiptool/gui/work/flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,18 @@
 
 from logging import debug
 from os import SEEK_SET, makedirs, stat
 from os.path import dirname
 from typing import Callable
 
 from ltchiptool import SocInterface
-from ltchiptool.util.flash import (
-    ClickProgressCallback,
-    FlashConnection,
-    FlashOp,
-    format_flash_guide,
-)
+from ltchiptool.util.flash import FlashConnection, FlashOp, format_flash_guide
 from ltchiptool.util.logging import LoggingHandler
 from ltchiptool.util.misc import sizeof
+from ltchiptool.util.streams import ClickProgressCallback
 from uf2tool import UploadContext
 
 from .base import BaseThread
 
 
 class FlashThread(BaseThread):
     callback: ClickProgressCallback
```

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/work/ports.py` & `ltchiptool-4.2.0/ltchiptool/gui/work/ports.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/gui/work/upk.py` & `ltchiptool-4.2.0/uf2tool/upload/esphome.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,148 +1,166 @@
-#  Copyright (c) Kuba Szczodrzyński 2023-5-13.
+# Copyright (c) Kuba Szczodrzyński 2022-08-06.
 
-from logging import debug, warning
+from enum import IntEnum
+from logging import debug
 from os import stat
-from os.path import isfile
-from socket import gethostbyname
-from time import sleep
-from typing import Callable
-from urllib.parse import urlparse
+from socket import (
+    AF_INET,
+    IPPROTO_TCP,
+    SO_SNDBUF,
+    SOCK_STREAM,
+    SOL_SOCKET,
+    TCP_NODELAY,
+    gethostbyname,
+    socket,
+)
+from typing import IO, Tuple, Union
+
+from ltchiptool.util.intbin import inttobe32
+from ltchiptool.util.logging import graph, verbose
+
+OTA_MAGIC = b"\x6C\x26\xF7\x5C\x45"
+
+
+def tohex(data: bytes) -> str:
+    out = []
+    for i in range(len(data)):
+        out.append(data[i : i + 1].hex())
+    return " ".join(out)
+
+
+class OTACode(IntEnum):
+    RESP_OK = 0
+    RESP_REQUEST_AUTH = 1
+    RESP_HEADER_OK = 64
+    RESP_AUTH_OK = 65
+    RESP_UPDATE_PREPARE_OK = 66
+    RESP_BIN_MD5_OK = 67
+    RESP_RECEIVE_OK = 68
+    RESP_UPDATE_END_OK = 69
+    RESP_SUPPORTS_COMPRESSION = 70
+
+    ERROR_MAGIC = 128
+    ERROR_UPDATE_PREPARE = 129
+    ERROR_AUTH_INVALID = 130
+    ERROR_WRITING_FLASH = 131
+    ERROR_UPDATE_END = 132
+    ERROR_INVALID_BOOTSTRAPPING = 133
+    ERROR_WRONG_CURRENT_FLASH_CONFIG = 134
+    ERROR_WRONG_NEW_FLASH_CONFIG = 135
+    ERROR_ESP8266_NOT_ENOUGH_SPACE = 136
+    ERROR_ESP32_NOT_ENOUGH_SPACE = 137
+    ERROR_NO_UPDATE_PARTITION = 138
+    ERROR_UNKNOWN = 255
+
+    VERSION_1_0 = 1
+    FEATURE_SUPPORTS_COMPRESSION = 0x01
+
+
+class ESPHomeUploader:
+    file: IO[bytes]
+    file_size: int
+    file_md5: bytes
+
+    sock: socket
+    host: str
+    port: int
 
-import requests
-from bk7231tools.analysis.storage import TuyaStorage
+    password: str = None
 
-from ltchiptool.util.flash import ClickProgressCallback
-from ltchiptool.util.logging import LoggingHandler
-
-from .base import BaseThread
-
-
-class UpkThread(BaseThread):
     def __init__(
         self,
-        file: str = None,
-        url: str = None,
-        on_storage: Callable[[dict], None] = None,
-        on_error: Callable[[str], None] = None,
+        file: IO[bytes],
+        md5: bytes,
+        host: str,
+        port: int,
+        password: str = None,
     ):
-        super().__init__()
         self.file = file
-        self.url = url
-        self.on_storage = on_storage
-        self.on_error = on_error
-
-    def run_impl(self):
-        if self.file is not None:
-            self.run_file(self.file)
-        if self.url is not None:
-            self.run_url(self.url)
-
-    # noinspection HttpUrlsUsage
-    def run_url(self, url: str):
-        # grab storage data from Kickstart API
-        if not url.startswith("http"):
-            url = "http://" + url
-        url = urlparse(url)
-        url = url.netloc
-        if not url:
-            self.on_error(f"Invalid URL: {url}")
-            return
-
-        offset = 0x1E0000
-        start = 0x1E0000 - offset
-        end = 0x200000 - offset
-        init_size = 1024
-        block_size = 4096
-        buffer = bytearray(end - start)
-
-        with ClickProgressCallback(length=end - start) as bar:
-            bar.on_message(f"Resolving {url}...")
-            try:
-                ip = gethostbyname(url)
-            except Exception as e:
-                LoggingHandler.get().emit_exception(e, no_hook=True)
-                self.on_error(f"Couldn't find hostname: {url}")
-                return
-
-            url = f"http://{ip}/hub/flash_read"
-            params = dict(offset=0, length=init_size)
-
-            bar.on_message(f"Connecting to {ip}...")
-            with requests.get(url, params) as r:
-                data = r.content
-                if len(data) != init_size:
-                    self.on_error(
-                        f"Incomplete response read: {len(data)}/{init_size}\n\n"
-                        f"Is the chip running Kickstart firmware?"
-                    )
-                    return
-
-            while start < end and self.should_run():
-                bar.on_message(f"Reading from 0x{offset + start:06X}")
-                read_size = min(block_size, end - start)
-                params["offset"] = offset + start
-                params["length"] = read_size
-                sleep(0.05)
-                with requests.get(url, params) as r:
-                    data = r.content
-                    if len(data) != read_size:
-                        warning(f"Incomplete response read: {len(data)}/{read_size}")
-                        sleep(0.2)
-                        continue
-                    bar.on_update(read_size)
-                    buffer[start : start + read_size] = data
-                    start += read_size
-
-        if not self.should_run():
-            return
-
-        self.run_data(buffer)
-
-    def run_file(self, file: str):
-        # read storage from file
-        if not isfile(file):
-            self.on_error("File not found")
-            return
-        size = stat(file).st_size
-        if size > 0x200000:
-            # file too large
-            self.on_error("File larger than 2 MiB, refusing to load!")
-            return
-        if size == 0x200000:
-            # probably full flash dump
-            with open(file, "rb") as f:
-                # seek to approx. storage start (plus a fix for BkWriter etc.)
-                f.seek(0x1E0000 - 0x11000)
-                data = f.read()
-            self.run_data(data)
-            return
-        # try to search the entire file
-        with open(file, "rb") as f:
-            data = f.read()
-        self.run_data(data)
-
-    def run_data(self, data: bytes):
-        # parse raw storage
-        st = TuyaStorage()
-        if st.load_raw(data, allow_incomplete=True) is None:
-            self.on_error("File doesn't contain known storage area")
-            return
-        if not st.decrypt():
-            self.on_error("Couldn't decrypt the storage area")
-            return
-        keys = st.find_all_keys()
-        debug(f"Found {len(keys)} keys! {keys}")
-        if not keys:
-            self.on_error("No keys found in storage! Is the data corrupt?")
-            try:
-                from hexdump import hexdump
-
-                hexdump(st.data)
-            except (ImportError, ModuleNotFoundError):
-                pass
-            return
-        storage = st.read_all_keys()
-        self.on_storage(storage)
-
-    def stop(self):
-        super().stop()
+        self.file_size = stat(file.name).st_size
+        self.file_md5 = md5
+        self.host = host
+        self.port = port
+        self.password = password
+
+    def resolve_host(self):
+        debug(f"Resolving {self.host}")
+        parts = self.host.split(".")
+        if all(map(lambda x: x.isnumeric(), parts)):
+            if not all(map(lambda x: int(x) in range(0, 255), parts)):
+                raise ValueError(f"Invalid IP address: {self.host}")
+            return
+        ip_addr = gethostbyname(self.host)
+        graph(2, "Resolved {self.host} to {ip_addr}")
+        self.host = ip_addr
+
+    def connect(self):
+        debug(f"Connecting to {self.host}:{self.port}")
+        self.sock = socket(AF_INET, SOCK_STREAM)
+        self.sock.settimeout(10.0)
+        try:
+            self.sock.connect((self.host, self.port))
+        except OSError as e:
+            self.sock.close()
+            raise RuntimeError(f"Couldn't connect to {self.host}:{self.port} - {e}")
+        self.sock.setsockopt(IPPROTO_TCP, TCP_NODELAY, 1)
+
+    def send(self, data: Union[bytes, int]):
+        if isinstance(data, int):
+            data = bytes([data])
+        verbose(f"<-- TX: {tohex(data)}")
+        self.sock.sendall(data)
+
+    def receive(self, *codes: OTACode, size: int = 0) -> Tuple[OTACode, bytes]:
+        data = self.sock.recv(1)
+        response = OTACode(data[0])
+        verbose(f"--> RX: {response.name}")
+        if response not in codes:
+            raise ValueError(f"Received {response.name} instead of {codes}")
+        if size == 0:
+            return response, b""
+        data = self.sock.recv(size)
+        verbose(f"--> RX: {tohex(data)}")
+        return response, data
+
+    def upload(self):
+        self.resolve_host()
+        self.connect()
+
+        self.send(OTA_MAGIC)
+        _, ver = self.receive(OTACode.RESP_OK, size=1)
+        if ver[0] != OTACode.VERSION_1_0:
+            raise ValueError("Invalid OTA version")
+        graph(1, "Connected to ESPHome")
+
+        self.send(OTACode.FEATURE_SUPPORTS_COMPRESSION)
+        features, _ = self.receive(
+            OTACode.RESP_HEADER_OK, OTACode.RESP_SUPPORTS_COMPRESSION
+        )
+        if features == OTACode.RESP_SUPPORTS_COMPRESSION:
+            raise NotImplementedError("Compression is not implemented")
+
+        auth, _ = self.receive(OTACode.RESP_AUTH_OK, OTACode.RESP_REQUEST_AUTH)
+        if auth == OTACode.RESP_REQUEST_AUTH:
+            raise NotImplementedError("Authentication is not implemented")
+
+        self.send(inttobe32(self.file_size))
+        self.receive(OTACode.RESP_UPDATE_PREPARE_OK)
+
+        self.send(self.file_md5.hex().encode())
+        self.receive(OTACode.RESP_BIN_MD5_OK)
+
+        self.sock.setsockopt(IPPROTO_TCP, TCP_NODELAY, 0)
+        self.sock.setsockopt(SOL_SOCKET, SO_SNDBUF, 8192)
+        self.sock.settimeout(20.0)
+
+        graph(1, "Starting OTA upload")
+        while True:
+            data = self.file.read(1024)
+            if not data:
+                break
+            self.sock.sendall(data)
+
+        self.sock.setsockopt(IPPROTO_TCP, TCP_NODELAY, 1)
+        self.receive(OTACode.RESP_RECEIVE_OK)
+        self.receive(OTACode.RESP_UPDATE_END_OK)
+        self.send(OTACode.RESP_OK)
```

### Comparing `ltchiptool-4.1.1/ltchiptool/models/board.py` & `ltchiptool-4.2.0/ltchiptool/models/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         super().__init__(Board.get_data(board))
 
     @staticmethod
     def get_data(board: Union[str, dict]) -> dict:
         if not isinstance(board, dict):
             if isfile(board):
                 board = readjson(board)
+                if not board:
+                    raise FileNotFoundError(f"Board not found: {board}")
             else:
                 source = board
                 board = LVM.get().load_json(f"boards/{board}.json")
                 board["source"] = source
         if "_base" in board:
             base = board["_base"]
             if not isinstance(base, list):
```

### Comparing `ltchiptool-4.1.1/ltchiptool/models/family.py` & `ltchiptool-4.2.0/ltchiptool/models/family.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/platform.json` & `ltchiptool-4.2.0/ltchiptool/platform.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/ambz/binary.py` & `ltchiptool-4.2.0/ltchiptool/soc/ambz/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/ambz/flash.py` & `ltchiptool-4.2.0/ltchiptool/soc/ambz/flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from abc import ABC
 from io import BytesIO
 from time import sleep
 from typing import IO, Generator, List, Optional, Union
 
 from ltchiptool import SocInterface
-from ltchiptool.util.flash import FlashConnection, ProgressCallback
+from ltchiptool.util.flash import FlashConnection
 from ltchiptool.util.intbin import gen2bytes, inttole32, letoint
+from ltchiptool.util.streams import ProgressCallback
 from uf2tool import OTAScheme, UploadContext
 
 from .util.rtltool import CAN, RTL_ROM_BAUD, RTLXMD
 
 AMEBAZ_GUIDE = [
     "Connect UART2 of the Realtek chip to the USB-TTL adapter:",
     [
@@ -149,14 +150,15 @@
     def flash_write_uf2(
         self,
         ctx: UploadContext,
         verify: bool = True,
         callback: ProgressCallback = ProgressCallback(),
     ) -> None:
         # read system data to get active OTA index
+        callback.on_message("Checking OTA index...")
         system = gen2bytes(self.flash_read_raw(0x9000, 256))
         if len(system) != 256:
             raise ValueError(
                 f"Length invalid while reading from 0x9000 - {len(system)}"
             )
         # read OTA switch value
         ota_switch = f"{letoint(system[4:8]):032b}"
```

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/ambz/main.py` & `ltchiptool-4.2.0/ltchiptool/soc/ambz/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/ambz/util/rtltool.py` & `ltchiptool-4.2.0/ltchiptool/soc/ambz/util/rtltool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/binary.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/bkpackager.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/bkpackager.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/flash.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from binascii import crc32
 from logging import DEBUG, debug
 from typing import IO, Generator, List, Optional, Union
 
 from bk7231tools.serial import BK7231Serial
 
 from ltchiptool import SocInterface
-from ltchiptool.util.flash import FlashConnection, ProgressCallback
+from ltchiptool.util.flash import FlashConnection
 from ltchiptool.util.intbin import inttole32
 from ltchiptool.util.logging import VERBOSE, verbose
+from ltchiptool.util.streams import ProgressCallback
 from uf2tool import OTAScheme, UploadContext
 
 BK72XX_GUIDE = [
     "Connect UART1 of the BK7231 to the USB-TTL adapter:",
     [
         ("PC", "BK7231"),
         ("RX", "TX1 (GPIO11 / P11)"),
```

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/main.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/binary.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/crypto.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/models.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/models.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/rbl.py` & `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/rbl.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/common.py` & `ltchiptool-4.2.0/ltchiptool/soc/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     ld_ota2: Optional[str],
 ) -> List[Tuple[str, List[str]]]:
     args1 = list(args)
     args2 = list(args)
     elf1 = elf2 = None
     for i, arg in enumerate(args):
         if ".elf" in arg:
-            if not ld_ota1:
+            if ld_ota1 is None:
                 # single-OTA chip, return the output name
                 return [(arg, args)]
             # append OTA index in filename
             args1[i] = elf1 = chext(arg, "ota1.elf")
             args2[i] = elf2 = chext(arg, "ota2.elf")
-        if arg.endswith(".ld") and ld_ota1:
+        if arg.endswith(".ld") and ld_ota1 is not None:
             # use OTA2 linker script
             args2[i] = arg.replace(ld_ota1, ld_ota2)
     if not elf1 or not elf2:
         raise ValueError("Linker output .elf not found in arguments")
     return [(elf1, args1), (elf2, args2)]
```

### Comparing `ltchiptool-4.1.1/ltchiptool/soc/interface.py` & `ltchiptool-4.2.0/ltchiptool/soc/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) Kuba Szczodrzyński 2022-07-29.
 
 from abc import ABC
 from typing import IO, Dict, Generator, List, Optional, Union
 
 from ltchiptool import Board, Family
 from ltchiptool.models import OTAType
-from ltchiptool.util.flash import FlashConnection, ProgressCallback
+from ltchiptool.util.flash import FlashConnection
 from ltchiptool.util.fwbinary import FirmwareBinary
+from ltchiptool.util.streams import ProgressCallback
 from uf2tool import UploadContext
 
 
 class SocInterface(ABC):
     family: Family = None
     board: Board = None
     conn: FlashConnection = None
```

### Comparing `ltchiptool-4.1.1/ltchiptool/util/bitint.py` & `ltchiptool-4.2.0/ltchiptool/util/bitint.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/cli.py` & `ltchiptool-4.2.0/ltchiptool/util/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #  Copyright (c) Kuba Szczodrzyński 2022-10-5.
 
 import shlex
-from logging import WARNING, warning
+from logging import WARNING, error, info, warning
 from os.path import basename, dirname, join
-from typing import Dict, Iterable, List, Optional
+from subprocess import PIPE, Popen
+from threading import Thread
+from typing import IO, Callable, Dict, Iterable, List, Optional
 
 import click
 from click import Command, Context, MultiCommand
 
 from .fileio import readtext
 from .logging import graph
 from .misc import list_serial_ports
@@ -61,14 +63,37 @@
         if idx == 0:
             graph(2, "Selecting this port. To override, use -d/--device")
             if not is_usb:
                 graph(2, "This is not a USB COM port", loglevel=WARNING)
     return ports[0][0]
 
 
+def run_subprocess(*args) -> int:
+    def stream(io: IO[bytes], func: Callable[[str], None]):
+        for line in iter(io.readline, b""):
+            func(line.decode("utf-8").rstrip())
+        io.close()
+
+    p = Popen(
+        args=args,
+        stdout=PIPE,
+        stderr=PIPE,
+    )
+    threads = [
+        Thread(target=stream, args=(p.stdout, info)),
+        Thread(target=stream, args=(p.stderr, error)),
+        Thread(target=p.wait),
+    ]
+    for thread in threads:
+        thread.start()
+    for thread in threads:
+        thread.join()
+    return p.returncode
+
+
 class AutoIntParamType(click.ParamType):
     name = "DEC/HEX"
 
     def convert(self, value, param, ctx) -> int:
         try:
             return int(value, base=0)
         except ValueError as e:
```

### Comparing `ltchiptool-4.1.1/ltchiptool/util/crc16.py` & `ltchiptool-4.2.0/ltchiptool/util/crc16.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/crypto.py` & `ltchiptool-4.2.0/ltchiptool/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/detection.py` & `ltchiptool-4.2.0/ltchiptool/util/detection.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/dict.py` & `ltchiptool-4.2.0/ltchiptool/util/dict.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/fileio.py` & `ltchiptool-4.2.0/ltchiptool/util/fileio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (c) Kuba Szczodrzyński 2022-06-10.
 
 import json
 from io import SEEK_CUR, BytesIO
+from json import JSONDecodeError
+from os import makedirs
 from os.path import dirname, getmtime, isfile, join
 from typing import IO, List, Optional, Union
 
 
 def chname(path: str, name: str) -> str:
     """Change the basename of 'path' to 'name'."""
     return join(dirname(path), name)
@@ -43,24 +45,30 @@
         if isinstance(data, BytesIO):
             f.write(data.getvalue())
         else:
             f.write(data)
 
 
 # same as load_json
-def readjson(file: str) -> Union[dict, list]:
+def readjson(file: str) -> Optional[Union[dict, list]]:
     """Read a JSON file into a dict or list."""
+    if not isfile(file):
+        return None
     with open(file, "r", encoding="utf-8") as f:
-        return json.load(f)
+        try:
+            return json.load(f)
+        except JSONDecodeError:
+            return None
 
 
 def writejson(file: str, data: Union[dict, list]):
     """Write a dict or list to a JSON file."""
+    makedirs(dirname(file), exist_ok=True)
     with open(file, "w", encoding="utf-8") as f:
-        json.dump(data, f)
+        json.dump(data, f, indent="\t")
 
 
 def readtext(file: str) -> str:
     """Read a text file into a string."""
     with open(file, "r", encoding="utf-8") as f:
         data = f.read()
     return data
```

### Comparing `ltchiptool-4.1.1/ltchiptool/util/fwbinary.py` & `ltchiptool-4.2.0/ltchiptool/util/fwbinary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/intbin.py` & `ltchiptool-4.2.0/ltchiptool/util/intbin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/logging.py` & `ltchiptool-4.2.0/ltchiptool/util/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 #  Copyright (c) Kuba Szczodrzyński 2022-12-22.
 
 import logging
 import sys
-from logging import DEBUG, ERROR, INFO, Logger, LogRecord, StreamHandler, error, log
+from logging import (
+    CRITICAL,
+    DEBUG,
+    ERROR,
+    INFO,
+    Logger,
+    LogRecord,
+    StreamHandler,
+    error,
+    log,
+)
 from time import time
-from typing import Callable
+from typing import Callable, Optional
 
 import click
 
 VERBOSE = DEBUG // 2
+STREAM = CRITICAL + 1
 
 
 class LoggingHandler(StreamHandler):
     INSTANCE: "LoggingHandler" = None
     LOG_COLORS = {
         "V": "bright_cyan",
         "D": "bright_blue",
         "I": "bright_green",
         "W": "bright_yellow",
         "E": "bright_red",
         "C": "bright_magenta",
+        "S": "bright_magenta",
     }
-    exception_hook: Callable[[Exception], None] = None
+    exception_hook: Callable[[Exception, Optional[str]], None] = None
 
     @staticmethod
     def get() -> "LoggingHandler":
         if LoggingHandler.INSTANCE:
             return LoggingHandler.INSTANCE
         return LoggingHandler()
 
@@ -53,14 +65,15 @@
 
     @level.setter
     def level(self, value: int):
         logging.root.setLevel(value)
 
     def attach(self, logger: Logger = None):
         logging.addLevelName(VERBOSE, "VERBOSE")
+        logging.addLevelName(STREAM, "STREAM")
         if logger:
             root = logging.root
             logger.setLevel(root.level)
         else:
             logger = logging.root
         for h in logger.handlers:
             logger.removeHandler(h)
@@ -116,19 +129,21 @@
     @staticmethod
     def tb_echo(tb):
         filename = tb.tb_frame.f_code.co_filename
         name = tb.tb_frame.f_code.co_name
         line = tb.tb_lineno
         graph(1, f'File "{filename}", line {line}, in {name}', loglevel=ERROR)
 
-    def emit_exception(self, e: Exception, no_hook: bool = False):
+    def emit_exception(self, e: Exception, no_hook: bool = False, msg: str = None):
+        if msg:
+            error(msg)
         error(f"{type(e).__name__}: {e}")
         tb = e.__traceback__
         if self.exception_hook and not no_hook:
-            self.exception_hook(e)
+            self.exception_hook(e, msg)
         if not tb:
             return
         while tb.tb_next:
             if self.full_traceback:
                 self.tb_echo(tb)
             tb = tb.tb_next
         self.tb_echo(tb)
@@ -154,11 +169,15 @@
     ProgressBar.render_finish = render_finish
 
 
 def verbose(msg, *args, **kwargs):
     logging.log(VERBOSE, msg, *args, **kwargs)
 
 
+def stream(msg, *args, **kwargs):
+    logging.log(STREAM, msg, *args, **kwargs)
+
+
 def graph(level: int, *message, loglevel: int = INFO):
     prefix = (level - 1) * "|   " + "|-- " if level else ""
     message = " ".join(str(m) for m in message)
     log(loglevel, f"{prefix}{message}")
```

### Comparing `ltchiptool-4.1.1/ltchiptool/util/lvm.py` & `ltchiptool-4.2.0/ltchiptool/util/lvm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/misc.py` & `ltchiptool-4.2.0/ltchiptool/util/misc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Copyright (c) Kuba Szczodrzyński 2022-06-02.
 
 from functools import update_wrapper
-from typing import List, Tuple
+from logging import error
+from typing import Any, Callable, Generator, List, Optional, Tuple, TypeVar
 
 from click import get_current_context
 
+from .logging import LoggingHandler
+
 
 # https://stackoverflow.com/a/1094933/9438331
 def sizeof(num: int, suffix="B", base=1024.0) -> str:
     for unit in ["", "K", "M", "G", "T", "P", "E", "Z"]:
         if base == 1024 and unit:
             unit += "i"
         if abs(num) < base:
@@ -39,7 +42,57 @@
                 f"{port.manufacturer} ({port.vid:04X}/{port.pid:04X})"
             )
         else:
             description = f"{port.name} - {port.description}"
         ports.append((port.device, is_usb, description))
 
     return sorted(ports, key=lambda x: (not x[1], x[2]))
+
+
+T = TypeVar("T")
+
+
+def retry_catching(
+    retries: int,
+    doc: str,
+    func: Callable[[Any], T],
+    onerror: Optional[Callable[[], None]],
+    *args,
+    **kwargs,
+) -> T:
+    while True:
+        retries -= 1
+        try:
+            return func(*args, **kwargs)
+        except Exception as e:
+            if retries <= 0:
+                raise e
+            error(f"{doc}. Trying {retries} more times: {e}")
+            if onerror:
+                try:
+                    onerror()
+                except Exception as e:
+                    pass
+
+
+def retry_generator(
+    retries: int,
+    doc: str,
+    func: Callable[[Any], Generator[T, None, None]],
+    onerror: Optional[Callable[[], None]],
+    *args,
+    **kwargs,
+) -> Generator[T, None, None]:
+    while True:
+        retries -= 1
+        try:
+            yield from func(*args, **kwargs)
+            return
+        except Exception as e:
+            if retries <= 0:
+                raise e
+            error(f"{doc}. Trying {retries} more times: {e}")
+            if onerror:
+                try:
+                    onerror()
+                except Exception as e:
+                    pass
```

### Comparing `ltchiptool-4.1.1/ltchiptool/util/obj.py` & `ltchiptool-4.2.0/ltchiptool/util/obj.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/slice.py` & `ltchiptool-4.2.0/ltchiptool/util/slice.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/util/toolchain.py` & `ltchiptool-4.2.0/ltchiptool/util/toolchain.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/ltchiptool/version.py` & `ltchiptool-4.2.0/ltchiptool/version.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/pyproject.toml` & `ltchiptool-4.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "ltchiptool"
-version = "4.1.1"
+version = "4.2.0"
 description = "Universal flashing and binary manipulation tool for IoT chips"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 packages = [
     { include = "ltchiptool" },
+    { include = "ltctplugin/base" },
     { include = "uf2tool" },
 ]
 include = [
     "ltchiptool/platform.json",
     "ltchiptool/families.json",
 ]
 readme = "README.md"
@@ -20,28 +21,28 @@
 colorama = "^0.4.5"
 importlib-metadata = "^4.12.0"
 prettytable = "^3.3.0"
 bk7231tools = "^1.3.6"
 xmodem = "^0.4.6"
 wxPython = {version = "^4.2.0", optional = true}
 pywin32 = {version = "^305", optional = true, markers = "sys_platform == 'win32'"}
-py-datastruct = "^0.3.0"
+py-datastruct = "^0.4.0"
 semantic-version = "^2.10.0"
-upk2esphome = "^1.0.2"
+hexdump = "^3.3"
 
 [tool.poetry.dependencies.pycryptodomex]
 version = "^3.15.0"
 markers = "platform_machine not in 'armv6l,armv7l,armv8l,armv8b,aarch64'"
 
 [tool.poetry.dependencies.pyaes]
 version = "^1.6.1"
 markers = "platform_machine in 'armv6l,armv7l,armv8l,armv8b,aarch64'"
 
 [tool.poetry.extras]
-gui = ["wxPython", "pywin32", "upk2esphome"]
+gui = ["wxPython", "pywin32"]
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 autoflake = "^1.4"
 
 [tool.poetry.scripts]
```

### Comparing `ltchiptool-4.1.1/uf2tool/binpatch/bindiff.py` & `ltchiptool-4.2.0/uf2tool/binpatch/bindiff.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/binpatch/diff32.py` & `ltchiptool-4.2.0/uf2tool/binpatch/diff32.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/cli.py` & `ltchiptool-4.2.0/uf2tool/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/models/block.py` & `ltchiptool-4.2.0/uf2tool/models/block.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/models/context.py` & `ltchiptool-4.2.0/uf2tool/models/context.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/models/enums.py` & `ltchiptool-4.2.0/uf2tool/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/models/flags.py` & `ltchiptool-4.2.0/uf2tool/models/flags.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/models/image.py` & `ltchiptool-4.2.0/uf2tool/models/image.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/models/uf2.py` & `ltchiptool-4.2.0/uf2tool/models/uf2.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/uf2tool/writer.py` & `ltchiptool-4.2.0/uf2tool/writer.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.1/PKG-INFO` & `ltchiptool-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltchiptool
-Version: 4.1.1
+Version: 4.2.0
 Summary: Universal flashing and binary manipulation tool for IoT chips
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
 Requires-Dist: bk7231tools (>=1.3.6,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.5,<0.5.0)
+Requires-Dist: hexdump (>=3.3,<4.0)
 Requires-Dist: importlib-metadata (>=4.12.0,<5.0.0)
 Requires-Dist: prettytable (>=3.3.0,<4.0.0)
-Requires-Dist: py-datastruct (>=0.3.0,<0.4.0)
+Requires-Dist: py-datastruct (>=0.4.0,<0.5.0)
 Requires-Dist: pyaes (>=1.6.1,<2.0.0) ; platform_machine in "armv6l,armv7l,armv8l,armv8b,aarch64"
 Requires-Dist: pycryptodomex (>=3.15.0,<4.0.0) ; platform_machine not in "armv6l,armv7l,armv8l,armv8b,aarch64"
 Requires-Dist: pywin32 (>=305,<306) ; (sys_platform == "win32") and (extra == "gui")
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
-Requires-Dist: upk2esphome (>=1.0.2,<2.0.0) ; extra == "gui"
 Requires-Dist: wxPython (>=4.2.0,<5.0.0) ; extra == "gui"
 Requires-Dist: xmodem (>=0.4.6,<0.5.0)
 Description-Content-Type: text/markdown
 
 # ltchiptool
 
 Universal, easy-to-use GUI flashing/dumping tool for BK7231, RTL8710B and RTL8720C. Also contains some CLI utilities for binary firmware manipulation.
```

