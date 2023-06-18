# Comparing `tmp/py3d-0.1.4.tar.gz` & `tmp/py3d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.4.tar", last modified: Fri Jun 16 15:15:19 2023, max compression
+gzip compressed data, was "py3d-0.1.5.tar", last modified: Sun Jun 18 15:25:21 2023, max compression
```

## Comparing `py3d-0.1.4.tar` & `py3d-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 15:15:19.218850 py3d-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-16 15:15:19.218850 py3d-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-16 15:14:54.000000 py3d-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 15:15:19.218850 py3d-0.1.4/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-16 15:14:00.000000 py3d-0.1.4/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28904 2023-06-16 15:14:00.000000 py3d-0.1.4/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-06-16 15:14:00.000000 py3d-0.1.4/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 15:15:19.218850 py3d-0.1.4/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 15:15:19.000000 py3d-0.1.4/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 15:15:19.218850 py3d-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-16 15:14:00.000000 py3d-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 15:25:21.450456 py3d-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-18 15:25:21.450456 py3d-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-18 15:24:55.000000 py3d-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 15:25:21.450456 py3d-0.1.5/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-18 15:23:59.000000 py3d-0.1.5/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28904 2023-06-18 15:23:59.000000 py3d-0.1.5/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22694 2023-06-18 15:23:59.000000 py3d-0.1.5/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 15:25:21.450456 py3d-0.1.5/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-18 15:25:21.000000 py3d-0.1.5/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-18 15:25:21.450456 py3d-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-18 15:23:59.000000 py3d-0.1.5/setup.py
```

### Comparing `py3d-0.1.4/PKG-INFO` & `py3d-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.4
+Version: 0.1.5
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.4/README.md` & `py3d-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.4/py3d/core.py` & `py3d-0.1.5/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.1.4/py3d/viewer.html` & `py3d-0.1.5/py3d/viewer.html`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,19 @@
             return [
                 x ** 2 + (1 - x ** 2) * cos, -x * y * cos + x * y + z * sin, -x * z * cos + x * z - y * sin, 0,
                 -x * y * cos + x * y - z * sin, y ** 2 + (1 - y ** 2) * cos, x * sin - y * z * cos + y * z, 0,
                 -x * z * cos + x * z + y * sin, -x * sin - y * z * cos + y * z, z ** 2 + (1 - z ** 2) * cos, 0,
                 0, 0, 0, 1
             ]
         }
+        static add(a0, a1) {
+            return a0.map((item, index) => {
+                return item + a1[index];
+            });
+        }
         static vm(v, m) {
             console.assert(m.length == 16 && v.length >= 3, m, v)
             let ret = []
             for (let j of [0, 1, 2, 3]) {
                 ret.push(m[j] * v[0] + m[j + 4] * v[1] + m[j + 8] * v[2] + m[j + 12])
             }
             return ret
@@ -85,82 +90,77 @@
             ret[13] = -m[13]
             ret[14] = -m[14]
             return ret
         }
         static rgb2hex(r, g, b, a) {
             return "#" + ((1 << 24) + (r * 255 << 16) + (g * 255 << 8) + b * 255).toString(16).slice(1)
         }
-        static fround(value, digits) {
-            let tmp = 10 ** digits
-            return Math.round(value * tmp) / tmp
-        }
-        static fceil(value, digits) {
-            let tmp = 10 ** digits
-            return Math.ceil(value * tmp) / tmp
+        static floor(value, base) {
+            return Math.floor(value / base) * base
+        }
+        static ceil(value, base) {
+            return Math.ceil(value / base) * base
         }
         static ticks(min, max, step) {
             if (max <= min) {
                 return [[min], min, max]
             }
-            let dig = Math.max(0, -Math.round(Math.log10(step)))
-            let r_min = mat.fround(min, dig)
-            let r_max = mat.fround(max, dig)
-            let r_step = mat.fceil(step, dig)
+            let r_step = 10 ** Math.round(Math.log10(step))
+            let r_min = mat.floor(min, r_step)
+            let r_max = mat.ceil(max, r_step)
             let size = Math.ceil((r_max - r_min) / r_step) + 1
-            let ticks = Array.from({ length: size }, (v, i) => mat.fround(r_min + r_step * i, dig))
+            let ticks = Array.from({ length: size }, (v, i) => r_min + r_step * i)
             return [ticks, ticks[0], ticks[ticks.length - 1]]
         }
     }
     class Camera {
         PERSPECTIVE = "P"
         ORTHOGRAPHIC = "O"
         constructor(type, fovy, aspect, near, far, min, max) {
             this.fovy = fovy
             this.aspect = aspect
             this.near = -near
             this.far = -far
-            this.center = [(min[0] + max[0]) / 2, (min[1] + max[1]) / 2, (min[2] + max[2]) / 2]
+            this.origin_center = [(min[0] + max[0]) / 2, (min[1] + max[1]) / 2, (min[2] + max[2]) / 2]
+            this.center = structuredClone(this.origin_center)
             let ysize = Math.max((max[0] - min[0]) / this.aspect, max[1] - min[1]) + 2
-            Object.defineProperty(this, "origin_translation", {
-                "value": [0, 0, ysize / 2 / Math.tan(this.fovy / 2)],
-                "writable": false
-            })
-            this.translation = structuredClone(this.origin_translation)
+            this.origin_height = ysize / 2 / Math.tan(this.fovy / 2)
+            this.height = this.origin_height
             this.rotation = mat.identity() // intrinsic
             this.type = type
             this.update_projection()
         }
         position() {
-            let p = mat.vm(mat.vm(this.center, this.rotation), mat.translation(this.translation))
+            let p = mat.vm(mat.vm(this.center, this.rotation), mat.translation([0, 0, this.height]))
             return "camera position = " + p[0].toFixed(3) + ", " + p[1].toFixed(3) + ", " + p[2].toFixed(3)
         }
         update_projection() {
             this.projection = this.type == this.ORTHOGRAPHIC ? mat.orthographic(
                 this.fovy,
                 this.aspect,
                 this.near,
                 this.far,
-                this.translation[2]) : mat.perspective(this.fovy, this.aspect, this.near, this.far)
+                this.height) : mat.perspective(this.fovy, this.aspect, this.near, this.far)
         }
         reset() {
-            Object.assign(this.translation, this.origin_translation)
+            this.height = this.origin_height
+            this.center = this.origin_center
             this.rotation = mat.identity()
             this.update_projection()
         }
         resolution(width) {
-            let p = mat.vm([1, 0, this.translation[2]], this.projection)
+            let p = mat.vm([1, 0, this.height], this.projection)
             return Math.abs(2 * p[3] / p[0] / width)
         }
-        modelview() {
+        world2ndc() {
             return mat.mms(
                 mat.I(mat.translation(this.center)),
                 mat.I(this.rotation),
-                mat.I(mat.translation(this.translation)),
-                this.projection
-            )
+                mat.I(mat.translation([0, 0, this.height])),
+                this.projection)
         }
     }
     class ToolBar {
         constructor(cache) {
             this.bar = document.createElement("div")
             this.cache = cache
             this.ts = Object.keys(this.cache).sort((a, b) => { return a - b })
@@ -278,15 +278,15 @@
             this.canvasdiv.style.height = "300px"
             this.canvasdiv.style.overflow = "hidden"
             this.canvasdiv.style.resize = "vertical"
             this.canvasdiv.append(this.labeldiv, this.canvas)
             this.toolbar = new ToolBar(data.cache)
             this.min = data.min
             this.max = data.max
-            this.camera = new Camera(this.toolbar.btn_orth.innerHTML, Math.PI / 4, this.canvas.width / this.canvas.height, 0.1, 1000, data.min, data.max)
+            this.camera = new Camera(this.toolbar.btn_orth.innerHTML, Math.PI / 4, this.canvas.width / this.canvas.height, 0.1, 2000, data.min, data.max)
             this.parent = document.getElementById(id)
             this.parent.append(this.canvasdiv, this.toolbar.bar)
             const observer = new ResizeObserver(() => {
                 this.canvas.width = this.canvas.clientWidth
                 this.canvas.height = this.canvas.clientHeight
                 this.camera.aspect = this.canvas.width / this.canvas.height
                 this.camera.update_projection()
@@ -305,31 +305,30 @@
             }
             this.canvas.onmousemove = (ev) => {
                 let dx = ev.clientX - this.canvas_x
                 let dy = ev.clientY - this.canvas_y
                 let d = Math.hypot(dx, dy)
                 if (d) {
                     if (ev.ctrlKey | ev.buttons == 4) {
-                        this.camera.rotation = mat.mm(mat.angle_axis(d / 100, dy / d, dx / d, 0), this.camera.rotation)
+                        this.camera.rotation = mat.mm(mat.angle_axis(d / 100, -dy / d, dx / d, 0), this.camera.rotation)
                         this.render()
                     } else if (ev.shiftKey | ev.buttons == 1) {
-                        const ratio = this.camera.translation[2] / 200
-                        this.camera.translation[0] -= dx * ratio
-                        this.camera.translation[1] += dy * ratio
+                        const ratio = this.camera.height / 200
+                        this.camera.center = mat.add(this.camera.center, mat.vm([-dx * ratio, dy * ratio, 0], this.camera.rotation))
                         this.toolbar.tooltip.innerHTML = this.camera.position()
                         this.render()
                     }
                 }
                 this.canvas_x = ev.clientX
                 this.canvas_y = ev.clientY
             }
             this.canvas.onwheel = (ev) => {
                 ev.preventDefault()
-                let step = ev.deltaY * 10 ** (Math.round(Math.log10(this.camera.translation[2])) - 3)
-                this.camera.translation[2] = Math.max(0, this.camera.translation[2] - step)
+                let step = ev.deltaY * 10 ** (Math.round(Math.log10(this.camera.height)) - 3)
+                this.camera.height = Math.max(0, this.camera.height - step)
                 this.toolbar.tooltip.innerHTML = this.camera.position()
                 this.camera.update_projection()
                 this.render()
             }
             this.toolbar.btn_orth.onclick = (ev) => {
                 this.toolbar.btn_orth.innerHTML = this.toolbar.btn_orth.innerHTML == this.camera.ORTHOGRAPHIC ? this.camera.PERSPECTIVE : this.camera.ORTHOGRAPHIC
                 this.camera.type = this.toolbar.btn_orth.innerHTML
@@ -376,19 +375,19 @@
                 alert("webgl not work")
             }
             this.program = this.gl.createProgram()
             this.set_program(`
                 attribute vec4 position;
                 attribute vec4 color;
                 varying vec4 v_color;
-                uniform mat4 modelview;
+                uniform mat4 world2ndc;
                 void main(void) {
                     v_color = color;
                     gl_PointSize = 2.0;
-                    gl_Position = modelview * position;
+                    gl_Position = world2ndc * position;
                 }
             `, `
                 precision mediump float;
                 varying vec4 v_color;
                 void main(void) {
                     gl_FragColor = v_color;
                 } 
@@ -416,19 +415,19 @@
             this.set_shader(this.gl.VERTEX_SHADER, vertex_shader_code)
             this.set_shader(this.gl.FRAGMENT_SHADER, fragment_shader_code)
             this.gl.linkProgram(this.program)
             if (!this.gl.getProgramParameter(this.program, this.gl.LINK_STATUS)) {
                 alert('Unable to initialize the shader program: ' + this.gl.getProgramInfoLog(this.program))
             }
         }
-        drawText(text, position, color, modelview) {
+        drawText(text, position, color, world2ndc) {
             let div = document.createElement("div")
             div.innerHTML = text
             div.style.position = "absolute"
-            let p = mat.vm(position, modelview)
+            let p = mat.vm(position, world2ndc)
             let nx = p[0] / p[3]
             let ny = p[1] / p[3]
             let nz = p[2] / p[3]
             if (Math.abs(nx) <= 1 && Math.abs(ny) <= 1 && Math.abs(nz) <= 1) {
                 let x = 0.5 * (1 + nx) * this.canvas.width
                 let y = 0.5 * (1 - ny) * this.canvas.height
                 div.style.left = x + "px"
@@ -445,61 +444,63 @@
         }
         render() {
             this.labeldiv.innerHTML = ""
             this.gl.clearColor(0, 0, 0, 0)
             this.gl.enable(this.gl.DEPTH_TEST);
             this.gl.clear(this.gl.COLOR_BUFFER_BIT | this.gl.DEPTH_BUFFER_BIT);
             this.gl.useProgram(this.program)
-            let modelview = this.camera.modelview()
-            this.set_uniform("modelview", modelview)
+            let world2ndc = this.camera.world2ndc()
+            this.set_uniform("world2ndc", world2ndc)
             let current_t = this.toolbar.ts[this.toolbar.ti]
             for (let t in this.toolbar.cache) {
                 if (t == current_t) {
                     let frame = this.toolbar.cache[t]
                     for (let obj of frame) {
                         if (obj.mode == "TEXT") {
-                            this.drawText(obj.text, obj.vertex, obj.color, modelview)
+                            this.drawText(obj.text, obj.vertex, obj.color, world2ndc)
                         } else if (obj.mode) {
                             this.set_attribute("position", obj.vertex, 3)
                             this.set_attribute("color", obj.color, 4)
                             this.gl.drawArrays(this.gl[obj.mode], 0, obj.vertex.length / 3)
                         }
                     }
-                    if (this.toolbar.btn_grid.style.background == "grey") {
-                        let resolution = this.camera.resolution(this.canvas.width)
-                        this.grid(this.min, this.max, modelview, resolution)
-                    }
+                    if (this.toolbar.btn_grid.style.background == "grey")
+                        this.grid(world2ndc)
                     break
                 }
             }
         }
-        grid(min, max, modelview, resolution) {
+        grid(world2ndc) {
+            let resolution = this.camera.resolution(this.canvas.width)
             let step = 50 * resolution// meter per pixel
-            const [x_ticks, x_tick_min, x_tick_max] = mat.ticks(min[0], max[0], step)
-            const [y_ticks, y_tick_min, y_tick_max] = mat.ticks(min[1], max[1], step)
-            const [z_ticks, z_tick_min, z_tick_max] = mat.ticks(min[2], max[2], step)
+            const [x_ticks, x_tick_min, x_tick_max] = mat.ticks(this.min[0], this.max[0], step)
+            const [y_ticks, y_tick_min, y_tick_max] = mat.ticks(this.min[1], this.max[1], step)
+            const [z_ticks, z_tick_min, z_tick_max] = mat.ticks(this.min[2], this.max[2], step)
             let lines = []
             let text_color = [0.3, 0.3, 0.3, 0.6]
             for (let x of x_ticks) {
                 lines.push(x, y_tick_min, z_tick_min, x, y_tick_max, z_tick_min)
                 lines.push(x, y_tick_min, z_tick_min, x, y_tick_min, z_tick_max)
-                this.drawText(x, [x, y_tick_min, z_tick_min], text_color, modelview)
+                if (x != x_tick_min)
+                    this.drawText(x, [x, y_tick_min, z_tick_min], text_color, world2ndc)
             }
             for (let y of y_ticks) {
                 lines.push(x_tick_min, y, z_tick_min, x_tick_max, y, z_tick_min)
                 lines.push(x_tick_min, y, z_tick_min, x_tick_min, y, z_tick_max)
-                this.drawText(y, [x_tick_min, y, z_tick_min], text_color, modelview)
+                if (y != y_tick_min)
+                    this.drawText(y, [x_tick_min, y, z_tick_min], text_color, world2ndc)
             }
             for (let z of z_ticks) {
                 lines.push(x_tick_min, y_tick_min, z, x_tick_max, y_tick_min, z)
                 lines.push(x_tick_min, y_tick_min, z, x_tick_min, y_tick_max, z)
-                this.drawText(z, [x_tick_min, y_tick_min, z], text_color, modelview)
+                if (z != z_tick_min)
+                    this.drawText(z, [x_tick_min, y_tick_min, z], text_color, world2ndc)
             }
-            this.drawText("X", [x_tick_max + step, y_tick_min, z_tick_min], text_color, modelview)
-            this.drawText("Y", [x_tick_min, y_tick_max + step, z_tick_min], text_color, modelview)
-            this.drawText("Z", [x_tick_min, y_tick_min, z_tick_max + step], text_color, modelview)
+            this.drawText("X", [x_tick_max + step, y_tick_min, z_tick_min], text_color, world2ndc)
+            this.drawText("Y", [x_tick_min, y_tick_max + step, z_tick_min], text_color, world2ndc)
+            this.drawText("Z", [x_tick_min, y_tick_min, z_tick_max + step], text_color, world2ndc)
             this.set_attribute("position", lines, 3)
             this.set_attribute("color", Array.from({ length: lines.length / 3 * 4 }, (v, i) => i % 4 == 3 ? 0.6 : 0.3), 4)
             this.gl.drawArrays(this.gl.LINES, 0, lines.length / 3)
         }
     }
 </script>
```

### Comparing `py3d-0.1.4/py3d.egg-info/PKG-INFO` & `py3d-0.1.5/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.4
+Version: 0.1.5
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.4/setup.py` & `py3d-0.1.5/setup.py`

 * *Files identical despite different names*

