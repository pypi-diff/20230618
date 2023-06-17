# Comparing `tmp/boardgen-0.7.2.tar.gz` & `tmp/boardgen-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boardgen-0.7.2.tar", max compression
+gzip compressed data, was "boardgen-0.7.3.tar", max compression
```

## Comparing `boardgen-0.7.2.tar` & `boardgen-0.7.3.tar`

### file list

```diff
@@ -1,80 +1,84 @@
--rw-r--r--   0        0        0     1076 2023-06-17 19:13:30.746490 boardgen-0.7.2/LICENSE
--rw-r--r--   0        0        0     4785 2023-06-17 19:13:30.746490 boardgen-0.7.2/README.md
--rw-r--r--   0        0        0      353 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/__init__.py
--rw-r--r--   0        0        0     9220 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/cli.py
--rw-r--r--   0        0        0       92 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/core/__init__.py
--rw-r--r--   0        0        0     2978 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/core/cache.py
--rw-r--r--   0        0        0     9861 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/core/core.py
--rw-r--r--   0        0        0     1325 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/core/getters.py
--rw-r--r--   0        0        0     1891 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/draw_util.py
--rw-r--r--   0        0        0      773 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/mixins.py
--rw-r--r--   0        0        0      439 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/board.py
--rw-r--r--   0        0        0     1015 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/enums.py
--rw-r--r--   0        0        0     1156 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/flash_region.py
--rw-r--r--   0        0        0     1257 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/pcb.py
--rw-r--r--   0        0        0     2348 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/role.py
--rw-r--r--   0        0        0      358 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/models/template.py
--rw-r--r--   0        0        0      117 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/readme/__init__.py
--rw-r--r--   0        0        0     2229 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/readme/parts.py
--rw-r--r--   0        0        0     8123 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/readme/writer.py
--rw-r--r--   0        0        0      109 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/boards/README.md
--rw-r--r--   0        0        0      589 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/flash.json
--rw-r--r--   0        0        0      974 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/presets.json
--rw-r--r--   0        0        0     1497 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/roles.json
--rw-r--r--   0        0        0      500 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/label_line_down.json
--rw-r--r--   0        0        0      526 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/label_line_up.json
--rw-r--r--   0        0        0      156 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/pad.json
--rw-r--r--   0        0        0      133 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/pad_10x25.json
--rw-r--r--   0        0        0      481 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/pin_horz_cast_hole.json
--rw-r--r--   0        0        0      311 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/pin_horz_cast_nohole.json
--rw-r--r--   0        0        0      483 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/pin_vert_cast_hole.json
--rw-r--r--   0        0        0      312 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/pin_vert_cast_nohole.json
--rw-r--r--   0        0        0      350 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/r_labels_horz.json
--rw-r--r--   0        0        0       96 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/r_pins_horz.json
--rw-r--r--   0        0        0      153 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/r_pins_vert.json
--rw-r--r--   0        0        0       80 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/test_pad_1mm.json
--rw-r--r--   0        0        0      928 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/tuya2_pcb.json
--rw-r--r--   0        0        0      922 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/shapes/tuyau_pcb.json
--rw-r--r--   0        0        0     2937 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/custom-20x24-22.json
--rw-r--r--   0        0        0     2437 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/esp12e-21.json
--rw-r--r--   0        0        0     2483 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/esp12e-22.json
--rw-r--r--   0        0        0      256 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/esp12e-shield-nohole.json
--rw-r--r--   0        0        0      233 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/esp12e-shield.json
--rw-r--r--   0        0        0      233 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/esp12s-shield.json
--rw-r--r--   0        0        0     1666 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/esp12s.json
--rw-r--r--   0        0        0     1421 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/gui-design-test.json
--rw-r--r--   0        0        0     1504 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/rf-type1.json
--rw-r--r--   0        0        0      450 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuya-16x24.json
--rw-r--r--   0        0        0      227 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuya2-shield.json
--rw-r--r--   0        0        0     1407 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuya2.json
--rw-r--r--   0        0        0      229 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuya2l-shield.json
--rw-r--r--   0        0        0     1206 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuya2l.json
--rw-r--r--   0        0        0      234 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuyau-shield.json
--rw-r--r--   0        0        0     2878 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/res/templates/tuyau.json
--rw-r--r--   0        0        0      341 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/shapes/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/shapes/base.py
--rw-r--r--   0        0        0     1158 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/shapes/circle.py
--rw-r--r--   0        0        0     1283 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/shapes/fill_style.py
--rw-r--r--   0        0        0     2489 2023-06-17 19:13:30.746490 boardgen-0.7.2/boardgen/shapes/group.py
--rw-r--r--   0        0        0      182 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/shapes/label/__init__.py
--rw-r--r--   0        0        0     1782 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/shapes/label/block.py
--rw-r--r--   0        0        0      563 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/shapes/label/io_line.py
--rw-r--r--   0        0        0     3306 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/shapes/label/label.py
--rw-r--r--   0        0        0     1120 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/shapes/rect.py
--rw-r--r--   0        0        0      867 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/shapes/text.py
--rw-r--r--   0        0        0     2428 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/utils.py
--rw-r--r--   0        0        0      119 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/variant/__init__.py
--rw-r--r--   0        0        0      362 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/variant/features.py
--rw-r--r--   0        0        0     6271 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/variant/parts.py
--rw-r--r--   0        0        0      319 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/variant/section.py
--rw-r--r--   0        0        0     8502 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/variant/writer.py
--rw-r--r--   0        0        0     8765 2023-06-17 19:13:30.750490 boardgen-0.7.2/boardgen/vector.py
--rw-r--r--   0        0        0      503 2023-06-17 19:13:30.750490 boardgen-0.7.2/ltctplugin/boardgen/__init__.py
--rw-r--r--   0        0        0     8130 2023-06-17 19:13:30.750490 boardgen-0.7.2/ltctplugin/boardgen/boardgen.wxui
--rw-r--r--   0        0        0     9556 2023-06-17 19:13:30.750490 boardgen-0.7.2/ltctplugin/boardgen/boardgen.xrc
--rw-r--r--   0        0        0    34303 2023-06-17 19:13:30.750490 boardgen-0.7.2/ltctplugin/boardgen/gui.py
--rw-r--r--   0        0        0     1321 2023-06-17 19:13:30.750490 boardgen-0.7.2/ltctplugin/boardgen/svg.py
--rw-r--r--   0        0        0     4046 2023-06-17 19:13:30.750490 boardgen-0.7.2/ltctplugin/boardgen/utils.py
--rw-r--r--   0        0        0      668 2023-06-17 19:13:30.750490 boardgen-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-17 22:11:40.998737 boardgen-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4785 2023-06-17 22:11:40.998737 boardgen-0.7.3/README.md
+-rw-r--r--   0        0        0      353 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/__init__.py
+-rw-r--r--   0        0        0     9220 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/cli.py
+-rw-r--r--   0        0        0       92 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/__init__.py
+-rw-r--r--   0        0        0     2978 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/cache.py
+-rw-r--r--   0        0        0     9861 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/core.py
+-rw-r--r--   0        0        0     1325 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/core/getters.py
+-rw-r--r--   0        0        0     1891 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/draw_util.py
+-rw-r--r--   0        0        0      773 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/mixins.py
+-rw-r--r--   0        0        0      439 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/board.py
+-rw-r--r--   0        0        0     1015 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/enums.py
+-rw-r--r--   0        0        0     1156 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/flash_region.py
+-rw-r--r--   0        0        0     1257 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/pcb.py
+-rw-r--r--   0        0        0     2348 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/role.py
+-rw-r--r--   0        0        0      358 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/models/template.py
+-rw-r--r--   0        0        0      117 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/readme/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/readme/parts.py
+-rw-r--r--   0        0        0     8123 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/readme/writer.py
+-rw-r--r--   0        0        0      109 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/boards/README.md
+-rw-r--r--   0        0        0      589 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/flash.json
+-rw-r--r--   0        0        0      974 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/presets.json
+-rw-r--r--   0        0        0     1497 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/roles.json
+-rw-r--r--   0        0        0      273 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/chip.json
+-rw-r--r--   0        0        0      500 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/label_line_down.json
+-rw-r--r--   0        0        0      526 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/label_line_up.json
+-rw-r--r--   0        0        0      174 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/osc.json
+-rw-r--r--   0        0        0      156 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pad.json
+-rw-r--r--   0        0        0      133 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pad_10x25.json
+-rw-r--r--   0        0        0      481 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_horz_cast_hole.json
+-rw-r--r--   0        0        0      311 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_horz_cast_nohole.json
+-rw-r--r--   0        0        0      483 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_vert_cast_hole.json
+-rw-r--r--   0        0        0      312 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/pin_vert_cast_nohole.json
+-rw-r--r--   0        0        0      350 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/r_labels_horz.json
+-rw-r--r--   0        0        0       96 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/r_pins_horz.json
+-rw-r--r--   0        0        0      153 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/r_pins_vert.json
+-rw-r--r--   0        0        0       80 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/test_pad_1mm.json
+-rw-r--r--   0        0        0      928 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/tuya2_pcb.json
+-rw-r--r--   0        0        0     1026 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/tuyalc5_pcb.json
+-rw-r--r--   0        0        0      922 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/shapes/tuyau_pcb.json
+-rw-r--r--   0        0        0     2937 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/custom-20x24-22.json
+-rw-r--r--   0        0        0     2437 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-21.json
+-rw-r--r--   0        0        0     2483 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-22.json
+-rw-r--r--   0        0        0      256 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-shield-nohole.json
+-rw-r--r--   0        0        0      233 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12e-shield.json
+-rw-r--r--   0        0        0      233 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12s-shield.json
+-rw-r--r--   0        0        0     1666 2023-06-17 22:11:40.998737 boardgen-0.7.3/boardgen/res/templates/esp12s.json
+-rw-r--r--   0        0        0     1421 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/gui-design-test.json
+-rw-r--r--   0        0        0     1504 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/rf-type1.json
+-rw-r--r--   0        0        0      450 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya-16x24.json
+-rw-r--r--   0        0        0      227 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2-shield.json
+-rw-r--r--   0        0        0     1407 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2.json
+-rw-r--r--   0        0        0      229 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2l-shield.json
+-rw-r--r--   0        0        0     1206 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuya2l.json
+-rw-r--r--   0        0        0     4395 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuyalc5.json
+-rw-r--r--   0        0        0      234 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuyau-shield.json
+-rw-r--r--   0        0        0     2878 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/res/templates/tuyau.json
+-rw-r--r--   0        0        0      341 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/base.py
+-rw-r--r--   0        0        0     1158 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/circle.py
+-rw-r--r--   0        0        0     1283 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/fill_style.py
+-rw-r--r--   0        0        0     2489 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/group.py
+-rw-r--r--   0        0        0      182 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/__init__.py
+-rw-r--r--   0        0        0     1782 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/block.py
+-rw-r--r--   0        0        0      563 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/io_line.py
+-rw-r--r--   0        0        0     3306 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/label/label.py
+-rw-r--r--   0        0        0     1120 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/rect.py
+-rw-r--r--   0        0        0      867 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/shapes/text.py
+-rw-r--r--   0        0        0     2428 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/utils.py
+-rw-r--r--   0        0        0      119 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/features.py
+-rw-r--r--   0        0        0     6271 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/parts.py
+-rw-r--r--   0        0        0      319 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/section.py
+-rw-r--r--   0        0        0     8502 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/variant/writer.py
+-rw-r--r--   0        0        0     8765 2023-06-17 22:11:41.002738 boardgen-0.7.3/boardgen/vector.py
+-rw-r--r--   0        0        0      503 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/__init__.py
+-rw-r--r--   0        0        0     8130 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/boardgen.wxui
+-rw-r--r--   0        0        0     9556 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/boardgen.xrc
+-rw-r--r--   0        0        0    34303 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/gui.py
+-rw-r--r--   0        0        0     1321 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/svg.py
+-rw-r--r--   0        0        0     4046 2023-06-17 22:11:41.002738 boardgen-0.7.3/ltctplugin/boardgen/utils.py
+-rw-r--r--   0        0        0      668 2023-06-17 22:11:41.002738 boardgen-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 boardgen-0.7.3/PKG-INFO
```

### Comparing `boardgen-0.7.2/LICENSE` & `boardgen-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/README.md` & `boardgen-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/cli.py` & `boardgen-0.7.3/boardgen/cli.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/core/cache.py` & `boardgen-0.7.3/boardgen/core/cache.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/core/core.py` & `boardgen-0.7.3/boardgen/core/core.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/core/getters.py` & `boardgen-0.7.3/boardgen/core/getters.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/draw_util.py` & `boardgen-0.7.3/boardgen/draw_util.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/mixins.py` & `boardgen-0.7.3/boardgen/mixins.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/models/board.py` & `boardgen-0.7.3/boardgen/models/board.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/models/enums.py` & `boardgen-0.7.3/boardgen/models/enums.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/models/flash_region.py` & `boardgen-0.7.3/boardgen/models/flash_region.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/models/pcb.py` & `boardgen-0.7.3/boardgen/models/pcb.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/models/role.py` & `boardgen-0.7.3/boardgen/models/role.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/readme/parts.py` & `boardgen-0.7.3/boardgen/readme/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/readme/writer.py` & `boardgen-0.7.3/boardgen/readme/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/flash.json` & `boardgen-0.7.3/boardgen/res/flash.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/presets.json` & `boardgen-0.7.3/boardgen/res/presets.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/roles.json` & `boardgen-0.7.3/boardgen/res/roles.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/shapes/label_line_up.json` & `boardgen-0.7.3/boardgen/res/shapes/label_line_up.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/shapes/tuya2_pcb.json` & `boardgen-0.7.3/boardgen/res/shapes/tuya2_pcb.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/shapes/tuyau_pcb.json` & `boardgen-0.7.3/boardgen/res/shapes/tuyau_pcb.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/custom-20x24-22.json` & `boardgen-0.7.3/boardgen/res/templates/custom-20x24-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/esp12e-21.json` & `boardgen-0.7.3/boardgen/res/templates/esp12e-21.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/esp12e-22.json` & `boardgen-0.7.3/boardgen/res/templates/esp12e-22.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/esp12s.json` & `boardgen-0.7.3/boardgen/res/templates/esp12s.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/gui-design-test.json` & `boardgen-0.7.3/boardgen/res/templates/gui-design-test.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/rf-type1.json` & `boardgen-0.7.3/boardgen/res/templates/rf-type1.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/tuya2.json` & `boardgen-0.7.3/boardgen/res/templates/tuya2.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/tuya2l.json` & `boardgen-0.7.3/boardgen/res/templates/tuya2l.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/res/templates/tuyau.json` & `boardgen-0.7.3/boardgen/res/templates/tuyau.json`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/base.py` & `boardgen-0.7.3/boardgen/shapes/base.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/circle.py` & `boardgen-0.7.3/boardgen/shapes/circle.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/fill_style.py` & `boardgen-0.7.3/boardgen/shapes/fill_style.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/group.py` & `boardgen-0.7.3/boardgen/shapes/group.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/label/block.py` & `boardgen-0.7.3/boardgen/shapes/label/block.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/label/io_line.py` & `boardgen-0.7.3/boardgen/shapes/label/io_line.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/label/label.py` & `boardgen-0.7.3/boardgen/shapes/label/label.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/rect.py` & `boardgen-0.7.3/boardgen/shapes/rect.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/shapes/text.py` & `boardgen-0.7.3/boardgen/shapes/text.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/utils.py` & `boardgen-0.7.3/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/variant/parts.py` & `boardgen-0.7.3/boardgen/variant/parts.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/variant/writer.py` & `boardgen-0.7.3/boardgen/variant/writer.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/boardgen/vector.py` & `boardgen-0.7.3/boardgen/vector.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/ltctplugin/boardgen/boardgen.wxui` & `boardgen-0.7.3/ltctplugin/boardgen/boardgen.wxui`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/ltctplugin/boardgen/boardgen.xrc` & `boardgen-0.7.3/ltctplugin/boardgen/boardgen.xrc`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/ltctplugin/boardgen/gui.py` & `boardgen-0.7.3/ltctplugin/boardgen/gui.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/ltctplugin/boardgen/svg.py` & `boardgen-0.7.3/ltctplugin/boardgen/svg.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/ltctplugin/boardgen/utils.py` & `boardgen-0.7.3/ltctplugin/boardgen/utils.py`

 * *Files identical despite different names*

### Comparing `boardgen-0.7.2/pyproject.toml` & `boardgen-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boardgen"
-version = "0.7.2"
+version = "0.7.3"
 description = "Board pinout diagram generator (with ltchiptool plugin GUI editor)"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "boardgen" },
     { include = "ltctplugin/boardgen" },
```

### Comparing `boardgen-0.7.2/PKG-INFO` & `boardgen-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boardgen
-Version: 0.7.2
+Version: 0.7.3
 Summary: Board pinout diagram generator (with ltchiptool plugin GUI editor)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

