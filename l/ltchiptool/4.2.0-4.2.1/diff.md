# Comparing `tmp/ltchiptool-4.2.0.tar.gz` & `tmp/ltchiptool-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool-4.2.0.tar", max compression
+gzip compressed data, was "ltchiptool-4.2.1.tar", max compression
```

## Comparing `ltchiptool-4.2.0.tar` & `ltchiptool-4.2.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     1076 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/LICENSE
--rw-r--r--   0        0        0     2384 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/README.md
--rw-r--r--   0        0        0      376 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/__init__.py
--rw-r--r--   0        0        0     2769 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/__main__.py
--rw-r--r--   0        0        0      908 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/compile/elf2bin.py
--rw-r--r--   0        0        0      881 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/compile/link2bin.py
--rw-r--r--   0        0        0      502 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/__main__.py
--rw-r--r--   0        0        0     1724 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/_utils.py
--rw-r--r--   0        0        0     1610 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/file.py
--rw-r--r--   0        0        0     3192 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/read.py
--rw-r--r--   0        0        0     2442 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/split.py
--rw-r--r--   0        0        0     7188 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/flash/write.py
--rw-r--r--   0        0        0     2331 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/list.py
--rw-r--r--   0        0        0     3833 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/plugin/manage.py
--rw-r--r--   0        0        0     1022 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/plugin/run.py
--rw-r--r--   0        0        0      423 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/commands/soc.py
--rw-r--r--   0        0        0     2022 2023-06-18 15:43:28.866084 ltchiptool-4.2.0/ltchiptool/families.json
--rw-r--r--   0        0        0      127 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/__main__.py
--rw-r--r--   0        0        0     5990 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/colors.json
--rw-r--r--   0        0        0     3964 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/colors.py
--rw-r--r--   0        0        0     9477 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool-192x192.png
--rw-r--r--   0        0        0    15406 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.ico
--rw-r--r--   0        0        0    17134 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.wxui
--rw-r--r--   0        0        0    21898 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.xrc
--rw-r--r--   0        0        0    10596 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/main.py
--rw-r--r--   0        0        0       48 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/about.py
--rw-r--r--   0        0        0     5807 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/base.py
--rw-r--r--   0        0        0    17297 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/flash.py
--rw-r--r--   0        0        0     6885 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/log.py
--rw-r--r--   0        0        0    12398 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/panels/plugins.py
--rw-r--r--   0        0        0     1405 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/utils.py
--rw-r--r--   0        0        0       47 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/__init__.py
--rw-r--r--   0        0        0      950 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/base.py
--rw-r--r--   0        0        0     6041 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/flash.py
--rw-r--r--   0        0        0      798 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/plugins.py
--rw-r--r--   0        0        0     2528 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/gui/work/ports.py
--rw-r--r--   0        0        0      263 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/models/__init__.py
--rw-r--r--   0        0        0     3144 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/models/board.py
--rw-r--r--   0        0        0      155 2023-06-18 15:43:10.918024 ltchiptool-4.2.0/ltchiptool/models/enums.py
--rw-r--r--   0        0        0     5966 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/models/family.py
--rw-r--r--   0        0        0     3199 2023-06-18 15:43:28.866084 ltchiptool-4.2.0/ltchiptool/platform.json
--rw-r--r--   0        0        0      185 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/__init__.py
--rw-r--r--   0        0        0      111 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/__init__.py
--rw-r--r--   0        0        0     6198 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/binary.py
--rw-r--r--   0        0        0     6959 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/flash.py
--rw-r--r--   0        0        0      721 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/main.py
--rw-r--r--   0        0        0       48 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/util/__init__.py
--rw-r--r--   0        0        0    18071 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz/util/rtltool.py
--rw-r--r--   0        0        0      114 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/__init__.py
--rw-r--r--   0        0        0     7749 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/binary.py
--rw-r--r--   0        0        0     4791 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/flash.py
--rw-r--r--   0        0        0      648 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/main.py
--rw-r--r--   0        0        0     7691 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/parse_partition.py
--rw-r--r--   0        0        0       49 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/__init__.py
--rw-r--r--   0        0        0    17029 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/ambz2tool.py
--rw-r--r--   0        0        0       48 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/__init__.py
--rw-r--r--   0        0        0     1993 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/config.py
--rw-r--r--   0        0        0     1036 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/enums.py
--rw-r--r--   0        0        0     3188 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/headers.py
--rw-r--r--   0        0        0     5129 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/images.py
--rw-r--r--   0        0        0     4642 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/partitions.py
--rw-r--r--   0        0        0      619 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/utils.py
--rw-r--r--   0        0        0      111 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/__init__.py
--rw-r--r--   0        0        0     9025 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/binary.py
--rw-r--r--   0        0        0     8305 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/bkpackager.py
--rw-r--r--   0        0        0     6855 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/flash.py
--rw-r--r--   0        0        0      723 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/main.py
--rw-r--r--   0        0        0      317 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/__init__.py
--rw-r--r--   0        0        0     7069 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/binary.py
--rw-r--r--   0        0        0     6175 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/crypto.py
--rw-r--r--   0        0        0      515 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/models.py
--rw-r--r--   0        0        0     2940 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/rbl.py
--rw-r--r--   0        0        0     2843 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/common.py
--rw-r--r--   0        0        0     6513 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/soc/interface.py
--rw-r--r--   0        0        0       48 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/bitint.py
--rw-r--r--   0        0        0     3393 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/cli.py
--rw-r--r--   0        0        0     5642 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/crc16.py
--rw-r--r--   0        0        0     2277 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/crypto.py
--rw-r--r--   0        0        0     4441 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/curve25519.py
--rw-r--r--   0        0        0     6631 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/detection.py
--rw-r--r--   0        0        0     1987 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/dict.py
--rw-r--r--   0        0        0      252 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/env.py
--rw-r--r--   0        0        0     2661 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/fileio.py
--rw-r--r--   0        0        0     1746 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/flash.py
--rw-r--r--   0        0        0     3296 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/fwbinary.py
--rw-r--r--   0        0        0     6105 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/intbin.py
--rw-r--r--   0        0        0     5164 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/logging.py
--rw-r--r--   0        0        0     6332 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/lpm.py
--rw-r--r--   0        0        0     7308 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/lvm.py
--rw-r--r--   0        0        0     2670 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/misc.py
--rw-r--r--   0        0        0     1878 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/obj.py
--rw-r--r--   0        0        0      866 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/slice.py
--rw-r--r--   0        0        0     5747 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/streams.py
--rw-r--r--   0        0        0     1612 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/util/toolchain.py
--rw-r--r--   0        0        0      772 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltchiptool/version.py
--rw-r--r--   0        0        0      154 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltctplugin/base/__init__.py
--rw-r--r--   0        0        0     4431 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/ltctplugin/base/base.py
--rw-r--r--   0        0        0     1338 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/__init__.py
--rw-r--r--   0        0        0      251 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/__init__.py
--rw-r--r--   0        0        0      471 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/apply.py
--rw-r--r--   0        0        0     1027 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/bindiff.py
--rw-r--r--   0        0        0     1666 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/binpatch/diff32.py
--rw-r--r--   0        0        0     4306 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/cli.py
--rw-r--r--   0        0        0      360 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/block.py
--rw-r--r--   0        0        0     5803 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/context.py
--rw-r--r--   0        0        0     2210 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/enums.py
--rw-r--r--   0        0        0     1256 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/flags.py
--rw-r--r--   0        0        0     3311 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/image.py
--rw-r--r--   0        0        0      772 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/partition.py
--rw-r--r--   0        0        0     4552 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/models/uf2.py
--rw-r--r--   0        0        0      124 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/upload/__init__.py
--rw-r--r--   0        0        0     4846 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/upload/esphome.py
--rw-r--r--   0        0        0     7219 2023-06-18 15:43:10.922024 ltchiptool-4.2.0/uf2tool/writer.py
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 ltchiptool-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/LICENSE
+-rw-r--r--   0        0        0     2384 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/README.md
+-rw-r--r--   0        0        0      376 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/__init__.py
+-rw-r--r--   0        0        0     2769 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/__main__.py
+-rw-r--r--   0        0        0      908 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/compile/elf2bin.py
+-rw-r--r--   0        0        0      881 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/compile/link2bin.py
+-rw-r--r--   0        0        0      502 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/flash/__main__.py
+-rw-r--r--   0        0        0     1724 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/flash/_utils.py
+-rw-r--r--   0        0        0     1610 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/flash/file.py
+-rw-r--r--   0        0        0     3192 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/flash/read.py
+-rw-r--r--   0        0        0     2442 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/flash/split.py
+-rw-r--r--   0        0        0     7188 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/flash/write.py
+-rw-r--r--   0        0        0     2331 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/list.py
+-rw-r--r--   0        0        0     3833 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/plugin/manage.py
+-rw-r--r--   0        0        0     1022 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/plugin/run.py
+-rw-r--r--   0        0        0      423 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/commands/soc.py
+-rw-r--r--   0        0        0     2022 2023-06-18 15:54:16.992438 ltchiptool-4.2.1/ltchiptool/families.json
+-rw-r--r--   0        0        0      127 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/__main__.py
+-rw-r--r--   0        0        0     5990 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/colors.json
+-rw-r--r--   0        0        0     3964 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/colors.py
+-rw-r--r--   0        0        0     9477 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/ltchiptool-192x192.png
+-rw-r--r--   0        0        0    15406 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/ltchiptool.ico
+-rw-r--r--   0        0        0    17134 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/ltchiptool.wxui
+-rw-r--r--   0        0        0    21898 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/ltchiptool.xrc
+-rw-r--r--   0        0        0    10596 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/main.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/panels/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/panels/about.py
+-rw-r--r--   0        0        0     5807 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/panels/base.py
+-rw-r--r--   0        0        0    17297 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/panels/flash.py
+-rw-r--r--   0        0        0     6885 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/panels/log.py
+-rw-r--r--   0        0        0    12398 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/panels/plugins.py
+-rw-r--r--   0        0        0     1405 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/utils.py
+-rw-r--r--   0        0        0       47 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/work/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/work/base.py
+-rw-r--r--   0        0        0     6041 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/work/flash.py
+-rw-r--r--   0        0        0      798 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/work/plugins.py
+-rw-r--r--   0        0        0     2528 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/gui/work/ports.py
+-rw-r--r--   0        0        0      263 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/models/__init__.py
+-rw-r--r--   0        0        0     3144 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/models/board.py
+-rw-r--r--   0        0        0      155 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/models/enums.py
+-rw-r--r--   0        0        0     5966 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/models/family.py
+-rw-r--r--   0        0        0     3199 2023-06-18 15:54:16.992438 ltchiptool-4.2.1/ltchiptool/platform.json
+-rw-r--r--   0        0        0      185 2023-06-18 15:53:59.640045 ltchiptool-4.2.1/ltchiptool/soc/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz/__init__.py
+-rw-r--r--   0        0        0     6198 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz/binary.py
+-rw-r--r--   0        0        0     6959 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz/flash.py
+-rw-r--r--   0        0        0      721 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz/main.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz/util/__init__.py
+-rw-r--r--   0        0        0    18071 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz/util/rtltool.py
+-rw-r--r--   0        0        0      114 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/__init__.py
+-rw-r--r--   0        0        0     7749 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/binary.py
+-rw-r--r--   0        0        0     4791 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/flash.py
+-rw-r--r--   0        0        0      648 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/main.py
+-rw-r--r--   0        0        0     7691 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/parse_partition.py
+-rw-r--r--   0        0        0       49 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/__init__.py
+-rw-r--r--   0        0        0    17029 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/ambz2tool.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/__init__.py
+-rw-r--r--   0        0        0     1993 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/config.py
+-rw-r--r--   0        0        0     1036 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/enums.py
+-rw-r--r--   0        0        0     3188 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/headers.py
+-rw-r--r--   0        0        0     5129 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/images.py
+-rw-r--r--   0        0        0     4642 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/partitions.py
+-rw-r--r--   0        0        0      619 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/utils.py
+-rw-r--r--   0        0        0      111 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/__init__.py
+-rw-r--r--   0        0        0     9025 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/binary.py
+-rw-r--r--   0        0        0     8305 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/bkpackager.py
+-rw-r--r--   0        0        0     6855 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/flash.py
+-rw-r--r--   0        0        0      723 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/main.py
+-rw-r--r--   0        0        0      317 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/__init__.py
+-rw-r--r--   0        0        0     7069 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/binary.py
+-rw-r--r--   0        0        0     6175 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/crypto.py
+-rw-r--r--   0        0        0      515 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/models.py
+-rw-r--r--   0        0        0     2940 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/rbl.py
+-rw-r--r--   0        0        0     2843 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/common.py
+-rw-r--r--   0        0        0     6513 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/soc/interface.py
+-rw-r--r--   0        0        0       48 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/bitint.py
+-rw-r--r--   0        0        0     3393 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/cli.py
+-rw-r--r--   0        0        0     5642 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/crc16.py
+-rw-r--r--   0        0        0     2277 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/crypto.py
+-rw-r--r--   0        0        0     4441 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/curve25519.py
+-rw-r--r--   0        0        0     6631 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/detection.py
+-rw-r--r--   0        0        0     1987 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/dict.py
+-rw-r--r--   0        0        0      252 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/env.py
+-rw-r--r--   0        0        0     2661 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/fileio.py
+-rw-r--r--   0        0        0     1746 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/flash.py
+-rw-r--r--   0        0        0     3296 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/fwbinary.py
+-rw-r--r--   0        0        0     6105 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/intbin.py
+-rw-r--r--   0        0        0     5164 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/logging.py
+-rw-r--r--   0        0        0     6332 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/lpm.py
+-rw-r--r--   0        0        0     7308 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/lvm.py
+-rw-r--r--   0        0        0     2670 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/misc.py
+-rw-r--r--   0        0        0     1878 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/obj.py
+-rw-r--r--   0        0        0      866 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/slice.py
+-rw-r--r--   0        0        0     5747 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/streams.py
+-rw-r--r--   0        0        0     1612 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/util/toolchain.py
+-rw-r--r--   0        0        0      772 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltchiptool/version.py
+-rw-r--r--   0        0        0      154 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltctplugin/base/__init__.py
+-rw-r--r--   0        0        0     4431 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/ltctplugin/base/base.py
+-rw-r--r--   0        0        0     1338 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/__init__.py
+-rw-r--r--   0        0        0      251 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/binpatch/__init__.py
+-rw-r--r--   0        0        0      471 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/binpatch/apply.py
+-rw-r--r--   0        0        0     1027 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/binpatch/bindiff.py
+-rw-r--r--   0        0        0     1666 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/binpatch/diff32.py
+-rw-r--r--   0        0        0     4306 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/cli.py
+-rw-r--r--   0        0        0      360 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/block.py
+-rw-r--r--   0        0        0     5803 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/context.py
+-rw-r--r--   0        0        0     2210 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/enums.py
+-rw-r--r--   0        0        0     1256 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/flags.py
+-rw-r--r--   0        0        0     3311 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/image.py
+-rw-r--r--   0        0        0      772 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/partition.py
+-rw-r--r--   0        0        0     4552 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/models/uf2.py
+-rw-r--r--   0        0        0      124 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/upload/__init__.py
+-rw-r--r--   0        0        0     4846 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/upload/esphome.py
+-rw-r--r--   0        0        0     7219 2023-06-18 15:53:59.644045 ltchiptool-4.2.1/uf2tool/writer.py
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 ltchiptool-4.2.1/PKG-INFO
```

### Comparing `ltchiptool-4.2.0/LICENSE` & `ltchiptool-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/README.md` & `ltchiptool-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/__main__.py` & `ltchiptool-4.2.1/ltchiptool/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/compile/elf2bin.py` & `ltchiptool-4.2.1/ltchiptool/commands/compile/elf2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/compile/link2bin.py` & `ltchiptool-4.2.1/ltchiptool/commands/compile/link2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/flash/_utils.py` & `ltchiptool-4.2.1/ltchiptool/commands/flash/_utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/flash/file.py` & `ltchiptool-4.2.1/ltchiptool/commands/flash/file.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/flash/read.py` & `ltchiptool-4.2.1/ltchiptool/commands/flash/read.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/flash/split.py` & `ltchiptool-4.2.1/ltchiptool/commands/flash/split.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/flash/write.py` & `ltchiptool-4.2.1/ltchiptool/commands/flash/write.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/list.py` & `ltchiptool-4.2.1/ltchiptool/commands/list.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/plugin/manage.py` & `ltchiptool-4.2.1/ltchiptool/commands/plugin/manage.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/commands/plugin/run.py` & `ltchiptool-4.2.1/ltchiptool/commands/plugin/run.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/families.json` & `ltchiptool-4.2.1/ltchiptool/families.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/__main__.py` & `ltchiptool-4.2.1/ltchiptool/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/colors.json` & `ltchiptool-4.2.1/ltchiptool/gui/colors.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/colors.py` & `ltchiptool-4.2.1/ltchiptool/gui/colors.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool-192x192.png` & `ltchiptool-4.2.1/ltchiptool/gui/ltchiptool-192x192.png`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.ico` & `ltchiptool-4.2.1/ltchiptool/gui/ltchiptool.ico`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.wxui` & `ltchiptool-4.2.1/ltchiptool/gui/ltchiptool.wxui`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/ltchiptool.xrc` & `ltchiptool-4.2.1/ltchiptool/gui/ltchiptool.xrc`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/main.py` & `ltchiptool-4.2.1/ltchiptool/gui/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/panels/about.py` & `ltchiptool-4.2.1/ltchiptool/gui/panels/about.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/panels/base.py` & `ltchiptool-4.2.1/ltchiptool/gui/panels/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/panels/flash.py` & `ltchiptool-4.2.1/ltchiptool/gui/panels/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/panels/log.py` & `ltchiptool-4.2.1/ltchiptool/gui/panels/log.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/panels/plugins.py` & `ltchiptool-4.2.1/ltchiptool/gui/panels/plugins.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/utils.py` & `ltchiptool-4.2.1/ltchiptool/gui/utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/work/base.py` & `ltchiptool-4.2.1/ltchiptool/gui/work/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/work/flash.py` & `ltchiptool-4.2.1/ltchiptool/gui/work/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/work/plugins.py` & `ltchiptool-4.2.1/ltchiptool/gui/work/plugins.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/gui/work/ports.py` & `ltchiptool-4.2.1/ltchiptool/gui/work/ports.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/models/board.py` & `ltchiptool-4.2.1/ltchiptool/models/board.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/models/family.py` & `ltchiptool-4.2.1/ltchiptool/models/family.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/platform.json` & `ltchiptool-4.2.1/ltchiptool/platform.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz/binary.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz/flash.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz/main.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz/util/rtltool.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz/util/rtltool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/binary.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/flash.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/main.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/parse_partition.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/parse_partition.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/ambz2tool.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/ambz2tool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/config.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/config.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/enums.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/headers.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/headers.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/images.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/images.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/partitions.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/partitions.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/ambz2/util/models/utils.py` & `ltchiptool-4.2.1/ltchiptool/soc/ambz2/util/models/utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/binary.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/bkpackager.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/bkpackager.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/flash.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/main.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/binary.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/crypto.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/models.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/models.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/bk72xx/util/rbl.py` & `ltchiptool-4.2.1/ltchiptool/soc/bk72xx/util/rbl.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/common.py` & `ltchiptool-4.2.1/ltchiptool/soc/common.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/soc/interface.py` & `ltchiptool-4.2.1/ltchiptool/soc/interface.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/bitint.py` & `ltchiptool-4.2.1/ltchiptool/util/bitint.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/cli.py` & `ltchiptool-4.2.1/ltchiptool/util/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/crc16.py` & `ltchiptool-4.2.1/ltchiptool/util/crc16.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/crypto.py` & `ltchiptool-4.2.1/ltchiptool/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/curve25519.py` & `ltchiptool-4.2.1/ltchiptool/util/curve25519.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/detection.py` & `ltchiptool-4.2.1/ltchiptool/util/detection.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/dict.py` & `ltchiptool-4.2.1/ltchiptool/util/dict.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/fileio.py` & `ltchiptool-4.2.1/ltchiptool/util/fileio.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/flash.py` & `ltchiptool-4.2.1/ltchiptool/util/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/fwbinary.py` & `ltchiptool-4.2.1/ltchiptool/util/fwbinary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/intbin.py` & `ltchiptool-4.2.1/ltchiptool/util/intbin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/logging.py` & `ltchiptool-4.2.1/ltchiptool/util/logging.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/lpm.py` & `ltchiptool-4.2.1/ltchiptool/util/lpm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/lvm.py` & `ltchiptool-4.2.1/ltchiptool/util/lvm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/misc.py` & `ltchiptool-4.2.1/ltchiptool/util/misc.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/obj.py` & `ltchiptool-4.2.1/ltchiptool/util/obj.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/slice.py` & `ltchiptool-4.2.1/ltchiptool/util/slice.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/streams.py` & `ltchiptool-4.2.1/ltchiptool/util/streams.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/util/toolchain.py` & `ltchiptool-4.2.1/ltchiptool/util/toolchain.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltchiptool/version.py` & `ltchiptool-4.2.1/ltchiptool/version.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/ltctplugin/base/base.py` & `ltchiptool-4.2.1/ltctplugin/base/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/pyproject.toml` & `ltchiptool-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ltchiptool"
-version = "4.2.0"
+version = "4.2.1"
 description = "Universal flashing and binary manipulation tool for IoT chips"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 packages = [
     { include = "ltchiptool" },
     { include = "ltctplugin/base" },
     { include = "uf2tool" },
```

### Comparing `ltchiptool-4.2.0/uf2tool/binpatch/bindiff.py` & `ltchiptool-4.2.1/uf2tool/binpatch/bindiff.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/binpatch/diff32.py` & `ltchiptool-4.2.1/uf2tool/binpatch/diff32.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/cli.py` & `ltchiptool-4.2.1/uf2tool/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/block.py` & `ltchiptool-4.2.1/uf2tool/models/block.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/context.py` & `ltchiptool-4.2.1/uf2tool/models/context.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/enums.py` & `ltchiptool-4.2.1/uf2tool/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/flags.py` & `ltchiptool-4.2.1/uf2tool/models/flags.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/image.py` & `ltchiptool-4.2.1/uf2tool/models/image.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/partition.py` & `ltchiptool-4.2.1/uf2tool/models/partition.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/models/uf2.py` & `ltchiptool-4.2.1/uf2tool/models/uf2.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/upload/esphome.py` & `ltchiptool-4.2.1/uf2tool/upload/esphome.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/uf2tool/writer.py` & `ltchiptool-4.2.1/uf2tool/writer.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.2.0/PKG-INFO` & `ltchiptool-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltchiptool
-Version: 4.2.0
+Version: 4.2.1
 Summary: Universal flashing and binary manipulation tool for IoT chips
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

