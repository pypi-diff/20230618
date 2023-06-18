# Comparing `tmp/pypipr-1.0.5.tar.gz` & `tmp/pypipr-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.5.tar", max compression
+gzip compressed data, was "pypipr-1.0.6.tar", max compression
```

## Comparing `pypipr-1.0.5.tar` & `pypipr-1.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    33943 2023-06-17 12:42:40.571398 pypipr-1.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-16 19:13:28.991476 pypipr-1.0.5/pypipr/__init__.py
--rw-r--r--   0        0        0    43832 2023-06-16 20:16:42.367474 pypipr-1.0.5/pypipr/pypipr.py
--rw-r--r--   0        0        0      485 2023-06-17 12:42:44.951398 pypipr-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    34577 1970-01-01 00:00:00.000000 pypipr-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    33945 2023-06-17 12:44:16.519398 pypipr-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:28.991476 pypipr-1.0.6/pypipr/__init__.py
+-rw-r--r--   0        0        0    43832 2023-06-16 20:16:42.367474 pypipr-1.0.6/pypipr/pypipr.py
+-rw-r--r--   0        0        0      485 2023-06-17 12:44:21.495398 pypipr-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    34579 1970-01-01 00:00:00.000000 pypipr-1.0.6/PKG-INFO
```

### Comparing `pypipr-1.0.5/README.md` & `pypipr-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(generator.batchmaker(s))  
 print(batchmaker(s))  
 ```
 
 Output:
 ```py
-<generator object generator.batchmaker at 0x6f4e04bd00>
+<generator object generator.batchmaker at 0x6f9c4cfd00>
 ('Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.')
 ```
 
 ## calculate
 
 `calculate`
 
@@ -125,15 +125,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.chunck_array(array, 5))  
 print(chunck_array(array, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.chunck_array at 0x6f4e113e40>
+<generator object generator.chunck_array at 0x6f9c597e40>
 ([2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42])
 ```
 
 ## console_run
 
 `console_run`
 
@@ -184,17 +184,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2023-06-17 19:42:38.320047+07:00
-2023-06-17 12:42:38.321742+00:00
-2023-06-17 05:42:38.326459-07:00
+2023-06-17 19:44:14.760977+07:00
+2023-06-17 12:44:14.762637+00:00
+2023-06-17 05:44:14.766608-07:00
 ```
 
 ## dict_first
 
 `dict_first`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -285,15 +285,15 @@
         return [x for x in range(10)]  
 
 print(get_class_method(ExampleGetClassMethod))  
 ```
 
 Output:
 ```py
-(<function ExampleGetClassMethod.a at 0x6f4deca840>, <function ExampleGetClassMethod.b at 0x6f4deca7a0>, <function ExampleGetClassMethod.c at 0x6f4deca980>, <function ExampleGetClassMethod.d at 0x6f4decaa20>)
+(<function ExampleGetClassMethod.a at 0x6f9c336840>, <function ExampleGetClassMethod.b at 0x6f9c3367a0>, <function ExampleGetClassMethod.c at 0x6f9c336980>, <function ExampleGetClassMethod.d at 0x6f9c336a20>)
 ```
 
 ## get_filemtime
 
 `get_filemtime`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -377,15 +377,15 @@
 print(implode(arr, separator='</li>\n<li>', start='<li>', end='</li>', recursive_flat=True))  
 print(implode(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(implode(10, ' '))  
 ```
 
 Output:
 ```py
-weq, asd, qweqw, dfs
+qweqw, dfs, weq, asd
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -445,15 +445,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x6f4dfaaa80>, <Element a at 0x6f4dfab340>, <Element a at 0x6f4dd67110>, <Element a at 0x6f4dd671b0>, <Element a at 0x6f4dd67200>, <Element a at 0x6f4dd67250>, <Element a at 0x6f4dd672a0>, <Element a at 0x6f4dd672f0>, <Element a at 0x6f4dd67340>, <Element a at 0x6f4dd67390>, <Element a at 0x6f4dd673e0>, <Element a at 0x6f4dd67430>, <Element a at 0x6f4dd67480>, <Element a at 0x6f4dd674d0>, <Element a at 0x6f4dd67520>, <Element a at 0x6f4dd67570>, <Element a at 0x6f4dd675c0>, <Element a at 0x6f4dd67610>]
+[<Element a at 0x6f9c414ff0>, <Element a at 0x6f9c4154f0>, <Element a at 0x6f9c416fd0>, <Element a at 0x6f9c1971b0>, <Element a at 0x6f9c197250>, <Element a at 0x6f9c1972a0>, <Element a at 0x6f9c1972f0>, <Element a at 0x6f9c197340>, <Element a at 0x6f9c197390>, <Element a at 0x6f9c1973e0>, <Element a at 0x6f9c197430>, <Element a at 0x6f9c197480>, <Element a at 0x6f9c1974d0>, <Element a at 0x6f9c197520>, <Element a at 0x6f9c197570>, <Element a at 0x6f9c1975c0>, <Element a at 0x6f9c197610>, <Element a at 0x6f9c197660>]
 False
 ```
 
 ## irange
 
 `irange`
 
@@ -467,15 +467,15 @@
 # print(irange('a', 5, 3))  
 print(irange(-10, 4, 3))  
 print(irange(1, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.irange at 0x6f50d0cbf0>
+<generator object generator.irange at 0x6f9eb8cbf0>
 ['H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_', '`', 'a']
 ['1', '4']
 [1, 4]
 [-10, -7, -4, -1, 2]
 [1, 2, 3, 4, 5]
 ```
 
@@ -562,15 +562,15 @@
 ```python  
 print(generator.iscandir())  
 print(iscandir("./", recursive=False, scan_file=False))  
 ```
 
 Output:
 ```py
-<generator object generator.iscandir at 0x6f4e112040>
+<generator object generator.iscandir at 0x6f9c596040>
 (PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('dist'))
 ```
 
 ## log
 
 `log`
 
@@ -625,29 +625,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : 4220706935049599506
+            __hash__ : -6048772573965064464
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x6f4fa99cd0>
-               _hash : 4220706935049599506
+            _flavour : <pathlib._PosixFlavour object at 0x6f9df39c90>
+               _hash : -6048772573965064464
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -661,15 +661,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x6f4decf060>
+             iterdir : <generator object Path.iterdir at 0x6f9c33b060>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -891,15 +891,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 478028631296)>
+<Timer(Thread-2, started 479337626880)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered`
 
@@ -909,15 +909,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.sets_ordered(array))  
 print(sets_ordered(array))  
 ```
 
 Output:
 ```py
-<generator object generator.sets_ordered at 0x6f4df0e810>
+<generator object generator.sets_ordered at 0x6f9c37a810>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp`
 
@@ -1094,15 +1094,15 @@
    ':Rp. 945.000/gram (+3.000)',
    'Update harga LM Pegadaian :17 Juni 2023']],
  [['Spot Harga Emas Hari Ini (Market Close)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
   ['Ounce\xa0(oz)', '1.957,84 (+3,32)', '15.140,00', '29.641.698'],
   ['Gram\xa0(gr)', '62,95', '15.140,00', '953.003 (+1.616)'],
   ['Kilogram\xa0(kg)', '62.946,02', '15.140,00', '953.002.708'],
-  ['Update harga emas :17 Juni 2023, pukul 19:42Update kurs :13 Febuari 2023, '
+  ['Update harga emas :17 Juni 2023, pukul 19:44Update kurs :13 Febuari 2023, '
    'pukul 09:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100', '95.685.000', '956.850', '94.300.000', '943.000'],
   ['50', '47.895.000', '957.900', '47.150.000', '943.000'],
   ['25', '24.050.000', '962.000', '23.575.000', '943.000'],
@@ -1145,15 +1145,15 @@
   ['gr', '41,10', '+21,85+53,16%', '571.335', '+381.668+66,80%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
   ['USD', '62,95↑', '+0,11+0,18%'],
   ['KURS', '14.961,45↓', '-0,40-0,00%'],
   ['IDR', '941.763,70↑', '+1.571,86+0,17%'],
-  ['Sabtu, 17 Juni 2023 19:42']],
+  ['Sabtu, 17 Juni 2023 19:44']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
@@ -1208,23 +1208,23 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x6f4df0df20>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x6f9c379f20>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
-{'a': 158, 'b': 128, 'c': 100, 'd': 139}
-{'a': 160, 'b': 152, 'c': 100, 'd': 148}
-{'a': 137, 'b': 142, 'c': 100, 'd': 130}
-{'a': 113, 'b': 122, 'c': 100, 'd': 128}
-{'a': 133, 'b': 141, 'c': 100, 'd': 137}
+{'a': 149, 'b': 107, 'c': 100, 'd': 131}
+{'a': 149, 'b': 120, 'c': 100, 'd': 118}
+{'a': 128, 'b': 124, 'c': 100, 'd': 126}
+{'a': 129, 'b': 132, 'c': 100, 'd': 135}
+{'a': 131, 'b': 130, 'c': 100, 'd': 129}
 ```
 
 ## RunParallel
 
 `RunParallel`
 
 Menjalankan program secara bersamaan.
```

### Comparing `pypipr-1.0.5/pypipr/pypipr.py` & `pypipr-1.0.6/pypipr/pypipr.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.5/PKG-INFO` & `pypipr-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 1.0.5
+Version: 1.0.6
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -94,15 +94,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(generator.batchmaker(s))  
 print(batchmaker(s))  
 ```
 
 Output:
 ```py
-<generator object generator.batchmaker at 0x6f4e04bd00>
+<generator object generator.batchmaker at 0x6f9c4cfd00>
 ('Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.')
 ```
 
 ## calculate
 
 `calculate`
 
@@ -147,15 +147,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.chunck_array(array, 5))  
 print(chunck_array(array, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.chunck_array at 0x6f4e113e40>
+<generator object generator.chunck_array at 0x6f9c597e40>
 ([2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42])
 ```
 
 ## console_run
 
 `console_run`
 
@@ -206,17 +206,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2023-06-17 19:42:38.320047+07:00
-2023-06-17 12:42:38.321742+00:00
-2023-06-17 05:42:38.326459-07:00
+2023-06-17 19:44:14.760977+07:00
+2023-06-17 12:44:14.762637+00:00
+2023-06-17 05:44:14.766608-07:00
 ```
 
 ## dict_first
 
 `dict_first`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -307,15 +307,15 @@
         return [x for x in range(10)]  
 
 print(get_class_method(ExampleGetClassMethod))  
 ```
 
 Output:
 ```py
-(<function ExampleGetClassMethod.a at 0x6f4deca840>, <function ExampleGetClassMethod.b at 0x6f4deca7a0>, <function ExampleGetClassMethod.c at 0x6f4deca980>, <function ExampleGetClassMethod.d at 0x6f4decaa20>)
+(<function ExampleGetClassMethod.a at 0x6f9c336840>, <function ExampleGetClassMethod.b at 0x6f9c3367a0>, <function ExampleGetClassMethod.c at 0x6f9c336980>, <function ExampleGetClassMethod.d at 0x6f9c336a20>)
 ```
 
 ## get_filemtime
 
 `get_filemtime`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -399,15 +399,15 @@
 print(implode(arr, separator='</li>\n<li>', start='<li>', end='</li>', recursive_flat=True))  
 print(implode(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(implode(10, ' '))  
 ```
 
 Output:
 ```py
-weq, asd, qweqw, dfs
+qweqw, dfs, weq, asd
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -467,15 +467,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x6f4dfaaa80>, <Element a at 0x6f4dfab340>, <Element a at 0x6f4dd67110>, <Element a at 0x6f4dd671b0>, <Element a at 0x6f4dd67200>, <Element a at 0x6f4dd67250>, <Element a at 0x6f4dd672a0>, <Element a at 0x6f4dd672f0>, <Element a at 0x6f4dd67340>, <Element a at 0x6f4dd67390>, <Element a at 0x6f4dd673e0>, <Element a at 0x6f4dd67430>, <Element a at 0x6f4dd67480>, <Element a at 0x6f4dd674d0>, <Element a at 0x6f4dd67520>, <Element a at 0x6f4dd67570>, <Element a at 0x6f4dd675c0>, <Element a at 0x6f4dd67610>]
+[<Element a at 0x6f9c414ff0>, <Element a at 0x6f9c4154f0>, <Element a at 0x6f9c416fd0>, <Element a at 0x6f9c1971b0>, <Element a at 0x6f9c197250>, <Element a at 0x6f9c1972a0>, <Element a at 0x6f9c1972f0>, <Element a at 0x6f9c197340>, <Element a at 0x6f9c197390>, <Element a at 0x6f9c1973e0>, <Element a at 0x6f9c197430>, <Element a at 0x6f9c197480>, <Element a at 0x6f9c1974d0>, <Element a at 0x6f9c197520>, <Element a at 0x6f9c197570>, <Element a at 0x6f9c1975c0>, <Element a at 0x6f9c197610>, <Element a at 0x6f9c197660>]
 False
 ```
 
 ## irange
 
 `irange`
 
@@ -489,15 +489,15 @@
 # print(irange('a', 5, 3))  
 print(irange(-10, 4, 3))  
 print(irange(1, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.irange at 0x6f50d0cbf0>
+<generator object generator.irange at 0x6f9eb8cbf0>
 ['H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_', '`', 'a']
 ['1', '4']
 [1, 4]
 [-10, -7, -4, -1, 2]
 [1, 2, 3, 4, 5]
 ```
 
@@ -584,15 +584,15 @@
 ```python  
 print(generator.iscandir())  
 print(iscandir("./", recursive=False, scan_file=False))  
 ```
 
 Output:
 ```py
-<generator object generator.iscandir at 0x6f4e112040>
+<generator object generator.iscandir at 0x6f9c596040>
 (PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('dist'))
 ```
 
 ## log
 
 `log`
 
@@ -647,29 +647,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : 4220706935049599506
+            __hash__ : -6048772573965064464
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x6f4fa99cd0>
-               _hash : 4220706935049599506
+            _flavour : <pathlib._PosixFlavour object at 0x6f9df39c90>
+               _hash : -6048772573965064464
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -683,15 +683,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x6f4decf060>
+             iterdir : <generator object Path.iterdir at 0x6f9c33b060>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -913,15 +913,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 478028631296)>
+<Timer(Thread-2, started 479337626880)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered`
 
@@ -931,15 +931,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.sets_ordered(array))  
 print(sets_ordered(array))  
 ```
 
 Output:
 ```py
-<generator object generator.sets_ordered at 0x6f4df0e810>
+<generator object generator.sets_ordered at 0x6f9c37a810>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp`
 
@@ -1116,15 +1116,15 @@
    ':Rp. 945.000/gram (+3.000)',
    'Update harga LM Pegadaian :17 Juni 2023']],
  [['Spot Harga Emas Hari Ini (Market Close)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
   ['Ounce\xa0(oz)', '1.957,84 (+3,32)', '15.140,00', '29.641.698'],
   ['Gram\xa0(gr)', '62,95', '15.140,00', '953.003 (+1.616)'],
   ['Kilogram\xa0(kg)', '62.946,02', '15.140,00', '953.002.708'],
-  ['Update harga emas :17 Juni 2023, pukul 19:42Update kurs :13 Febuari 2023, '
+  ['Update harga emas :17 Juni 2023, pukul 19:44Update kurs :13 Febuari 2023, '
    'pukul 09:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100', '95.685.000', '956.850', '94.300.000', '943.000'],
   ['50', '47.895.000', '957.900', '47.150.000', '943.000'],
   ['25', '24.050.000', '962.000', '23.575.000', '943.000'],
@@ -1167,15 +1167,15 @@
   ['gr', '41,10', '+21,85+53,16%', '571.335', '+381.668+66,80%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
   ['USD', '62,95↑', '+0,11+0,18%'],
   ['KURS', '14.961,45↓', '-0,40-0,00%'],
   ['IDR', '941.763,70↑', '+1.571,86+0,17%'],
-  ['Sabtu, 17 Juni 2023 19:42']],
+  ['Sabtu, 17 Juni 2023 19:44']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
@@ -1230,23 +1230,23 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x6f4df0df20>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x6f9c379f20>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
-{'a': 158, 'b': 128, 'c': 100, 'd': 139}
-{'a': 160, 'b': 152, 'c': 100, 'd': 148}
-{'a': 137, 'b': 142, 'c': 100, 'd': 130}
-{'a': 113, 'b': 122, 'c': 100, 'd': 128}
-{'a': 133, 'b': 141, 'c': 100, 'd': 137}
+{'a': 149, 'b': 107, 'c': 100, 'd': 131}
+{'a': 149, 'b': 120, 'c': 100, 'd': 118}
+{'a': 128, 'b': 124, 'c': 100, 'd': 126}
+{'a': 129, 'b': 132, 'c': 100, 'd': 135}
+{'a': 131, 'b': 130, 'c': 100, 'd': 129}
 ```
 
 ## RunParallel
 
 `RunParallel`
 
 Menjalankan program secara bersamaan.
```

