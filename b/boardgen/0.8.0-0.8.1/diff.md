# Comparing `tmp/boardgen-0.8.0.tar.gz` & `tmp/boardgen-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boardgen-0.8.0.tar", max compression
+gzip compressed data, was "boardgen-0.8.1.tar", max compression
```

## Comparing `boardgen-0.8.0.tar` & `boardgen-0.8.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1076 2023-06-18 14:13:52.410080 boardgen-0.8.0/LICENSE
--rw-r--r--   0        0        0     4785 2023-06-18 14:13:52.410080 boardgen-0.8.0/README.md
--rw-r--r--   0        0        0      353 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/__init__.py
--rw-r--r--   0        0        0     9220 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/cli.py
--rw-r--r--   0        0        0       92 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/__init__.py
--rw-r--r--   0        0        0     2978 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/cache.py
--rw-r--r--   0        0        0     9838 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/core.py
--rw-r--r--   0        0        0     1325 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/getters.py
--rw-r--r--   0        0        0     1891 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/draw_util.py
--rw-r--r--   0        0        0      773 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/mixins.py
--rw-r--r--   0        0        0      439 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/board.py
--rw-r--r--   0        0        0     1015 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/enums.py
--rw-r--r--   0        0        0     1156 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/flash_region.py
--rw-r--r--   0        0        0     1257 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/pcb.py
--rw-r--r--   0        0        0     2348 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/role.py
--rw-r--r--   0        0        0      358 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/template.py
--rw-r--r--   0        0        0      117 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/readme/__init__.py
--rw-r--r--   0        0        0     2229 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/readme/parts.py
--rw-r--r--   0        0        0     8123 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/readme/writer.py
--rw-r--r--   0        0        0      109 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/boards/README.md
--rw-r--r--   0        0        0      589 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/flash.json
--rw-r--r--   0        0        0      974 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/presets.json
--rw-r--r--   0        0        0     1497 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/roles.json
--rw-r--r--   0        0        0      273 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/chip.json
--rw-r--r--   0        0        0      500 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/label_line_down.json
--rw-r--r--   0        0        0      526 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/label_line_up.json
--rw-r--r--   0        0        0      174 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/osc.json
--rw-r--r--   0        0        0      156 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pad.json
--rw-r--r--   0        0        0      133 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pad_10x25.json
--rw-r--r--   0        0        0      481 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_horz_cast_hole.json
--rw-r--r--   0        0        0      311 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_horz_cast_nohole.json
--rw-r--r--   0        0        0      483 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_vert_cast_hole.json
--rw-r--r--   0        0        0      312 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_vert_cast_nohole.json
--rw-r--r--   0        0        0      350 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/r_labels_horz.json
--rw-r--r--   0        0        0       96 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/r_pins_horz.json
--rw-r--r--   0        0        0      153 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/r_pins_vert.json
--rw-r--r--   0        0        0       80 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/test_pad_1mm.json
--rw-r--r--   0        0        0     2650 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/esp12e-21.json
--rw-r--r--   0        0        0     2696 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/esp12e-22.json
--rw-r--r--   0        0        0     1879 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/esp12s.json
--rw-r--r--   0        0        0     1421 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/gui-design-test.json
--rw-r--r--   0        0        0      203 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/pcb-black.json
--rw-r--r--   0        0        0      218 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/pcb-blue-light.json
--rw-r--r--   0        0        0      203 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/pcb-white.json
--rw-r--r--   0        0        0     1504 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/rf-type1.json
--rw-r--r--   0        0        0      341 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/base.py
--rw-r--r--   0        0        0     1158 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/circle.py
--rw-r--r--   0        0        0     1283 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/fill_style.py
--rw-r--r--   0        0        0     2489 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/group.py
--rw-r--r--   0        0        0      182 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/__init__.py
--rw-r--r--   0        0        0     1782 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/block.py
--rw-r--r--   0        0        0      563 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/io_line.py
--rw-r--r--   0        0        0     3306 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/label.py
--rw-r--r--   0        0        0     1120 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/rect.py
--rw-r--r--   0        0        0      867 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/text.py
--rw-r--r--   0        0        0     2428 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/utils.py
--rw-r--r--   0        0        0      119 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/__init__.py
--rw-r--r--   0        0        0      362 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/features.py
--rw-r--r--   0        0        0     6271 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/parts.py
--rw-r--r--   0        0        0      319 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/section.py
--rw-r--r--   0        0        0     8502 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/writer.py
--rw-r--r--   0        0        0     8765 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/vector.py
--rw-r--r--   0        0        0      503 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/__init__.py
--rw-r--r--   0        0        0     8707 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/boardgen.wxui
--rw-r--r--   0        0        0     9995 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/boardgen.xrc
--rw-r--r--   0        0        0    35662 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/gui.py
--rw-r--r--   0        0        0     1321 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/svg.py
--rw-r--r--   0        0        0     4046 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/utils.py
--rw-r--r--   0        0        0      668 2023-06-18 14:13:52.414080 boardgen-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 18:47:16.071004 boardgen-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4785 2023-06-18 18:47:16.071004 boardgen-0.8.1/README.md
+-rw-r--r--   0        0        0      353 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/__init__.py
+-rw-r--r--   0        0        0     9220 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/cli.py
+-rw-r--r--   0        0        0       92 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/core/__init__.py
+-rw-r--r--   0        0        0     2978 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/core/cache.py
+-rw-r--r--   0        0        0     9838 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/core/core.py
+-rw-r--r--   0        0        0     1325 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/core/getters.py
+-rw-r--r--   0        0        0     1891 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/draw_util.py
+-rw-r--r--   0        0        0      773 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/mixins.py
+-rw-r--r--   0        0        0      439 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/board.py
+-rw-r--r--   0        0        0     1015 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/enums.py
+-rw-r--r--   0        0        0     1156 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/flash_region.py
+-rw-r--r--   0        0        0     1257 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/pcb.py
+-rw-r--r--   0        0        0     2348 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/role.py
+-rw-r--r--   0        0        0      358 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/models/template.py
+-rw-r--r--   0        0        0      117 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/readme/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-18 18:47:16.071004 boardgen-0.8.1/boardgen/readme/parts.py
+-rw-r--r--   0        0        0     8123 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/readme/writer.py
+-rw-r--r--   0        0        0      109 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/boards/README.md
+-rw-r--r--   0        0        0      589 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/flash.json
+-rw-r--r--   0        0        0      974 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/presets.json
+-rw-r--r--   0        0        0     1497 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/roles.json
+-rw-r--r--   0        0        0      273 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/chip.json
+-rw-r--r--   0        0        0      500 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/label_line_down.json
+-rw-r--r--   0        0        0      526 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/label_line_up.json
+-rw-r--r--   0        0        0      174 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/osc.json
+-rw-r--r--   0        0        0      156 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/pad.json
+-rw-r--r--   0        0        0      133 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/pad_10x25.json
+-rw-r--r--   0        0        0      481 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/pin_horz_cast_hole.json
+-rw-r--r--   0        0        0      311 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/pin_horz_cast_nohole.json
+-rw-r--r--   0        0        0      483 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/pin_vert_cast_hole.json
+-rw-r--r--   0        0        0      312 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/pin_vert_cast_nohole.json
+-rw-r--r--   0        0        0      350 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/r_labels_horz.json
+-rw-r--r--   0        0        0       96 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/r_pins_horz.json
+-rw-r--r--   0        0        0      153 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/r_pins_vert.json
+-rw-r--r--   0        0        0       80 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/shapes/test_pad_1mm.json
+-rw-r--r--   0        0        0     2650 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/esp12e-21.json
+-rw-r--r--   0        0        0     2696 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/esp12e-22.json
+-rw-r--r--   0        0        0     1879 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/esp12s.json
+-rw-r--r--   0        0        0     1421 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/gui-design-test.json
+-rw-r--r--   0        0        0      203 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/pcb-black.json
+-rw-r--r--   0        0        0      218 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/pcb-blue-light.json
+-rw-r--r--   0        0        0      203 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/pcb-white.json
+-rw-r--r--   0        0        0     1504 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/res/templates/rf-type1.json
+-rw-r--r--   0        0        0      341 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/base.py
+-rw-r--r--   0        0        0     1158 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/circle.py
+-rw-r--r--   0        0        0     1283 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/fill_style.py
+-rw-r--r--   0        0        0     2489 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/group.py
+-rw-r--r--   0        0        0      182 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/label/__init__.py
+-rw-r--r--   0        0        0     1782 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/label/block.py
+-rw-r--r--   0        0        0      563 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/label/io_line.py
+-rw-r--r--   0        0        0     3306 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/label/label.py
+-rw-r--r--   0        0        0     1120 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/rect.py
+-rw-r--r--   0        0        0      867 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/shapes/text.py
+-rw-r--r--   0        0        0     2428 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/utils.py
+-rw-r--r--   0        0        0      119 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/variant/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/variant/features.py
+-rw-r--r--   0        0        0     6271 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/variant/parts.py
+-rw-r--r--   0        0        0      319 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/variant/section.py
+-rw-r--r--   0        0        0     8502 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/variant/writer.py
+-rw-r--r--   0        0        0     8765 2023-06-18 18:47:16.075004 boardgen-0.8.1/boardgen/vector.py
+-rw-r--r--   0        0        0      503 2023-06-18 18:47:16.075004 boardgen-0.8.1/ltctplugin/boardgen/__init__.py
+-rw-r--r--   0        0        0     8707 2023-06-18 18:47:16.075004 boardgen-0.8.1/ltctplugin/boardgen/boardgen.wxui
+-rw-r--r--   0        0        0     9995 2023-06-18 18:47:16.075004 boardgen-0.8.1/ltctplugin/boardgen/boardgen.xrc
+-rw-r--r--   0        0        0    37448 2023-06-18 18:47:16.075004 boardgen-0.8.1/ltctplugin/boardgen/gui.py
+-rw-r--r--   0        0        0     1321 2023-06-18 18:47:16.075004 boardgen-0.8.1/ltctplugin/boardgen/svg.py
+-rw-r--r--   0        0        0     4046 2023-06-18 18:47:16.075004 boardgen-0.8.1/ltctplugin/boardgen/utils.py
+-rw-r--r--   0        0        0      668 2023-06-18 18:47:16.079004 boardgen-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.8.1/PKG-INFO
```

### Comparing `boardgen-0.8.0/LICENSE` & `boardgen-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/README.md` & `boardgen-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/cli.py` & `boardgen-0.8.1/boardgen/cli.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/core/cache.py` & `boardgen-0.8.1/boardgen/core/cache.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/core/core.py` & `boardgen-0.8.1/boardgen/core/core.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/core/getters.py` & `boardgen-0.8.1/boardgen/core/getters.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/draw_util.py` & `boardgen-0.8.1/boardgen/draw_util.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/mixins.py` & `boardgen-0.8.1/boardgen/mixins.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/models/board.py` & `boardgen-0.8.1/boardgen/models/board.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/models/enums.py` & `boardgen-0.8.1/boardgen/models/enums.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/models/flash_region.py` & `boardgen-0.8.1/boardgen/models/flash_region.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/models/pcb.py` & `boardgen-0.8.1/boardgen/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/models/role.py` & `boardgen-0.8.1/boardgen/models/role.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/readme/parts.py` & `boardgen-0.8.1/boardgen/readme/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/readme/writer.py` & `boardgen-0.8.1/boardgen/readme/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/flash.json` & `boardgen-0.8.1/boardgen/res/flash.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/presets.json` & `boardgen-0.8.1/boardgen/res/presets.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/roles.json` & `boardgen-0.8.1/boardgen/res/roles.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/shapes/label_line_up.json` & `boardgen-0.8.1/boardgen/res/shapes/label_line_up.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/templates/esp12e-21.json` & `boardgen-0.8.1/boardgen/res/templates/esp12e-21.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/templates/esp12e-22.json` & `boardgen-0.8.1/boardgen/res/templates/esp12e-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/templates/esp12s.json` & `boardgen-0.8.1/boardgen/res/templates/esp12s.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/templates/gui-design-test.json` & `boardgen-0.8.1/boardgen/res/templates/gui-design-test.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/res/templates/rf-type1.json` & `boardgen-0.8.1/boardgen/res/templates/rf-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/base.py` & `boardgen-0.8.1/boardgen/shapes/base.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/circle.py` & `boardgen-0.8.1/boardgen/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/fill_style.py` & `boardgen-0.8.1/boardgen/shapes/fill_style.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/group.py` & `boardgen-0.8.1/boardgen/shapes/group.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/label/block.py` & `boardgen-0.8.1/boardgen/shapes/label/block.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/label/io_line.py` & `boardgen-0.8.1/boardgen/shapes/label/io_line.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/label/label.py` & `boardgen-0.8.1/boardgen/shapes/label/label.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/rect.py` & `boardgen-0.8.1/boardgen/shapes/rect.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/shapes/text.py` & `boardgen-0.8.1/boardgen/shapes/text.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/utils.py` & `boardgen-0.8.1/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/variant/parts.py` & `boardgen-0.8.1/boardgen/variant/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/variant/writer.py` & `boardgen-0.8.1/boardgen/variant/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/boardgen/vector.py` & `boardgen-0.8.1/boardgen/vector.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/ltctplugin/boardgen/boardgen.wxui` & `boardgen-0.8.1/ltctplugin/boardgen/boardgen.wxui`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/ltctplugin/boardgen/boardgen.xrc` & `boardgen-0.8.1/ltctplugin/boardgen/boardgen.xrc`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/ltctplugin/boardgen/gui.py` & `boardgen-0.8.1/ltctplugin/boardgen/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ltchiptool import Family
 from ltchiptool.gui.panels.base import BasePanel
 from ltchiptool.gui.utils import on_event, with_event
 from ltchiptool.util.lvm import LVM
 
 from boardgen import Core, HasVars, V
 from boardgen.draw_util import draw_shapes, get_pcb_images
-from boardgen.models import Board, Template
+from boardgen.models import Board, RoleType, Template
 from boardgen.shapes import Shape, ShapeGroup
 
 from .svg import SvgPanel
 from .utils import jsonpath, jsonwalk
 
 INIT_BOARD = {
     "_base": [],
@@ -49,16 +49,15 @@
     "back": [],
     "pads": {},
     "test_pads": {},
 }
 INIT_SHAPE = []
 ROLE_DEFAULTS: dict[str, str | int | None] = {
     "ADC": 0,
-    "ARD_A": "A0",
-    "ARD_D": "D0",
+    "ARD": "D0",
     "CTRL": "CEN",
     "C_NAME": "GPIO_00",
     "DVP": "PD0",
     "FLASH": "^FCS",
     "GND": None,
     "GPIO": "P0",
     "GPIONUM": 35,
@@ -348,17 +347,19 @@
 
     def UpdateEditItem(self) -> None:
         item = self.edit_item
         if not item:
             return
         item_name, obj = item
         self.edit_selection = item_name
+        scroll_pos = self.Data.GetScrollPos(wx.VERTICAL)
         cursor_pos = self.Data.GetInsertionPoint()
         self.Data.ChangeValue(json.dumps(obj, indent=4))
         self.Data.SetInsertionPoint(cursor_pos)
+        self.Data.SetScrollPos(wx.VERTICAL, scroll_pos)
         self.Format.Enable(True)
         self.Revert.Enable(item_name in self.modified)
         self.UpdateDataPosition()
         if "pcb" in obj:
             obj = obj["pcb"]
         self.vars = obj["vars"] if "vars" in obj else {}
 
@@ -751,28 +752,66 @@
                     selected=this_value,
                     sort=False,
                     anchor=self.Choose,
                 )
             case EditType.ROLE:
                 roles = set(i.name for i in self.core.roles.keys())
                 roles.update(ROLE_DEFAULTS.keys())
+                roles = sorted(roles)
+                roles.remove("IC")
+                roles.insert(0, "IC")
                 role = self.AskSingleChoice(
                     title="Choose pin role to add",
-                    items=list(roles),
+                    items=roles,
+                    sort=False,
                     anchor=self.Choose,
                 )
-                if role not in this_dict:
-                    this_dict[role] = ROLE_DEFAULTS.get(role, "")
+                if not role:
+                    return
+                role_value = ROLE_DEFAULTS.get(role, "")
+                if (
+                    role == "IC"
+                    and self.draw_item.startswith("boards/")
+                    and self.draw_object
+                    and self.draw_object.pcb
+                    and self.draw_object.pcb.ic
+                ):
+                    ic_pins = {}
+                    for ic_pin, role_map in self.draw_object.pcb.ic.items():
+                        pin_roles = []
+                        for role_type, functions in role_map.items():
+                            if role_type == RoleType.IO:
+                                continue
+                            role_obj = self.core.role(role_type)
+                            if not role_obj:
+                                continue
+                            pin_roles += role_obj.format(functions, long=False)
+                        ic_pins[" / ".join(pin_roles)] = ic_pin
+                    ic_role = self.AskSingleChoice(
+                        title="Choose pin to add",
+                        items=list(ic_pins.keys()),
+                        anchor=self.Choose,
+                    )
+                    if not ic_role:
+                        return
+                    role_value = ic_pins[ic_role]
+                ex_roles = ["PWR", "GND", "NC"]
+                for ex_role in ex_roles:
+                    if role == ex_role:
+                        this_dict.clear()
+                    else:
+                        this_dict.pop(ex_role, None)
+                this_dict[role] = role_value
             case EditType.FLASH:
                 region = self.AskSingleChoice(
                     title="Choose flash region to add",
                     items=list(self.core.flash.keys()),
                     anchor=self.Choose,
                 )
-                if region in this_dict:
+                if region not in this_dict:
                     this_dict[region] = "0x000000+0x0000"
             # other
             case EditType.COLOR:
                 cdata = wx.ColourData()
                 cdata.SetChooseFull(True)
                 cdata.SetChooseAlpha(False)
                 cdata.SetColour(this_value)
@@ -785,18 +824,18 @@
                     color: wx.Colour = cdata.GetColour()
                     new_value = color.GetAsString(wx.C2S_NAME | wx.C2S_HTML_SYNTAX)
                     new_value = new_value.replace(" ", "")
                 dialog.Destroy()
 
         if new_value and new_value != this_value and isinstance(parent, (dict, list)):
             parent[key] = new_value
-        if new_dict and new_dict is not this_dict:
+        elif new_dict and new_dict is not this_dict:
             this_dict.clear()
             this_dict.update(new_dict)
-        if new_list and new_list is not this_list:
+        elif new_list and new_list is not this_list:
             this_list.clear()
             this_list += new_list
         self.UpdateEditItem()
         self.UpdateDrawItem()
         self.MarkModified()
 
     def AskFileName(self, value: str = "") -> str | None:
@@ -833,15 +872,15 @@
             items.insert(0, item)
 
         if anchor:
             menu = wx.Menu()
             for item in items:
                 menu_item: wx.MenuItem = menu.AppendCheckItem(wx.ID_ANY, item)
                 menu_item.Check(item in selected)
-            if anchor.PopupMenu(menu):
+            if anchor.PopupMenu(menu, 0, 25):
                 choice = [
                     items[idx]
                     for idx, item in enumerate(menu.GetMenuItems())
                     if item.IsChecked()
                 ]
             menu.Destroy()
         else:
@@ -873,24 +912,24 @@
 
         if anchor:
             menu = wx.Menu()
             if selected:
                 for item in items:
                     menu_item: wx.MenuItem = menu.AppendRadioItem(wx.ID_ANY, item)
                     menu_item.Check(item == selected)
-                if anchor.PopupMenu(menu):
+                if anchor.PopupMenu(menu, 0, 25):
                     choice = next(
                         items[idx]
                         for idx, item in enumerate(menu.GetMenuItems())
                         if item.IsChecked()
                     )
             else:
                 for item in items:
                     menu.Append(wx.ID_ANY, item)
-                selection = anchor.GetPopupMenuSelectionFromUser(menu)
+                selection = anchor.GetPopupMenuSelectionFromUser(menu, 0, 25)
                 if selection != -1:
                     for i, item in enumerate(items):
                         if menu.FindItemByPosition(i).GetId() == selection:
                             choice = item
                             break
             menu.Destroy()
         else:
```

### Comparing `boardgen-0.8.0/ltctplugin/boardgen/svg.py` & `boardgen-0.8.1/ltctplugin/boardgen/svg.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/ltctplugin/boardgen/utils.py` & `boardgen-0.8.1/ltctplugin/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.8.0/pyproject.toml` & `boardgen-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boardgen"
-version = "0.8.0"
+version = "0.8.1"
 description = "Board pinout diagram generator (with ltchiptool plugin GUI editor)"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "boardgen" },
     { include = "ltctplugin/boardgen" },
```

### Comparing `boardgen-0.8.0/PKG-INFO` & `boardgen-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boardgen
-Version: 0.8.0
+Version: 0.8.1
 Summary: Board pinout diagram generator (with ltchiptool plugin GUI editor)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

