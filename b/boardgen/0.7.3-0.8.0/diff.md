# Comparing `tmp/boardgen-0.7.3.tar.gz` & `tmp/boardgen-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boardgen-0.7.3.tar", max compression
+gzip compressed data, was "boardgen-0.8.0.tar", max compression
```

## Comparing `boardgen-0.7.3.tar` & `boardgen-0.8.0.tar`

### file list

```diff
@@ -1,84 +1,72 @@
--rw-r--r--   0        0        0     1076 2023-06-17 22:11:40.998737 boardgen-0.7.3/LICENSE
--rw-r--r--   0        0        0     4785 2023-06-17 22:11:40.998737 boardgen-0.7.3/README.md
--rw-r--r--   0        0        0      353 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/__init__.py
--rw-r--r--   0        0        0     9220 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/cli.py
--rw-r--r--   0        0        0       92 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/__init__.py
--rw-r--r--   0        0        0     2978 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/cache.py
--rw-r--r--   0        0        0     9861 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/core.py
--rw-r--r--   0        0        0     1325 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/getters.py
--rw-r--r--   0        0        0     1891 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/draw_util.py
--rw-r--r--   0        0        0      773 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/mixins.py
--rw-r--r--   0        0        0      439 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/board.py
--rw-r--r--   0        0        0     1015 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/enums.py
--rw-r--r--   0        0        0     1156 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/flash_region.py
--rw-r--r--   0        0        0     1257 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/pcb.py
--rw-r--r--   0        0        0     2348 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/role.py
--rw-r--r--   0        0        0      358 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/template.py
--rw-r--r--   0        0        0      117 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/readme/__init__.py
--rw-r--r--   0        0        0     2229 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/readme/parts.py
--rw-r--r--   0        0        0     8123 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/readme/writer.py
--rw-r--r--   0        0        0      109 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/boards/README.md
--rw-r--r--   0        0        0      589 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/flash.json
--rw-r--r--   0        0        0      974 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/presets.json
--rw-r--r--   0        0        0     1497 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/roles.json
--rw-r--r--   0        0        0      273 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/chip.json
--rw-r--r--   0        0        0      500 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/label_line_down.json
--rw-r--r--   0        0        0      526 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/label_line_up.json
--rw-r--r--   0        0        0      174 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/osc.json
--rw-r--r--   0        0        0      156 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pad.json
--rw-r--r--   0        0        0      133 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pad_10x25.json
--rw-r--r--   0        0        0      481 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_horz_cast_hole.json
--rw-r--r--   0        0        0      311 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_horz_cast_nohole.json
--rw-r--r--   0        0        0      483 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_vert_cast_hole.json
--rw-r--r--   0        0        0      312 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_vert_cast_nohole.json
--rw-r--r--   0        0        0      350 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/r_labels_horz.json
--rw-r--r--   0        0        0       96 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/r_pins_horz.json
--rw-r--r--   0        0        0      153 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/r_pins_vert.json
--rw-r--r--   0        0        0       80 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/test_pad_1mm.json
--rw-r--r--   0        0        0      928 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/tuya2_pcb.json
--rw-r--r--   0        0        0     1026 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/tuyalc5_pcb.json
--rw-r--r--   0        0        0      922 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/tuyau_pcb.json
--rw-r--r--   0        0        0     2937 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/custom-20x24-22.json
--rw-r--r--   0        0        0     2437 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-21.json
--rw-r--r--   0        0        0     2483 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-22.json
--rw-r--r--   0        0        0      256 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-shield-nohole.json
--rw-r--r--   0        0        0      233 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-shield.json
--rw-r--r--   0        0        0      233 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12s-shield.json
--rw-r--r--   0        0        0     1666 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12s.json
--rw-r--r--   0        0        0     1421 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/gui-design-test.json
--rw-r--r--   0        0        0     1504 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/rf-type1.json
--rw-r--r--   0        0        0      450 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya-16x24.json
--rw-r--r--   0        0        0      227 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2-shield.json
--rw-r--r--   0        0        0     1407 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2.json
--rw-r--r--   0        0        0      229 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2l-shield.json
--rw-r--r--   0        0        0     1206 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2l.json
--rw-r--r--   0        0        0     4395 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuyalc5.json
--rw-r--r--   0        0        0      234 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuyau-shield.json
--rw-r--r--   0        0        0     2878 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuyau.json
--rw-r--r--   0        0        0      341 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/base.py
--rw-r--r--   0        0        0     1158 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/circle.py
--rw-r--r--   0        0        0     1283 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/fill_style.py
--rw-r--r--   0        0        0     2489 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/group.py
--rw-r--r--   0        0        0      182 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/__init__.py
--rw-r--r--   0        0        0     1782 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/block.py
--rw-r--r--   0        0        0      563 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/io_line.py
--rw-r--r--   0        0        0     3306 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/label.py
--rw-r--r--   0        0        0     1120 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/rect.py
--rw-r--r--   0        0        0      867 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/text.py
--rw-r--r--   0        0        0     2428 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/utils.py
--rw-r--r--   0        0        0      119 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/__init__.py
--rw-r--r--   0        0        0      362 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/features.py
--rw-r--r--   0        0        0     6271 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/parts.py
--rw-r--r--   0        0        0      319 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/section.py
--rw-r--r--   0        0        0     8502 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/writer.py
--rw-r--r--   0        0        0     8765 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/vector.py
--rw-r--r--   0        0        0      503 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/__init__.py
--rw-r--r--   0        0        0     8130 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/boardgen.wxui
--rw-r--r--   0        0        0     9556 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/boardgen.xrc
--rw-r--r--   0        0        0    34303 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/gui.py
--rw-r--r--   0        0        0     1321 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/svg.py
--rw-r--r--   0        0        0     4046 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/utils.py
--rw-r--r--   0        0        0      668 2023-06-17 22:11:41.002738 boardgen-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 14:13:52.410080 boardgen-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4785 2023-06-18 14:13:52.410080 boardgen-0.8.0/README.md
+-rw-r--r--   0        0        0      353 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/__init__.py
+-rw-r--r--   0        0        0     9220 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/cli.py
+-rw-r--r--   0        0        0       92 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/__init__.py
+-rw-r--r--   0        0        0     2978 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/cache.py
+-rw-r--r--   0        0        0     9838 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/core.py
+-rw-r--r--   0        0        0     1325 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/core/getters.py
+-rw-r--r--   0        0        0     1891 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/draw_util.py
+-rw-r--r--   0        0        0      773 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/mixins.py
+-rw-r--r--   0        0        0      439 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/board.py
+-rw-r--r--   0        0        0     1015 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/enums.py
+-rw-r--r--   0        0        0     1156 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/flash_region.py
+-rw-r--r--   0        0        0     1257 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/pcb.py
+-rw-r--r--   0        0        0     2348 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/role.py
+-rw-r--r--   0        0        0      358 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/models/template.py
+-rw-r--r--   0        0        0      117 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/readme/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/readme/parts.py
+-rw-r--r--   0        0        0     8123 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/readme/writer.py
+-rw-r--r--   0        0        0      109 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/boards/README.md
+-rw-r--r--   0        0        0      589 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/flash.json
+-rw-r--r--   0        0        0      974 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/presets.json
+-rw-r--r--   0        0        0     1497 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/roles.json
+-rw-r--r--   0        0        0      273 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/chip.json
+-rw-r--r--   0        0        0      500 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/label_line_down.json
+-rw-r--r--   0        0        0      526 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/label_line_up.json
+-rw-r--r--   0        0        0      174 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/osc.json
+-rw-r--r--   0        0        0      156 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pad.json
+-rw-r--r--   0        0        0      133 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pad_10x25.json
+-rw-r--r--   0        0        0      481 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_horz_cast_hole.json
+-rw-r--r--   0        0        0      311 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_horz_cast_nohole.json
+-rw-r--r--   0        0        0      483 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_vert_cast_hole.json
+-rw-r--r--   0        0        0      312 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/pin_vert_cast_nohole.json
+-rw-r--r--   0        0        0      350 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/r_labels_horz.json
+-rw-r--r--   0        0        0       96 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/r_pins_horz.json
+-rw-r--r--   0        0        0      153 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/r_pins_vert.json
+-rw-r--r--   0        0        0       80 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/shapes/test_pad_1mm.json
+-rw-r--r--   0        0        0     2650 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/esp12e-21.json
+-rw-r--r--   0        0        0     2696 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/esp12e-22.json
+-rw-r--r--   0        0        0     1879 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/esp12s.json
+-rw-r--r--   0        0        0     1421 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/gui-design-test.json
+-rw-r--r--   0        0        0      203 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/pcb-black.json
+-rw-r--r--   0        0        0      218 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/pcb-blue-light.json
+-rw-r--r--   0        0        0      203 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/pcb-white.json
+-rw-r--r--   0        0        0     1504 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/res/templates/rf-type1.json
+-rw-r--r--   0        0        0      341 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/base.py
+-rw-r--r--   0        0        0     1158 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/circle.py
+-rw-r--r--   0        0        0     1283 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/fill_style.py
+-rw-r--r--   0        0        0     2489 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/group.py
+-rw-r--r--   0        0        0      182 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/__init__.py
+-rw-r--r--   0        0        0     1782 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/block.py
+-rw-r--r--   0        0        0      563 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/io_line.py
+-rw-r--r--   0        0        0     3306 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/label/label.py
+-rw-r--r--   0        0        0     1120 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/rect.py
+-rw-r--r--   0        0        0      867 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/shapes/text.py
+-rw-r--r--   0        0        0     2428 2023-06-18 14:13:52.410080 boardgen-0.8.0/boardgen/utils.py
+-rw-r--r--   0        0        0      119 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/features.py
+-rw-r--r--   0        0        0     6271 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/parts.py
+-rw-r--r--   0        0        0      319 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/section.py
+-rw-r--r--   0        0        0     8502 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/variant/writer.py
+-rw-r--r--   0        0        0     8765 2023-06-18 14:13:52.414080 boardgen-0.8.0/boardgen/vector.py
+-rw-r--r--   0        0        0      503 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/__init__.py
+-rw-r--r--   0        0        0     8707 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/boardgen.wxui
+-rw-r--r--   0        0        0     9995 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/boardgen.xrc
+-rw-r--r--   0        0        0    35662 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/gui.py
+-rw-r--r--   0        0        0     1321 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/svg.py
+-rw-r--r--   0        0        0     4046 2023-06-18 14:13:52.414080 boardgen-0.8.0/ltctplugin/boardgen/utils.py
+-rw-r--r--   0        0        0      668 2023-06-18 14:13:52.414080 boardgen-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.8.0/PKG-INFO
```

### Comparing `boardgen-0.7.3/LICENSE` & `boardgen-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/README.md` & `boardgen-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/cli.py` & `boardgen-0.8.0/boardgen/cli.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/core/cache.py` & `boardgen-0.8.0/boardgen/core/cache.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/core/core.py` & `boardgen-0.8.0/boardgen/core/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,36 +29,37 @@
     _dirs_boards: list[str]
     _dirs_shapes: list[str]
     _dirs_templates: list[str]
 
     def __init__(self) -> None:
         self.dir_base = join(dirname(__file__), "..", "res")
         self._dirs_boards = [
-            join(dirname(__file__), "..", "..", "..", "..", "boards"),
             join(self.dir_base, "boards"),
             "boards",
         ]
         self._dirs_shapes = [
             join(self.dir_base, "shapes"),
+            "boards/shapes",
+            "shapes",
         ]
         self._dirs_templates = [
             join(self.dir_base, "templates"),
+            "boards/templates",
+            "templates",
         ]
         self._file_presets = join(self.dir_base, "presets.json")
         self._file_roles = join(self.dir_base, "roles.json")
         self._file_flash = join(self.dir_base, "flash.json")
         self.shape_ctors = {
             ShapeType.RECT: Rect,
             ShapeType.CIRCLE: Circle,
             ShapeType.SUBSHAPE: ShapeGroup,
             ShapeType.TEXT: Text,
         }
-        self.is_libretiny = isfile(
-            join(dirname(__file__), "..", "..", "..", "..", "platform.json")
-        ) or isfile("families.json")
+        self.is_libretiny = isfile("families.json")
 
     @property
     def version(self) -> str | None:
         pyproject = join(dirname(__file__), "..", "..", "pyproject.toml")
         if isfile(pyproject):
             with open(pyproject, "r", encoding="utf-8") as f:
                 text = f.read()
@@ -222,14 +223,15 @@
             Side.BACK: [],
         }
         sources: list[HasId] = []
         all_vars = dict(pcb.vars)
         pcb.vars = all_vars
         for template_name in pcb.templates:
             template = Template(**deepcopy(self.load_template(template_name)))
+            template.vars |= pcb.vars
             all_vars |= template.vars
             template.vars = all_vars
             pcb.pads |= template.pads
             pcb.test_pads |= template.test_pads
             sources.append(template)
         sources.append(pcb)
```

### Comparing `boardgen-0.7.3/boardgen/core/getters.py` & `boardgen-0.8.0/boardgen/core/getters.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/draw_util.py` & `boardgen-0.8.0/boardgen/draw_util.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/mixins.py` & `boardgen-0.8.0/boardgen/mixins.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/models/board.py` & `boardgen-0.8.0/boardgen/models/board.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/models/enums.py` & `boardgen-0.8.0/boardgen/models/enums.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/models/flash_region.py` & `boardgen-0.8.0/boardgen/models/flash_region.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/models/pcb.py` & `boardgen-0.8.0/boardgen/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/models/role.py` & `boardgen-0.8.0/boardgen/models/role.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/readme/parts.py` & `boardgen-0.8.0/boardgen/readme/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/readme/writer.py` & `boardgen-0.8.0/boardgen/readme/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/res/flash.json` & `boardgen-0.8.0/boardgen/res/flash.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/res/presets.json` & `boardgen-0.8.0/boardgen/res/presets.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/res/roles.json` & `boardgen-0.8.0/boardgen/res/roles.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/res/shapes/label_line_up.json` & `boardgen-0.8.0/boardgen/res/shapes/label_line_up.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/res/templates/custom-20x24-22.json` & `boardgen-0.8.0/boardgen/res/templates/esp12e-22.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7404497354497355%*

 * *Differences: {"'back'": "{0: {'size': '16,24'}, 1: {'comment': 'Pins (9-16)', 'repeat': 8}, 2: {'comment': "*

 * *           "'Pins (1-8)', 'repeat': 8, 'pos': '16,8.5'}, 3: {'comment': 'Pins (17-22)', 'repeat': "*

 * *           '6}, delete: [4]}',*

 * * "'front'": "{0: {'size': '16,24'}, 2: {'comment': 'Pins (1-8)', 'repeat': 8}, 3: {'comment': "*

 * *            "'Pins (9-16)', 'repeat': 8, 'pos': '16,8.5'}, 4: {'comment': 'Pins (17-22)', "*

 * *            "'repeat': 6}, 5: {'comment': 'Pin labels (17-22)', 'repeat': 6}, insert: [(1, "*

 * *     […]*

```diff
@@ -1,141 +1,132 @@
 {
     "back": [
         {
             "comment": "PCB soldermask",
             "pos": "0,0",
             "preset": "${MASK_PRESET}",
-            "size": "20,24",
+            "size": "16,24",
             "type": "rect"
         },
         {
-            "comment": "Pins (8-15)",
+            "comment": "Pins (9-16)",
             "id": "right",
             "name": "r_pins_vert",
             "pos": "0,8.5",
-            "repeat": 7,
+            "repeat": 8,
             "vars": {
                 "PINDIR": "left"
             }
         },
         {
-            "comment": "Pins (1-7)",
+            "comment": "Pins (1-8)",
             "id": "left",
             "name": "r_pins_vert",
-            "pos": "20,8.5",
-            "repeat": 7,
+            "pos": "16,8.5",
+            "repeat": 8,
             "vars": {
                 "PINDIR": "right"
             }
         },
         {
-            "comment": "Pins (16-22)",
+            "comment": "Pins (17-22)",
             "name": "r_pins_horz",
             "pos": "3,24",
-            "repeat": 8,
-            "vars": {
-                "PINDIR": "down"
-            }
-        },
-        {
-            "comment": "Pin labels (16-22)",
-            "id": "down",
-            "name": "r_labels_horz",
-            "pos": "3,24",
-            "repeat": 8,
+            "repeat": 6,
             "vars": {
                 "PINDIR": "down"
             }
         }
     ],
     "front": [
         {
             "comment": "PCB soldermask",
             "pos": "0,0",
             "preset": "${MASK_PRESET}",
-            "size": "20,24",
+            "size": "16,24",
+            "type": "rect"
+        },
+        {
+            "comment": "Metal shielding",
+            "pos": "1.2 + 0.8 * ${PINHOLE} , 6.95",
+            "preset": "shield",
+            "size": "13.6 - 1.6 * ${PINHOLE} , 15.8",
             "type": "rect"
         },
         {
-            "comment": "Pins (1-7)",
+            "comment": "Pins (1-8)",
             "id": "left",
             "name": "r_pins_vert",
             "pos": "0,8.5",
-            "repeat": 7,
+            "repeat": 8,
             "vars": {
                 "PINDIR": "left"
             }
         },
         {
-            "comment": "Pins (8-15)",
+            "comment": "Pins (9-16)",
             "id": "right",
             "name": "r_pins_vert",
-            "pos": "20,8.5",
-            "repeat": 7,
+            "pos": "16,8.5",
+            "repeat": 8,
             "vars": {
                 "PINDIR": "right"
             }
         },
         {
-            "comment": "Pins (16-22)",
+            "comment": "Pins (17-22)",
             "name": "r_pins_horz",
             "pos": "3,24",
-            "repeat": 8,
+            "repeat": 6,
             "vars": {
                 "PINDIR": "down"
             }
         },
         {
-            "comment": "Pin labels (16-22)",
+            "comment": "Pin labels (17-22)",
             "id": "down",
             "name": "r_labels_horz",
             "pos": "3,24",
-            "repeat": 8,
+            "repeat": 6,
             "vars": {
                 "PINDIR": "down"
             }
-        },
-        {
-            "comment": "Metal shielding",
-            "pos": "1.2,6.95",
-            "preset": "shield",
-            "size": "17.6,15.8",
-            "type": "rect"
         }
     ],
     "height": 24,
-    "name": "custom-20x24-22",
+    "name": "esp12e-22",
     "pads": {
-        "1": "custom-20x24-22.front.left.pin1",
-        "10": "custom-20x24-22.front.right.pin5",
-        "11": "custom-20x24-22.front.right.pin4",
-        "12": "custom-20x24-22.front.right.pin3",
-        "13": "custom-20x24-22.front.right.pin2",
-        "14": "custom-20x24-22.front.right.pin1",
-        "15": "custom-20x24-22.front.down.label1.anchor",
-        "16": "custom-20x24-22.front.down.label2.anchor",
-        "17": "custom-20x24-22.front.down.label3.anchor",
-        "18": "custom-20x24-22.front.down.label4.anchor",
-        "19": "custom-20x24-22.front.down.label5.anchor",
-        "2": "custom-20x24-22.front.left.pin2",
-        "20": "custom-20x24-22.front.down.label6.anchor",
-        "21": "custom-20x24-22.front.down.label7.anchor",
-        "22": "custom-20x24-22.front.down.label8.anchor",
-        "3": "custom-20x24-22.front.left.pin3",
-        "4": "custom-20x24-22.front.left.pin4",
-        "5": "custom-20x24-22.front.left.pin5",
-        "6": "custom-20x24-22.front.left.pin6",
-        "7": "custom-20x24-22.front.left.pin7",
-        "8": "custom-20x24-22.front.right.pin7",
-        "9": "custom-20x24-22.front.right.pin6"
+        "1": "esp12e-22.front.left.pin1",
+        "10": "esp12e-22.front.right.pin7",
+        "11": "esp12e-22.front.right.pin6",
+        "12": "esp12e-22.front.right.pin5",
+        "13": "esp12e-22.front.right.pin4",
+        "14": "esp12e-22.front.right.pin3",
+        "15": "esp12e-22.front.right.pin2",
+        "16": "esp12e-22.front.right.pin1",
+        "17": "esp12e-22.front.down.label1.anchor",
+        "18": "esp12e-22.front.down.label2.anchor",
+        "19": "esp12e-22.front.down.label3.anchor",
+        "2": "esp12e-22.front.left.pin2",
+        "20": "esp12e-22.front.down.label4.anchor",
+        "21": "esp12e-22.front.down.label5.anchor",
+        "22": "esp12e-22.front.down.label6.anchor",
+        "3": "esp12e-22.front.left.pin3",
+        "4": "esp12e-22.front.left.pin4",
+        "5": "esp12e-22.front.left.pin5",
+        "6": "esp12e-22.front.left.pin6",
+        "7": "esp12e-22.front.left.pin7",
+        "8": "esp12e-22.front.left.pin8",
+        "9": "esp12e-22.front.right.pin8"
     },
     "test_pads": {},
-    "title": "Custom 20x24mm form factor (22-pin)",
+    "title": "ESP-12E form factor (22-pin)",
     "vars": {
+        "PINHOLE": 1,
         "PINTYPE_HORZ": "pin_horz_cast_nohole",
-        "PINTYPE_VERT": "pin_vert_cast_nohole",
+        "PINTYPE_VERT": "pin_vert_cast_<'' if ${PINHOLE} else 'no'>hole",
         "RASTER": 2,
-        "RF_H": 6.5,
-        "RF_W": 20
+        "RF_H": 6.1,
+        "RF_W": 16
     },
-    "width": 20
+    "width": 16
 }
```

### Comparing `boardgen-0.7.3/boardgen/res/templates/esp12e-21.json` & `boardgen-0.8.0/boardgen/res/templates/esp12e-21.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.976851851851852%*

 * *Differences: {"'front'": "{insert: [(1, OrderedDict([('comment', 'Metal shielding'), ('type', 'rect'), ('pos', "*

 * *            "'1.2 + 0.8 * ${PINHOLE} , 6.95'), ('size', '13.6 - 1.6 * ${PINHOLE} , 15.8'), "*

 * *            "('preset', 'shield')]))]}",*

 * * "'vars'": '{\'PINTYPE_VERT\': "pin_vert_cast_<\'\' if ${PINHOLE} else \'no\'>hole", \'PINHOLE\': '*

 * *           '1}'}*

```diff
@@ -42,14 +42,21 @@
             "comment": "PCB soldermask",
             "pos": "0,0",
             "preset": "${MASK_PRESET}",
             "size": "16,24",
             "type": "rect"
         },
         {
+            "comment": "Metal shielding",
+            "pos": "1.2 + 0.8 * ${PINHOLE} , 6.95",
+            "preset": "shield",
+            "size": "13.6 - 1.6 * ${PINHOLE} , 15.8",
+            "type": "rect"
+        },
+        {
             "comment": "Pins (1-8)",
             "id": "left",
             "name": "r_pins_vert",
             "pos": "0,8.5",
             "repeat": 8,
             "vars": {
                 "PINDIR": "left"
@@ -109,15 +116,16 @@
         "7": "esp12e-21.front.left.pin7",
         "8": "esp12e-21.front.left.pin8",
         "9": "esp12e-21.front.right.pin8"
     },
     "test_pads": {},
     "title": "ESP-12E form factor (21-pin)",
     "vars": {
+        "PINHOLE": 1,
         "PINTYPE_HORZ": "pin_horz_cast_nohole",
-        "PINTYPE_VERT": "pin_vert_cast_nohole",
+        "PINTYPE_VERT": "pin_vert_cast_<'' if ${PINHOLE} else 'no'>hole",
         "RASTER": 2,
         "RF_H": 6.1,
         "RF_W": 16
     },
     "width": 16
 }
```

### Comparing `boardgen-0.7.3/boardgen/res/templates/esp12s.json` & `boardgen-0.8.0/boardgen/res/templates/esp12s.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9694444444444444%*

 * *Differences: {"'front'": "{insert: [(1, OrderedDict([('comment', 'Metal shielding'), ('type', 'rect'), ('pos', "*

 * *            "'1.2 + 0.8 * ${PINHOLE} , 6.95'), ('size', '13.6 - 1.6 * ${PINHOLE} , 16.8'), "*

 * *            "('preset', 'shield')]))]}",*

 * * "'vars'": '{\'PINTYPE_VERT\': "pin_vert_cast_<\'\' if ${PINHOLE} else \'no\'>hole", \'PINHOLE\': '*

 * *           '0}'}*

```diff
@@ -33,14 +33,21 @@
             "comment": "PCB soldermask",
             "pos": "0,0",
             "preset": "${MASK_PRESET}",
             "size": "16,24",
             "type": "rect"
         },
         {
+            "comment": "Metal shielding",
+            "pos": "1.2 + 0.8 * ${PINHOLE} , 6.95",
+            "preset": "shield",
+            "size": "13.6 - 1.6 * ${PINHOLE} , 16.8",
+            "type": "rect"
+        },
+        {
             "comment": "Pins (1-8)",
             "id": "left",
             "name": "r_pins_vert",
             "pos": "0,8.5",
             "repeat": 8,
             "vars": {
                 "PINDIR": "left"
@@ -76,14 +83,15 @@
         "7": "esp12s.front.left.pin7",
         "8": "esp12s.front.left.pin8",
         "9": "esp12s.front.right.pin8"
     },
     "test_pads": {},
     "title": "ESP-12S form factor",
     "vars": {
-        "PINTYPE_VERT": "pin_vert_cast_nohole",
+        "PINHOLE": 0,
+        "PINTYPE_VERT": "pin_vert_cast_<'' if ${PINHOLE} else 'no'>hole",
         "RASTER": 2,
         "RF_H": 6.1,
         "RF_W": 16
     },
     "width": 16
 }
```

### Comparing `boardgen-0.7.3/boardgen/res/templates/gui-design-test.json` & `boardgen-0.8.0/boardgen/res/templates/gui-design-test.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/res/templates/rf-type1.json` & `boardgen-0.8.0/boardgen/res/templates/rf-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/base.py` & `boardgen-0.8.0/boardgen/shapes/base.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/circle.py` & `boardgen-0.8.0/boardgen/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/fill_style.py` & `boardgen-0.8.0/boardgen/shapes/fill_style.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/group.py` & `boardgen-0.8.0/boardgen/shapes/group.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/label/block.py` & `boardgen-0.8.0/boardgen/shapes/label/block.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/label/io_line.py` & `boardgen-0.8.0/boardgen/shapes/label/io_line.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/label/label.py` & `boardgen-0.8.0/boardgen/shapes/label/label.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/rect.py` & `boardgen-0.8.0/boardgen/shapes/rect.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/shapes/text.py` & `boardgen-0.8.0/boardgen/shapes/text.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/utils.py` & `boardgen-0.8.0/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/variant/parts.py` & `boardgen-0.8.0/boardgen/variant/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/variant/writer.py` & `boardgen-0.8.0/boardgen/variant/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/boardgen/vector.py` & `boardgen-0.8.0/boardgen/vector.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/ltctplugin/boardgen/boardgen.wxui` & `boardgen-0.8.0/ltctplugin/boardgen/boardgen.wxui`

 * *Files 2% similar despite different names*

#### Comparing `boardgen-0.7.3/ltctplugin/boardgen/boardgen.wxui` & `boardgen-0.8.0/ltctplugin/boardgen/boardgen.wxui`

```diff
@@ -39,16 +39,17 @@
         <node class="wxTextCtrl" style="wxTE_MULTILINE" var_name="input_data" font="Courier New,10" flags="wxEXPAND" proportion="3"/>
         <node class="wxBoxSizer" var_name="box_sizer_3" border_size="0" flags="wxEXPAND" proportion="1">
           <node class="wxBoxSizer" orientation="wxVERTICAL" var_name="box_sizer_4" border_size="0" flags="wxEXPAND" proportion="1">
             <node class="wxStaticText" label="Default variables" var_name="m_staticText_4" borders="wxTOP|wxRIGHT|wxLEFT"/>
             <node class="wxTextCtrl" style="wxTE_MULTILINE|wxTE_DONTWRAP" value="MASK__PRESET=mask__blue__light
 TRACE__COLOR=#58839B
 SILK__COLOR=white
-PINTYPE__VERT=pin__vert__2mm__cast__nohole
-PINTYPE__HORZ=pin__horz__2mm__cast__nohole
+PINHOLE=0
+PINTYPE__VERT=pin__vert__cast__nohole
+PINTYPE__HORZ=pin__horz__cast__nohole
 SYMBOL=dummy" var_name="input_vars" font="Courier New,9" flags="wxEXPAND" proportion="1"/>
           </node>
           <node class="wxBoxSizer" orientation="wxVERTICAL" var_name="box_sizer_5" border_size="0" flags="wxEXPAND" proportion="1">
             <node class="wxStaticText" label="Drawing errors" var_name="m_staticText_2" borders="wxTOP|wxRIGHT|wxLEFT"/>
             <node class="wxTextCtrl" style="wxTE_MULTILINE|wxTE_READONLY" var_name="input_error" font="Courier New,9" flags="wxEXPAND" proportion="1"/>
           </node>
         </node>
@@ -61,16 +62,22 @@
             <node class="wxMenuItem" label="LibreTiny directory" var_name="new_board_lt"/>
             <node class="wxMenuItem" label="boardgen directory" var_name="new_board_res"/>
           </node>
           <node class="submenu" label="Board base..." var_name="submenu_3">
             <node class="wxMenuItem" label="LibreTiny directory" var_name="new_board_lt_2"/>
             <node class="wxMenuItem" label="boardgen directory" var_name="new_board_res_2"/>
           </node>
-          <node class="wxMenuItem" label="Template" var_name="new_template"/>
-          <node class="wxMenuItem" label="Shape" var_name="new_shape"/>
+          <node class="submenu" label="Template..." var_name="submenu_4">
+            <node class="wxMenuItem" label="LibreTiny directory" var_name="new_board_lt_3"/>
+            <node class="wxMenuItem" label="boardgen directory" var_name="new_board_res_3"/>
+          </node>
+          <node class="submenu" label="Shape..." var_name="submenu_5">
+            <node class="wxMenuItem" label="LibreTiny directory" var_name="new_board_lt_4"/>
+            <node class="wxMenuItem" label="boardgen directory" var_name="new_board_res_4"/>
+          </node>
         </node>
         <node class="wxMenuItem" label="Rename item" var_name="rename"/>
         <node class="wxMenuItem" label="Delete item" var_name="delete"/>
         <node class="wxMenuItem" label="Duplicate item" var_name="duplicate"/>
       </node>
     </node>
   </node>
```

### Comparing `boardgen-0.7.3/ltctplugin/boardgen/boardgen.xrc` & `boardgen-0.8.0/ltctplugin/boardgen/boardgen.xrc`

 * *Files 5% similar despite different names*

#### Comparing `boardgen-0.7.3/ltctplugin/boardgen/boardgen.xrc` & `boardgen-0.8.0/ltctplugin/boardgen/boardgen.xrc`

```diff
@@ -218,23 +218,25 @@
                 <flag>wxALL|wxEXPAND</flag>
                 <border>5</border>
                 <option>1</option>
                 <object class="wxTextCtrl" name="input_vars">
                   <value>MASK__PRESET=mask__blue__light
 TRACE__COLOR=#58839B
 SILK__COLOR=white
-PINTYPE__VERT=pin__vert__2mm__cast__nohole
-PINTYPE__HORZ=pin__horz__2mm__cast__nohole
+PINHOLE=0
+PINTYPE__VERT=pin__vert__cast__nohole
+PINTYPE__HORZ=pin__horz__cast__nohole
 SYMBOL=dummy</value>
                   <style>wxTE_MULTILINE|wxTE_DONTWRAP</style>
                   <value>MASK__PRESET=mask__blue__light
 TRACE__COLOR=#58839B
 SILK__COLOR=white
-PINTYPE__VERT=pin__vert__2mm__cast__nohole
-PINTYPE__HORZ=pin__horz__2mm__cast__nohole
+PINHOLE=0
+PINTYPE__VERT=pin__vert__cast__nohole
+PINTYPE__HORZ=pin__horz__cast__nohole
 SYMBOL=dummy</value>
                   <font>
                     <size>9</size>
                     <face>Courier New</face>
                   </font>
                 </object>
               </object>
@@ -291,19 +293,31 @@
           <object class="wxMenuItem" name="new_board_lt_2">
             <label>LibreTiny directory</label>
           </object>
           <object class="wxMenuItem" name="new_board_res_2">
             <label>boardgen directory</label>
           </object>
         </object>
-        <object class="wxMenuItem" name="new_template">
-          <label>Template</label>
+        <object class="wxMenu" name="submenu_4">
+          <label>Template...</label>
+          <object class="wxMenuItem" name="new_board_lt_3">
+            <label>LibreTiny directory</label>
+          </object>
+          <object class="wxMenuItem" name="new_board_res_3">
+            <label>boardgen directory</label>
+          </object>
         </object>
-        <object class="wxMenuItem" name="new_shape">
-          <label>Shape</label>
+        <object class="wxMenu" name="submenu_5">
+          <label>Shape...</label>
+          <object class="wxMenuItem" name="new_board_lt_4">
+            <label>LibreTiny directory</label>
+          </object>
+          <object class="wxMenuItem" name="new_board_res_4">
+            <label>boardgen directory</label>
+          </object>
         </object>
       </object>
       <object class="wxMenuItem" name="rename">
         <label>Rename item</label>
       </object>
       <object class="wxMenuItem" name="delete">
         <label>Delete item</label>
```

### Comparing `boardgen-0.7.3/ltctplugin/boardgen/gui.py` & `boardgen-0.8.0/ltctplugin/boardgen/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,32 +186,52 @@
         self.Modified: wx.adv.HyperlinkCtrl = self.BindWindow(
             "label_modified",
             (wx.adv.EVT_HYPERLINK, self.OnModifiedClick),
         )
 
         self.lvm = LVM.get()
         self.core = Core()
-        self.core.add_custom_dirs(boards=join(self.lvm.path(), "boards"))
+        self.core.add_custom_dirs(
+            boards=join(self.lvm.path(), "boards"),
+            shapes=join(self.lvm.path(), "boards", "shapes"),
+            templates=join(self.lvm.path(), "boards", "templates"),
+        )
         self.core.json_hook = self.AddEditItem
 
         self.file_map = {}
         self.draw_items = {}
         self.edit_items = {}
         self.modified = {}
 
         self.ReloadLists()
 
     def GetSettings(self) -> dict:
-        return dict()
+        return dict(
+            draw_item=self.draw_item,
+            edit_item=self.edit_item and self.edit_item[0],
+            split=self.Splitter.GetSashPosition(),
+            user_vars=self.user_vars,
+        )
 
     def SetSettings(
         self,
+        draw_item: str = None,
+        edit_item: str = None,
+        split: int = None,
+        user_vars: dict[str, str] = None,
         **_,
     ) -> None:
-        pass
+        if draw_item:
+            self.draw_item = draw_item
+        if edit_item:
+            self.edit_item = edit_item
+        if split:
+            self.Splitter.SetSashPosition(split)
+        if user_vars:
+            self.user_vars = user_vars
 
     def ReloadLists(self) -> None:
         self.core.clear_cache()
         draw_selection = self.DrawItem.GetStringSelection()
         items = {}
 
         for board_name in self.core.list_json("boards"):
@@ -482,49 +502,56 @@
         owner_menu_parent: wx.Menu = owner_menu.GetParent()
         if owner_menu_parent:
             for item in owner_menu_parent.GetMenuItems():
                 if item.GetSubMenu() == owner_menu:
                     parent_label = item.GetItemLabel()
                     break
 
-        match label:
-            case "LibreTiny directory" if parent_label == "Board...":
+        match parent_label, label:
+            case "Board...", "LibreTiny directory":
                 self.CreateNewFile("boards", self.lvm.path(), INIT_BOARD)
-            case "boardgen directory" if parent_label == "Board...":
+            case "Board...", "boardgen directory":
                 self.CreateNewFile("boards", self.core.dir_base, INIT_BOARD)
 
-            case "LibreTiny directory" if parent_label == "Board base...":
+            case "Board base...", "LibreTiny directory":
                 new_name = self.AskFileName()
                 new_path = join(
                     self.lvm.path(),
                     "boards",
                     "_base",
                     f"{new_name}.json",
                 )
                 makedirs(dirname(new_path), exist_ok=True)
                 with open(new_path, "w") as f:
                     f.write("{}\n")
-            case "boardgen directory" if parent_label == "Board base...":
+            case "Board base...", "boardgen directory":
                 new_name = self.AskFileName()
                 new_path = join(
                     self.core.dir_base,
                     "boards",
                     "_base",
                     f"{new_name}.json",
                 )
                 makedirs(dirname(new_path), exist_ok=True)
                 with open(new_path, "w") as f:
                     f.write("{}\n")
 
-            case "Template":
+            case "Template...", "LibreTiny directory":
+                boards_dir = join(self.lvm.path(), "boards")
+                self.CreateNewFile("templates", boards_dir, INIT_TEMPLATE)
+            case "Template...", "boardgen directory":
                 self.CreateNewFile("templates", self.core.dir_base, INIT_TEMPLATE)
-            case "Shape":
+
+            case "Shape...", "LibreTiny directory":
+                boards_dir = join(self.lvm.path(), "boards")
+                self.CreateNewFile("shapes", boards_dir, INIT_SHAPE)
+            case "Shape...", "boardgen directory":
                 self.CreateNewFile("shapes", self.core.dir_base, INIT_SHAPE)
 
-            case "Rename item" | "Delete item" | "Duplicate item":
+            case _:
                 if self.modified:
                     wx.MessageBox("Please save the changes first", "Information")
                     return
                 if not self.edit_item:
                     return
                 draw_item = self.draw_item
                 old_path = self.file_map.get(draw_item, None)
@@ -893,14 +920,15 @@
         if value is INIT_BOARD:
             value["build"]["variant"] = name
             value["name"] = name
         if value is INIT_TEMPLATE:
             value["name"] = name
             value["title"] = name
 
+        makedirs(join(directory, item_type), exist_ok=True)
         with open(join(directory, item_type, f"{name}.json"), "w") as f:
             json.dump(value, f, indent="\t")
             f.write("\n")
         self.ReloadLists()
         self.draw_item = f"{item_type}/{name}"
         self.Svg.ClearSvg()
         self.UpdateDrawItem()
@@ -932,20 +960,29 @@
         self.modified.pop(file)
         self.Modified.SetLabel(f"Modified: {len(self.modified)}")
         self.Save.Enable(len(self.modified) > 0)
         self.Discard.Enable(len(self.modified) > 0)
         self.Revert.Enable(False)
 
     @property
-    def vars(self) -> dict[str, str]:
+    def user_vars(self) -> dict[str, str]:
         lines: list[str] = self.Vars.GetValue().splitlines()
         data = {}
         for line in lines:
             key, _, value = line.strip().partition("=")
             data[key] = value
+        return data
+
+    @user_vars.setter
+    def user_vars(self, value: dict[str, str]) -> None:
+        self.Vars.SetValue("\n".join(f"{k}={v}" for k, v in value.items()))
+
+    @property
+    def vars(self) -> dict[str, str]:
+        data = self.user_vars
         data |= self._vars
         return data
 
     @vars.setter
     def vars(self, value: dict[str, str]) -> None:
         self._vars.clear()
         self._vars.update(value)
```

### Comparing `boardgen-0.7.3/ltctplugin/boardgen/svg.py` & `boardgen-0.8.0/ltctplugin/boardgen/svg.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/ltctplugin/boardgen/utils.py` & `boardgen-0.8.0/ltctplugin/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.3/pyproject.toml` & `boardgen-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boardgen"
-version = "0.7.3"
+version = "0.8.0"
 description = "Board pinout diagram generator (with ltchiptool plugin GUI editor)"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "boardgen" },
     { include = "ltctplugin/boardgen" },
```

### Comparing `boardgen-0.7.3/PKG-INFO` & `boardgen-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boardgen
-Version: 0.7.3
+Version: 0.8.0
 Summary: Board pinout diagram generator (with ltchiptool plugin GUI editor)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

