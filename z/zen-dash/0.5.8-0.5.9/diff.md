# Comparing `tmp/zen_dash-0.5.8.tar.gz` & `tmp/zen_dash-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_dash-0.5.8.tar", max compression
+gzip compressed data, was "zen_dash-0.5.9.tar", max compression
```

## Comparing `zen_dash-0.5.8.tar` & `zen_dash-0.5.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.5.8/LICENSE
--rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.5.8/README.md
--rw-r--r--   0        0        0     1281 2023-05-29 16:13:15.181817 zen_dash-0.5.8/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.5.8/zen_dash/__init__.py
--rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.5.8/zen_dash/cli/__init__.py
--rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.5.8/zen_dash/cli/main.py
--rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.5.8/zen_dash/cli/project_management.py
--rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/flex_data.py
--rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/instances.py
--rw-r--r--   0        0        0     1283 2023-05-05 02:57:58.536338 zen_dash-0.5.8/zen_dash/objects/__init__.py
--rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/objects/flex_data.py
--rw-r--r--   0        0        0    12356 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/objects/instances.py
--rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/objects/page.py
--rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/objects/scripts.py
--rw-r--r--   0        0        0      720 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/objects/sidebar.py
--rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/page.py
--rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/route.py
--rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/scripts.py
--rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.5.8/zen_dash/sidebar.py
--rw-r--r--   0        0        0  1017714 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/275.44cd52f9d992445f.js
--rw-r--r--   0        0        0    57081 2023-05-28 22:24:38.224031 zen_dash-0.5.8/zen_dash/static/3rdpartylicenses.txt
--rw-r--r--   0        0        0   128180 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
--rw-r--r--   0        0        0   143258 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
--rw-r--r--   0        0        0    44300 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
--rw-r--r--   0        0        0    57620 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
--rw-r--r--   0        0        0      948 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/favicon.ico
--rw-r--r--   0        0        0     2137 2023-05-28 22:24:38.960041 zen_dash-0.5.8/zen_dash/static/index.html
--rw-r--r--   0        0        0    85970 2023-05-28 22:03:36.786349 zen_dash-0.5.8/zen_dash/static/main.8dfb947bbad7d7cf.js
--rw-r--r--   0        0        0    33759 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/polyfills.0a8881ff36766b1e.js
--rw-r--r--   0        0        0     3285 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/runtime.6a9b461ae5a72237.js
--rw-r--r--   0        0        0   152653 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/styles.362a8260c32d36d9.css
--rw-r--r--   0        0        0  3061083 2023-05-28 21:00:33.782603 zen_dash-0.5.8/zen_dash/static/vendor.43228e876ccc446f.js
--rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.5.8/zen_dash/support/__init__.py
--rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.5.8/zen_dash/support/encoder.py
--rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.5.8/zen_dash/tag/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.5.8/zen_dash/websocket/__init__.py
--rw-r--r--   0        0        0     9010 2023-05-29 16:13:31.245629 zen_dash-0.5.8/setup.py
--rw-r--r--   0        0        0     8752 2023-05-29 16:13:31.245935 zen_dash-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.5.9/LICENSE
+-rw-r--r--   0        0        0     7781 2023-05-05 01:59:51.099742 zen_dash-0.5.9/README.md
+-rw-r--r--   0        0        0     1281 2023-06-16 01:54:02.529644 zen_dash-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.5.9/zen_dash/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.5.9/zen_dash/cli/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.5.9/zen_dash/cli/main.py
+-rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.5.9/zen_dash/cli/project_management.py
+-rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/flex_data.py
+-rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/instances.py
+-rw-r--r--   0        0        0     1283 2023-05-05 02:57:58.536338 zen_dash-0.5.9/zen_dash/objects/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/objects/flex_data.py
+-rw-r--r--   0        0        0    12356 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/objects/instances.py
+-rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/objects/page.py
+-rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/objects/scripts.py
+-rw-r--r--   0        0        0      750 2023-06-16 02:37:03.983233 zen_dash-0.5.9/zen_dash/objects/sidebar.py
+-rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/page.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/route.py
+-rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/scripts.py
+-rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.5.9/zen_dash/sidebar.py
+-rw-r--r--   0        0        0  1017714 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/275.44cd52f9d992445f.js
+-rw-r--r--   0        0        0    57081 2023-06-16 16:45:36.150328 zen_dash-0.5.9/zen_dash/static/3rdpartylicenses.txt
+-rw-r--r--   0        0        0   128180 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
+-rw-r--r--   0        0        0   143258 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
+-rw-r--r--   0        0        0    44300 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
+-rw-r--r--   0        0        0    57620 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
+-rw-r--r--   0        0        0      948 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/favicon.ico
+-rw-r--r--   0        0        0     2137 2023-06-16 16:45:36.738336 zen_dash-0.5.9/zen_dash/static/index.html
+-rw-r--r--   0        0        0    88222 2023-06-16 16:45:29.874239 zen_dash-0.5.9/zen_dash/static/main.ff31141e0ae54f2d.js
+-rw-r--r--   0        0        0    33759 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/polyfills.0a8881ff36766b1e.js
+-rw-r--r--   0        0        0     3285 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/runtime.6a9b461ae5a72237.js
+-rw-r--r--   0        0        0   152653 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/styles.362a8260c32d36d9.css
+-rw-r--r--   0        0        0  3061114 2023-06-16 16:43:13.088321 zen_dash-0.5.9/zen_dash/static/vendor.923d0d3ca0754580.js
+-rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.5.9/zen_dash/support/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.5.9/zen_dash/support/encoder.py
+-rw-r--r--   0        0        0     7055 2023-05-29 16:12:36.409345 zen_dash-0.5.9/zen_dash/tag/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.5.9/zen_dash/websocket/__init__.py
+-rw-r--r--   0        0        0     9010 2023-06-16 16:46:46.176340 zen_dash-0.5.9/setup.py
+-rw-r--r--   0        0        0     8752 2023-06-16 16:46:46.176690 zen_dash-0.5.9/PKG-INFO
```

### Comparing `zen_dash-0.5.8/LICENSE` & `zen_dash-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/README.md` & `zen_dash-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/pyproject.toml` & `zen_dash-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen_dash"
-version = "0.5.8"
+version = "0.5.9"
 license = "MIT"
 description = "Simple yet scable and production ready python dashboard that is better than shiny application for business."
 readme = "README.md"
 authors = ["Zen <zenreportz@pm.me>"]
 homepage = "https://zen-reportz.github.io/zen_dash/index.html"
 repository = "https://github.com/Zen-Reportz/zen_dash"
 include = [
```

### Comparing `zen_dash-0.5.8/zen_dash/cli/project_management.py` & `zen_dash-0.5.9/zen_dash/cli/project_management.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/objects/__init__.py` & `zen_dash-0.5.9/zen_dash/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/objects/instances.py` & `zen_dash-0.5.9/zen_dash/objects/instances.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/objects/scripts.py` & `zen_dash-0.5.9/zen_dash/objects/scripts.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/objects/sidebar.py` & `zen_dash-0.5.9/zen_dash/objects/sidebar.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,11 +19,12 @@
     tabs: List[Union[SidebarTab, SidebarGroup]]
     filters: List[FilterInfo]
     size: str = '300px'
     library_version: str = version("zen-dash")
 
     @validator('tabs')
     def first_cant_be_group(cls, v):
-        if not isinstance(v[0], SidebarTab):
-            raise Exception("First tab can't be SidebarGroup")
+        if len(v)> 1:
+            if not isinstance(v[0], SidebarTab):
+                raise Exception("First tab can't be SidebarGroup")
         return v
```

### Comparing `zen_dash-0.5.8/zen_dash/page.py` & `zen_dash-0.5.9/zen_dash/page.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/275.44cd52f9d992445f.js` & `zen_dash-0.5.9/zen_dash/static/275.44cd52f9d992445f.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/3rdpartylicenses.txt` & `zen_dash-0.5.9/zen_dash/static/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf` & `zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot` & `zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2` & `zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff` & `zen_dash-0.5.9/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/favicon.ico` & `zen_dash-0.5.9/zen_dash/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/index.html` & `zen_dash-0.5.9/zen_dash/static/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,14 @@
   <title>Frontend</title>
   <base href="./">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <link rel="icon" type="image/x-icon" href="favicon.ico">
   <!-- <link rel="preconnect" href="https://fonts.gstatic.com">
   <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">
   <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"> -->
-  <style type="text/css">@font-face{font-family:'Material Symbols Outlined';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialsymbolsoutlined/v114/kJF1BvYX7BgnkSrUwT8OhrdQw4oELdPIeeII9v6oDMzByHX9rA6RzaxHMPdY43zj-jCxv3fzvRNU22ZXGJpEpjC_1n-q_4MrImHCIJIZrDCvHOelbd5zrDAt.woff) format('woff');}.material-symbols-outlined{font-family:'Material Symbols Outlined';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
+  <style type="text/css">@font-face{font-family:'Material Symbols Outlined';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialsymbolsoutlined/v120/kJF1BvYX7BgnkSrUwT8OhrdQw4oELdPIeeII9v6oDMzByHX9rA6RzaxHMPdY43zj-jCxv3fzvRNU22ZXGJpEpjC_1n-q_4MrImHCIJIZrDCvHOelbd5zrDAt.woff) format('woff');}.material-symbols-outlined{font-family:'Material Symbols Outlined';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased;}</style>
 <style>.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}.mat-typography{font:400 14px/20px Roboto,Helvetica Neue,sans-serif;letter-spacing:normal}body{font-family:Roboto,Helvetica Neue,sans-serif;margin:0;position:relative;overflow:auto;display:inline-block;overflow:hidden}html{margin:0;height:100%;width:100%}body{margin:0;min-height:100%;width:100%}</style><link rel="stylesheet" href="styles.362a8260c32d36d9.css" media="print" onload="this.media='all'"><noscript><link rel="stylesheet" href="styles.362a8260c32d36d9.css"></noscript></head>
 <body class="mat-typography">
   <app-root></app-root>
-<script src="runtime.6a9b461ae5a72237.js" type="module"></script><script src="polyfills.0a8881ff36766b1e.js" type="module"></script><script src="vendor.43228e876ccc446f.js" type="module"></script><script src="main.8dfb947bbad7d7cf.js" type="module"></script>
+<script src="runtime.6a9b461ae5a72237.js" type="module"></script><script src="polyfills.0a8881ff36766b1e.js" type="module"></script><script src="vendor.923d0d3ca0754580.js" type="module"></script><script src="main.ff31141e0ae54f2d.js" type="module"></script>
 
 </body></html>
```

### Comparing `zen_dash-0.5.8/zen_dash/static/main.8dfb947bbad7d7cf.js` & `zen_dash-0.5.9/zen_dash/static/main.ff31141e0ae54f2d.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -21,63 +21,63 @@
                     ngOnInit() {
                         this.checkFunction(this.dataService.all_input.get(this.url)?.highchart_data?.config), "chart" == this.dataService.all_input.get(this.url)?.highchart_data?.type && (this.data = new angular_highcharts__WEBPACK_IMPORTED_MODULE_0__.kL(this.dataService.all_input.get(this.url)?.highchart_data?.config)), "stock" == this.dataService.all_input.get(this.url)?.highchart_data?.type && (this.data = new angular_highcharts__WEBPACK_IMPORTED_MODULE_0__.Du(this.dataService.all_input.get(this.url)?.highchart_data?.config)), setTimeout(this.resize_it, 1e3)
                     }
                     resize_it() {
                         window.dispatchEvent(new Event("resize"))
                     }
                 }
-                return HighchartComponent.\u0275fac = function D(J) {
-                    return new(J || HighchartComponent)(_angular_core__WEBPACK_IMPORTED_MODULE_1__.Y36(src_app_services_data_service__WEBPACK_IMPORTED_MODULE_2__.D))
+                return HighchartComponent.\u0275fac = function D(O) {
+                    return new(O || HighchartComponent)(_angular_core__WEBPACK_IMPORTED_MODULE_1__.Y36(src_app_services_data_service__WEBPACK_IMPORTED_MODULE_2__.D))
                 }, HighchartComponent.\u0275cmp = _angular_core__WEBPACK_IMPORTED_MODULE_1__.Xpm({
                     type: HighchartComponent,
                     selectors: [
                         ["app-highchart"]
                     ],
                     inputs: {
                         url: "url"
                     },
                     decls: 1,
                     vars: 1,
                     consts: [
                         [3, "chart"]
                     ],
-                    template: function D(J, p) {
-                        1 & J && _angular_core__WEBPACK_IMPORTED_MODULE_1__._UZ(0, "div", 0), 2 & J && _angular_core__WEBPACK_IMPORTED_MODULE_1__.Q6J("chart", p.data)
+                    template: function D(O, p) {
+                        1 & O && _angular_core__WEBPACK_IMPORTED_MODULE_1__._UZ(0, "div", 0), 2 & O && _angular_core__WEBPACK_IMPORTED_MODULE_1__.Q6J("chart", p.data)
                     },
                     dependencies: [angular_highcharts__WEBPACK_IMPORTED_MODULE_0__.Dm],
                     styles: [".highcharts-container[_ngcontent-%COMP%], .highcharts-root[_ngcontent-%COMP%]{width:100%!important}"]
                 }), HighchartComponent
             })()
         },
-        52468: (D, J, p) => {
-            p.d(J, {
-                D: () => ot
+        52468: (D, O, p) => {
+            p.d(O, {
+                D: () => pt
             });
             var v = p(64537),
                 t = p(21312);
-            let ot = (() => {
+            let pt = (() => {
                 class T {
                     constructor(c, u) {
                         this.router = c, this.activatedRoute = u, this.defaul_page = "page_0", this.all_input = new Map, this.input_emitter = new v.vpe, this.data = {
                             global: {
                                 device_information: ["device_information", {
                                     browser: navigator.userAgent,
                                     screen_info: {
                                         height: screen.availHeight,
                                         width: screen.availWidth
                                     }
                                 }]
                             }
-                        }, this.data_setter = new v.vpe, this.refresh = new v.vpe, window.data_service = this, window.data_service_get_page = this.get_page, window.data_service_get_all = this.get_all, this.data_setter.subscribe(m => {
-                            console.log(m), this.reset_path(u), void 0 === this.data[m.page] && (this.data[m.page] = {}), this.data[m.page][m.url] = [m.key, m.value]
+                        }, this.data_setter = new v.vpe, this.refresh = new v.vpe, window.data_service = this, window.data_service_get_page = this.get_page, window.data_service_get_all = this.get_all, this.data_setter.subscribe(h => {
+                            console.log(h), this.reset_path(u), void 0 === this.data[h.page] && (this.data[h.page] = {}), this.data[h.page][h.url] = [h.key, h.value]
                         })
                     }
                     reset_path(c) {
-                        let m = {};
-                        m = {
+                        let h = {};
+                        h = {
                             page: this.get_page()[0]
                         };
                         let b = new URL(window.location.href),
                             C = new URLSearchParams(b.search);
                         null !== C.get("document_id") && (null !== C.get("page") ? this.router.navigate([], {
                             relativeTo: c,
                             queryParams: {
@@ -87,193 +87,193 @@
                             relativeTo: c,
                             queryParams: {}
                         }))
                     }
                     get_page() {
                         let c = new URL(window.location.href),
                             u = new URLSearchParams(c.search),
-                            m = "page_0";
-                        return m = null !== u.get("page") ? u.get("page") : this.defaul_page, m
+                            h = "page_0";
+                        return h = null !== u.get("page") ? u.get("page") : this.defaul_page, h
                     }
                     get_data(c, u) {
                         if (void 0 !== this.data[c]) return this.data[c][u]
                     }
                     get_all() {
                         let c;
                         try {
                             c = this.get_page()
                         } catch {
                             c = window.data_service_get_page()
                         }
-                        let m, b, u = {
+                        let h, b, u = {
                             url: window.location.href
                         };
                         try {
-                            m = this.data[c] ?? {}
+                            h = this.data[c] ?? {}
                         } catch {
-                            m = window.data_service.data[c] ?? {}
+                            h = window.data_service.data[c] ?? {}
                         }
-                        Object.entries(m).forEach(([C, P]) => {
+                        Object.entries(h).forEach(([C, P]) => {
                             u[P[0]] = P[1]
                         });
                         try {
                             b = this.data.global ?? {}
                         } catch {
                             b = window.data_service.data.global ?? {}
                         }
                         return Object.entries(b).forEach(([C, P]) => {
                             "page" === C ? u[C] = P : u[P[0]] = P[1]
                         }), u
                     }
                     get_input_data(c) {
                         return this.all_input.get(c)
                     }
-                    set_data(c, u, m) {
-                        void 0 === this.data[c] && (this.data[c] = {}), this.data[c][u] = m
+                    set_data(c, u, h) {
+                        void 0 === this.data[c] && (this.data[c] = {}), this.data[c][u] = h
                     }
                     input_lookup(c, u) {
                         return u + "$ZenLookup$" + c
                     }
                     trueTypeOf(c) {
                         return Object.prototype.toString.call(c).slice(8, -1).toLowerCase()
                     }
                     dataLookup(c) {
                         return c ? "global" : this.get_page()
                     }
-                    save_instance(c, u, m) {
+                    save_instance(c, u, h) {
                         switch (c.type) {
                             case "date":
                                 let b = c.date_data;
-                                b.second_date ? (b.first_date = u[0], b.second_date = u[1]) : b.first_date = u, c.date_data = b, this.all_input.set(m, c);
+                                b.second_date ? (b.first_date = u[0], b.second_date = u[1]) : b.first_date = u, c.date_data = b, this.all_input.set(h, c);
                                 break;
                             case "radio":
                                 let C = c.radio_data;
-                                C.selected = u, c.radio_data = C, this.all_input.set(m, c);
+                                C.selected = u, c.radio_data = C, this.all_input.set(h, c);
                                 break;
                             case "checkbox":
                                 let P = c.checkbox_data;
-                                P.data = u, c.checkbox_data = P, this.all_input.set(m, c);
+                                P.data = u, c.checkbox_data = P, this.all_input.set(h, c);
                                 break;
                             case "slider":
-                                let O = c.slider_data;
-                                O.value = u, c.slider_data = O, this.all_input.set(m, c);
+                                let M = c.slider_data;
+                                M.value = u, c.slider_data = M, this.all_input.set(h, c);
                                 break;
                             case "button_toggle":
                                 let B = c.button_toggle_data;
                                 if (B.multi)
                                     for (let Q of B.data) Q.selected = -1 !== u.indexOf(Q.name);
                                 else
                                     for (let Q of B.data) Q.selected = Q.name === u;
-                                c.button_toggle_data = B, this.all_input.set(m, c);
+                                c.button_toggle_data = B, this.all_input.set(h, c);
                                 break;
                             case "toggle":
-                                let lt = c.toggle_data;
-                                lt.checked = u, c.toggle_data = lt, this.all_input.set(m, c);
+                                let ct = c.toggle_data;
+                                ct.checked = u, c.toggle_data = ct, this.all_input.set(h, c);
                                 break;
                             case "simple_filter":
                                 let z = c.simple_filter_data;
-                                z.selected = z.multi ? u : [u], c.simple_filter_data = z, this.all_input.set(m, c);
+                                z.selected = z.multi ? u : [u], c.simple_filter_data = z, this.all_input.set(h, c);
                                 break;
                             case "simple_server_filter":
                                 let K = c.simple_server_filter_data;
-                                K.selected = K.multi ? u : [u], c.simple_server_filter_data = K, this.all_input.set(m, c);
+                                K.selected = K.multi ? u : [u], c.simple_server_filter_data = K, this.all_input.set(h, c);
                                 break;
                             case "group_filter":
                                 let X = c.group_filter_data;
-                                X.selected = X.multi ? u : [u], c.group_filter_data = X, this.all_input.set(m, c);
+                                X.selected = X.multi ? u : [u], c.group_filter_data = X, this.all_input.set(h, c);
                                 break;
                             case "input":
-                                let rt = c.input_data;
-                                rt.value = u, c.input_data = rt, this.all_input.set(m, c);
+                                let dt = c.input_data;
+                                dt.value = u, c.input_data = dt, this.all_input.set(h, c);
                                 break;
                             default:
                                 console.error(c.type)
                         }
                     }
                     save_default() {
                         let c = this.get_page();
-                        for (const [u, m] of Object.entries(this.data.global)) try {
+                        for (const [u, h] of Object.entries(this.data.global)) try {
                             if ("page" !== u) {
-                                let b = m,
+                                let b = h,
                                     C = this.all_input.get(u);
                                 this.save_instance(C, b[1], u)
                             }
                         } catch {}
                         try {
-                            for (const [u, m] of Object.entries(this.data[c])) {
-                                let b = m,
+                            for (const [u, h] of Object.entries(this.data[c])) {
+                                let b = h,
                                     C = this.all_input.get(u);
                                 this.save_instance(C, b[1], u)
                             }
                         } catch {}
                     }
                     isFullCustom(c) {
                         return null != this.all_input.get(c)?.custom_html_data?.full_custom && this.all_input.get(c)?.custom_html_data?.full_custom
                     }
                     makeid(c) {
                         let u = "";
-                        const m = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789",
-                            b = m.length;
+                        const h = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789",
+                            b = h.length;
                         let C = 0;
-                        for (; C < c;) u += m.charAt(Math.floor(Math.random() * b)), C += 1;
+                        for (; C < c;) u += h.charAt(Math.floor(Math.random() * b)), C += 1;
                         return u
                     }
                 }
                 return T.\u0275fac = function(c) {
                     return new(c || T)(v.LFG(t.F0), v.LFG(t.gz))
                 }, T.\u0275prov = v.Yz7({
                     token: T,
                     factory: T.\u0275fac,
                     providedIn: "root"
                 }), T
             })()
         },
-        79: (D, J, p) => {
+        41877: (D, O, p) => {
             var v = p(5998),
                 t = p(64537),
-                ot = p(68014),
+                pt = p(68014),
                 T = p(52612);
             class x {}
-            class It {}
-            var E = p(7666),
+            class Et {}
+            var N = p(7666),
                 g = p(88692);
 
-            function Pt(a, s) {
+            function Nt(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 3)(1, "span", 4), t._uU(2), t.qZA(), t._UZ(3, "br"), t.TgZ(4, "span", 4), t._uU(5, " Built using Zen Dash "), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.hij(" ", e.data.message, "")
                 }
             }
 
-            function Qt(a, s) {
+            function Lt(a, s) {
                 if (1 & a && (t.TgZ(0, "span")(1, "span", 5), t._uU(2), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.hij(" ", e.data.message, "")
                 }
             }
 
-            function Yt(a, s) {
+            function Rt(a, s) {
                 if (1 & a && (t.TgZ(0, "span")(1, "span", 6), t._uU(2), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.hij(" ", e.data.message, "")
                 }
             }
 
-            function Ut(a, s) {
+            function qt(a, s) {
                 1 & a && (t.TgZ(0, "span", 3)(1, "span", 4), t._uU(2, " Built using Zen Dash "), t.qZA()())
             }
-            let w = (() => {
+            let Z = (() => {
                 class a {
                     constructor(e) {
                         this.data = e
                     }
                     ngOnInit() {}
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(E.qD))
+                    return new(e || a)(t.Y36(N.qD))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-loading"]
                     ],
                     decls: 4,
                     vars: 4,
@@ -283,27 +283,27 @@
                         ["style", "width: 100%; display: inline-block;", 4, "ngIf"],
                         [2, "width", "100%", "display", "inline-block"],
                         [1, "success"],
                         [1, "warn"],
                         [1, "error"]
                     ],
                     template: function(e, n) {
-                        1 & e && (t.YNc(0, Pt, 6, 1, "span", 0), t.YNc(1, Qt, 3, 1, "span", 1), t.YNc(2, Yt, 3, 1, "span", 1), t.YNc(3, Ut, 3, 0, "span", 2)), 2 & e && (t.Q6J("ngIf", "success" === n.data.status), t.xp6(1), t.Q6J("ngIf", "warn" === n.data.status), t.xp6(1), t.Q6J("ngIf", "error" === n.data.status), t.xp6(1), t.Q6J("ngIf", "loading" === n.data.status))
+                        1 & e && (t.YNc(0, Nt, 6, 1, "span", 0), t.YNc(1, Lt, 3, 1, "span", 1), t.YNc(2, Rt, 3, 1, "span", 1), t.YNc(3, qt, 3, 0, "span", 2)), 2 & e && (t.Q6J("ngIf", "success" === n.data.status), t.xp6(1), t.Q6J("ngIf", "warn" === n.data.status), t.xp6(1), t.Q6J("ngIf", "error" === n.data.status), t.xp6(1), t.Q6J("ngIf", "loading" === n.data.status))
                     },
                     dependencies: [g.O5],
                     styles: [".warn[_ngcontent-%COMP%]{color:#ffffe0}.error[_ngcontent-%COMP%]{color:#ff69b4}.success[_ngcontent-%COMP%]{color:#90ee90;margin:auto;width:50%;padding:10px}"]
                 }), a
             })();
-            var bt = p(21444),
-                N = p(35732),
+            var yt = p(21444),
+                L = p(35732),
                 f = p(52468),
                 F = p(21312),
-                pt = p(89284),
-                Et = p(98826);
-            let Ct = (() => {
+                ut = p(89284),
+                Ht = p(98826);
+            let Tt = (() => {
                     class a {
                         constructor(e, n) {
                             this.aRoute = e, this.ds = n
                         }
                         request_change() {
                             let e = this.ds.get_all();
                             void 0 !== this.subject && this.subject.next(e)
@@ -339,15 +339,15 @@
                             }
                         }
                         connect(e, n) {
                             "complete" === n && delete this.subject, void 0 !== n && console.log(n);
                             let i = this.ws_or_wss() + e,
                                 o = this.ds.get_all();
                             new Promise(r => setTimeout(r, 1e4)).then(() => {
-                                this.subject = (0, Et.j)(i), this.subject.subscribe({
+                                this.subject = (0, Ht.j)(i), this.subject.subscribe({
                                     next: r => this.save_data(r, this.ds),
                                     error: r => this.connect(i, r),
                                     complete: () => this.connect(i, "complete")
                                 }), this.subject.next(o)
                             })
                         }
                     }
@@ -355,15 +355,15 @@
                         return new(e || a)(t.LFG(F.gz), t.LFG(f.D))
                     }, a.\u0275prov = t.Yz7({
                         token: a,
                         factory: a.\u0275fac,
                         providedIn: "root"
                     }), a
                 })(),
-                Z = (() => {
+                w = (() => {
                     class a {
                         constructor(e, n, i) {
                             this.http = e, this.dataService = n, this.ws = i, this.refresh_listener = new t.vpe, this.config = {
                                 retry_count: 2,
                                 show_right_sidebar: !1,
                                 refresh: {
                                     refresh: !0,
@@ -404,100 +404,100 @@
                                 let _ = this.my_url();
                                 "/" === e[0] && (e = e.substring(1)), o = _ + e
                             }
                             let l = {};
                             if (void 0 !== i) {
                                 l = i;
                                 let _ = this.dataService.get_all();
-                                Object.entries(_).forEach((I, R) => {
-                                    l.append(R, I)
+                                Object.entries(_).forEach((I, q) => {
+                                    l.append(q, I)
                                 })
                             } else l = this.dataService.get_all();
                             let r, d = this.get_retry();
-                            return r = void 0 === n ? this.http.post(o, l).pipe((0, pt.X)({
+                            return r = void 0 === n ? this.http.post(o, l).pipe((0, ut.X)({
                                 count: d,
                                 delay: 2e3
-                            })) : this.http.post(o, l, n).pipe((0, pt.X)({
+                            })) : this.http.post(o, l, n).pipe((0, ut.X)({
                                 count: d,
                                 delay: 2e3
                             })), r
                         }
                         second_call_response(e, n, i) {
                             let o;
                             if (e.includes("http")) o = e;
                             else {
                                 let _ = this.my_url();
                                 "/" === e[0] && (e = e.substring(1)), o = _ + e
                             }
                             let l = this.dataService.get_all();
                             l[n] = i;
                             let r, d = this.get_retry();
-                            return r = this.http.post(o, l).pipe((0, pt.X)({
+                            return r = this.http.post(o, l).pipe((0, ut.X)({
                                 count: d,
                                 delay: 2e3
                             })), r
                         }
                         my_url() {
                             return window.location.href.split("?")[0]
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.LFG(N.eN), t.LFG(f.D), t.LFG(Ct))
+                        return new(e || a)(t.LFG(L.eN), t.LFG(f.D), t.LFG(Tt))
                     }, a.\u0275prov = t.Yz7({
                         token: a,
                         factory: a.\u0275fac,
                         providedIn: "root"
                     }), a
                 })();
-            var ct = p(24580),
+            var _t = p(24580),
                 S = p(46842),
-                L = p(9638),
-                q = p(83331),
-                H = p(50814),
-                W = p(83319),
-                et = p(42094),
-                dt = p(64639),
-                vt = p(25295),
-                yt = p(46438),
+                R = p(9638),
+                H = p(83331),
+                G = p(50814),
+                $ = p(83319),
+                at = p(42094),
+                mt = p(64639),
+                St = p(25295),
+                wt = p(46438),
                 Y = p(47408);
-            const Nt = ["script"];
+            const Gt = ["script"];
 
-            function Lt(a, s) {
+            function jt(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-card-footer", 4), t._uU(1), t.qZA()), 2 & a) {
                     const e = t.oxw(2);
                     t.xp6(1), t.hij(" ", e.getFooter(), " ")
                 }
             }
 
-            function Rt(a, s) {
+            function Bt(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-card")(1, "mat-card-header", 1)(2, "h4"), t._uU(3), t.qZA()(), t.TgZ(4, "mat-card-content")(5, "app-sub-entry-point", 2), t.NdJ("rd", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.rd.emit(i))
                     })("fd", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.fx.emit(i))
-                    }), t.qZA()(), t.YNc(6, Lt, 2, 1, "mat-card-footer", 3), t.qZA()
+                    }), t.qZA()(), t.YNc(6, jt, 2, 1, "mat-card-footer", 3), t.qZA()
                 }
                 if (2 & a) {
                     const e = t.oxw();
                     t.xp6(3), t.Oqu(e.getTitle()), t.xp6(2), t.Q6J("url", e.url)("isSidebar", e.isSidebar), t.xp6(1), t.Q6J("ngIf", e.getFooter())
                 }
             }
 
-            function qt(a, s) {
+            function zt(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-custom-html", 5), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.url)
                 }
             }
-            let $ = (() => {
+            let W = (() => {
                 class a {
                     constructor(e, n) {
                         this.ds = e, this.cd = n, this.fx = new t.vpe, this.rd = new t.vpe, this.pulled = !1, this.script_code = ""
                     }
                     ngOnInit() {
                         let e = "";
                         e = this.isSidebar ? "sidebar" : this.ds.get_page(), this.look_up = this.ds.input_lookup(e, this.url)
@@ -521,15 +521,15 @@
                     return new(e || a)(t.Y36(f.D), t.Y36(t.sBO))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-entry-point"]
                     ],
                     viewQuery: function(e, n) {
-                        if (1 & e && t.Gf(Nt, 5), 2 & e) {
+                        if (1 & e && t.Gf(Gt, 5), 2 & e) {
                             let i;
                             t.iGM(i = t.CRH()) && (n.script = i.first)
                         }
                     },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
@@ -545,65 +545,72 @@
                         [2, "display", "flex", "justify-content", "center", "align-items", "center"],
                         [3, "url", "isSidebar", "rd", "fd"],
                         ["style", "font-size: 10px; text-align: center", 4, "ngIf"],
                         [2, "font-size", "10px", "text-align", "center"],
                         [3, "url"]
                     ],
                     template: function(e, n) {
-                        1 & e && (t.YNc(0, Rt, 7, 4, "mat-card", 0), t.YNc(1, qt, 2, 1, "span", 0)), 2 & e && (t.Q6J("ngIf", !n.ds.isFullCustom(n.look_up)), t.xp6(1), t.Q6J("ngIf", n.ds.isFullCustom(n.look_up)))
+                        1 & e && (t.YNc(0, Bt, 7, 4, "mat-card", 0), t.YNc(1, zt, 2, 1, "span", 0)), 2 & e && (t.Q6J("ngIf", !n.ds.isFullCustom(n.look_up)), t.xp6(1), t.Q6J("ngIf", n.ds.isFullCustom(n.look_up)))
                     }
                 }), a
             })();
 
-            function Ht(a, s) {
+            function Kt(a, s) {
                 1 & a && t._UZ(0, "p")
             }
-            const Tt = function(a) {
+            const Zt = function(a) {
                 return {
                     page: a
                 }
             };
 
-            function Gt(a, s) {
+            function Xt(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-list-option", 6)(1, "a", 7)(2, "mat-icon"), t._uU(3), t.qZA(), t._uU(4), t.qZA()()), 2 & a) {
                     const e = t.oxw(),
                         n = e.index,
                         i = e.$implicit,
-                        o = t.oxw(2);
-                    t.Q6J("selected", "page_" + n === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, Tt, "page_" + n)), t.xp6(2), t.hij("", i.icon, " "), t.xp6(1), t.hij(" ", i.label, " ")
+                        o = t.oxw(3);
+                    t.Q6J("selected", "page_" + n === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, Zt, "page_" + n)), t.xp6(2), t.hij("", i.icon, " "), t.xp6(1), t.hij(" ", i.label, " ")
                 }
             }
 
-            function jt(a, s) {
+            function $t(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-list-option", 6)(1, "a", 7)(2, "mat-icon"), t._uU(3), t.qZA(), t._uU(4), t.qZA()()), 2 & a) {
                     const e = s.$implicit,
                         n = s.index,
                         i = t.oxw(2).index,
-                        o = t.oxw(2);
-                    t.Q6J("selected", "page_" + i + "_" + n === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, Tt, "page_" + i + "_" + n)), t.xp6(2), t.hij("", e.icon, " "), t.xp6(1), t.hij(" ", e.label, " ")
+                        o = t.oxw(3);
+                    t.Q6J("selected", "page_" + i + "_" + n === o.page), t.xp6(1), t.Udp("height", "45px"), t.Q6J("routerLink", ".")("queryParams", t.VKq(7, Zt, "page_" + i + "_" + n)), t.xp6(2), t.hij("", e.icon, " "), t.xp6(1), t.hij(" ", e.label, " ")
                 }
             }
 
-            function Bt(a, s) {
-                if (1 & a && (t.TgZ(0, "mat-expansion-panel")(1, "mat-expansion-panel-header"), t._uU(2), t.qZA(), t.TgZ(3, "mat-nav-list"), t.YNc(4, jt, 5, 9, "mat-list-option", 8), t.qZA()()), 2 & a) {
+            function Wt(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-expansion-panel")(1, "mat-expansion-panel-header"), t._uU(2), t.qZA(), t.TgZ(3, "mat-nav-list"), t.YNc(4, $t, 5, 9, "mat-list-option", 8), t.qZA()()), 2 & a) {
                     const e = t.oxw().$implicit;
                     t.ekj("mat-elevation-z0", !0), t.xp6(2), t.hij(" ", e.name, " "), t.xp6(2), t.Q6J("ngForOf", e.subtabs)
                 }
             }
 
-            function zt(a, s) {
-                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, Ht, 1, 0, "p", 3), t.YNc(2, Gt, 5, 9, "ng-template", null, 4, t.W1O), t.YNc(4, Bt, 5, 4, "ng-template", null, 5, t.W1O), t.qZA()), 2 & a) {
+            function Vt(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, Kt, 1, 0, "p", 3), t.YNc(2, Xt, 5, 9, "ng-template", null, 4, t.W1O), t.YNc(4, Wt, 5, 4, "ng-template", null, 5, t.W1O), t.qZA()), 2 & a) {
                     const e = s.$implicit,
                         n = t.MAs(3),
                         i = t.MAs(5);
                     t.xp6(1), t.Q6J("ngIf", e.icon)("ngIfThen", n)("ngIfElse", i)
                 }
             }
 
-            function Kt(a, s) {
+            function te(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, Vt, 6, 3, "span", 2), t.qZA()), 2 & a) {
+                    const e = t.oxw(2);
+                    t.xp6(1), t.Q6J("ngForOf", e.getSideData())
+                }
+            }
+
+            function ee(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.ynx(0), t._UZ(1, "mat-divider")(2, "br"), t.TgZ(3, "app-entry-point", 9), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
@@ -616,21 +623,21 @@
                     const e = s.$implicit,
                         n = t.oxw(2);
                     let i;
                     t.xp6(3), t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !0)
                 }
             }
 
-            function Xt(a, s) {
-                if (1 & a && (t.TgZ(0, "span")(1, "mat-selection-list", 1), t.YNc(2, zt, 6, 3, "span", 2), t.qZA(), t._UZ(3, "br")(4, "br"), t.YNc(5, Kt, 5, 3, "ng-container", 2), t._UZ(6, "br"), t.qZA()), 2 & a) {
+            function ne(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "mat-selection-list", 1), t.YNc(2, te, 2, 1, "span", 0), t.qZA(), t._UZ(3, "br")(4, "br"), t.YNc(5, ee, 5, 3, "ng-container", 2), t._UZ(6, "br"), t.qZA()), 2 & a) {
                     const e = t.oxw();
-                    t.xp6(1), t.Q6J("multiple", !1), t.xp6(1), t.Q6J("ngForOf", e.getSideData()), t.xp6(3), t.Q6J("ngForOf", e.side_data.filters)
+                    t.xp6(1), t.Q6J("multiple", !1), t.xp6(1), t.Q6J("ngIf", e.isSideData()), t.xp6(3), t.Q6J("ngForOf", e.side_data.filters)
                 }
             }
-            let Wt = (() => {
+            let ae = (() => {
                 class a {
                     constructor(e, n, i, o) {
                         this.http = e, this.aRoute = n, this.call = i, this.ds = o, this.size = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.page = null, this.aRoute.queryParamMap.subscribe(l => {
                             this.page = l.get("page")
                         })
                     }
                     ngOnInit() {
@@ -643,23 +650,26 @@
                             } catch {}
                             this.size.emit(this.side_data.size)
                         })
                     }
                     getSideData() {
                         return this.side_data?.tabs
                     }
+                    isSideData() {
+                        return this.side_data?.tabs.length > 0
+                    }
                     setFlex(e, n) {
                         this.flexData.set(e, n)
                     }
                     setReactivity(e, n) {
                         this.reactivityData.set(e, n)
                     }
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(N.eN), t.Y36(F.gz), t.Y36(Z), t.Y36(f.D))
+                    return new(e || a)(t.Y36(L.eN), t.Y36(F.gz), t.Y36(w), t.Y36(f.D))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-sidebar"]
                     ],
                     inputs: {
                         url: "url"
@@ -678,35 +688,35 @@
                         ["elseBlock2", ""],
                         [3, "selected"],
                         ["mat-list-item", "", "type", "button", 3, "routerLink", "queryParams"],
                         [3, "selected", 4, "ngFor", "ngForOf"],
                         [3, "hidden", "url", "isSidebar", "fx", "rd"]
                     ],
                     template: function(e, n) {
-                        1 & e && t.YNc(0, Xt, 7, 3, "span", 0), 2 & e && t.Q6J("ngIf", void 0 !== n.side_data)
+                        1 & e && t.YNc(0, ne, 7, 3, "span", 0), 2 & e && t.Q6J("ngIf", void 0 !== n.side_data)
                     },
-                    dependencies: [yt.d, Y.ib, Y.yz, q.Hw, H.Hk, H.Tg, H.Ub, H.vS, g.sg, g.O5, F.yS, $],
+                    dependencies: [wt.d, Y.ib, Y.yz, H.Hw, G.Hk, G.Tg, G.Ub, G.vS, g.sg, g.O5, F.yS, W],
                     styles: [".mat-icon[_ngcontent-%COMP%]{vertical-align:middle}.toolbar-item-spacer[_ngcontent-%COMP%]{flex:1 1 auto}.app-container[_ngcontent-%COMP%]{height:90%;margin:0}.app-sidenav[_ngcontent-%COMP%]{width:230px}.app-sidenav-content[_ngcontent-%COMP%]{display:flex;height:100%;align-items:center;justify-content:center}"]
                 }), a
             })();
 
-            function $t(a, s) {
+            function ie(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "button", 1), t.NdJ("click", function() {
                         t.CHM(e), t.oxw();
                         const i = t.MAs(27);
                         return t.KtG(i.toggle())
                     }), t.TgZ(2, "mat-icon"), t._uU(3, "menu"), t.qZA()()()
                 }
             }
-            let Vt = (() => {
+            let se = (() => {
                     class a {
-                        constructor(e, n, i, o, l, r, d, _, I, R) {
-                            this.http = i, this.ds = o, this._snackBar = l, this.aRoute = r, this.call = d, this.titleService = _, this.clipboard = I, this.ws = R, this.durationInSeconds = 5, this.mySize = "500px", this.mySize2 = "500px", this.color = "primary", this.checked = !1, this.mobileQuery = n.matchMedia("(max-width: 600px)"), this._mobileQueryListener = () => e.detectChanges(), this.mobileQuery.addListener(this._mobileQueryListener)
+                        constructor(e, n, i, o, l, r, d, _, I, q) {
+                            this.http = i, this.ds = o, this._snackBar = l, this.aRoute = r, this.call = d, this.titleService = _, this.clipboard = I, this.ws = q, this.durationInSeconds = 5, this.mySize = "500px", this.mySize2 = "500px", this.color = "primary", this.checked = !1, this.mobileQuery = n.matchMedia("(max-width: 600px)"), this._mobileQueryListener = () => e.detectChanges(), this.mobileQuery.addListener(this._mobileQueryListener)
                         }
                         ngOnDestroy() {
                             this.mobileQuery.removeListener(this._mobileQueryListener)
                         }
                         setTitle() {
                             this.http.get(this.call.my_url() + "backend/title").subscribe(e => {
                                 this.titleService.setTitle(e), this.title = e
@@ -717,15 +727,15 @@
                             let e = this.ds.get_page();
                             void 0 === this.ds.data.global && (this.ds.data.global = {}), this.ds.data.global.page = e, this.color = "primary"
                         }
                         sendWSRequest() {
                             this.call.config.websocket.active && this.ws.request_change()
                         }
                         trigger_load() {
-                            this._snackBar.openFromComponent(w, {
+                            this._snackBar.openFromComponent(Z, {
                                 duration: 5e3,
                                 panelClass: ["full_width"],
                                 data: {
                                     message: "API called Sucessfully ",
                                     status: "loading"
                                 }
                             })
@@ -738,15 +748,15 @@
                             }), this.trigger_load(), this.show_right_sidebar = this.call.config.show_right_sidebar, this.getScripts(), this.setTitle(), this.call.refresh_listener.subscribe(e => {
                                 this.checked = !0, this.set_auto({
                                     checked: !0
                                 })
                             })
                         }
                         refresh_data() {
-                            this.color = "primary", this.call.config.websocket.active ? this.ws.request_change() : this.ds.refresh.emit("RefreshButton"), this.ds.save_default(), this._snackBar.openFromComponent(w, {
+                            this.color = "primary", this.call.config.websocket.active ? this.ws.request_change() : this.ds.refresh.emit("RefreshButton"), this.ds.save_default(), this._snackBar.openFromComponent(Z, {
                                 duration: 1e3 * this.durationInSeconds,
                                 data: {
                                     message: "Refreshing data",
                                     status: "success"
                                 }
                             })
                         }
@@ -771,23 +781,23 @@
                             n ? this.mySize2 = e : this.mySize = e
                         }
                         saveReport() {
                             this.document_id = this.ds.makeid(32);
                             let e = new x;
                             e.key = "document_id", e.value = this.document_id, this.ds.data_setter.emit(e), this.refresh_data(), this.call.call_response(this.call.my_url() + "backend/document", void 0, void 0).subscribe(n => {
                                 const i = new URL(window.location.href);
-                                i.searchParams.set("document_id", this.document_id), this.clipboard.copy(i.href), this._snackBar.openFromComponent(w, {
+                                i.searchParams.set("document_id", this.document_id), this.clipboard.copy(i.href), this._snackBar.openFromComponent(Z, {
                                     duration: 1e3 * this.durationInSeconds,
                                     data: {
                                         message: "Document URL copied",
                                         status: "success"
                                     }
                                 })
                             }, n => {
-                                this._snackBar.openFromComponent(w, {
+                                this._snackBar.openFromComponent(Z, {
                                     duration: 1e3 * this.durationInSeconds,
                                     data: {
                                         message: "Saving report failed",
                                         status: "error"
                                     }
                                 })
                             })
@@ -796,15 +806,15 @@
                             console.log("call refresh"), e.config.websocket.active ? i.request_change() : n.refresh.emit("AutoRefresh")
                         }
                         set_auto(e) {
                             e.checked ? this.runRefresh = setInterval(this.call_refresh, 1e3 * this.call.config.refresh.rate_in_seconds, this.call, this.ds, this.ws) : clearInterval(this.runRefresh)
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.Y36(t.sBO), t.Y36(bt.vx), t.Y36(N.eN), t.Y36(f.D), t.Y36(E.ux), t.Y36(F.gz), t.Y36(Z), t.Y36(v.Dx), t.Y36(ct.TU), t.Y36(Ct))
+                        return new(e || a)(t.Y36(t.sBO), t.Y36(yt.vx), t.Y36(L.eN), t.Y36(f.D), t.Y36(N.ux), t.Y36(F.gz), t.Y36(w), t.Y36(v.Dx), t.Y36(_t.TU), t.Y36(Tt))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-root"]
                         ],
                         decls: 39,
                         vars: 14,
@@ -833,15 +843,15 @@
                         template: function(e, n) {
                             if (1 & e) {
                                 const i = t.EpF();
                                 t.TgZ(0, "mat-toolbar", 0)(1, "button", 1), t.NdJ("click", function() {
                                     t.CHM(i);
                                     const l = t.MAs(23);
                                     return t.KtG(l.toggle())
-                                }), t.TgZ(2, "mat-icon"), t._uU(3, "menu"), t.qZA()(), t.TgZ(4, "span"), t._uU(5), t.qZA(), t.TgZ(6, "div", 2), t.YNc(7, $t, 4, 0, "span", 3), t.TgZ(8, "button", 4)(9, "mat-icon"), t._uU(10, "more_vert"), t.qZA()()(), t.TgZ(11, "mat-menu", null, 5)(13, "button", 6), t.NdJ("click", function() {
+                                }), t.TgZ(2, "mat-icon"), t._uU(3, "menu"), t.qZA()(), t.TgZ(4, "span"), t._uU(5), t.qZA(), t.TgZ(6, "div", 2), t.YNc(7, ie, 4, 0, "span", 3), t.TgZ(8, "button", 4)(9, "mat-icon"), t._uU(10, "more_vert"), t.qZA()()(), t.TgZ(11, "mat-menu", null, 5)(13, "button", 6), t.NdJ("click", function() {
                                     return n.saveReport()
                                 }), t.TgZ(14, "mat-icon"), t._uU(15, "saved_search"), t.qZA(), t.TgZ(16, "span"), t._uU(17, "Save Report"), t.qZA()(), t.TgZ(18, "button", 7)(19, "mat-slide-toggle", 8), t.NdJ("change", function(l) {
                                     return n.set_auto(l)
                                 }), t._uU(20, " Auto Refresh "), t.qZA()()()(), t.TgZ(21, "mat-sidenav-container", 9)(22, "mat-sidenav", 10, 11)(24, "mat-nav-list")(25, "app-sidebar", 12), t.NdJ("size", function(l) {
                                     return n.set_size(l, !1)
                                 }), t.qZA()()(), t.TgZ(26, "mat-sidenav", 13, 14)(28, "mat-nav-list")(29, "app-sidebar", 12), t.NdJ("size", function(l) {
                                     return n.set_size(l, !0)
@@ -850,19 +860,19 @@
                                 }), t.TgZ(36, "mat-icon"), t._uU(37, "refresh"), t.qZA()()()()()(), t._UZ(38, "router-outlet"), t.qZA()()
                             }
                             if (2 & e) {
                                 const i = t.MAs(12);
                                 t.xp6(5), t.Oqu(n.title), t.xp6(2), t.Q6J("ngIf", n.call.show_right_sidebar()), t.xp6(1), t.Q6J("matMenuTriggerFor", i), t.xp6(11), t.Q6J("checked", n.checked), t.xp6(3), t.Udp("width", n.mySize), t.Q6J("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar"), t.xp6(1), t.Udp("width", n.mySize2), t.Q6J("position", "end")("mode", "over"), t.xp6(3), t.Q6J("url", "backend/sidebar2"), t.xp6(6), t.Q6J("color", n.color)
                             }
                         },
-                        dependencies: [S.Wh, S.yH, L.lW, q.Hw, H.Hk, W.VK, W.OP, W.p6, et.JX, et.TM, et.Rh, dt.Rr, vt.Ye, g.O5, F.lC, Wt],
+                        dependencies: [S.Wh, S.yH, R.lW, H.Hw, G.Hk, $.VK, $.OP, $.p6, at.JX, at.TM, at.Rh, mt.Rr, St.Ye, g.O5, F.lC, ae],
                         styles: ["[_nghost-%COMP%]{position:absolute;left:0;right:0;bottom:0;top:0}mat-sidenav-container[_ngcontent-%COMP%]{margin:0;min-height:100%;height:100%;width:100%;display:inline-block}.increase-size[_ngcontent-%COMP%]{width:200px}mat-sidenav[_ngcontent-%COMP%]{min-width:200px}.float[_ngcontent-%COMP%]{position:fixed;bottom:1rem;right:1rem;z-index:5}.app-container[_ngcontent-%COMP%]{height:90%;margin:0}.app-sidenav[_ngcontent-%COMP%]{width:230px}.app-sidenav-content[_ngcontent-%COMP%]{display:flex;height:100%;align-items:center;justify-content:center}.toolbar-item-spacer[_ngcontent-%COMP%]{flex:1 1 auto}"]
                     }), a
                 })(),
-                te = (() => {
+                oe = (() => {
                     class a {
                         constructor() {}
                         set_title(e, n, i) {
                             e.fragment.subscribe(o => {
                                 null !== o ? n.setTitle(o) : i.get("/backend/title").subscribe(l => {
                                     n.setTitle(l)
                                 })
@@ -873,17 +883,17 @@
                         return new(e || a)
                     }, a.\u0275prov = t.Yz7({
                         token: a,
                         factory: a.\u0275fac,
                         providedIn: "root"
                     }), a
                 })();
-            var A = p(11997);
+            var J = p(11997);
 
-            function ee(a, s) {
+            function le(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "app-entry-point", 5), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
@@ -896,38 +906,38 @@
                     const e = s.$implicit,
                         n = t.oxw(3);
                     let i, o, l, r, d;
                     t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !1)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "33%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "33%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (d = n.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
                 }
             }
 
-            function ne(a, s) {
-                if (1 & a && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, ee, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & a) {
+            function re(a, s) {
+                if (1 & a && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, le, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & a) {
                     const e = s.$implicit;
                     t.xp6(4), t.Q6J("ngForOf", e.data)
                 }
             }
 
-            function ae(a, s) {
-                if (1 & a && (t.TgZ(0, "div"), t.YNc(1, ne, 5, 1, "div", 1), t.qZA()), 2 & a) {
+            function pe(a, s) {
+                if (1 & a && (t.TgZ(0, "div"), t.YNc(1, re, 5, 1, "div", 1), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", null == e.page ? null : e.page.rows)
                 }
             }
-            const ie = [{
+            const ce = [{
                 path: "**",
                 component: (() => {
                     class a {
                         constructor(e, n, i, o, l) {
                             this.http = e, this.titleService = n, this.aRoute = i, this.call = o, this.dataService = l, this.page = void 0, this.reactivityData = new Map, this.flexData = new Map
                         }
                         ngOnInit() {
-                            (new te).set_title(this.aRoute, this.titleService, this.http), this.aRoute.queryParamMap.subscribe(e => {
+                            (new oe).set_title(this.aRoute, this.titleService, this.http), this.aRoute.queryParamMap.subscribe(e => {
                                 let n = this.dataService.get_page(),
-                                    i = (new N.LE).set("fragment", n);
+                                    i = (new L.LE).set("fragment", n);
                                 this.http.get(this.call.my_url() + "backend/page_detail", {
                                     params: i
                                 }).subscribe(o => {
                                     this.page = o
                                 })
                             })
                         }
@@ -935,15 +945,15 @@
                             this.flexData.set(e, n)
                         }
                         setReactivity(e, n) {
                             this.reactivityData.set(e, n)
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.Y36(N.eN), t.Y36(v.Dx), t.Y36(F.gz), t.Y36(Z), t.Y36(f.D))
+                        return new(e || a)(t.Y36(L.eN), t.Y36(v.Dx), t.Y36(F.gz), t.Y36(w), t.Y36(f.D))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-page"]
                         ],
                         decls: 1,
                         vars: 1,
@@ -952,70 +962,70 @@
                             ["style", "padding: 10px", 4, "ngFor", "ngForOf"],
                             [2, "padding", "10px"],
                             ["fxLayout", "row wrap", "fxLayout.lt-sm", "column", "fxLayoutGap", "row_data.layoutGap", "fxLayoutAlign", "space-around center", "fxLayoutAlign.lt-sm", "space-around stretch", "fxFlexFill", ""],
                             ["class", "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd", 4, "ngFor", "ngForOf"],
                             [1, "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd"]
                         ],
                         template: function(e, n) {
-                            1 & e && t.YNc(0, ae, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", n.page)
+                            1 & e && t.YNc(0, pe, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", n.page)
                         },
-                        dependencies: [S.xw, S.SQ, S.Wh, S.s9, S.yH, A.a8, A.dn, g.sg, g.O5, $],
+                        dependencies: [S.xw, S.SQ, S.Wh, S.s9, S.yH, J.a8, J.dn, g.sg, g.O5, W],
                         styles: [".padding[_ngcontent-%COMP%]{padding:5px;margin-bottom:1em;min-width:100px}.max[_ngcontent-%COMP%]{max-height:200px}"]
                     }), a
                 })()
             }];
-            let se = (() => {
+            let de = (() => {
                 class a {}
                 return a.\u0275fac = function(e) {
                     return new(e || a)
                 }, a.\u0275mod = t.oAB({
                     type: a
                 }), a.\u0275inj = t.cJS({
-                    imports: [F.Bz.forRoot(ie, {
+                    imports: [F.Bz.forRoot(ce, {
                         relativeLinkResolution: "legacy"
                     }), F.Bz]
                 }), a
             })();
-            var oe = p(25544),
-                le = p(38954),
-                re = p(58698),
-                pe = p(27165),
-                ce = p(18632),
-                de = p(76342),
-                ue = p(59269),
-                ut = p(9286),
-                _e = p(55211),
-                me = p(61637),
-                he = p(65719),
-                ge = p(56226),
-                _t = p(50108),
-                St = p(71561),
-                fe = p(27084),
-                xe = p(65429),
+            var ue = p(25544),
+                _e = p(38954),
+                me = p(58698),
+                he = p(27165),
+                ge = p(18632),
+                fe = p(76342),
+                xe = p(59269),
+                ht = p(9286),
+                be = p(55211),
+                Ce = p(61637),
+                ve = p(65719),
+                ye = p(56226),
+                gt = p(50108),
+                Dt = p(71561),
+                Te = p(27084),
+                Se = p(65429),
                 U = p(83704),
                 V = p(88696),
                 tt = p(25237),
-                nt = p(39665),
-                mt = p(53538),
-                G = p(40827),
-                be = p(8697),
-                ht = p(53556),
-                at = p(18033),
-                wt = p(96219),
-                it = p(56558),
-                M = p(80418),
-                gt = p(72516),
-                Zt = p(2940),
-                Ce = p(18849),
-                ve = p(19596),
-                h = p(20092),
-                ye = p(96100),
-                Dt = p(40512);
+                it = p(39665),
+                ft = p(53538),
+                j = p(40827),
+                we = p(8697),
+                xt = p(53556),
+                et = p(18033),
+                Ft = p(96219),
+                st = p(56558),
+                A = p(80418),
+                bt = p(72516),
+                kt = p(2940),
+                Ze = p(18849),
+                De = p(19596),
+                m = p(20092),
+                Fe = p(96100),
+                Jt = p(40512);
 
-            function Te(a, s) {
+            function ke(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "app-entry-point", 5), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(3);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
@@ -1028,28 +1038,28 @@
                     const e = s.$implicit,
                         n = t.oxw(3);
                     let i, o, l, r, d;
                     t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", !1)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "33%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "33%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (d = n.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
                 }
             }
 
-            function Se(a, s) {
-                if (1 & a && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, Te, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & a) {
+            function Je(a, s) {
+                if (1 & a && (t.TgZ(0, "div", 2)(1, "mat-card")(2, "mat-card-content")(3, "div", 3), t.YNc(4, ke, 1, 7, "app-entry-point", 4), t.qZA()()()()), 2 & a) {
                     const e = s.$implicit;
                     t.xp6(4), t.Q6J("ngForOf", e.data)
                 }
             }
 
-            function we(a, s) {
-                if (1 & a && (t.TgZ(0, "div"), t.YNc(1, Se, 5, 1, "div", 1), t.qZA()), 2 & a) {
+            function Ae(a, s) {
+                if (1 & a && (t.TgZ(0, "div"), t.YNc(1, Je, 5, 1, "div", 1), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", null == e.page ? null : e.page.rows)
                 }
             }
-            let Ze = (() => {
+            let Oe = (() => {
                 class a {
                     constructor(e, n, i, o, l, r) {
                         this.dialogRef = e, this.dialog_url = n, this.http = i, this.aRoute = o, this.call = l, this.dataService = r, this.page = void 0, this.reactivityData = new Map, this.flexData = new Map
                     }
                     ngOnInit() {
                         let e;
                         if (this.dialog_url.includes("http")) e = this.dialog_url;
@@ -1066,15 +1076,15 @@
                         this.flexData.set(e, n)
                     }
                     setReactivity(e, n) {
                         this.reactivityData.set(e, n)
                     }
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(V.so), t.Y36(V.WI), t.Y36(N.eN), t.Y36(F.gz), t.Y36(Z), t.Y36(f.D))
+                    return new(e || a)(t.Y36(V.so), t.Y36(V.WI), t.Y36(L.eN), t.Y36(F.gz), t.Y36(w), t.Y36(f.D))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-dialog"]
                     ],
                     decls: 1,
                     vars: 1,
@@ -1083,21 +1093,21 @@
                         ["style", "padding: 10px", 4, "ngFor", "ngForOf"],
                         [2, "padding", "10px"],
                         ["fxLayout", "row wrap", "fxLayout.lt-sm", "column", "fxLayoutGap", "row_data.layoutGap", "fxLayoutAlign", "space-around center", "fxLayoutAlign.lt-sm", "space-around stretch", "fxFlexFill", ""],
                         ["class", "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd", 4, "ngFor", "ngForOf"],
                         [1, "padding", 3, "hidden", "url", "isSidebar", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "fx", "rd"]
                     ],
                     template: function(e, n) {
-                        1 & e && t.YNc(0, we, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", n.page)
+                        1 & e && t.YNc(0, Ae, 2, 1, "div", 0), 2 & e && t.Q6J("ngIf", n.page)
                     },
-                    dependencies: [S.xw, S.SQ, S.Wh, S.s9, S.yH, A.a8, A.dn, g.sg, g.O5, $]
+                    dependencies: [S.xw, S.SQ, S.Wh, S.s9, S.yH, J.a8, J.dn, g.sg, g.O5, W]
                 }), a
             })();
-            var De = p(8239);
-            let Ft = (() => {
+            var Me = p(8239);
+            let At = (() => {
                     class a {
                         constructor(e, n, i) {
                             this.ds = e, this.callService = n, this.dialog = i, this.input_types = ["date", "checkbox", "radio", "simple_filter", "simple_server_filter", "group_filter", "slider", "button_toggle", "toggle", "input", "download", "upload", "button", "form"], this.subscription_lookup = {}, this.d = new Map, this.data_type = ["box", "table", "chart", "image", "highchart", "custom_html"], this.call_this = new t.vpe, this.call_api = {}, this.data_ = {}, this.call_this.subscribe(o => {
                                 this.getData(o.forced, o.url, o.look_up, o.page, o.isSidebar, "")
                             })
                         }
                         get_multi_url(e) {
@@ -1169,15 +1179,15 @@
                                 lookup: l,
                                 t: o,
                                 message: void 0
                             })
                         }
                         getData(e, n, i, o, l, r) {
                             var d = this;
-                            return (0, De.Z)(function*() {
+                            return (0, Me.Z)(function*() {
                                 let _ = d.ds.all_input.get(i);
                                 if (void 0 !== _ && !e) return void d.ds.input_emitter.emit({
                                     calling: !1,
                                     lookup: i,
                                     t: _,
                                     message: void 0
                                 });
@@ -1191,23 +1201,23 @@
                                 let I = d.callService.call_response(n, void 0, void 0);
                                 return d.ds.input_emitter.emit({
                                     calling: !0,
                                     lookup: i,
                                     t: void 0,
                                     message: void 0
                                 }), d.ds.all_input.delete(i), d.subscription_lookup[i] = yield I.subscribe({
-                                    next: R => {
-                                        d.updateData(l, n, o, R, i)
+                                    next: q => {
+                                        d.updateData(l, n, o, q, i)
                                     },
-                                    error: R => {
+                                    error: q => {
                                         d.ds.input_emitter.emit({
                                             calling: !1,
                                             lookup: i,
                                             t: void 0,
-                                            message: R.message
+                                            message: q.message
                                         })
                                     }
                                 }), {
                                     error: "not called"
                                 }
                             })()
                         }
@@ -1265,22 +1275,22 @@
                                 delete l.page[o], 0 === Object.keys(l.page).length && delete l.page
                             } catch {}
                             let r = JSON.stringify(l);
                             this.data_[o] = r
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.LFG(f.D), t.LFG(Z), t.LFG(V.uw))
+                        return new(e || a)(t.LFG(f.D), t.LFG(w), t.LFG(V.uw))
                     }, a.\u0275prov = t.Yz7({
                         token: a,
                         factory: a.\u0275fac,
                         providedIn: "root"
                     }), a
                 })(),
-                Fe = (() => {
+                Ie = (() => {
                     class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnDestroy() {}
                         ngOnInit() {}
                         getIcon() {
@@ -1317,15 +1327,15 @@
                         },
                         dependencies: [tt.Il, tt.DX],
                         styles: [".material-symbols-outlined[_ngcontent-%COMP%]{font-size:50px;height:50px;width:50px;line-height:50px}"]
                     }), a
                 })();
             var y = p(88659);
 
-            function ke(a, s) {
+            function Pe(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div")(1, "mat-form-field", 3)(2, "mat-label"), t._uU(3), t.qZA(), t.TgZ(4, "mat-date-range-input", 4)(5, "input", 5), t.NdJ("dateChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.changeValue(i))
                     }), t.qZA(), t.TgZ(6, "input", 6), t.NdJ("dateChange", function(i) {
@@ -1337,42 +1347,42 @@
                 if (2 & a) {
                     const e = t.MAs(11),
                         n = t.oxw();
                     t.xp6(3), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formGroup", n.getForm())("rangePicker", e)("comparisonStart", n.form_data.value.start)("comparisonEnd", n.form_data.value.end), t.xp6(5), t.Q6J("for", e)
                 }
             }
 
-            function Ae(a, s) {
+            function Qe(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div")(1, "mat-form-field", 9)(2, "mat-label"), t._uU(3), t.qZA(), t.TgZ(4, "input", 10), t.NdJ("dateChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.changeValue(i))
                     }), t.qZA(), t.TgZ(5, "mat-hint"), t._uU(6, "MM/DD/YYYY"), t.qZA(), t._UZ(7, "mat-datepicker-toggle", 7)(8, "mat-datepicker", null, 11), t.qZA()()
                 }
                 if (2 & a) {
                     const e = t.MAs(9),
                         n = t.oxw();
                     t.xp6(3), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("matDatepicker", e)("formControl", n.form_control), t.xp6(3), t.Q6J("for", e)
                 }
             }
-            let Me = (() => {
+            let Ye = (() => {
                 class a {
                     constructor(e) {
                         this.ds = e
                     }
                     ngOnInit() {
                         this.getData()
                     }
                     getData() {
-                        this.data = this.ds.all_input.get(this.url)?.date_data, this.data.second_date ? (this.single = !1, this.form_data = new h.nJ({
-                            start: new h.p4(new Date(this.data.first_date + "T00:00:00")),
-                            end: new h.p4(new Date(this.data.second_date + "T00:00:00"))
-                        })) : (this.single = !0, this.form_control = new h.p4(new Date(this.data.first_date + "T00:00:00")))
+                        this.data = this.ds.all_input.get(this.url)?.date_data, this.data.second_date ? (this.single = !1, this.form_data = new m.nJ({
+                            start: new m.p4(new Date(this.data.first_date + "T00:00:00")),
+                            end: new m.p4(new Date(this.data.second_date + "T00:00:00"))
+                        })) : (this.single = !0, this.form_control = new m.p4(new Date(this.data.first_date + "T00:00:00")))
                     }
                     getForm() {
                         return this.form_data
                     }
                     isSingle() {
                         return this.single
                     }
@@ -1409,87 +1419,87 @@
                         ["matSuffix", "", 3, "for"],
                         ["campaignOnePicker", ""],
                         ["appearance", "standard", "floatLabel", "always"],
                         ["matInput", "", 3, "matDatepicker", "formControl", "dateChange"],
                         ["dp", ""]
                     ],
                     template: function(e, n) {
-                        1 & e && (t.TgZ(0, "mat-grid-list", 0)(1, "mat-grid-tile", 1), t.YNc(2, ke, 12, 6, "div", 2), t.YNc(3, Ae, 10, 4, "div", 2), t._UZ(4, "br"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("colspan", 4)("rowspan", 1), t.xp6(1), t.Q6J("ngIf", !n.isSingle()), t.xp6(1), t.Q6J("ngIf", n.isSingle()))
+                        1 & e && (t.TgZ(0, "mat-grid-list", 0)(1, "mat-grid-tile", 1), t.YNc(2, Pe, 12, 6, "div", 2), t.YNc(3, Qe, 10, 4, "div", 2), t._UZ(4, "br"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("colspan", 4)("rowspan", 1), t.xp6(1), t.Q6J("ngIf", !n.isSingle()), t.xp6(1), t.Q6J("ngIf", n.isSingle()))
                     },
-                    dependencies: [h.Fj, h.JJ, h.JL, h.oH, h.sg, h.u, U.Mq, U.hl, U.nW, U.wx, U.zY, U.By, U._g, tt.Il, tt.DX, y.KE, y.bx, y.hX, y.R9, nt.Nt, g.O5]
+                    dependencies: [m.Fj, m.JJ, m.JL, m.oH, m.sg, m.u, U.Mq, U.hl, U.nW, U.wx, U.zY, U.By, U._g, tt.Il, tt.DX, y.KE, y.bx, y.hX, y.R9, it.Nt, g.O5]
                 }), a
             })();
-            var Je = p(95834);
+            var Ue = p(95834);
 
-            function Oe(a, s) {
+            function Ee(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "button", 14), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.value = "")
                     }), t.TgZ(1, "mat-icon"), t._uU(2, "close"), t.qZA()()
                 }
             }
 
-            function Ie(a, s) {
+            function Ne(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-header-cell", 18), t._uU(1), t.qZA()), 2 & a) {
                     const e = t.oxw().$implicit;
                     t.xp6(1), t.Oqu(e.header)
                 }
             }
 
-            function Pe(a, s) {
+            function Le(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-cell"), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit,
                         n = t.oxw().$implicit;
                     t.xp6(1), t.Oqu(e[n.columnDef])
                 }
             }
 
-            function Qe(a, s) {
-                1 & a && (t.ynx(0, 15), t.YNc(1, Ie, 2, 1, "mat-header-cell", 16), t.YNc(2, Pe, 2, 1, "mat-cell", 17), t.BQk()), 2 & a && t.Q6J("matColumnDef", s.$implicit.columnDef)
+            function Re(a, s) {
+                1 & a && (t.ynx(0, 15), t.YNc(1, Ne, 2, 1, "mat-header-cell", 16), t.YNc(2, Le, 2, 1, "mat-cell", 17), t.BQk()), 2 & a && t.Q6J("matColumnDef", s.$implicit.columnDef)
             }
 
-            function Ye(a, s) {
+            function qe(a, s) {
                 1 & a && t._UZ(0, "mat-header-row")
             }
 
-            function Ue(a, s) {
+            function He(a, s) {
                 1 & a && t._UZ(0, "mat-row")
             }
 
-            function Ee(a, s) {
+            function Ge(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div", 19)(1, "div", 20)(2, "button", 21), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.download())
                     }), t._uU(3, "Download"), t.qZA()(), t.TgZ(4, "div", 22), t._UZ(5, "mat-paginator", 23), t.qZA()()
                 }
                 if (2 & a) {
                     const e = t.oxw();
                     t.xp6(5), t.Q6J("pageSizeOptions", e.items_per_page_options)("pageSize", e.items_per_page)
                 }
             }
 
-            function Ne(a, s) {
+            function je(a, s) {
                 if (1 & a && (t.TgZ(0, "div"), t._UZ(1, "mat-paginator", 23), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("pageSizeOptions", e.items_per_page_options)("pageSize", e.items_per_page)
                 }
             }
-            let Le = (() => {
+            let Be = (() => {
                     class a {
                         constructor(e) {
-                            this.dataService = e, this.selection = new Je.Ov(!0, []), this.displayedColumns = []
+                            this.dataService = e, this.selection = new Ue.Ov(!0, []), this.displayedColumns = []
                         }
                         ngOnInit() {
-                            this.columns = this.dataService.all_input.get(this.url)?.table_data?.columns, this.dataSource = new M.by(this.dataService.all_input.get(this.url)?.table_data?.data), this.allow_download = this.dataService.all_input.get(this.url)?.table_data?.allow_download, this.items_per_page = this.dataService.all_input.get(this.url)?.table_data?.items_per_page, this.items_per_page_options = this.dataService.all_input.get(this.url)?.table_data?.items_per_page_options, this.displayedColumns = this.displayedColumns.concat(this.columns.map(e => e.columnDef))
+                            this.columns = this.dataService.all_input.get(this.url)?.table_data?.columns, this.dataSource = new A.by(this.dataService.all_input.get(this.url)?.table_data?.data), this.allow_download = this.dataService.all_input.get(this.url)?.table_data?.allow_download, this.items_per_page = this.dataService.all_input.get(this.url)?.table_data?.items_per_page, this.items_per_page_options = this.dataService.all_input.get(this.url)?.table_data?.items_per_page_options, this.displayedColumns = this.displayedColumns.concat(this.columns.map(e => e.columnDef))
                         }
                         ngAfterViewInit() {
                             this.dataSource.paginator = this.paginator, this.dataSource.sort = this.sort
                         }
                         isAllSelected() {
                             return this.selection.selected.length === this.dataSource.data.length
                         }
@@ -1519,15 +1529,15 @@
                         return new(e || a)(t.Y36(f.D))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-table"]
                         ],
                         viewQuery: function(e, n) {
-                            if (1 & e && (t.Gf(mt.NW, 5), t.Gf(it.YE, 5)), 2 & e) {
+                            if (1 & e && (t.Gf(ft.NW, 5), t.Gf(st.YE, 5)), 2 & e) {
                                 let i;
                                 t.iGM(i = t.CRH()) && (n.paginator = i.first), t.iGM(i = t.CRH()) && (n.sort = i.first)
                             }
                         },
                         inputs: {
                             url: "url"
                         },
@@ -1560,21 +1570,21 @@
                             ["showFirstLastButtons", "", 3, "pageSizeOptions", "pageSize"]
                         ],
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "div", 0)(1, "div", 1)(2, "mat-form-field", 2)(3, "mat-icon", 3), t._uU(4, "search"), t.qZA(), t.TgZ(5, "mat-label"), t._uU(6, "Search"), t.qZA(), t.TgZ(7, "input", 4), t.NdJ("ngModelChange", function(o) {
                                 return n.value = o
                             })("keyup", function(o) {
                                 return n.applyFilter(o)
-                            }), t.qZA(), t.YNc(8, Oe, 3, 0, "button", 5), t.qZA()()(), t.TgZ(9, "div", 6)(10, "mat-table", 7, 8), t.YNc(12, Qe, 3, 1, "ng-container", 9), t.YNc(13, Ye, 1, 0, "mat-header-row", 10), t.YNc(14, Ue, 1, 0, "mat-row", 11), t.qZA(), t.TgZ(15, "div"), t.YNc(16, Ee, 6, 2, "div", 12), t.YNc(17, Ne, 2, 2, "div", 13), t.qZA()()), 2 & e && (t.xp6(7), t.Q6J("ngModel", n.value), t.xp6(1), t.Q6J("ngIf", n.value), t.xp6(2), t.Q6J("dataSource", n.dataSource), t.xp6(2), t.Q6J("ngForOf", n.columns), t.xp6(1), t.Q6J("matHeaderRowDef", n.displayedColumns), t.xp6(1), t.Q6J("matRowDefColumns", n.displayedColumns), t.xp6(2), t.Q6J("ngIf", n.allow_download), t.xp6(1), t.Q6J("ngIf", !n.allow_download))
+                            }), t.qZA(), t.YNc(8, Ee, 3, 0, "button", 5), t.qZA()()(), t.TgZ(9, "div", 6)(10, "mat-table", 7, 8), t.YNc(12, Re, 3, 1, "ng-container", 9), t.YNc(13, qe, 1, 0, "mat-header-row", 10), t.YNc(14, He, 1, 0, "mat-row", 11), t.qZA(), t.TgZ(15, "div"), t.YNc(16, Ge, 6, 2, "div", 12), t.YNc(17, je, 2, 2, "div", 13), t.qZA()()), 2 & e && (t.xp6(7), t.Q6J("ngModel", n.value), t.xp6(1), t.Q6J("ngIf", n.value), t.xp6(2), t.Q6J("dataSource", n.dataSource), t.xp6(2), t.Q6J("ngForOf", n.columns), t.xp6(1), t.Q6J("matHeaderRowDef", n.displayedColumns), t.xp6(1), t.Q6J("matRowDefColumns", n.displayedColumns), t.xp6(2), t.Q6J("ngIf", n.allow_download), t.xp6(1), t.Q6J("ngIf", !n.allow_download))
                         },
-                        dependencies: [h.Fj, h.JJ, h.On, ut.O_, ut.D5, L.lW, q.Hw, y.KE, y.hX, y.qo, y.R9, nt.Nt, mt.NW, it.YE, it.nU, M.BZ, M.as, M.w1, M.nj, M.ge, M.ev, M.XQ, M.Gk, g.sg, g.O5],
+                        dependencies: [m.Fj, m.JJ, m.On, ht.O_, ht.D5, R.lW, H.Hw, y.KE, y.hX, y.qo, y.R9, it.Nt, ft.NW, st.YE, st.nU, A.BZ, A.as, A.w1, A.nj, A.ge, A.ev, A.XQ, A.Gk, g.sg, g.O5],
                         styles: ['.search-box[_ngcontent-%COMP%]   mat-form-field[_ngcontent-%COMP%]{width:100%}.table-responsive[_ngcontent-%COMP%]{display:block;overflow-x:scroll}.table-responsive[_ngcontent-%COMP%]   .mat-table[_ngcontent-%COMP%]{width:100%;max-width:100%;margin-bottom:1rem;display:table;border-collapse:collapse;margin:0}.table-responsive[_ngcontent-%COMP%]   .mat-row[_ngcontent-%COMP%], .table-responsive[_ngcontent-%COMP%]   .mat-header-row[_ngcontent-%COMP%]{display:table-row}.table-responsive[_ngcontent-%COMP%]   .mat-cell[_ngcontent-%COMP%], .table-responsive[_ngcontent-%COMP%]   .mat-header-cell[_ngcontent-%COMP%]{word-wrap:initial;display:table-cell;padding:0 5px;line-break:unset;width:auto;white-space:nowrap;overflow:hidden;vertical-align:middle}.material-symbols-outlined[_ngcontent-%COMP%]{font-variation-settings:"FILL" 1,"wght" 700,"GRAD" 200,"opsz" 48}']
                     }), a
                 })(),
-                Re = (() => {
+                ze = (() => {
                     class a {
                         constructor(e) {
                             this.dataService = e
                         }
                         ngOnInit() {}
                         get_options() {
                             return this.dataService.all_input.get(this.url)?.chart_data?.data
@@ -1594,19 +1604,19 @@
                         vars: 1,
                         consts: [
                             ["echarts", "", 1, "demo-chart", 3, "options"]
                         ],
                         template: function(e, n) {
                             1 & e && t._UZ(0, "div", 0), 2 & e && t.Q6J("options", n.get_options())
                         },
-                        dependencies: [Dt._w]
+                        dependencies: [Jt._w]
                     }), a
                 })();
 
-            function qe(a, s) {
+            function Ke(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "div")(1, "mat-checkbox", 4), t.NdJ("ngModelChange", function(i) {
                         const l = t.CHM(e).$implicit;
                         return t.KtG(l.selected = i)
                     })("ngModelChange", function() {
                         t.CHM(e);
@@ -1616,22 +1626,22 @@
                 }
                 if (2 & a) {
                     const e = s.$implicit;
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(1), t.hij(" ", e.name, " ")
                 }
             }
 
-            function He(a, s) {
-                if (1 & a && (t.TgZ(0, "section", 2), t.YNc(1, qe, 3, 2, "div", 3), t.qZA()), 2 & a) {
+            function Xe(a, s) {
+                if (1 & a && (t.TgZ(0, "section", 2), t.YNc(1, Ke, 3, 2, "div", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", e.my_data())
                 }
             }
 
-            function Ge(a, s) {
+            function $e(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "li")(1, "mat-checkbox", 5), t.NdJ("ngModelChange", function(i) {
                         const l = t.CHM(e).$implicit;
                         return t.KtG(l.selected = i)
                     })("ngModelChange", function() {
                         t.CHM(e);
@@ -1641,21 +1651,21 @@
                 }
                 if (2 & a) {
                     const e = s.$implicit;
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(1), t.hij(" ", e.name, " ")
                 }
             }
 
-            function je(a, s) {
-                if (1 & a && (t.TgZ(0, "section")(1, "ul"), t.YNc(2, Ge, 3, 2, "li", 3), t.qZA()()), 2 & a) {
+            function We(a, s) {
+                if (1 & a && (t.TgZ(0, "section")(1, "ul"), t.YNc(2, $e, 3, 2, "li", 3), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.Q6J("ngForOf", e.my_data())
                 }
             }
-            let Be = (() => {
+            let Ve = (() => {
                 class a {
                     constructor(e) {
                         this.ds = e
                     }
                     ngOnInit() {
                         this.getData()
                     }
@@ -1691,73 +1701,73 @@
                         [4, "ngIf"],
                         [1, "example-section"],
                         [4, "ngFor", "ngForOf"],
                         [1, "example-margin", 3, "ngModel", "ngModelChange"],
                         [1, "example-margin-top", 3, "ngModel", "ngModelChange"]
                     ],
                     template: function(e, n) {
-                        1 & e && (t.YNc(0, He, 2, 1, "section", 0), t.YNc(1, je, 3, 1, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === n.get_style()), t.xp6(1), t.Q6J("ngIf", "Vertical" === n.get_style()))
+                        1 & e && (t.YNc(0, Xe, 2, 1, "section", 0), t.YNc(1, We, 3, 1, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === n.get_style()), t.xp6(1), t.Q6J("ngIf", "Vertical" === n.get_style()))
                     },
-                    dependencies: [h.JJ, h.On, St.oG, g.sg, g.O5],
+                    dependencies: [m.JJ, m.On, Dt.oG, g.sg, g.O5],
                     styles: [".example-margin[_ngcontent-%COMP%]{margin-left:10px}.example-margin-top[_ngcontent-%COMP%]{margin-bottom:10px}ul[_ngcontent-%COMP%]{list-style-type:none;margin-top:4px}.example-section[_ngcontent-%COMP%]{display:flex;align-content:center;align-items:center;height:60px}"]
                 }), a
             })();
 
-            function ze(a, s) {
+            function tn(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-radio-button", 5), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.Oqu(e)
                 }
             }
 
-            function Ke(a, s) {
+            function en(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "section", 2)(1, "mat-radio-group", 3), t.NdJ("ngModelChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.selected = i)
                     })("change", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.update())
-                    }), t.YNc(2, ze, 2, 2, "mat-radio-button", 4), t.qZA()()
+                    }), t.YNc(2, tn, 2, 2, "mat-radio-button", 4), t.qZA()()
                 }
                 if (2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(1), t.Q6J("ngForOf", e.getData())
                 }
             }
 
-            function Xe(a, s) {
+            function nn(a, s) {
                 if (1 & a && (t.TgZ(0, "li")(1, "mat-radio-button", 7), t._uU(2), t.qZA()()), 2 & a) {
                     const e = s.$implicit;
                     t.xp6(1), t.Q6J("value", e), t.xp6(1), t.Oqu(e)
                 }
             }
 
-            function We(a, s) {
+            function an(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "section")(1, "mat-radio-group", 3), t.NdJ("ngModelChange", function(i) {
                         t.CHM(e);
                         const o = t.oxw();
                         return t.KtG(o.selected = i)
                     })("change", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.update())
-                    }), t.TgZ(2, "ul"), t.YNc(3, Xe, 3, 2, "li", 6), t.qZA()()()
+                    }), t.TgZ(2, "ul"), t.YNc(3, nn, 3, 2, "li", 6), t.qZA()()()
                 }
                 if (2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngModel", e.selected), t.xp6(2), t.Q6J("ngForOf", e.getData())
                 }
             }
-            let $e = (() => {
+            let sn = (() => {
                     class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {
                             this.selected = this.ds.all_input.get(this.url)?.radio_data?.selected
                         }
@@ -1792,21 +1802,21 @@
                             [3, "ngModel", "ngModelChange", "change"],
                             ["class", "example-radio-button", 3, "value", 4, "ngFor", "ngForOf"],
                             [1, "example-radio-button", 3, "value"],
                             [4, "ngFor", "ngForOf"],
                             [1, "example-radio-button-bottom", 3, "value"]
                         ],
                         template: function(e, n) {
-                            1 & e && (t.YNc(0, Ke, 3, 2, "section", 0), t.YNc(1, We, 4, 2, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === n.getStyle()), t.xp6(1), t.Q6J("ngIf", "Vertical" === n.getStyle()))
+                            1 & e && (t.YNc(0, en, 3, 2, "section", 0), t.YNc(1, an, 4, 2, "section", 1)), 2 & e && (t.Q6J("ngIf", "Horizontal" === n.getStyle()), t.xp6(1), t.Q6J("ngIf", "Vertical" === n.getStyle()))
                         },
-                        dependencies: [h.JJ, h.On, ht.VQ, ht.U0, g.sg, g.O5],
+                        dependencies: [m.JJ, m.On, xt.VQ, xt.U0, g.sg, g.O5],
                         styles: [".mat-radio-button[_ngcontent-%COMP%] ~ .mat-radio-button[_ngcontent-%COMP%]{margin-left:16px}.example-radio-group[_ngcontent-%COMP%]{display:flex;flex-direction:column;margin:15px 0;align-items:flex-start}.example-radio-button[_ngcontent-%COMP%]{margin:5px}.example-radio-button-bottom[_ngcontent-%COMP%]{margin-bottom:5px}ul[_ngcontent-%COMP%]{list-style-type:none;margin-top:4px}"]
                     }), a
                 })(),
-                Ve = (() => {
+                on = (() => {
                     class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {
                             this.value = this.ds.all_input.get(this.url)?.slider_data?.value
                         }
@@ -1852,26 +1862,26 @@
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-slider", 0), t.NdJ("ngModelChange", function(o) {
                                 return n.value = o
                             })("change", function() {
                                 return n.detectChange()
                             }), t.qZA()), 2 & e && t.Q6J("invert", n.isInverted())("max", n.isMax())("min", n.isMin())("step", n.step())("thumbLabel", n.isThumbLabel())("ngModel", n.value)("vertical", n.isVertical())
                         },
-                        dependencies: [h.JJ, h.On, wt.pH],
+                        dependencies: [m.JJ, m.On, Ft.pH],
                         styles: [".mat-slider-horizontal[_ngcontent-%COMP%]{width:300px}.mat-slider-vertical[_ngcontent-%COMP%]{height:150px}"]
                     }), a
                 })();
 
-            function tn(a, s) {
+            function ln(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-button-toggle", 2), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e.name), t.xp6(1), t.hij(" ", e.name, "")
                 }
             }
-            let en = (() => {
+            let rn = (() => {
                     class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {
                             this.selected_data = this.isMultiple() ? [] : ""
                         }
@@ -1917,20 +1927,20 @@
                             [3, "value", "multiple", "change"],
                             [3, "value", 4, "ngFor", "ngForOf"],
                             [3, "value"]
                         ],
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-button-toggle-group", 0), t.NdJ("change", function(o) {
                                 return n.onChange(o)
-                            }), t.YNc(1, tn, 2, 2, "mat-button-toggle", 1), t.qZA()), 2 & e && (t.Q6J("value", n.get_value())("multiple", n.isMultiple()), t.xp6(1), t.Q6J("ngForOf", n.get_buton_data()))
+                            }), t.YNc(1, ln, 2, 2, "mat-button-toggle", 1), t.qZA()), 2 & e && (t.Q6J("value", n.get_value())("multiple", n.isMultiple()), t.xp6(1), t.Q6J("ngForOf", n.get_buton_data()))
                         },
-                        dependencies: [_t.A9, _t.Yi, g.sg]
+                        dependencies: [gt.A9, gt.Yi, g.sg]
                     }), a
                 })(),
-                nn = (() => {
+                pn = (() => {
                     class a {
                         constructor(e) {
                             this.ds = e
                         }
                         ngOnInit() {}
                         checkData() {
                             return this.ds.all_input.get(this.url)?.toggle_data?.checked
@@ -1963,44 +1973,44 @@
                             [3, "checked", "change"]
                         ],
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-slide-toggle", 0), t.NdJ("change", function(o) {
                                 return n.saveData(o)
                             }), t._uU(1), t.qZA()), 2 & e && (t.Q6J("checked", n.checkData()), t.xp6(1), t.Oqu(n.get_name()))
                         },
-                        dependencies: [dt.Rr]
+                        dependencies: [mt.Rr]
                     }), a
                 })();
-            var ft = p(5557),
-                xt = p(38023),
-                kt = p(65598),
-                j = p(13528),
-                st = p(64325);
-            const an = ["dataSelect"];
+            var ot = p(5557),
+                lt = p(38023),
+                Ot = p(65598),
+                E = p(13528),
+                nt = p(64325);
+            const cn = ["dataSelect"];
 
-            function sn(a, s) {
+            function dn(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
-            let on = (() => {
+            let un = (() => {
                 class a {
                     constructor(e) {
-                        this.ds = e, this.dataForm = new h.p4, this.compareFn = (n, i) => n && i && n.id === i.id, this.data_select_control = new h.p4, this.data_search_control = new h.p4, this.data_search = new ft.t(1), this.searching = !1, this._onDestroy = new xt.x
+                        this.ds = e, this.dataForm = new m.p4, this.compareFn = (n, i) => n && i && n.id === i.id, this.data_select_control = new m.p4, this.data_search_control = new m.p4, this.data_search = new ot.t(1), this.searching = !1, this._onDestroy = new lt.x
                     }
                     ngOnInit() {
                         this.originalData(), this.searchData()
                     }
                     ngAfterViewInit() {}
                     ngOnDestroy() {
                         this._onDestroy.next(), this._onDestroy.complete()
                     }
                     setInitialValue() {
-                        this.data_search.pipe((0, kt.q)(1), (0, j.R)(this._onDestroy)).subscribe(() => {
+                        this.data_search.pipe((0, Ot.q)(1), (0, E.R)(this._onDestroy)).subscribe(() => {
                             this.dataSelect.compareWith = (e, n) => e === n
                         })
                     }
                     filterMulti() {
                         if (!this.data) return;
                         let e = this.data_search_control.value;
                         e ? (e = e.toLowerCase(), this.data_search.next(this.data.filter(n => n.toLowerCase().indexOf(e) > -1))) : this.data_search.next(this.data.slice())
@@ -2011,38 +2021,35 @@
                     isMulti() {
                         return this.ds.all_input.get(this.url)?.simple_filter_data?.multi
                     }
                     originalData() {
                         this.data = this.ds.all_input.get(this.url)?.simple_filter_data?.data, void 0 !== this.selectedData() && this.selectedData().length > 0 && (this.isMulti() ? this.data_select_control.setValue(this.selectedData()) : this.data_select_control.setValue(this.selectedData()[0])), this.data_search.next(this.data.slice())
                     }
                     searchData() {
-                        this.data_search_control.valueChanges.pipe((0, j.R)(this._onDestroy)).subscribe(() => {
+                        this.data_search_control.valueChanges.pipe((0, E.R)(this._onDestroy)).subscribe(() => {
                             this.filterMulti()
                         }), this.setInitialValue()
                     }
                     getLabel() {
                         return this.ds.all_input.get(this.url)?.simple_filter_data?.name
                     }
                     detectChange(e) {
                         let n = new x;
                         n.key = this.ds.all_input.get(this.url)?.simple_filter_data?.name, n.value = e.value, n.page = this.ds.dataLookup(this.isSidebar), n.url = this.url, this.ds.data_setter.emit(n)
                     }
-                    isServerSide() {
-                        return null !== this.dataUrl
-                    }
                 }
                 return a.\u0275fac = function(e) {
                     return new(e || a)(t.Y36(f.D))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-simple-filter"]
                     ],
                     viewQuery: function(e, n) {
-                        if (1 & e && t.Gf(an, 7), 2 & e) {
+                        if (1 & e && t.Gf(cn, 7), 2 & e) {
                             let i;
                             t.iGM(i = t.CRH()) && (n.dataSelect = i.first)
                         }
                     },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
@@ -2056,61 +2063,61 @@
                         [3, "formControl"],
                         [3, "value", 4, "ngFor", "ngForOf"],
                         [3, "value"]
                     ],
                     template: function(e, n) {
                         1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "mat-select", 1, 2), t.NdJ("selectionChange", function(o) {
                             return n.detectChange(o)
-                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, sn, 2, 2, "mat-option", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formControl", n.data_select_control)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, n.data_search)))
+                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, dn, 2, 2, "mat-option", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formControl", n.data_select_control)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, n.data_search)))
                     },
-                    dependencies: [h.JJ, h.oH, T.ey, y.KE, y.hX, at.gD, g.sg, st.nu, g.Ov]
+                    dependencies: [m.JJ, m.oH, T.ey, y.KE, y.hX, et.gD, g.sg, nt.nu, g.Ov]
                 }), a
             })();
-            const ln = ["dataSelect"];
+            const _n = ["dataSelect"];
 
-            function rn(a, s) {
+            function mn(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-option", 7), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
 
-            function pn(a, s) {
-                if (1 & a && (t.TgZ(0, "mat-optgroup", 5), t.YNc(1, rn, 2, 2, "mat-option", 6), t.qZA()), 2 & a) {
+            function hn(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-optgroup", 5), t.YNc(1, mn, 2, 2, "mat-option", 6), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("label", e.group_name), t.xp6(1), t.Q6J("ngForOf", e.group_data)
                 }
             }
-            let cn = (() => {
+            let gn = (() => {
                 class a {
                     constructor(e) {
-                        this.ds = e, this.dataForm = new h.p4, this.data_select_control = new h.p4, this.data_search_control = new h.p4, this.data_search = new ft.t(1), this._onDestroy = new xt.x
+                        this.ds = e, this.dataForm = new m.p4, this.data_select_control = new m.p4, this.data_search_control = new m.p4, this.data_search = new ot.t(1), this._onDestroy = new lt.x
                     }
                     ngOnInit() {
                         this.myData()
                     }
                     ngAfterViewInit() {}
                     ngOnDestroy() {
                         this._onDestroy.next(), this._onDestroy.complete()
                     }
                     setInitialValue() {
-                        this.data_search.pipe((0, kt.q)(1), (0, j.R)(this._onDestroy)).subscribe(() => {
+                        this.data_search.pipe((0, Ot.q)(1), (0, E.R)(this._onDestroy)).subscribe(() => {
                             this.dataSelect.compareWith = (e, n) => e === n
                         })
                     }
                     filterMulti() {
                         if (!this.group_data) return;
                         let e = this.data_search_control.value;
                         const n = this.copyGroups(this.group_data);
                         e ? (e = e.toLowerCase(), this.data_search.next(n.filter(i => (i.group_name.toLowerCase().indexOf(e) > -1 || (i.group_data = i.group_data.filter(l => l.toLowerCase().indexOf(e) > -1)), i.group_data.length > 0)))) : this.data_search.next(this.group_data.slice())
                     }
                     myData() {
                         this.data = this.ds.all_input.get(this.url)?.group_filter_data, this.multi = this.ds.all_input.get(this.url)?.group_filter_data?.multi, this.group_data = this.data.data;
                         let e = this.ds.all_input.get(this.url)?.group_filter_data?.selected;
-                        void 0 !== e && e.length > 0 && (this.isMulti() ? this.data_select_control.setValue(e) : this.data_select_control.setValue(e[0])), this.data_search.next(this.group_data.slice()), this.data_search_control.valueChanges.pipe((0, j.R)(this._onDestroy)).subscribe(() => {
+                        void 0 !== e && e.length > 0 && (this.isMulti() ? this.data_select_control.setValue(e) : this.data_select_control.setValue(e[0])), this.data_search.next(this.group_data.slice()), this.data_search_control.valueChanges.pipe((0, E.R)(this._onDestroy)).subscribe(() => {
                             this.filterMulti()
                         }), this.setInitialValue()
                     }
                     getLabel() {
                         return this.ds.all_input.get(this.url)?.group_filter_data?.name
                     }
                     detectChange(e) {
@@ -2134,15 +2141,15 @@
                     return new(e || a)(t.Y36(f.D))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-group-filter"]
                     ],
                     viewQuery: function(e, n) {
-                        if (1 & e && t.Gf(ln, 7), 2 & e) {
+                        if (1 & e && t.Gf(_n, 7), 2 & e) {
                             let i;
                             t.iGM(i = t.CRH()) && (n.dataSelect = i.first)
                         }
                     },
                     inputs: {
                         url: "url",
                         isSidebar: "isSidebar"
@@ -2158,31 +2165,31 @@
                         [3, "label"],
                         [3, "value", 4, "ngFor", "ngForOf"],
                         [3, "value"]
                     ],
                     template: function(e, n) {
                         1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "mat-select", 1, 2), t.NdJ("selectionChange", function(o) {
                             return n.detectChange(o)
-                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, pn, 2, 2, "mat-optgroup", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formControl", n.data_select_control)("multiple", n.multi), t.xp6(3), t.Q6J("formControl", n.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, n.data_search)))
+                        }), t.TgZ(5, "mat-option"), t._UZ(6, "ngx-mat-select-search", 3), t.qZA(), t.YNc(7, hn, 2, 2, "mat-optgroup", 4), t.ALo(8, "async"), t.qZA()()), 2 & e && (t.xp6(2), t.Oqu(n.getLabel()), t.xp6(1), t.Q6J("formControl", n.data_select_control)("multiple", n.multi), t.xp6(3), t.Q6J("formControl", n.data_search_control), t.xp6(1), t.Q6J("ngForOf", t.lcZ(8, 5, n.data_search)))
                     },
-                    dependencies: [h.JJ, h.oH, T.ey, T.Nv, y.KE, y.hX, at.gD, g.sg, st.nu, g.Ov]
+                    dependencies: [m.JJ, m.oH, T.ey, T.Nv, y.KE, y.hX, et.gD, g.sg, nt.nu, g.Ov]
                 }), a
             })();
 
-            function dn(a, s) {
+            function fn(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "button", 3), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.clearData())
                     }), t.TgZ(1, "mat-icon"), t._uU(2, "close"), t.qZA()()
                 }
             }
-            let un = (() => {
+            let xn = (() => {
                 class a {
                     constructor(e) {
                         this.ds = e
                     }
                     ngOnInit() {
                         let e = this.ds.all_input.get(this.url)?.input_data?.value;
                         void 0 !== e && (this.data = e)
@@ -2223,25 +2230,25 @@
                         ["matSuffix", "", "mat-icon-button", "", "aria-label", "Clear", 3, "click"]
                     ],
                     template: function(e, n) {
                         1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-label"), t._uU(2), t.qZA(), t.TgZ(3, "input", 1), t.NdJ("ngModelChange", function(o) {
                             return n.data = o
                         })("ngModelChange", function() {
                             return n.saveData()
-                        }), t.qZA(), t.YNc(4, dn, 3, 0, "button", 2), t.qZA()), 2 & e && (t.xp6(2), t.hij(" ", n.getLabel(), ""), t.xp6(1), t.Q6J("ngModel", n.data), t.xp6(1), t.Q6J("ngIf", n.data))
+                        }), t.qZA(), t.YNc(4, fn, 3, 0, "button", 2), t.qZA()), 2 & e && (t.xp6(2), t.hij(" ", n.getLabel(), ""), t.xp6(1), t.Q6J("ngModel", n.data), t.xp6(1), t.Q6J("ngIf", n.data))
                     },
-                    dependencies: [h.Fj, h.JJ, h.On, L.lW, q.Hw, y.KE, y.hX, y.R9, nt.Nt, g.O5]
+                    dependencies: [m.Fj, m.JJ, m.On, R.lW, H.Hw, y.KE, y.hX, y.R9, it.Nt, g.O5]
                 }), a
             })();
-            var At = p(33441);
+            var Mt = p(33441);
 
-            function _n(a, s) {
+            function bn(a, s) {
                 1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
             }
-            let mn = (() => {
+            let Cn = (() => {
                 class a {
                     constructor(e, n, i, o) {
                         this.ds = e, this.fileSaverService = n, this.callService = i, this._snackBar = o, this.show = !1
                     }
                     getFileName(e) {
                         let n = /filename\*=UTF-8''([\w%\-\.]+)(?:; ?|$)/i,
                             i = /^filename=(["']?)(.*?[^\\])\1(?:; ?|$)/i,
@@ -2268,15 +2275,15 @@
                         this.downloadCall = e.subscribe(n => {
                             let i = new x;
                             i.page = this.ds.dataLookup(!1), i.key = this.ds.all_input.get(this.url)?.download_data?.name, i.value = this.ds.makeid(2), i.url = this.url, this.ds.data_setter.emit(i);
                             let o = n.headers.get("content-disposition"),
                                 l = this.getFileName(o);
                             this.fileSaverService.save(n.body, l), this.show = !1
                         }, n => {
-                            this.show = !1, this._snackBar.openFromComponent(w, {
+                            this.show = !1, this._snackBar.openFromComponent(Z, {
                                 duration: 5e3,
                                 data: {
                                     message: "Failed download",
                                     status: "error"
                                 }
                             })
                         })
@@ -2287,15 +2294,15 @@
                     fileLabel() {
                         return this.data?.label
                     }
                     onSuc(e) {}
                     onErr(e) {}
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(f.D), t.Y36(At.m9), t.Y36(Z), t.Y36(E.ux))
+                    return new(e || a)(t.Y36(f.D), t.Y36(Mt.m9), t.Y36(w), t.Y36(N.ux))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-app-download"]
                     ],
                     inputs: {
                         url: "url"
@@ -2310,24 +2317,24 @@
                     template: function(e, n) {
                         1 & e && (t.TgZ(0, "button", 0), t.NdJ("click", function() {
                             return n.onSave()
                         })("success", function(o) {
                             return n.onSuc(o)
                         })("error", function(o) {
                             return n.onErr(o)
-                        }), t._uU(1), t.qZA(), t.YNc(2, _n, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.hij(" Download ", n.fileLabel(), "\n"), t.xp6(1), t.Q6J("ngIf", n.show))
+                        }), t._uU(1), t.qZA(), t.YNc(2, bn, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.hij(" Download ", n.fileLabel(), "\n"), t.xp6(1), t.Q6J("ngIf", n.show))
                     },
-                    dependencies: [L.lW, G.pW, g.O5]
+                    dependencies: [R.lW, j.pW, g.O5]
                 }), a
             })();
 
-            function hn(a, s) {
+            function vn(a, s) {
                 1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
             }
-            let gn = (() => {
+            let yn = (() => {
                     class a {
                         constructor(e, n, i) {
                             this.ds = e, this.callService = n, this._snackBar = i, this.myFiles = [], this.show = !1
                         }
                         ngOnInit() {
                             this.data = this.ds.all_input.get(this.url)?.upload_data
                         }
@@ -2338,36 +2345,36 @@
                             this.show = !0;
                             for (var n = 0; n < e.target.files.length; n++) this.myFiles.push(e.target.files[n]);
                             const i = new FormData;
                             for (n = 0; n < this.myFiles.length; n++) i.append("files", this.myFiles[n]);
                             void 0 !== this.uploadCall && this.uploadCall.unsubscribe();
                             let o = this.callService.call_response(this.data?.url, void 0, i);
                             this.uploadCall = o.subscribe(l => {
-                                this._snackBar.openFromComponent(w, {
+                                this._snackBar.openFromComponent(Z, {
                                     duration: 5e3,
                                     data: {
                                         message: "Sucessfully Uploaded file",
                                         status: "success"
                                     }
                                 });
                                 let r = new x;
                                 r.page = this.ds.dataLookup(!1), r.key = this.ds.all_input.get(this.url)?.upload_data?.name, r.value = this.ds.makeid(2), r.url = this.url, this.ds.data_setter.emit(r), this.myFiles = [], this.show = !1
                             }, l => {
-                                this.show = !1, this._snackBar.openFromComponent(w, {
+                                this.show = !1, this._snackBar.openFromComponent(Z, {
                                     duration: 5e3,
                                     data: {
                                         message: "Failed Uploaded file",
                                         status: "error"
                                     }
                                 })
                             })
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.Y36(f.D), t.Y36(Z), t.Y36(E.ux))
+                        return new(e || a)(t.Y36(f.D), t.Y36(w), t.Y36(N.ux))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-app-upload"]
                         ],
                         inputs: {
                             url: "url"
@@ -2378,20 +2385,20 @@
                             ["type", "file", 1, "file-upload", 3, "multiple", "change"],
                             [4, "ngIf"],
                             ["mode", "indeterminate"]
                         ],
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "input", 0), t.NdJ("change", function(o) {
                                 return n.saveData(o)
-                            }), t.qZA(), t.YNc(1, hn, 5, 0, "span", 1)), 2 & e && (t.Q6J("multiple", n.getMultiple()), t.xp6(1), t.Q6J("ngIf", n.show))
+                            }), t.qZA(), t.YNc(1, vn, 5, 0, "span", 1)), 2 & e && (t.Q6J("multiple", n.getMultiple()), t.xp6(1), t.Q6J("ngIf", n.show))
                         },
-                        dependencies: [G.pW, g.O5]
+                        dependencies: [j.pW, g.O5]
                     }), a
                 })(),
-                fn = (() => {
+                Tn = (() => {
                     class a {
                         constructor(e, n, i) {
                             this.dataService = e, this.sanitizer = n, this.callService = i
                         }
                         get_data() {
                             this.data = this.dataService.get_input_data(this.url)?.image_data
                         }
@@ -2406,15 +2413,15 @@
                             })
                         }
                         ngOnInit() {
                             this.get_data(), this.get_image()
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.Y36(f.D), t.Y36(v.H7), t.Y36(Z))
+                        return new(e || a)(t.Y36(f.D), t.Y36(v.H7), t.Y36(w))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-app-image"]
                         ],
                         inputs: {
                             url: "url"
@@ -2423,36 +2430,36 @@
                         vars: 5,
                         consts: [
                             ["mat-card-sm-image", "", 3, "src"]
                         ],
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "span"), t._UZ(1, "img", 0), t.qZA()), 2 & e && (t.xp6(1), t.Udp("height", n.height)("width", n.width), t.Q6J("src", n.imageURL, t.LSH))
                         },
-                        dependencies: [A.vP]
+                        dependencies: [J.vP]
                     }), a
                 })();
-            var xn = p(63156),
-                bn = p(74970),
-                Cn = p(98168),
-                vn = p(83151),
-                yn = p(27969);
+            var Sn = p(63156),
+                It = p(74970),
+                Pt = p(98168),
+                Qt = p(83151),
+                Yt = p(27969);
 
-            function Tn(a, s) {
+            function wn(a, s) {
                 if (1 & a && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & a) {
                     const e = s.$implicit;
                     t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
                 }
             }
-            let Sn = (() => {
+            let Zn = (() => {
                     class a {
                         constructor(e, n) {
-                            this.ds = e, this.callService = n, this.multi = !1, this.compareFn = (i, o) => i && o && i.id === o.id, this.items = [], this.ServerSideCtrl = new h.p4, this.ServerSideFilteringCtrl = new h.p4, this.searching = !1, this.filteredServerSideBanks = new ft.t(1), this._onDestroy = new xt.x
+                            this.ds = e, this.callService = n, this.multi = !1, this.compareFn = (i, o) => i && o && i.id === o.id, this.items = [], this.ServerSideCtrl = new m.p4, this.ServerSideFilteringCtrl = new m.p4, this.searching = !1, this.filteredServerSideBanks = new ot.t(1), this._onDestroy = new lt.x
                         }
                         ngOnInit() {
-                            this.originalData(), this.ServerSideFilteringCtrl.valueChanges.pipe((0, bn.h)(e => !!e), (0, Cn.b)(() => this.searching = !0), (0, j.R)(this._onDestroy), (0, vn.b)(200), (0, yn.U)(e => this.items && e ? e : []), (0, j.R)(this._onDestroy)).subscribe(e => {
+                            this.originalData(), this.ServerSideFilteringCtrl.valueChanges.pipe((0, It.h)(e => !!e), (0, Pt.b)(() => this.searching = !0), (0, E.R)(this._onDestroy), (0, Qt.b)(200), (0, Yt.U)(e => this.items && e ? e : []), (0, E.R)(this._onDestroy)).subscribe(e => {
                                 this.pullData(e).subscribe(i => {
                                     this.searching = !1;
                                     let r, o = this.ServerSideCtrl.value,
                                         l = i.simple_fitler_data;
                                     r = null !== o ? l.concat(o) : l, this.filteredServerSideBanks.next(r)
                                 }, i => {
                                     this.searching = !1
@@ -2477,15 +2484,15 @@
                         }
                         detectChange(e) {
                             let n = new x;
                             n.key = this.ds.all_input.get(this.url)?.simple_server_filter_data?.name, n.value = e.value, n.page = this.ds.dataLookup(this.isSidebar), n.url = this.url, this.ds.data_setter.emit(n)
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.Y36(f.D), t.Y36(Z))
+                        return new(e || a)(t.Y36(f.D), t.Y36(w))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-simple-server-filter"]
                         ],
                         inputs: {
                             url: "url",
@@ -2500,20 +2507,20 @@
                             [3, "formControl", "searching"],
                             [3, "value", 4, "ngFor", "ngForOf"],
                             [3, "value"]
                         ],
                         template: function(e, n) {
                             1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-select", 1, 2), t.NdJ("selectionChange", function(o) {
                                 return n.detectChange(o)
-                            }), t.TgZ(3, "mat-option"), t._UZ(4, "ngx-mat-select-search", 3), t.qZA(), t.YNc(5, Tn, 2, 2, "mat-option", 4), t.ALo(6, "async"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("formControl", n.ServerSideCtrl)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.ServerSideFilteringCtrl)("searching", n.searching), t.xp6(1), t.Q6J("ngForOf", t.lcZ(6, 5, n.filteredServerSideBanks)))
+                            }), t.TgZ(3, "mat-option"), t._UZ(4, "ngx-mat-select-search", 3), t.qZA(), t.YNc(5, wn, 2, 2, "mat-option", 4), t.ALo(6, "async"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("formControl", n.ServerSideCtrl)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.ServerSideFilteringCtrl)("searching", n.searching), t.xp6(1), t.Q6J("ngForOf", t.lcZ(6, 5, n.filteredServerSideBanks)))
                         },
-                        dependencies: [h.JJ, h.oH, T.ey, y.KE, at.gD, g.sg, st.nu, g.Ov]
+                        dependencies: [m.JJ, m.oH, T.ey, y.KE, et.gD, g.sg, nt.nu, g.Ov]
                     }), a
                 })(),
-                wn = (() => {
+                Dn = (() => {
                     class a {
                         constructor(e) {
                             this.sanitizer = e
                         }
                         transform(e) {
                             return this.sanitizer.bypassSecurityTrustResourceUrl(e)
                         }
@@ -2522,15 +2529,15 @@
                         return new(e || a)(t.Y36(v.H7, 16))
                     }, a.\u0275pipe = t.Yjl({
                         name: "safe",
                         type: a,
                         pure: !0
                     }), a
                 })(),
-                Zn = (() => {
+                Fn = (() => {
                     class a {
                         constructor(e, n) {
                             this.sanitizer = e, this.ds = n
                         }
                         ngOnInit() {
                             this.data = this.ds.get_input_data(this.url)?.iframe_data
                         }
@@ -2549,18 +2556,18 @@
                         vars: 5,
                         consts: [
                             [3, "src", "height", "width"]
                         ],
                         template: function(e, n) {
                             1 & e && (t._UZ(0, "iframe", 0), t.ALo(1, "safe")), 2 & e && t.Q6J("src", t.lcZ(1, 3, n.data.url), t.uOi)("height", n.data.height)("width", n.data.width)
                         },
-                        dependencies: [wn]
+                        dependencies: [Dn]
                     }), a
                 })(),
-                Mt = (() => {
+                Ut = (() => {
                     class a {
                         constructor(e, n, i, o, l) {
                             this.ds = e, this.sanitizer = n, this.api = i, this.renderer = o, this.document = l, this.loading = !0
                         }
                         ngOnInit() {
                             this.look_up = this.api.lookup(!1, this.url), this.page = this.ds.get_page(), this.ds.input_emitter.subscribe(n => {
                                 if (n.lookup === this.look_up)
@@ -2584,15 +2591,15 @@
                             })
                         }
                         striptHide() {
                             return void 0 === this.scriptStr
                         }
                     }
                     return a.\u0275fac = function(e) {
-                        return new(e || a)(t.Y36(f.D), t.Y36(v.H7), t.Y36(Ft), t.Y36(t.Qsj), t.Y36(g.K0))
+                        return new(e || a)(t.Y36(f.D), t.Y36(v.H7), t.Y36(At), t.Y36(t.Qsj), t.Y36(g.K0))
                     }, a.\u0275cmp = t.Xpm({
                         type: a,
                         selectors: [
                             ["app-custom-html"]
                         ],
                         inputs: {
                             url: "url"
@@ -2605,18 +2612,18 @@
                         ],
                         template: function(e, n) {
                             1 & e && t._UZ(0, "span", 0, 1), 2 & e && t.Q6J("innerHTML", n.htmlStr, t.oJD)
                         }
                     }), a
                 })();
 
-            function Dn(a, s) {
+            function kn(a, s) {
                 1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 2), t.qZA())
             }
-            let Fn = (() => {
+            let Jn = (() => {
                 class a {
                     constructor(e, n, i) {
                         this.ds = e, this.callService = n, this._snackBar = i, this.myFiles = [], this.show = !1
                     }
                     reactiveity(e, n = "") {
                         let i = new x;
                         i.page = this.ds.dataLookup(!1), i.key = this.ds.all_input.get(this.url)?.button_data?.name + "_" + e, i.value = "" === n ? this.ds.makeid(2) : n, i.url = this.url + "_" + e, this.ds.data_setter.emit(i)
@@ -2627,34 +2634,34 @@
                     trigger() {
                         this.reactiveity("triggered"), void 0 !== this.second_call && this.second_call.unsubscribe();
                         let e = this.callService.second_call_response(this.data.url, this.data.name, "");
                         this.second_call = e.subscribe(n => {
                             try {
                                 this.reactiveity("result", n.button_result)
                             } catch {}
-                            this._snackBar.openFromComponent(w, {
+                            this._snackBar.openFromComponent(Z, {
                                 duration: 5e3,
                                 data: {
                                     message: "API called Sucessfully ",
                                     status: "success"
                                 }
                             }), this.reactiveity("success"), this.show = !1
                         }, n => {
-                            this.show = !1, this.reactiveity("failed"), this._snackBar.openFromComponent(w, {
+                            this.show = !1, this.reactiveity("failed"), this._snackBar.openFromComponent(Z, {
                                 duration: 5e3,
                                 data: {
                                     message: "API called Failed",
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(f.D), t.Y36(Z), t.Y36(E.ux))
+                    return new(e || a)(t.Y36(f.D), t.Y36(w), t.Y36(N.ux))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-button"]
                     ],
                     inputs: {
                         url: "url"
@@ -2665,62 +2672,122 @@
                         ["mat-raised-button", "", "color", "primary", 2, "display", "inline-block", "position", "relative", 3, "click"],
                         [4, "ngIf"],
                         ["mode", "indeterminate"]
                     ],
                     template: function(e, n) {
                         1 & e && (t.TgZ(0, "button", 0), t.NdJ("click", function() {
                             return n.trigger()
-                        }), t._uU(1), t.qZA(), t.YNc(2, Dn, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.Oqu(n.data.name), t.xp6(1), t.Q6J("ngIf", n.show))
+                        }), t._uU(1), t.qZA(), t.YNc(2, kn, 5, 0, "span", 1)), 2 & e && (t.xp6(1), t.Oqu(n.data.name), t.xp6(1), t.Q6J("ngIf", n.show))
                     },
-                    dependencies: [L.lW, G.pW, g.O5]
+                    dependencies: [R.lW, j.pW, g.O5]
                 }), a
             })();
-            var Jt = p(31308),
-                Ot = p(89181);
+            var Ct = p(31308),
+                rt = p(14984),
+                vt = p(89181);
 
-            function kn(a, s) {
+            function An(a, s) {
+                if (1 & a && (t.TgZ(0, "mat-option", 5), t._uU(1), t.qZA()), 2 & a) {
+                    const e = s.$implicit;
+                    t.Q6J("value", e), t.xp6(1), t.hij(" ", e, " ")
+                }
+            }
+            let On = (() => {
+                class a extends Ct.mL {
+                    constructor(e, n) {
+                        super(n), this.callService = e, this.isLoading = !0, this.server_url = "", this.multi = !1, this.name = "", this.compareFn = (i, o) => i && o && i.id === o.id, this.items = [], this.ServerSideCtrl = new m.p4, this.ServerSideFilteringCtrl = new m.p4, this.searching = !1, this.filteredServerSideBanks = new ot.t(1), this._onDestroy = new lt.x
+                    }
+                    ngOnInit() {
+                        super.ngOnInit(), this.server_url = this.scopedSchema.url, this.multi = "true" === this.scopedSchema.multi || !1, this.name = this.scopedSchema.search_name, this.ServerSideFilteringCtrl.valueChanges.pipe((0, It.h)(e => !!e), (0, Pt.b)(() => this.searching = !0), (0, E.R)(this._onDestroy), (0, Qt.b)(200), (0, Yt.U)(e => this.items && e ? e : []), (0, E.R)(this._onDestroy)).subscribe(e => {
+                            this.pullData(e).subscribe(i => {
+                                this.searching = !1;
+                                let r, o = this.ServerSideCtrl.value,
+                                    l = i.simple_fitler_data;
+                                r = null !== o ? l.concat(o) : l, this.filteredServerSideBanks.next(r)
+                            }, i => {
+                                this.searching = !1, console.log(i)
+                            })
+                        })
+                    }
+                    isMulti() {
+                        return this.multi
+                    }
+                    pullData(e) {
+                        return this.callService.second_call_response(this.server_url, this.name, e)
+                    }
+                }
+                return a.\u0275fac = function(e) {
+                    return new(e || a)(t.Y36(w), t.Y36(vt.KT))
+                }, a.\u0275cmp = t.Xpm({
+                    type: a,
+                    selectors: [
+                        ["app-json-forms-server-side"]
+                    ],
+                    features: [t.qOj],
+                    decls: 7,
+                    vars: 7,
+                    consts: [
+                        ["appearance", "fill"],
+                        [3, "formControl", "multiple"],
+                        ["dataSelect", ""],
+                        [3, "formControl", "searching"],
+                        [3, "value", 4, "ngFor", "ngForOf"],
+                        [3, "value"]
+                    ],
+                    template: function(e, n) {
+                        1 & e && (t.TgZ(0, "mat-form-field", 0)(1, "mat-select", 1, 2)(3, "mat-option"), t._UZ(4, "ngx-mat-select-search", 3), t.qZA(), t.YNc(5, An, 2, 2, "mat-option", 4), t.ALo(6, "async"), t.qZA()()), 2 & e && (t.xp6(1), t.Q6J("formControl", n.form)("multiple", n.isMulti()), t.xp6(3), t.Q6J("formControl", n.ServerSideFilteringCtrl)("searching", n.searching), t.xp6(1), t.Q6J("ngForOf", t.lcZ(6, 5, n.filteredServerSideBanks)))
+                    },
+                    dependencies: [m.JJ, m.oH, T.ey, y.KE, et.gD, g.sg, nt.nu, g.Ov]
+                }), a
+            })();
+
+            function Mn(a, s) {
                 1 & a && (t.TgZ(0, "span"), t._UZ(1, "br")(2, "br")(3, "br")(4, "mat-progress-bar", 3), t.qZA())
             }
-            let An = (() => {
+            const In = (0, rt.xDy)((0, rt.TDq)("string"), (0, rt.wcO)(a => a.hasOwnProperty("url")));
+            let Pn = (() => {
                 class a {
                     constructor(e, n, i) {
-                        this.ds = e, this.callService = n, this._snackBar = i, this.show = !1, this.renderers = [...Jt.x]
+                        this.ds = e, this.callService = n, this._snackBar = i, this.show = !1, this.renderers = [...Ct.x, {
+                            tester: (0, rt.yMz)(5, In),
+                            renderer: On
+                        }]
                     }
                     ngOnInit() {
                         this.data = this.ds.all_input.get(this.url)?.form_data, this.formData = this.data.data
                     }
                     reactiveity(e) {
                         let n = new x;
                         n.page = this.ds.dataLookup(!1), n.key = this.ds.all_input.get(this.url)?.form_data?.name + "_" + e, n.value = this.ds.makeid(2), n.url = this.url + "_" + e, this.ds.data_setter.emit(n)
                     }
                     trigger() {
                         let e = new x;
                         e.page = this.ds.dataLookup(!1), e.url = this.url, e.key = this.data.name, e.value = this.formData, this.show = !0, this.ds.data_setter.emit(e), this.reactiveity("triggered");
                         let n = this.callService.call_response(this.data.submit_info.url, void 0, void 0);
                         this.call = n.subscribe(i => {
-                            this.reactiveity("success"), this._snackBar.openFromComponent(w, {
+                            this.reactiveity("success"), this._snackBar.openFromComponent(Z, {
                                 duration: 5e3,
                                 data: {
                                     message: "API called Sucessfully ",
                                     status: "success"
                                 }
                             }), this.show = !1
                         }, i => {
-                            this.reactiveity("failed"), this.show = !1, this._snackBar.openFromComponent(w, {
+                            this.reactiveity("failed"), this.show = !1, this._snackBar.openFromComponent(Z, {
                                 duration: 5e3,
                                 data: {
                                     message: "API called Failed",
                                     status: "error"
                                 }
                             })
                         })
                     }
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(f.D), t.Y36(Z), t.Y36(E.ux))
+                    return new(e || a)(t.Y36(f.D), t.Y36(w), t.Y36(N.ux))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-form"]
                     ],
                     inputs: {
                         url: "url"
@@ -2734,84 +2801,84 @@
                         ["mode", "indeterminate"]
                     ],
                     template: function(e, n) {
                         1 & e && (t.TgZ(0, "jsonforms", 0), t.NdJ("dataChange", function(o) {
                             return n.formData = o
                         }), t.qZA(), t.TgZ(1, "button", 1), t.NdJ("click", function() {
                             return n.trigger()
-                        }), t._uU(2), t.qZA(), t._UZ(3, "br"), t.YNc(4, kn, 5, 0, "span", 2)), 2 & e && (t.Q6J("data", n.formData)("schema", n.data.form_schema)("uischema", n.data.ui_schema)("renderers", n.renderers), t.xp6(2), t.Oqu(n.data.submit_info.name), t.xp6(2), t.Q6J("ngIf", n.show))
+                        }), t._uU(2), t.qZA(), t._UZ(3, "br"), t.YNc(4, Mn, 5, 0, "span", 2)), 2 & e && (t.Q6J("data", n.formData)("schema", n.data.form_schema)("uischema", n.data.ui_schema)("renderers", n.renderers), t.xp6(2), t.Oqu(n.data.submit_info.name), t.xp6(2), t.Q6J("ngIf", n.show))
                     },
-                    dependencies: [L.lW, G.pW, g.O5, Ot.C]
+                    dependencies: [R.lW, j.pW, g.O5, vt.C]
                 }), a
             })();
 
-            function Mn(a, s) {
+            function Qn(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-box", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Jn(a, s) {
+            function Yn(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-datetime", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function On(a, s) {
+            function Un(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-table", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function In(a, s) {
+            function En(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-plot", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Pn(a, s) {
+            function Nn(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-checkbox", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Qn(a, s) {
+            function Ln(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-radio", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function Yn(a, s) {
+            function Rn(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-slider", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function Un(a, s) {
+            function qn(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-button-toggle", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function En(a, s) {
+            function Hn(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-toggle", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function Nn(a, s) {
+            function Gn(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "app-entry-point", 7), t.NdJ("fx", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setFlex(l.url, i))
                     })("rd", function(i) {
@@ -2824,22 +2891,22 @@
                     const e = s.$implicit,
                         n = t.oxw(2);
                     let i, o, l, r, d;
                     t.xp6(1), t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", n.isSidebar)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "100%%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "100%")("fxFlex.xs", (null == (d = n.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
                 }
             }
 
-            function Ln(a, s) {
-                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, Nn, 3, 7, "span", 6), t.qZA()), 2 & a) {
+            function jn(a, s) {
+                if (1 & a && (t.TgZ(0, "span"), t.YNc(1, Gn, 3, 7, "span", 6), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("ngForOf", e.getURLs())
                 }
             }
 
-            function Rn(a, s) {
+            function Bn(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "mat-tab", 9), t._UZ(1, "br"), t.TgZ(2, "app-sub-entry-point", 10), t.NdJ("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setReactivity(l.url, i))
                     })("rd", function(i) {
@@ -2856,22 +2923,22 @@
                     const e = s.$implicit,
                         n = t.oxw(2);
                     let i, o, l, r, d;
                     t.Q6J("label", e.name || ""), t.xp6(2), t.Q6J("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("url", e.url)("isSidebar", n.isSidebar)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "100%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "100%")("fxFlex.xs", (null == (d = n.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
                 }
             }
 
-            function qn(a, s) {
-                if (1 & a && (t.TgZ(0, "span")(1, "mat-tab-group"), t.YNc(2, Rn, 3, 8, "mat-tab", 8), t.qZA()()), 2 & a) {
+            function zn(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "mat-tab-group"), t.YNc(2, Bn, 3, 8, "mat-tab", 8), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(2), t.Q6J("ngForOf", e.getURLs())
                 }
             }
 
-            function Hn(a, s) {
+            function Kn(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "mat-expansion-panel")(2, "mat-expansion-panel-header")(3, "mat-panel-title"), t._uU(4), t.qZA()(), t._UZ(5, "br"), t.TgZ(6, "mat-panel-description", 5)(7, "app-sub-entry-point", 11), t.NdJ("rd", function(i) {
                         const l = t.CHM(e).$implicit,
                             r = t.oxw(2);
                         return t.KtG(r.setReactivity(l.url, i))
                     })("fd", function(i) {
@@ -2884,127 +2951,127 @@
                     const e = s.$implicit,
                         n = t.oxw(2);
                     let i, o, l, r, d;
                     t.xp6(4), t.hij(" ", e.name, " "), t.xp6(3), t.Q6J("url", e.url)("isSidebar", n.isSidebar)("hidden", null == (i = n.reactivityData.get(e.url)) ? null : i.hidden)("fxFlex", (null == (o = n.flexData.get(e.url)) ? null : o.fxFlex) || "100%")("fxFlex.md", (null == (l = n.flexData.get(e.url)) ? null : l.fxFlex_md) || "100%")("fxFlex.sm", (null == (r = n.flexData.get(e.url)) ? null : r.fxFlex_sm) || "50%")("fxFlex.xs", (null == (d = n.flexData.get(e.url)) ? null : d.fxFlex_sm) || "100%")
                 }
             }
 
-            function Gn(a, s) {
-                if (1 & a && (t.TgZ(0, "span")(1, "mat-accordion"), t._UZ(2, "br")(3, "br"), t.YNc(4, Hn, 8, 8, "span", 6), t.qZA()()), 2 & a) {
+            function Xn(a, s) {
+                if (1 & a && (t.TgZ(0, "span")(1, "mat-accordion"), t._UZ(2, "br")(3, "br"), t.YNc(4, Kn, 8, 8, "span", 6), t.qZA()()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(4), t.Q6J("ngForOf", e.getURLs())
                 }
             }
 
-            function jn(a, s) {
+            function $n(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-simple-filter", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function Bn(a, s) {
+            function Wn(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-simple-server-filter", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function zn(a, s) {
+            function Vn(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-group-filter", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function Kn(a, s) {
+            function ta(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-input", 4), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)("isSidebar", e.isSidebar)
                 }
             }
 
-            function Xn(a, s) {
+            function ea(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-app-download", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Wn(a, s) {
+            function na(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-app-upload", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function $n(a, s) {
+            function aa(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-app-image", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function Vn(a, s) {
+            function ia(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-highchart", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function ta(a, s) {
+            function sa(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-app-iframe", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function ea(a, s) {
+            function oa(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-custom-html", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.url)
                 }
             }
 
-            function na(a, s) {
+            function la(a, s) {
                 if (1 & a && (t.TgZ(0, "span", 5), t._UZ(1, "app-button", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function aa(a, s) {
+            function ra(a, s) {
                 if (1 & a && (t.TgZ(0, "span"), t._UZ(1, "app-form", 3), t.qZA()), 2 & a) {
                     const e = t.oxw();
                     t.xp6(1), t.Q6J("url", e.look_up)
                 }
             }
 
-            function ia(a, s) {
+            function pa(a, s) {
                 1 & a && (t.TgZ(0, "span"), t._UZ(1, "mat-progress-bar", 12), t.qZA())
             }
 
-            function sa(a, s) {
+            function ca(a, s) {
                 if (1 & a) {
                     const e = t.EpF();
                     t.TgZ(0, "span")(1, "button", 13), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.copy_error())
                     }), t.TgZ(2, "mat-icon"), t._uU(3, "content_copy"), t.qZA(), t.TgZ(4, "span"), t._uU(5, "Copy Error"), t.qZA()(), t.TgZ(6, "button", 13), t.NdJ("click", function() {
                         t.CHM(e);
                         const i = t.oxw();
                         return t.KtG(i.force_refresh())
                     }), t.TgZ(7, "mat-icon"), t._uU(8, "refresh"), t.qZA(), t.TgZ(9, "span"), t._uU(10, "Refresh Data"), t.qZA()()()
                 }
             }
-            let oa = (() => {
+            let da = (() => {
                 class a {
                     constructor(e, n, i, o) {
-                        this.ds = e, this.clipboard = n, this.dialog = i, this.api = o, this.rd = new t.vpe, this.fd = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.reactive = new It, this.d = new Map, this.loading = !0, this.failed = !1
+                        this.ds = e, this.clipboard = n, this.dialog = i, this.api = o, this.rd = new t.vpe, this.fd = new t.vpe, this.reactivityData = new Map, this.flexData = new Map, this.reactive = new Et, this.d = new Map, this.loading = !0, this.failed = !1
                     }
                     ngOnInit() {
                         this.look_up = this.api.lookup(this.isSidebar, this.url), this.page = this.ds.get_page(), this.ds.input_emitter.subscribe(n => {
                             if (n.lookup === this.look_up)
                                 if (void 0 !== n.message) this.loading = !0, this.failed = !0, this.error = n.message, this.tooltip_data = void 0, this.dialog_data = void 0, this.name = void 0, this.type = void 0;
                                 else if (n.calling) this.loading = !0, this.failed = !1, this.tooltip_data = void 0, this.dialog_data = void 0, this.name = void 0, this.type = void 0;
                             else {
@@ -3033,23 +3100,23 @@
                     copy_error() {
                         this.clipboard.copy(this.error)
                     }
                     force_refresh() {
                         this.api.getData(!0, this.url, this.look_up, this.page, this.isSidebar, "")
                     }
                     openDialog() {
-                        this.dialog_data && this.dialog.open(Ze, {
+                        this.dialog_data && this.dialog.open(Oe, {
                             height: this.dialog_data.height,
                             width: this.dialog_data.width,
                             data: this.dialog_data.url
                         })
                     }
                 }
                 return a.\u0275fac = function(e) {
-                    return new(e || a)(t.Y36(f.D), t.Y36(ct.TU), t.Y36(V.uw), t.Y36(Ft))
+                    return new(e || a)(t.Y36(f.D), t.Y36(_t.TU), t.Y36(V.uw), t.Y36(At))
                 }, a.\u0275cmp = t.Xpm({
                     type: a,
                     selectors: [
                         ["app-sub-entry-point"]
                     ],
                     inputs: {
                         url: "url",
@@ -3076,41 +3143,41 @@
                         [3, "url", "isSidebar", "hidden", "fxFlex", "fxFlex.md", "fxFlex.sm", "fxFlex.xs", "rd", "fd"],
                         ["mode", "query"],
                         ["mat-menu-item", "", 3, "click"]
                     ],
                     template: function(e, n) {
                         if (1 & e && (t.TgZ(0, "span", 0), t.NdJ("click", function() {
                                 return n.openDialog()
-                            }), t.YNc(1, Mn, 2, 1, "span", 1), t.YNc(2, Jn, 2, 2, "span", 1), t.YNc(3, On, 2, 1, "span", 1), t.YNc(4, In, 2, 1, "span", 1), t.YNc(5, Pn, 2, 1, "span", 2), t.YNc(6, Qn, 2, 2, "span", 2), t.YNc(7, Yn, 2, 2, "span", 2), t.YNc(8, Un, 2, 2, "span", 2), t.YNc(9, En, 2, 2, "span", 2), t.YNc(10, Ln, 2, 1, "span", 1), t.YNc(11, qn, 3, 1, "span", 1), t.YNc(12, Gn, 5, 1, "span", 1), t.YNc(13, jn, 2, 2, "span", 2), t.YNc(14, Bn, 2, 2, "span", 2), t.YNc(15, zn, 2, 2, "span", 2), t.YNc(16, Kn, 2, 2, "span", 2), t.YNc(17, Xn, 2, 1, "span", 2), t.YNc(18, Wn, 2, 1, "span", 2), t.YNc(19, $n, 2, 1, "span", 1), t.YNc(20, Vn, 2, 1, "span", 1), t.YNc(21, ta, 2, 1, "span", 1), t.YNc(22, ea, 2, 1, "span", 1), t.YNc(23, na, 2, 1, "span", 2), t.YNc(24, aa, 2, 1, "span", 1), t.YNc(25, ia, 2, 0, "span", 1), t._UZ(26, "br"), t.YNc(27, sa, 11, 0, "span", 1), t.qZA()), 2 & e) {
+                            }), t.YNc(1, Qn, 2, 1, "span", 1), t.YNc(2, Yn, 2, 2, "span", 1), t.YNc(3, Un, 2, 1, "span", 1), t.YNc(4, En, 2, 1, "span", 1), t.YNc(5, Nn, 2, 1, "span", 2), t.YNc(6, Ln, 2, 2, "span", 2), t.YNc(7, Rn, 2, 2, "span", 2), t.YNc(8, qn, 2, 2, "span", 2), t.YNc(9, Hn, 2, 2, "span", 2), t.YNc(10, jn, 2, 1, "span", 1), t.YNc(11, zn, 3, 1, "span", 1), t.YNc(12, Xn, 5, 1, "span", 1), t.YNc(13, $n, 2, 2, "span", 2), t.YNc(14, Wn, 2, 2, "span", 2), t.YNc(15, Vn, 2, 2, "span", 2), t.YNc(16, ta, 2, 2, "span", 2), t.YNc(17, ea, 2, 1, "span", 2), t.YNc(18, na, 2, 1, "span", 2), t.YNc(19, aa, 2, 1, "span", 1), t.YNc(20, ia, 2, 1, "span", 1), t.YNc(21, sa, 2, 1, "span", 1), t.YNc(22, oa, 2, 1, "span", 1), t.YNc(23, la, 2, 1, "span", 2), t.YNc(24, ra, 2, 1, "span", 1), t.YNc(25, pa, 2, 0, "span", 1), t._UZ(26, "br"), t.YNc(27, ca, 11, 0, "span", 1), t.qZA()), 2 & e) {
                             let i;
                             t.Q6J("matTooltip", null !== (i = null == n.tooltip_data ? null : n.tooltip_data.label) && void 0 !== i ? i : "")("matTooltipDisabled", void 0 === n.tooltip_data), t.xp6(1), t.Q6J("ngIf", "box" === n.type), t.xp6(1), t.Q6J("ngIf", "date" === n.type), t.xp6(1), t.Q6J("ngIf", "table" === n.type), t.xp6(1), t.Q6J("ngIf", "chart" === n.type), t.xp6(1), t.Q6J("ngIf", "checkbox" === n.type), t.xp6(1), t.Q6J("ngIf", "radio" === n.type), t.xp6(1), t.Q6J("ngIf", "slider" === n.type), t.xp6(1), t.Q6J("ngIf", "button_toggle" === n.type), t.xp6(1), t.Q6J("ngIf", "toggle" === n.type), t.xp6(1), t.Q6J("ngIf", "multi_list" === n.type), t.xp6(1), t.Q6J("ngIf", "multi_tabs" === n.type), t.xp6(1), t.Q6J("ngIf", "multi_expand" === n.type), t.xp6(1), t.Q6J("ngIf", "simple_filter" == n.type), t.xp6(1), t.Q6J("ngIf", "simple_server_filter" == n.type), t.xp6(1), t.Q6J("ngIf", "group_filter" == n.type), t.xp6(1), t.Q6J("ngIf", "input" == n.type), t.xp6(1), t.Q6J("ngIf", "download" == n.type), t.xp6(1), t.Q6J("ngIf", "upload" == n.type), t.xp6(1), t.Q6J("ngIf", "image" == n.type), t.xp6(1), t.Q6J("ngIf", "highchart" == n.type), t.xp6(1), t.Q6J("ngIf", "iframe" == n.type), t.xp6(1), t.Q6J("ngIf", "custom_html" == n.type), t.xp6(1), t.Q6J("ngIf", "button" == n.type), t.xp6(1), t.Q6J("ngIf", "form" == n.type), t.xp6(1), t.Q6J("ngIf", n.loading), t.xp6(2), t.Q6J("ngIf", n.failed)
                         }
                     },
-                    dependencies: [S.yH, Y.pp, Y.ib, Y.yz, Y.yK, Y.u4, q.Hw, W.OP, G.pW, gt.SP, gt.uX, Zt.gM, g.sg, g.O5, Fe, Me, Le, Re, Be, $e, $, Ve, en, nn, on, cn, a, un, mn, gn, fn, xn.q, Sn, Zn, Mt, Fn, An],
+                    dependencies: [S.yH, Y.pp, Y.ib, Y.yz, Y.yK, Y.u4, H.Hw, $.OP, j.pW, bt.SP, bt.uX, kt.gM, g.sg, g.O5, Ie, Ye, Be, ze, Ve, sn, W, on, rn, pn, un, gn, a, xn, Cn, yn, Tn, Sn.q, Zn, Fn, Ut, Jn, Pn],
                     styles: [".center[_ngcontent-%COMP%]{display:flex;justify-content:center;align-items:center}.full[_ngcontent-%COMP%]{width:100%;display:flex;justify-content:center;align-items:center}"]
                 }), a
             })();
-            var la = p(44740),
-                ra = p(44083);
-            let pa = (() => {
+            var ua = p(44740),
+                _a = p(44083);
+            let ma = (() => {
                 class a {}
                 return a.\u0275fac = function(e) {
                     return new(e || a)
                 }, a.\u0275mod = t.oAB({
                     type: a,
-                    bootstrap: [Vt]
+                    bootstrap: [se]
                 }), a.\u0275inj = t.cJS({
-                    providers: [ra.N],
-                    imports: [ye.o9, h.u5, h.UX, le.rt, re.XD, ct.Iq, ue.U5, ut.HT, _e.nZ, pe._t, me.Bb, he.g, ge._r, L.ot, _t.vV, A.QW, St.p9, fe.Hi, xe.T5, U.FA, V.Is, yt.t, Y.To, tt.N6, q.Ps, nt.c, H.ie, W.Tx, T.XK, mt.TU, G.Cv, be.Cq, ht.Fk, T.si, at.LD, et.SJ, wt.KP, dt.rP, E.ZX, it.JX, M.p0, gt.Nh, vt.g0, Zt.AV, Ce.dp, ve.U8, ce.eL, de.Cl, v.b2, N.JF, se, F.Bz, oe.PW, bt.xu, Dt.Ns.forRoot({
+                    providers: [_a.N],
+                    imports: [Fe.o9, m.u5, m.UX, _e.rt, me.XD, _t.Iq, xe.U5, ht.HT, be.nZ, he._t, Ce.Bb, ve.g, ye._r, R.ot, gt.vV, J.QW, Dt.p9, Te.Hi, Se.T5, U.FA, V.Is, wt.t, Y.To, tt.N6, H.Ps, it.c, G.ie, $.Tx, T.XK, ft.TU, j.Cv, we.Cq, xt.Fk, T.si, et.LD, at.SJ, Ft.KP, mt.rP, N.ZX, st.JX, A.p0, bt.Nh, St.g0, kt.AV, Ze.dp, De.U8, ge.eL, fe.Cl, v.b2, L.JF, de, F.Bz, ue.PW, yt.xu, Jt.Ns.forRoot({
                         echarts: () => p.e(275).then(p.bind(p, 36275))
-                    }), st.Co, At.pL, la.SD, Ot.R2, Jt.D]
+                    }), nt.Co, Mt.pL, ua.SD, vt.R2, Ct.D]
                 }), a
             })();
-            t.B6R($, function() {
-                return [A.a8, A.dk, A.dn, A.rt, g.O5, oa, Mt]
-            }, []), (0, t.G48)(), v.q6().bootstrapModule(pa).catch(a => console.error(a)), console.info("Angular CDK version", ot.q.full), console.info("Angular Material version", T.q4.full)
+            t.B6R(W, function() {
+                return [J.a8, J.dk, J.dn, J.rt, g.O5, da, Ut]
+            }, []), (0, t.G48)(), v.q6().bootstrapModule(ma).catch(a => console.error(a)), console.info("Angular CDK version", pt.q.full), console.info("Angular Material version", T.q4.full)
         }
     },
     D => {
-        D.O(0, [736], () => D(D.s = 79)), D.O()
+        D.O(0, [736], () => D(D.s = 41877)), D.O()
     }
 ]);
```

### Comparing `zen_dash-0.5.8/zen_dash/static/polyfills.0a8881ff36766b1e.js` & `zen_dash-0.5.9/zen_dash/static/polyfills.0a8881ff36766b1e.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/runtime.6a9b461ae5a72237.js` & `zen_dash-0.5.9/zen_dash/static/runtime.6a9b461ae5a72237.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/styles.362a8260c32d36d9.css` & `zen_dash-0.5.9/zen_dash/static/styles.362a8260c32d36d9.css`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/static/vendor.43228e876ccc446f.js` & `zen_dash-0.5.9/zen_dash/static/vendor.923d0d3ca0754580.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,13 @@
 (self.webpackChunkfrontend = self.webpackChunkfrontend || []).push([
     [736], {
         31308: (At, mt, V) => {
             "use strict";
             V.d(mt, {
+                mL: () => w,
                 D: () => xn,
                 x: () => Vi
             }), V(11524);
             var z = V(88692),
                 K = V(96100),
                 C = V(20092),
                 h = V(61637),
@@ -1839,14 +1840,15 @@
                 Ohw: () => xi,
                 OmS: () => un,
                 OrV: () => Qo,
                 PDY: () => vn,
                 PUn: () => bo,
                 Q8v: () => Ke,
                 RCH: () => Rn,
+                TDq: () => Bi,
                 U1p: () => Tr,
                 UvK: () => rr,
                 W52: () => fs,
                 WX3: () => Xs,
                 Wdb: () => Pr,
                 XuX: () => xo,
                 YC9: () => Yi,
@@ -1865,14 +1867,15 @@
                 or: () => Ge,
                 qPj: () => en,
                 sJu: () => lt,
                 spq: () => Kr,
                 uog: () => ye,
                 v6: () => as,
                 wZT: () => Hn,
+                wcO: () => Le,
                 xDy: () => Fe,
                 xq9: () => ms,
                 yMz: () => zi,
                 zY3: () => Zi
             });
             var A = V(12232),
                 z = V.n(A),
```

### Comparing `zen_dash-0.5.8/zen_dash/support/__init__.py` & `zen_dash-0.5.9/zen_dash/support/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/tag/__init__.py` & `zen_dash-0.5.9/zen_dash/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/zen_dash/websocket/__init__.py` & `zen_dash-0.5.9/zen_dash/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.8/setup.py` & `zen_dash-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'websockets>=10.4,<11.0']
 
 entry_points = \
 {'console_scripts': ['create_zen = zen_dash.cli.main:create_zen']}
 
 setup_kwargs = {
     'name': 'zen-dash',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'Simple yet scable and production ready python dashboard that is better than shiny application for business.',
     'long_description': "# What is Zen Dash?\nZen Dash, a python package, simplifies the building analytics/BI dashboard process while providing enterprise-level scalability, stability, and performance. You can use FastAPI and Flask to host the application. \n\n\n[![Downloads](https://static.pepy.tech/badge/zen-dash)](https://pepy.tech/project/zen-dash)\n[![python](https://img.shields.io/pypi/pyversions/zen-dash.svg?color=green)](https://img.shields.io/pypi/pyversions/zen-dash.svg?color=green)\n[![license](https://img.shields.io/github/license/Zen-Reportz/zen_dash?color=green)](https://img.shields.io/github/license/Zen-Reportz/zen_dash?color=green)\n[![version](https://img.shields.io/pypi/v/zen-dash?color=green&label=pypi%20package)](https://img.shields.io/pypi/v/zen-dash?color=green&label=pypi%20package)\n\n# How to run demo\nLearn more about how to run demo here: [Link](https://github.com/Zen-Reportz/zen_dash/wiki/How-can-I-run-demo-%3F)\n\n# How to create zen dash\nLearn more about how to crate zen dash: [Link](https://github.com/Zen-Reportz/zen_dash/wiki/How-to-create-new-zen-dash)\n\n# How to Contribute\nPlease visit this page to learn how to contribute: [Link](https://github.com/Zen-Reportz/zen_dash/blob/main/how_to_contribute.md)\n\n# Why did I build Zen Dash?\n\nThere are many dashboarding solutions, like shiny (R, python), Streamlit, and others. I have used all of these solutions. I enjoy building solutions. However, all of these tools and libraries lack one vital point. They are not enterprise-ready solutions. They are fragile and not scalable solutions. So, whenever I built analytics/ BI Dashboards, Even after many bandages, dashboards were delicate and unstable. \n\nBefore explaining the problem and its reasons, I like to describe the issues we are trying to solve. \n\n* Some of our dashboards need to be used by more than 200 people simultaneously and require a sub-second response to be practical. They will use more than 8 hours straight for work. The dashboard should not crash during usage.\n\n* more than a hundred field team members are using our other dashboard, which is spread across multiple countries. Their internet speed is not ideal like office, so the analytics dashboard needs to be anti-fragile. They should be able to share their data with our customers on the ground without worrying about the dashboard crashing or refreshing data. \n\n* the Third group of the dashboard is far more complex and sensitive since we integrated it into one of our company production environments. This dashboard needs to better code isolation for testing, so they deployed it, so we can be sure it is not breaking the company production environment. \n\nSo, I invested time in the zen-dash, which addresses these problems. Before jumping into the zen-dash, I want to show you what we have done to make anti-fragile systems using other analytics solutions. I will also explain why it is failing. You might want to try a zen dash to elevate pains in these stages. \n\n\n* Building plumber or fastapi/flask to offload computation. \nGood thing: application becomes somewhat better at responding\nBad thing: now, code is in multiple locations, which makes it difficult to onboard and debug. If we use shiny with python, it is difficult for some team members to understand what they are doing.\n\n* Rather than dashboards, we started to provide more reports. However, this, in turn, created more work to report on building and maintenance.\n\n* Building simpler dashboards with limited functionality or exploration. We also get pushed back on this type of dashboard because people want to know more than what limited functionality dashboard what returns\n\n* Using Tableau to deliver data to field or high requirements teams. Tableau is not a perfect solution, either. It limits what analytics tools we can use.\n\n\nIf you see these signs in your analytics dashboarding solutions, you face a similar and painful situation.\n\n\n# Why are other tools creating such issues?\n\nLet me explain in technical detail. Here I am focusing on specifically Shiny and Streamlit because both face similar situations. After all, they are using the same architecture and software design. In a single word, it is due to incompatible architecture and software design. \n\nThey are facing two main issues.\n\n* Websocket\n* Lack of separation between UI and backend (specifically with shiny).\n\n\nWebsocket is one great tool where you can connect the front and back end once and send as much data as you want between them. \n\nThe chat system uses Websocket. Websocket simplifies your communication architecture when you use WebSocket over the rest API. It is an effective tool for communicating real-time data with lower overhead. Websocket keeps the connection open to the backend server so that new data transfers don't require creating a new link and overhead related to it. \n\nHowever, this constant connection makes a delicate system. It can break for any reason. So, when shiny apps WebSocket crashes, it grays out the screen, and you must start again from scratch. You will lose all filter selections you have made. I believe this is done to reduce overhead to the complexity of code on the shiny side. Because of it, it is not an enterprise-grade solution. Due to these design selections, we are facing problems 1 and 2.\n\nAnother issue with the WebSocket will create an artificial choke point at the backend level since R is a single thread with poor async support. In R, code usually runs sequentially. You have to use the API pool to redistribute the load on other machines. However, R is choking data push even when an API pool is used. So if we offload work on other services using the rest API pool, it has to wait until all processes are finished. Even if threading support is in python, we are not thinking about additional processing we need where threading is not a good option. The best option is to do multiprocessing. To do that, you need a different type of software design. I have seen situations regularly where shiny renders time well over 1 min when you have too many things to render on the page. These limitations are attributing problems 2 and 3\n\nIf WebSocket is used, you select only one machine/service to respond. So single service needs to process all requests and respond to them. Because of it, we had to create situation one to address this. These design is attributing problem 1\n\nThe second biggest issue with shiny is not separating UI from the backend. This design is excellent for rapid development, but if misused, it can slow down your application. It creates problems precisely when you want to render a large data example table. Shiny, rather than sending data for the table, the backend converts to HTML code and pushes HTML code as a string through WebSocket. This process becomes cumbersome very quickly because sending just data will be light, but sending HTML as a string adds quite a bit of load. In addition, you have to use eval or similar code to evaluate the code base, which adds security venerability and other overhead processes. It also slowdowns applications.\n\n\n# How much does zen dash make a difference?\nA dashboard that regularly took more than 60 seconds to load response data within ten or fewer seconds. \n\nOur dashboard has become more stable. If the internet connection is slow or fast, it doesn't impact the entire application.\n\nThe dashboard can run for days at a time without stability issues.\n\nHow do we achieve it? After understanding the limitation of the WebSocket, I decided to remove the WebSocket for communicating information. Instead, it will send data using a traditional HTTP request. \n\nUI is prebuilt in angular and complies, where you can provide what to render using angular flex and material design. \n\n# Docs\nhttps://zen-reportz.github.io/zen_dash/index.html\n",
     'author': 'Zen',
     'author_email': 'zenreportz@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://zen-reportz.github.io/zen_dash/index.html',
```

### Comparing `zen_dash-0.5.8/PKG-INFO` & `zen_dash-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-dash
-Version: 0.5.8
+Version: 0.5.9
 Summary: Simple yet scable and production ready python dashboard that is better than shiny application for business.
 Home-page: https://zen-reportz.github.io/zen_dash/index.html
 License: MIT
 Author: Zen
 Author-email: zenreportz@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

