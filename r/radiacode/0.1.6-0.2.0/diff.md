# Comparing `tmp/radiacode-0.1.6.tar.gz` & `tmp/radiacode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiacode-0.1.6.tar", max compression
+gzip compressed data, was "radiacode-0.2.0.tar", max compression
```

## Comparing `radiacode-0.1.6.tar` & `radiacode-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1070 2021-11-21 12:23:13.303252 radiacode-0.1.6/LICENSE
--rw-r--r--   0        0        0     1520 2021-11-21 12:23:13.303252 radiacode-0.1.6/README.md
--rw-r--r--   0        0        0      957 2021-11-21 12:23:13.303252 radiacode-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      147 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode/__init__.py
--rw-r--r--   0        0        0      694 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode/bytes_buffer.py
--rw-r--r--   0        0        0        0 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode/decoders/__init__.py
--rw-r--r--   0        0        0     3709 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode/decoders/databuf.py
--rw-r--r--   0        0        0      426 2021-11-21 12:23:13.307252 radiacode-0.1.6/radiacode/decoders/spectrum.py
--rw-r--r--   0        0        0     6664 2021-11-21 12:23:13.307252 radiacode-0.1.6/radiacode/radiacode.py
--rw-r--r--   0        0        0        0 2021-11-21 12:23:13.307252 radiacode-0.1.6/radiacode/transports/__init__.py
--rw-r--r--   0        0        0     1720 2021-11-21 12:23:13.307252 radiacode-0.1.6/radiacode/transports/bluetooth.py
--rw-r--r--   0        0        0      711 2021-11-21 12:23:13.307252 radiacode-0.1.6/radiacode/transports/usb.py
--rw-r--r--   0        0        0     2144 2021-11-21 12:23:13.307252 radiacode-0.1.6/radiacode/types.py
--rw-r--r--   0        0        0     1040 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode-examples/README.md
--rw-r--r--   0        0        0     1215 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode-examples/README_ru.md
--rw-r--r--   0        0        0      933 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode-examples/basic.py
--rw-r--r--   0        0        0     2711 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode-examples/narodmon.py
--rw-r--r--   0        0        0     3971 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode-examples/webserver.html
--rw-r--r--   0        0        0     3414 2021-11-21 12:23:13.303252 radiacode-0.1.6/radiacode-examples/webserver.py
--rw-r--r--   0        0        0     2372 2021-11-21 12:23:57.752440 radiacode-0.1.6/setup.py
--rw-r--r--   0        0        0     2421 2021-11-21 12:23:57.752841 radiacode-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-18 13:36:03.683282 radiacode-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1520 2023-06-18 13:36:03.683282 radiacode-0.2.0/README.md
+-rw-r--r--   0        0        0      981 2023-06-18 13:36:03.683282 radiacode-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/bytes_buffer.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/decoders/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/decoders/databuf.py
+-rw-r--r--   0        0        0     1573 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/decoders/spectrum.py
+-rw-r--r--   0        0        0     7253 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/radiacode.py
+-rw-r--r--   0        0        0        0 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/transports/__init__.py
+-rw-r--r--   0        0        0     1720 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/transports/bluetooth.py
+-rw-r--r--   0        0        0      954 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/transports/usb.py
+-rw-r--r--   0        0        0     2310 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode/types.py
+-rw-r--r--   0        0        0     1296 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/README.md
+-rw-r--r--   0        0        0     1215 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/README_ru.md
+-rw-r--r--   0        0        0      933 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/basic.py
+-rw-r--r--   0        0        0     2711 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/narodmon.py
+-rw-r--r--   0        0        0     1820 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/radiacode-exporter.py
+-rw-r--r--   0        0        0     4276 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/webserver.html
+-rw-r--r--   0        0        0     3509 2023-06-18 13:36:03.683282 radiacode-0.2.0/radiacode-examples/webserver.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 radiacode-0.2.0/PKG-INFO
```

### Comparing `radiacode-0.1.6/LICENSE` & `radiacode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/README.md` & `radiacode-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/pyproject.toml` & `radiacode-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 [tool.poetry]
 name = "radiacode"
-version = "0.1.6"
+version = "0.2.0"
 description = "Library for RadiaCode-101"
 authors = ["Maxim Andreev <andreevmaxim@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cdump/radiacode"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
 ]
 include = ["radiacode-examples/*"]
 
 [tool.poetry.dependencies]
-python = "^3.6.2 || ^3.7"
-bluepy = "^1.3.0"
-pyusb = "^1.1.1"
-aiohttp = {version = "^3.7.4", optional = true}
+python = "^3.8.1"
+bluepy = "^1.3"
+pyusb = "^1.2"
+aiohttp = {version = "^3.8", optional = true}
+prometheus-client = {version = "^0.17", optional = true}
 
 [tool.poetry.dev-dependencies]
-wemake-python-styleguide = "^0.15.2"
-jedi = "^0.18.0"
-mypy = "^0.812"
-pytest = "^6.2.4"
-black = "^21.5b2"
+wemake-python-styleguide = "^0.18"
+mypy = "^1.3"
+black = "^23.3"
 
 [tool.poetry.extras]
-examples = ["aiohttp"]
+examples = ["aiohttp", "prometheus-client"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 130
-target-version = ["py36"]
+target-version = ["py310"]
 skip-string-normalization = true
 
 [tool.isort]
 line_length = 130
```

### Comparing `radiacode-0.1.6/radiacode/bytes_buffer.py` & `radiacode-0.2.0/radiacode/bytes_buffer.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/radiacode/decoders/databuf.py` & `radiacode-0.2.0/radiacode/decoders/databuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from typing import List, Union
 
 from radiacode.bytes_buffer import BytesBuffer
 from radiacode.types import CountRate, DoseRate, DoseRateDB, Event, RareData
 
 
 def decode_VS_DATA_BUF(
-    br: BytesBuffer, base_time: datetime.datetime
+    br: BytesBuffer,
+    base_time: datetime.datetime,
 ) -> List[Union[CountRate, DoseRate, DoseRateDB, RareData, Event]]:
     ret: List[Union[CountRate, DoseRate, DoseRateDB, RareData, Event]] = []
     next_seq = None
     while br.size() > 0:
         seq, eid, gid, ts_offset = br.unpack('<BBBi')
         dt = base_time + datetime.timedelta(milliseconds=ts_offset)
         if next_seq is not None and next_seq != seq:
```

### Comparing `radiacode-0.1.6/radiacode/radiacode.py` & `radiacode-0.2.0/radiacode/radiacode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import struct
-from typing import List, Union
+from typing import List, Optional, Union
 
 from radiacode.bytes_buffer import BytesBuffer
 from radiacode.decoders.databuf import decode_VS_DATA_BUF
 from radiacode.decoders.spectrum import decode_RC_VS_SPECTRUM
 from radiacode.transports.bluetooth import Bluetooth
 from radiacode.transports.usb import Usb
 from radiacode.types import CTRL, VS, VSFR, CountRate, DisplayDirection, DoseRate, DoseRateDB, Event, RareData, Spectrum
@@ -14,31 +14,37 @@
 def spectrum_channel_to_energy(channel_number: int, a0: float, a1: float, a2: float) -> float:
     return a0 + a1 * channel_number + a2 * channel_number * channel_number
 
 
 class RadiaCode:
     _connection: Union[Bluetooth, Usb]
 
-    def __init__(self, bluetooth_mac: str = None):
+    def __init__(self, bluetooth_mac: Optional[str] = None):
         self._seq = 0
         if bluetooth_mac is not None:
             self._connection = Bluetooth(bluetooth_mac)
         else:
             self._connection = Usb()
 
         # init
         self.execute(b'\x07\x00', b'\x01\xff\x12\xff')
         self._base_time = datetime.datetime.now()
         self.set_local_time(self._base_time)
         self.device_time(0)
 
+        self._spectrum_format_version = 0
+        for line in self.configuration().split('\n'):
+            if line.startswith('SpecFormatVersion'):
+                self._spectrum_format_version = int(line.split('=')[1])
+                break
+
     def base_time(self) -> datetime.datetime:
         return self._base_time
 
-    def execute(self, reqtype: bytes, args: bytes = None) -> BytesBuffer:
+    def execute(self, reqtype: bytes, args: Optional[bytes] = None) -> BytesBuffer:
         assert len(reqtype) == 2
         req_seq_no = 0x80 + self._seq
         self._seq = (self._seq + 1) % 32
 
         req_header = reqtype + b'\x00' + struct.pack('<B', req_seq_no)
         request = req_header + (args or b'')
         full_request = struct.pack('<I', len(request)) + request
@@ -60,23 +66,23 @@
         retcode = r.unpack('<I')[0]
         assert retcode == 1
         assert r.size() == 0
 
     def batch_read_vsfrs(self, vsfr_ids: List[VSFR]) -> List[int]:
         assert len(vsfr_ids)
         r = self.execute(b'\x2a\x08', b''.join(struct.pack('<I', int(c)) for c in vsfr_ids))
-        ret = [r.unpack('<I')[0] for _ in enumerate(vsfr_ids)]
+        ret = [r.unpack('<I')[0] for _ in range(len(vsfr_ids))]
         assert r.size() == 0
         return ret
 
     def status(self) -> str:
         r = self.execute(b'\x05\x00')
         flags = r.unpack('<I')
         assert r.size() == 0
-        return f'statuc flags: {flags}'
+        return f'status flags: {flags}'
 
     def set_local_time(self, dt: datetime.datetime) -> None:
         d = struct.pack('<BBBBBBBB', dt.day, dt.month, dt.year - 2000, 0, dt.second, dt.minute, dt.hour, 0)
         self.execute(b'\x04\x0a', d)
 
     def fw_signature(self) -> str:
         r = self.execute(b'\x01\x01')
@@ -102,14 +108,18 @@
         assert r.size() == 0
         return '-'.join(f'{v:08X}' for v in serial_groups)
 
     def configuration(self) -> str:
         r = self.read_request(VS.CONFIGURATION)
         return r.data().decode('cp1251')
 
+    def text_message(self) -> str:
+        r = self.read_request(VS.TEXT_MESSAGE)
+        return r.data().decode('ascii')
+
     def serial_number(self) -> str:
         r = self.read_request(8)
         return r.data().decode('ascii')
 
     def commands(self) -> str:
         br = self.read_request(257)
         return br.data().decode('ascii')
@@ -120,15 +130,19 @@
 
     def data_buf(self) -> List[Union[CountRate, DoseRate, DoseRateDB, RareData, Event]]:
         r = self.read_request(VS.DATA_BUF)
         return decode_VS_DATA_BUF(r, self._base_time)
 
     def spectrum(self) -> Spectrum:
         r = self.read_request(VS.SPECTRUM)
-        return decode_RC_VS_SPECTRUM(r)
+        return decode_RC_VS_SPECTRUM(r, self._spectrum_format_version)
+
+    def spectrum_accum(self) -> Spectrum:
+        r = self.read_request(VS.SPEC_ACCUM)
+        return decode_RC_VS_SPECTRUM(r, self._spectrum_format_version)
 
     # used in spectrum_channel_to_energy
     def energy_calib(self) -> List[float]:
         r = self.read_request(VS.ENERGY_CALIB)
         return list(r.unpack('<fff'))
 
     def set_language(self, lang='ru') -> None:
@@ -158,15 +172,15 @@
 
     def set_display_brightness(self, brightness: int) -> None:
         assert 0 <= brightness and brightness <= 9  # noqa: WPS309, WPS333
         self.write_request(VSFR.DISP_BRT, struct.pack('<I', brightness))
 
     def set_display_direction(self, direction: DisplayDirection) -> None:
         assert isinstance(direction, DisplayDirection)
-        self.write_request(VSFR.DISP_DR, struct.pack('<I', int(direction)))
+        self.write_request(VSFR.DISP_DIR, struct.pack('<I', int(direction)))
 
     def set_vibro_ctrl(self, ctrls: List[CTRL]) -> None:
         flags = 0
         for c in ctrls:
             assert c != CTRL.CLICKS, 'CTRL.CLICKS not supported for vibro'
             flags |= int(c)
         self.write_request(VSFR.VIBRO_CTRL, struct.pack('<I', flags))
```

### Comparing `radiacode-0.1.6/radiacode/transports/bluetooth.py` & `radiacode-0.2.0/radiacode/transports/bluetooth.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/radiacode/transports/usb.py` & `radiacode-0.2.0/radiacode/transports/usb.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 
 
 class DeviceNotFound(Exception):
     pass
 
 
 class Usb:
-    def __init__(self):
+    def __init__(self, timeout_ms=3000):
         self._device = usb.core.find(idVendor=0x483, idProduct=0xF123)
+        self._timeout_ms = timeout_ms
         if self._device is None:
             raise DeviceNotFound
+        while True:
+            try:
+                self._device.read(0x81, 256, timeout=100)
+            except usb.core.USBTimeoutError:
+                break
 
     def execute(self, request: bytes) -> BytesBuffer:
         self._device.write(0x1, request)
 
-        data = self._device.read(0x81, 256).tobytes()
+        data = self._device.read(0x81, 256, timeout=self._timeout_ms).tobytes()
         response_length = struct.unpack_from('<I', data)[0]
         data = data[4:]
 
         while len(data) < response_length:
             r = self._device.read(0x81, response_length - len(data)).tobytes()
             data += r
```

### Comparing `radiacode-0.1.6/radiacode/types.py` & `radiacode-0.2.0/radiacode/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     DEVICE_LANG = 1282
     DEVICE_TIME = 1284
     DISP_CTRL = 1296
     DISP_BRT = 1297
     DISP_CONTR = 1298
     DISP_OFF_TIME = 1299
     DISP_ON = 1300
-    DISP_DR = 1301
+    DISP_DIR = 1301
     SOUND_CTRL = 1312
     SOUND_VOL = 1313
     SOUND_ON = 1314
     SOUND_BUTTON = 1315
     PLAY_SIGNAL = 1505
     VIBRO_CTRL = 1328
     VIBRO_ON = 1329
@@ -95,20 +95,24 @@
     MS_MODE = 1537
     MS_SUB_MODE = 1538
     MS_RUN = 1539
 
     def __int__(self) -> int:
         return self.value
 
-
 class VS(Enum):
     CONFIGURATION = 2
+    TEXT_MESSAGE = 15
     DATA_BUF = 256
     SPECTRUM = 512
     ENERGY_CALIB = 514
+    SPEC_ACCUM = 517
+    SPEC_DIFF = 518  # TODO: what's that? Can be decoded by spectrum decoder
+    # UNKNOWN_13 = 13
+    # UNKNOWN_240 = 240
 
     def __int__(self) -> int:
         return self.value
 
 
 class CTRL(Enum):
     BUTTONS = 1 << 0
```

### Comparing `radiacode-0.1.6/radiacode-examples/README.md` & `radiacode-0.2.0/radiacode-examples/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,7 +18,14 @@
 ```
 
 ### 3. [narodmon.py](./narodmon.py)
 Sends measurements to the service [public monitoring project narodmon.ru](https://narodmon.ru).
 ```
 $ python3 -m radiacode-examples.narodmon --bluetooth-mac 52:43:01:02:03:04
 ```
+
+### 3. [radiacode-exporter.py](./radiacode-exporter.py)
+Exports metrics for [prometheus](https://prometheus.io/)
+```
+$ python3 -m radiacode-examples.radiacode-exporter --bluetooth-mac 52:43:01:02:03:04 --port 5432
+$ curl http://127.0.0.1:5432/metrics
+```
```

### Comparing `radiacode-0.1.6/radiacode-examples/README_ru.md` & `radiacode-0.2.0/radiacode-examples/README_ru.md`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/radiacode-examples/basic.py` & `radiacode-0.2.0/radiacode-examples/basic.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/radiacode-examples/narodmon.py` & `radiacode-0.2.0/radiacode-examples/narodmon.py`

 * *Files identical despite different names*

### Comparing `radiacode-0.1.6/radiacode-examples/webserver.html` & `radiacode-0.2.0/radiacode-examples/webserver.html`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,21 @@
 </style>
 <body>
 <div id="app">
   <div>
     <apexchart type="bar" height="350" :options="spectrumChartOptions" :series="spectrum_series"></apexchart>
     <div>
       <fieldset>
+        <input type="checkbox" id="spectrum_x_accum" v-model="spectrum_accum">
+        <label for="spectrum_x_accum">Accumulated</label>
+      </fieldset>
+      <fieldset>
         <input type="radio" id="spectrum_x_channel" v-bind:value="false" v-model="spectrum_energy">
         <label for="spectrum_x_channel">Channel</label>
+
         <input type="radio" id="spectrum_x_energy" v-bind:value="true" v-model="spectrum_energy">
         <label for="spectrum_x_energy">Energy</label>
       </fieldset>
       <fieldset>
         <input type="radio" id="spectrum_linear" v-bind:value="false" v-model="spectrum_logarithmic">
         <label for="spectrum_linear">Linear</label>
         <input type="radio" id="spectrum_log" v-bind:value="true" v-model="spectrum_logarithmic">
@@ -65,14 +70,15 @@
   },
   data: function() {
     return {
       ws: null,
       spectrum_duration: 0,
       rates_autoupdate: true,
       rates_series: [],
+      spectrum_accum: false,
       spectrum_series: [],
       spectrum_coef: [0, 0, 0],
       spectrum_logarithmic: true,
       spectrum_energy: true,
       ratesChartOptions: {
         ...common_options,
         title: {text: 'CountRate & DoseRate'},
@@ -80,14 +86,19 @@
         yaxis: [
           {seriesName: 'countrate', title: {text: 'CPS'}, labels: {formatter:(v) => v.toFixed(2) + ' CPS'}},
           {seriesName: 'doserate',  title: {text: 'μSv/h'}, labels: {formatter:(v) => v.toFixed(4) + ' μSv/h'}, opposite: true},
         ],
       },
     };
   },
+  watch: {
+    spectrum_accum() {
+      this.updateSpectrum();
+    }
+  },
   computed: {
     spectrumChartOptions() {
       const a0 = this.spectrum_coef[0], a1 = this.spectrum_coef[1], a2 = this.spectrum_coef[2];
       const fmt = this.spectrum_energy ? ((c) => (a0 + a1*c + a2*c*c).toFixed(0)) : undefined;
       const title = this.spectrum_energy ? 'keV' : 'channel';
       return{
         ...common_options,
@@ -111,15 +122,15 @@
       if (!this.rates_autoupdate) {
         return;
       }
       const d = JSON.parse(ev.data);
       this.rates_series = d.series;
     },
     updateSpectrum() {
-      fetch('/spectrum')
+      fetch(`/spectrum?accum=${this.spectrum_accum}`)
         .then(response => response.json())
         .then(data => (this.spectrum_duration=data.duration, this.spectrum_coef=data.coef, this.spectrum_series=data.series));
     },
   },
 });
 </script>
 </body>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 options="spectrumChartOptions" :series="spectrum_series">
- o Channel o Energy   o Linear o Logarithmic
+ ⁰ Accumulated   o Channel o Energy   o Linear o Logarithmic
 click="updateSpectrum">Update spectrum
 options="ratesChartOptions" :series="rates_series">
 click="rates_autoupdate = !rates_autoupdate">Rates autoupdate: {
 { rates_autoupdate ? "ON" : "OFF" }}
```

### Comparing `radiacode-0.1.6/radiacode-examples/webserver.py` & `radiacode-0.2.0/radiacode-examples/webserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     async for _ in ws:  # noqa: WPS328
         pass
     request.app.ws_clients.remove(ws)
     return ws
 
 
 async def handle_spectrum(request):
-    spectrum = request.app.rc_conn.spectrum()
+    cn = request.app.rc_conn
+    accum = request.query.get('accum') == 'true'
+    spectrum = cn.spectrum_accum() if accum else cn.spectrum()
     # apexcharts can't handle 0 in logarithmic view
     spectrum_data = [
         (channel, cnt if cnt > 0 else 0.5)
         for channel, cnt in enumerate(spectrum.counts)
     ]
     print('Spectrum updated')
     return web.json_response(
```

### Comparing `radiacode-0.1.6/PKG-INFO` & `radiacode-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: radiacode
-Version: 0.1.6
+Version: 0.2.0
 Summary: Library for RadiaCode-101
 Home-page: https://github.com/cdump/radiacode
 License: MIT
 Author: Maxim Andreev
 Author-email: andreevmaxim@gmail.com
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: examples
-Requires-Dist: aiohttp (>=3.7.4,<4.0.0); extra == "examples"
-Requires-Dist: bluepy (>=1.3.0,<2.0.0)
-Requires-Dist: pyusb (>=1.1.1,<2.0.0)
+Requires-Dist: aiohttp (>=3.8,<4.0) ; extra == "examples"
+Requires-Dist: bluepy (>=1.3,<2.0)
+Requires-Dist: prometheus-client (>=0.17,<0.18) ; extra == "examples"
+Requires-Dist: pyusb (>=1.2,<2.0)
 Project-URL: Repository, https://github.com/cdump/radiacode
 Description-Content-Type: text/markdown
 
 ## RadiaCode
 
 [Описание на русском языке](README_ru.md)
```

