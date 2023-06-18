# Comparing `tmp/airsupply-0.3.2.tar.gz` & `tmp/airsupply-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airsupply-0.3.2.tar", max compression
+gzip compressed data, was "airsupply-0.4.tar", max compression
```

## Comparing `airsupply-0.3.2.tar` & `airsupply-0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0        0 2020-01-24 03:52:19.000000 airsupply-0.3.2/airsupply/__init__.py
--rw-r--r--   0        0        0       30 2020-01-24 03:52:44.000000 airsupply-0.3.2/airsupply/__main__.py
--rw-r--r--   0        0        0      369 2020-01-29 08:19:41.000000 airsupply-0.3.2/airsupply/apk.py
--rw-r--r--   0        0        0     1974 2021-08-13 17:22:43.697357 airsupply-0.3.2/airsupply/cli.py
--rw-r--r--   0        0        0     4470 2021-08-09 18:09:48.584753 airsupply-0.3.2/airsupply/html.jinja2
--rw-r--r--   0        0        0     3634 2021-05-11 18:40:43.740378 airsupply-0.3.2/airsupply/ipa.py
--rw-r--r--   0        0        0     1673 2021-05-11 18:41:16.178945 airsupply-0.3.2/airsupply/ipa_manifest.jinja2
--rw-r--r--   0        0        0      934 2021-08-09 15:12:41.149734 airsupply-0.3.2/airsupply/local.py
--rw-r--r--   0        0        0     4557 2021-09-02 03:55:31.275493 airsupply-0.3.2/airsupply/push.py
--rw-r--r--   0        0        0     1372 2021-08-13 17:22:37.682840 airsupply-0.3.2/airsupply/s3.py
--rw-r--r--   0        0        0      166 2020-01-29 08:19:41.000000 airsupply-0.3.2/airsupply/templates.py
--rw-r--r--   0        0        0      481 2021-09-02 03:55:42.237739 airsupply-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      793 2021-09-02 03:56:03.952309 airsupply-0.3.2/setup.py
--rw-r--r--   0        0        0      584 2021-09-02 03:56:03.952525 airsupply-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-01-24 03:52:19.000000 airsupply-0.4/airsupply/__init__.py
+-rw-r--r--   0        0        0       30 2020-01-24 03:52:44.000000 airsupply-0.4/airsupply/__main__.py
+-rw-r--r--   0        0        0      369 2020-01-29 08:19:41.000000 airsupply-0.4/airsupply/apk.py
+-rw-r--r--   0        0        0     2042 2023-06-18 18:04:25.108912 airsupply-0.4/airsupply/cli.py
+-rw-r--r--   0        0        0     6987 2023-06-18 20:13:03.097247 airsupply-0.4/airsupply/html.jinja2
+-rw-r--r--   0        0        0     3822 2023-06-18 20:46:16.489617 airsupply-0.4/airsupply/ipa.py
+-rw-r--r--   0        0        0     1673 2021-05-11 18:41:16.178945 airsupply-0.4/airsupply/ipa_manifest.jinja2
+-rw-r--r--   0        0        0      987 2023-06-18 20:40:42.782744 airsupply-0.4/airsupply/local.py
+-rw-r--r--   0        0        0     5746 2023-06-18 18:35:47.415996 airsupply-0.4/airsupply/push.py
+-rw-r--r--   0        0        0     1441 2023-06-18 20:40:55.247744 airsupply-0.4/airsupply/s3.py
+-rw-r--r--   0        0        0      166 2020-01-29 08:19:41.000000 airsupply-0.4/airsupply/templates.py
+-rw-r--r--   0        0        0      497 2023-06-18 20:46:34.081842 airsupply-0.4/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 airsupply-0.4/PKG-INFO
```

### Comparing `airsupply-0.3.2/airsupply/cli.py` & `airsupply-0.4/airsupply/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,29 +39,33 @@
     )
 
     url = push(target, packages, prefix=prefix, overwrite_index=overwrite_index)
     click.echo(url)
 
 @click.command('local:push')
 @click.option('--url', required=True)
+@click.option('--root')
 @click.option('--prefix')
 @click.option('--overwrite-index', is_flag=True, default=False)
 @click.argument('packages', nargs=-1, required=True)
-def local_push(packages, url, prefix, overwrite_index):
+def local_push(packages, url, root, prefix, overwrite_index):
     from .local import LocalTarget
     from .push import push
 
     # it's surprising when the final segment is chopped off by urljoin
     # so ensure there's always a trailing slash
     if not url.endswith('/'):
         url += '/'
 
+    if not root:
+        root = os.getcwd()
+
     target = LocalTarget(
         url=url,
-        root_dir=os.getcwd(),
+        root_dir=root,
     )
 
     url = push(target, packages, prefix=prefix, overwrite_index=overwrite_index)
     click.echo(url)
 
 main.add_command(s3_push)
 main.add_command(local_push)
```

### Comparing `airsupply-0.3.2/airsupply/html.jinja2` & `airsupply-0.4/airsupply/html.jinja2`

 * *Files 26% similar despite different names*

```diff
@@ -5,53 +5,99 @@
   <meta name="viewport" content="initial-scale=1.0, user-scalable=no">
   <title>
     {{ packages[0].display_name }}
     v{{ packages[0].version_name }}
     ({{ packages[0].version_code }})
   </title>
   <style type="text/css">
+    button {
+      all: unset;
+    }
+
+    .hidden {
+      display: none;
+    }
+    .disabled {
+      opacity: 0.5;
+    }
+
+    .modal {
+      display: none;
+      position: fixed; /* Stay in place */
+      z-index: 1; /* Sit on top */
+      left: 0;
+      top: 0;
+      width: 100%; /* Full width */
+      height: 100%; /* Full height */
+      overflow: auto; /* Enable scroll if needed */
+      background-color: rgb(0,0,0); /* Fallback color */
+      background-color: rgba(0,0,0,0.4); /* Black w/ opacity */
+    }
+    .modal-content {
+      background-color: #fefefe;
+      margin: 15% auto; /* 15% from the top and centered */
+      padding: 20px;
+      border: 1px solid #888;
+      border-radius: 20px;
+      width: 80%; /* Could be more or less, depending on screen size */
+      max-width: 400px;
+    }
+    .modal-close {
+      color: #aaa;
+      float: right;
+      font-size: 28px;
+      font-weight: bold;
+      line-height: 0px;
+    }
+    .modal-close:hover,
+    .modal-close:focus {
+      color: black;
+      text-decoration: none;
+      cursor: pointer;
+    }
+
     body {
       font-family: Helvetica, Arial, sans-serif;
       text-align: center;
       color: #444;
       font-size: 18px;
     }
-    img {
-      display: block;
-      margin: 1em auto;
-      border: none;
-      width: 120px;
-      height: 120px;
-      border-radius: 20px;
+    p {
+      color: #999
     }
-    .btn, a.btn, a.btn:visited, a.btn:hover, a.btn:link {
+
+    .btn, .btn:visited, .btn:hover, .btn:link {
       display: inline-block;
       border-radius: 3px;
       background-color: #0095c8;
       color: white;
       padding: .8em 1em;
       text-decoration: none;
     }
-    a.btn:hover {
+    .btn:hover {
       background-color: #00bbfb;
       color: white;
     }
-    p {
-      color: #999
-    }
-    .hidden {
-      display: none;
+
+    .app-icon {
+      display: block;
+      margin: 1em auto;
+      border: none;
+      width: 120px;
+      height: 120px;
+      border-radius: 20px;
     }
-    .disabled {
-      opacity: 0.5;
+
+    #qrcode img, #qrcode canvas {
+      margin: auto;
     }
   </style>
 </head>
 <body>
-  <select id="package-select" class="hidden">
+  <select id="package-select">
     {% for pkg in packages %}
     <option value="pkg-{{ loop.index }}">
       [{{ pkg.package_type }}]
       {{ pkg.display_name }}
       v{{ pkg.version_name }}
       ({{ pkg.version_code }})
     </option>
@@ -62,49 +108,53 @@
     id="pkg-{{ loop.index }}"
     class="package"
     data-title="{{ pkg.display_name }} v{{ pkg.version_name }} ({{ pkg.version_code }})"
     data-type="{{ pkg.package_type }}"
   >
     <h1>{{ pkg.display_name }}</h1>
     <h2>{{ pkg.version_name }} ({{ pkg.version_code }})</h2>
-  {% if pkg.package_type == 'ipa' %}
     {% if pkg.image_url %}
-    <img src="{{ pkg.image_url | safe }}">
+    <img class="app-icon" src="{{ pkg.image_url | safe }}">
     {% endif %}
     <a
-      href="itms-services://?action=download-manifest&amp;url={{ pkg.manifest_url | urlencode }}"
+      href="{{ pkg.install_url | safe }}"
       class="btn install-btn"
     >
-      Tap to install
+      Install
     </a>
-  {% elif pkg.package_type == 'apk' %}
-    {% if pkg.image_url %}
-    <img src="{{ pkg.image_url | safe }}">
-    {% endif %}
+    <button class="btn show-qr-btn">
+      Show QR
+    </button>
     <a
-      href="{{ pkg.apk_url | safe }}"
-      class="btn install-btn"
+      href="{{ pkg.download_url | safe }}"
+      class="btn"
     >
-      Tap to install
+      Download
     </a>
-  {% else %}
-    {{ die('Unsupported package type') }}
-  {% endif %}
     <p class="comment">
       {% set os = 'Android' if pkg.package_type == 'apk' else 'WatchOS' if pkg.platform == 'watchos' else 'iOS' %}
       {% if pkg.minimum_os_version is defined %}
       This app requires <b>{{ os }} {{ pkg.minimum_os_version }}</b> or higher.
       {% else %}
       This app requires <b>{{ os }}</b>.
       {% endif %}
     </p>
     <p class="comment">{{ pkg.app_id }}</p>
   </div>
 {% endfor %}
 
+  <div id="qr-modal" class="modal">
+    <div class="modal-content">
+      <span class="modal-close">&times;</span>
+      <div id="qrcode"></div>
+    </div>
+  </div>
+
+  <!-- https://cdnjs.com/libraries/qrcodejs -->
+  <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js" integrity="sha512-CNgIRecGo7nphbeZ04Sc13ka07paqdeTu0WR1IM4kNcpmBAUSHSQX0FslNhTDadL4O5SAGapGt4FodqL8My0mA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
   <script>
   var OS = (function() {
     var ua = navigator.userAgent || '';
     // test windows first because it contains android
     if (/windows phone/i.test(ua)) {
       return 'windows';
     }
@@ -115,53 +165,95 @@
       return 'ios';
     }
     return 'unknown';
   })();
 
   var select = document.getElementById('package-select');
   var packages = document.querySelectorAll('.package');
+  var modal = document.getElementById('qr-modal');
+  var modalClose = document.getElementsByClassName('modal-close')[0];
+  var qrcode = new QRCode(document.getElementById('qrcode'), {
+    text: window.location.href,
+    width: 256,
+    height: 256,
+    colorDark : "#000000",
+    colorLight : "#ffffff",
+    correctLevel : QRCode.CorrectLevel.H,
+  });
 
-  // do not show the selector if there's only one package
-  if (packages.length > 1) {
-    select.classList.remove('hidden');
-  }
   select.addEventListener('change', function (e) {
     selectPackageById(e.target.value);
   });
 
+  modalClose.addEventListener('click', function () {
+    modal.style.display = 'none';
+  });
+
+  window.addEventListener('click', function (e) {
+    if (e.target == modal) {
+      modal.style.display = 'none';
+    }
+  });
+
+  window.addEventListener('keydown', function (e) {
+    if (modal.style.display === 'none') return;
+    if (e.key === 'Escape') {
+      modal.style.display = 'none';
+    }
+  });
+
   var defaultPackageId = null;
   for (var i = 0 ; i < packages.length ; ++i) {
     var pkg = packages[i];
     var isPackageInstallable = (
       (OS === 'android' && pkg.dataset.type === 'apk')
       || (OS === 'ios' && pkg.dataset.type === 'ipa')
     );
-    if (isPackageInstallable) {
-      if (defaultPackageId === null) {
+    if (!isPackageInstallable) {
+      var installBtn = pkg.querySelector('.install-btn');
+      installBtn.classList.add('disabled');
+    }
+    else if (defaultPackageId === null) {
+      defaultPackageId = pkg.id;
+    }
+
+    var qrBtn = pkg.querySelector('.show-qr-btn');
+    qrBtn.addEventListener('click', function () {
+      modal.style.display = 'block';
+      qrcode.makeCode(window.location.href);
+    });
+  }
+
+  // if a fragment is set then search for that item first
+  if (window.location.hash) {
+    for (var i = 0 ; i < packages.length ; ++i) {
+      var pkg = packages[i];
+      if (window.location.hash === '#' + pkg.id) {
         defaultPackageId = pkg.id;
       }
     }
-    else {
-      var btn = pkg.querySelector('.install-btn');
-      btn.classList.add('disabled');
-    }
+  }
+  // if we still don't have an initial package then use the first
+  if (!defaultPackageId) {
+    defaultPackageId = packages[0].id;
   }
 
-  if (defaultPackageId === null) defaultPackageId = packages[0].id;
+  // mark the default package as selected
   for (var i = 0 ; i < select.options.length ; ++i) {
     var opt = select.options[i];
     opt.selected = opt.value === defaultPackageId;
   }
   selectPackageById(defaultPackageId);
 
   function selectPackageById(id) {
     for (var i = 0 ; i < packages.length ; ++i) {
       var pkg = packages[i];
       if (pkg.id === id) {
         document.title = pkg.dataset.title;
+        window.location.hash = '#' + pkg.id;
         pkg.classList.remove('hidden');
       }
       else {
         pkg.classList.add('hidden');
       }
     }
   }
```

#### html2text {}

```diff
@@ -2,18 +2,17 @@
 {% for pkg in packages %}
 [{{ pkg.package_type }}] {{ pkg.display_name }} v{{ pkg.version_name }} ({
 { pkg.version_code }})
 {% endfor %}
  {% for pkg in packages %}
 ****** {{ pkg.display_name }} ******
 ***** {{ pkg.version_name }} ({{ pkg.version_code }}) *****
-{% if pkg.package_type == 'ipa' %} {% if pkg.image_url %} [{{ pkg.image_url |
-safe }}] {% endif %} Tap_to_install {% elif pkg.package_type == 'apk' %} {% if
-pkg.image_url %} [{{ pkg.image_url | safe }}] {% endif %} Tap_to_install {%
-else %} {{ die('Unsupported package type') }} {% endif %}
+{% if pkg.image_url %} [{{ pkg.image_url | safe }}] {% endif %} Install  Show
+QR  Download
 {% set os = 'Android' if pkg.package_type == 'apk' else 'WatchOS' if
 pkg.platform == 'watchos' else 'iOS' %} {% if pkg.minimum_os_version is defined
 %} This app requires {{ os }} {{ pkg.minimum_os_version }} or higher. {% else
 %} This app requires {{ os }}. {% endif %}
 {{ pkg.app_id }}
 {% endfor %}
+×
```

### Comparing `airsupply-0.3.2/airsupply/ipa.py` & `airsupply-0.4/airsupply/ipa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import attr
+import attrs
 from contextlib import contextmanager
+import io
 import plistlib
 import posixpath
+import pyipng
 import re
 import typing
 import zipfile
 
-@attr.s(auto_attribs=True)
+@attrs.define
 class Icon:
     size: int
     name: str
 
-@attr.s(auto_attribs=True)
+@attrs.define
 class IPA:
     filename: str
     zip: zipfile.ZipFile
     app_path: str
 
     id: str
     display_name: str
@@ -25,14 +27,18 @@
     minimum_os_version: str
     icons: typing.Dict[int, Icon]
     plist: typing.Dict[str, typing.Any]
 
     @contextmanager
     def open_asset(self, name):
         with self.zip.open(f'{self.app_path}/{name}') as fp:
+            # http://iphonedevwiki.net/index.php/CgBI_file_format
+            if name.endswith('.png'):
+                raw = pyipng.convert(fp.read())
+                fp = io.BytesIO(raw)
             yield fp
 
     def find_best_icon(self, target_size=1024):
         best_icon = best_dist = None
         for size, icon in self.icons.items():
             dist = abs(target_size - size)
             if best_dist is None or dist < best_dist:
```

### Comparing `airsupply-0.3.2/airsupply/ipa_manifest.jinja2` & `airsupply-0.4/airsupply/ipa_manifest.jinja2`

 * *Files identical despite different names*

### Comparing `airsupply-0.3.2/airsupply/local.py` & `airsupply-0.4/airsupply/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import attr
+import attrs
 import os
 from urllib.parse import urljoin
 
 log = __import__('logging').getLogger(__name__)
 
-@attr.s(auto_attribs=True)
+@attrs.define
 class LocalTarget:
     url: str
     root_dir: str
 
     def put_object(self, path, data, content_type):
-        url = urljoin(self.url, path)
+        local_path = os.path.join(self.root_dir, path)
+        local_dir = os.path.dirname(local_path)
 
-        path = os.path.join(self.root_dir, path)
-        root_dir = os.path.dirname(path)
-
-        os.makedirs(root_dir, exist_ok=True)
+        os.makedirs(local_dir, exist_ok=True)
 
         log.info(f'uploading object to {path}')
-        with open(path, 'wb') as fp:
+        with open(local_path, 'wb') as fp:
             if not isinstance(data, bytes):
                 data = data.read()
             fp.write(data)
 
-        return url
+        return self.get_url(path)
+
+    def get_url(self, path):
+        return urljoin(self.url, path)
 
     def get_object(self, path, *, raise_if_not_found=True):
         path = os.path.join(self.root_dir, path)
         try:
             with open(path, 'rb') as fp:
                 return fp.read()
         except FileNotFoundError:
```

### Comparing `airsupply-0.3.2/airsupply/push.py` & `airsupply-0.4/airsupply/push.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime
 import importlib.resources
 import json
 import mimetypes
 import os.path
+from urllib.parse import quote_plus
 
 from .apk import is_apk, open_apk
 from .ipa import is_ipa, open_ipa
 from .templates import render_template
 
 log = __import__('logging').getLogger(__name__)
 
@@ -68,20 +69,25 @@
         package_type='ipa',
         uploaded_at=datetime.now().isoformat(),
         app_id=ipa.id,
         display_name=ipa.display_name,
         version_name=ipa.short_version,
         version_code=ipa.version,
         minimum_os_version=ipa.minimum_os_version,
+        platform=ipa.platform,
         image_url=image_url,
         ipa_url=ipa_url,
         manifest_url=manifest_url,
-        platform=ipa.platform,
+        install_url=make_ipa_install_url(manifest_url),
+        download_url=ipa_url,
     )
 
+def make_ipa_install_url(manifest_url):
+    return f'itms-services://?action=download-manifest&url={quote_plus(manifest_url)}'
+
 def push_apk(apk, s3, prefix):
     location = f'{prefix}/apks/{os.path.basename(prefix)}.v{apk.version_code}'
     image_url = None
     icon = apk.get_app_icon(512)
     if icon and not icon.endswith('.xml'):
         image_data = apk.get_file(icon)
         image_ext = os.path.splitext(icon)[1]
@@ -97,47 +103,70 @@
         uploaded_at=datetime.now().isoformat(),
         app_id=apk.package,
         display_name=apk.application,
         version_name=apk.version_name,
         version_code=apk.version_code,
         image_url=image_url,
         apk_url=apk_url,
+        install_url=apk_url,
+        download_url=apk_url,
     )
 
 def update_index(target, packages, prefix, *, overwrite=False, readonly=False):
-    data = target.get_object(
-        f'{prefix}/index.json',
-        raise_if_not_found=False,
-    )
+    index_path = f'{prefix}/index.json'
+    index_url = target.get_url(index_path)
+    data = target.get_object(index_path, raise_if_not_found=False)
     if not data or overwrite:
         index = {
+            'index_url': index_url,
             'packages': [],
             'created_at': datetime.now().isoformat(),
         }
     else:
         index = json.loads(data.decode('utf8'))
 
+    # old index.json did not have index_url
+    if 'index_url' not in index:
+        index['index_url'] = index_url
+
     # de-duplicate packages by using the new copy of the same build
     prev_packages = index['packages']
     out_packages = list(packages)
     codes = {(p['app_id'], p['version_code']) for p in packages}
     for prev_pkg in prev_packages:
+        pkg_type = prev_pkg['package_type']
         if (prev_pkg['app_id'], prev_pkg['version_code']) in codes:
             log.debug(
                 f'overwriting index entry for '
                 f'package={prev_pkg["app_id"]} '
                 f'version={prev_pkg["version_code"]}'
             )
             continue
+        
+        # old index.json did not have install_url so let's add it
+        if 'install_url' not in prev_pkg:
+            if pkg_type == 'ipa':
+                prev_pkg['install_url'] = make_ipa_install_url(prev_pkg['manifest_url'])
+            elif pkg_type == 'apk':
+                prev_pkg['install_url'] = prev_pkg['apk_url']
+
+        # old index.json did not have download_url so let's add it
+        if 'download_url' not in prev_pkg:
+            if pkg_type == 'ipa':
+                prev_pkg['download_url'] = prev_pkg['ipa_url']
+            elif pkg_type == 'apk':
+                prev_pkg['download_url'] = prev_pkg['apk_url']
+
         out_packages.append(prev_pkg)
 
     out_packages.sort(key=lambda p: p['uploaded_at'], reverse=True)
     index['packages'] = out_packages
     index['updated_at'] = datetime.now().isoformat()
 
     if not readonly:
         target.put_object(
-            f'{prefix}/index.json',
+            index_path,
             json.dumps(index, indent=2).encode('utf8'),
             'application/json',
         )
+
     return index
```

### Comparing `airsupply-0.3.2/airsupply/s3.py` & `airsupply-0.4/airsupply/s3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import attr
+import attrs
 import boto3
 import typing
 
 log = __import__('logging').getLogger(__name__)
 
-@attr.s(auto_attribs=True)
+@attrs.define
 class S3Target:
     bucket: str
     acl: str
     public: bool
     expires: int
     client: typing.Any = None
 
@@ -21,27 +21,30 @@
         self.client.put_object(
             Bucket=self.bucket,
             Key=path,
             Body=data,
             ACL=self.acl,
             ContentType=content_type,
         )
+        url = self.get_url(path)
+        log.debug(f'object url={url}')
+        return url
 
+    def get_url(self, path):
         url = self.client.generate_presigned_url(
             'get_object',
             Params=dict(
                 Bucket=self.bucket,
                 Key=path,
             ),
             ExpiresIn=self.expires,
         )
         if self.public:
             i = url.index('?')
             url = url[:i]
-        log.debug(f'object url={url}')
         return url
 
     def get_object(self, path, *, raise_if_not_found=True):
         try:
             response = self.client.get_object(
                 Bucket=self.bucket,
                 Key=path,
```

### Comparing `airsupply-0.3.2/PKG-INFO` & `airsupply-0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: airsupply
-Version: 0.3.2
+Version: 0.4
 Summary: Manage OTA distribution for IPA and APK files.
 License: MIT
 Author: Michael Merickel
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20.2.0)
 Requires-Dist: boto3 (>=1.14.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: pyaxmlparser (>=0.3.24)
+Requires-Dist: pyipng (>=1.0.3,<2.0.0)
```

