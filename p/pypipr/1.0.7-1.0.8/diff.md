# Comparing `tmp/pypipr-1.0.7.tar.gz` & `tmp/pypipr-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.7.tar", max compression
+gzip compressed data, was "pypipr-1.0.8.tar", max compression
```

## Comparing `pypipr-1.0.7.tar` & `pypipr-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       18 2023-06-18 04:21:11.715384 pypipr-1.0.7/README.md
--rw-r--r--   0        0        0        0 2023-06-17 13:04:18.403397 pypipr-1.0.7/pypipr/__init__.py
--rw-r--r--   0        0        0     4510 2023-06-18 04:20:02.639384 pypipr-1.0.7/pypipr/console.py
--rw-r--r--   0        0        0      861 2023-06-18 03:56:02.427385 pypipr-1.0.7/pypipr/engineering.py
--rw-r--r--   0        0        0     1144 2023-06-18 04:28:45.283384 pypipr-1.0.7/pypipr/flow.py
--rw-r--r--   0        0        0      436 2023-06-18 04:18:24.039384 pypipr-1.0.7/pypipr/lib.py
--rw-r--r--   0        0        0      665 2023-06-18 02:32:08.963389 pypipr-1.0.7/pypipr/libstd.py
--rw-r--r--   0        0        0      348 2023-06-18 02:32:28.879389 pypipr-1.0.7/pypipr/libvendor.py
--rw-r--r--   0        0        0    42809 2023-06-18 03:39:21.579386 pypipr-1.0.7/pypipr/pypipr copy.py
--rw-r--r--   0        0        0      305 2023-06-18 04:29:44.763384 pypipr-1.0.7/pypipr/pypipr.py
--rw-r--r--   0        0        0    37454 2023-06-18 04:29:16.079384 pypipr-1.0.7/pypipr/uncategorize.py
--rw-r--r--   0        0        0      485 2023-06-18 04:30:05.739384 pypipr-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pypipr-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-06-18 04:21:11.715384 pypipr-1.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 13:04:18.403397 pypipr-1.0.8/pypipr/__init__.py
+-rw-r--r--   0        0        0     4037 2023-06-18 07:01:19.167393 pypipr-1.0.8/pypipr/console.py
+-rw-r--r--   0        0        0      854 2023-06-18 07:15:20.971392 pypipr-1.0.8/pypipr/engineering.py
+-rw-r--r--   0        0        0     1148 2023-06-18 07:16:20.467392 pypipr-1.0.8/pypipr/flow.py
+-rw-r--r--   0        0        0     9143 2023-06-18 07:12:55.259392 pypipr-1.0.8/pypipr/ifunctions.py
+-rw-r--r--   0        0        0      436 2023-06-18 04:18:24.039384 pypipr-1.0.8/pypipr/lib.py
+-rw-r--r--   0        0        0      665 2023-06-18 02:32:08.963389 pypipr-1.0.8/pypipr/libstd.py
+-rw-r--r--   0        0        0      348 2023-06-18 02:32:28.879389 pypipr-1.0.8/pypipr/libvendor.py
+-rw-r--r--   0        0        0    42809 2023-06-18 03:39:21.579386 pypipr-1.0.8/pypipr/pypipr copy.py
+-rw-r--r--   0        0        0      332 2023-06-18 06:35:45.735394 pypipr-1.0.8/pypipr/pypipr.py
+-rw-r--r--   0        0        0    25749 2023-06-18 07:13:14.523392 pypipr-1.0.8/pypipr/uncategorize.py
+-rw-r--r--   0        0        0      485 2023-06-18 07:17:19.443392 pypipr-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pypipr-1.0.8/PKG-INFO
```

### Comparing `pypipr-1.0.7/pypipr/console.py` & `pypipr-1.0.8/pypipr/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,31 +164,9 @@
                 print(r)
             else:
                 print(f"{i: >{m}} : {r}")
         except:
             pass
 
 
-def iexec(python_syntax, import_pypipr=True):
-    """
-    improve exec() python function untuk mendapatkan outputnya
-
-    ```python
-    print(iexec('print(9*9)'))
-    ```
-    """
-    if import_pypipr:
-        python_syntax = f"from pypipr.pypipr import *\n\n{python_syntax}"
-
-    stdout_backup = sys.stdout
-
-    sys.stdout = io.StringIO()
-    exec(python_syntax)
-    output = sys.stdout.getvalue()
-
-    sys.stdout = stdout_backup
-
-    return output
-
-
 if __name__ == "__main__":
     print_colorize("Anda menjalankan module pypipr", color=colorama.Fore.RED)
```

### Comparing `pypipr-1.0.7/pypipr/engineering.py` & `pypipr-1.0.8/pypipr/engineering.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     print(res)
     print(res.to_base_units())
     print(res.to_compact())
     print(f"{res:~P}")
     print(f"{res:~H}")
     ```
     """
-    return __calculate__quantity__(teks)
+    return PintUregQuantity(teks)
 
 
 if __name__ == "__main__":
     print_colorize("Anda menjalankan module pypipr", color=colorama.Fore.RED)
```

### Comparing `pypipr-1.0.7/pypipr/flow.py` & `pypipr-1.0.8/pypipr/flow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Modul berisi fungsi-fungsi umum
+Runtutan prosedur untuk third party
 '''
 
 
 from .lib import *
 from .console import *
```

### Comparing `pypipr-1.0.7/pypipr/libstd.py` & `pypipr-1.0.8/pypipr/libstd.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.7/pypipr/pypipr copy.py` & `pypipr-1.0.8/pypipr/pypipr copy.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.7/pypipr/uncategorize.py` & `pypipr-1.0.8/pypipr/uncategorize.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,220 +18,105 @@
 __batchmaker__regex_pattern__ = r"{(?:[^a-zA-Z0-9{}]+)?([a-zA-Z]|\d+)[^a-zA-Z0-9{}]+([a-zA-Z]|\d+)(?:[^a-zA-Z0-9{}]+(\d+))?(?:[^a-zA-Z0-9{}]+)?}"
 __batchmaker__regex_compile__ = re.compile(__batchmaker__regex_pattern__)
 # is_valid_url()
 __is_valid_url__pattern__ = "^(?:(?:(?:https?|ftp):)?\/\/)(?:\S+(?::\S*)?@)?(?:(?!(?:10|127)(?:\.\d{1,3}){3})(?!(?:169\.254|192\.168)(?:\.\d{1,3}){2})(?!172\.(?:1[6-9]|2\d|3[0-1])(?:\.\d{1,3}){2})(?:[1-9]\d?|1\d\d|2[01]\d|22[0-3])(?:\.(?:1?\d{1,2}|2[0-4]\d|25[0-5])){2}(?:\.(?:[1-9]\d?|1\d\d|2[0-4]\d|25[0-4]))|(?:(?:[a-z0-9\u00a1-\uffff][a-z0-9\u00a1-\uffff_-]{0,62})?[a-z0-9\u00a1-\uffff]\.)+(?:[a-z\u00a1-\uffff]{2,}\.?))(?::\d{2,5})?(?:[/?#]\S*)?$"
 __is_valid_url__regex__ = re.compile(__is_valid_url__pattern__, flags=re.IGNORECASE)
 
 
-class generator:
-    """
-    Class ini menyediakan beberapa fungsi yang bisa mengembalikan generator.
-    Digunakan untuk mengoptimalkan program.
-
-    Class ini dibuat karena python generator yang disimpan dalam variabel
-    hanya dapat diakses satu kali.
+def get_class_method(cls):
     """
+    Mengembalikan berupa tuple yg berisi list dari method dalam class
 
-    @staticmethod
-    def iscandir(
-        folder_name=".",
-        glob_pattern="*",
-        recursive=True,
-        scan_file=True,
-        scan_folder=True,
-    ):
-        """
-        Mempermudah scandir untuk mengumpulkan folder dan file.
-
-        ```python
-        print(generator.iscandir())
-        print(iscandir("./", recursive=False, scan_file=False))
-        ```
-        """
-        path_obj = pathlib.Path(folder_name)
-        if recursive:
-            path_obj = path_obj.rglob(glob_pattern)
-        else:
-            path_obj = path_obj.glob(glob_pattern)
-
-        for i in path_obj:
-            if scan_folder and i.is_dir():
-                yield i
-            if scan_file and i.is_file():
-                yield i
-
-    @staticmethod
-    def get_class_method(cls):
-        """
-        Mengembalikan berupa tuple yg berisi list dari method dalam class
-
-        ```python
-        class ExampleGetClassMethod:
-            def a():
-                return [x for x in range(10)]
-
-            def b():
-                return [x for x in range(10)]
-
-            def c():
-                return [x for x in range(10)]
+    ```python
+    class ExampleGetClassMethod:
+        def a():
+            return [x for x in range(10)]
 
-            def d():
-                return [x for x in range(10)]
+        def b():
+            return [x for x in range(10)]
 
-        print(get_class_method(ExampleGetClassMethod))
-        ```
-        """
-        for x in dir(cls):
-            a = getattr(cls, x)
-            if not x.startswith("__") and callable(a):
-                yield a
+        def c():
+            return [x for x in range(10)]
 
-    @staticmethod
-    def chunck_array(array, size, start=0):
-        """
-        Membagi array menjadi potongan-potongan dengan besaran yg diinginkan
+        def d():
+            return [x for x in range(10)]
 
-        ```python
-        array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]
-        print(generator.chunck_array(array, 5))
-        print(chunck_array(array, 5))
-        ```
-        """
-        for i in range(start, len(array), size):
-            yield array[i : i + size]
+    print(get_class_method(ExampleGetClassMethod))
+    ```
+    """
+    for x in dir(cls):
+        a = getattr(cls, x)
+        if not x.startswith("__") and callable(a):
+            yield a
 
-    @staticmethod
-    def irange(start, finish, step=1):
-        """
-        Meningkatkan fungsi range() dari python untuk pengulangan menggunakan huruf
+def chunck_array(array, size, start=0):
+    """
+    Membagi array menjadi potongan-potongan dengan besaran yg diinginkan
 
-        ```python
-        print(generator.irange('a', 'c'))
-        print(irange('z', 'a', 10))
-        print(irange('a', 'z', 10))
-        print(irange(1, '7'))
-        print(irange(10, 5))
-        ```
-        """
+    ```python
+    array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]
+    print(chunck_array(array, 5))
+    print(list(chunck_array(array, 5)))
+    ```
+    """
+    for i in range(start, len(array), size):
+        yield array[i : i + size]
 
-        def casting_class():
-            start_int = isinstance(start, int)
-            finish_int = isinstance(finish, int)
-            start_str = isinstance(start, str)
-            finish_str = isinstance(finish, str)
-            start_numeric = start.isnumeric() if start_str else False
-            finish_numeric = finish.isnumeric() if finish_str else False
-
-            if start_numeric and finish_numeric:
-                # irange("1", "5")
-                return (int, str)
-
-            if (start_numeric or start_int) and (finish_numeric or finish_int):
-                # irange("1", "5")
-                # irange("1", 5)
-                # irange(1, "5")
-                # irange(1, 5)
-                return (int, int)
-
-            if start_str and finish_str:
-                # irange("a", "z")
-                # irange("p", "g")
-                return (ord, chr)
-
-            """
-            kedua if dibawah ini sudah bisa berjalan secara logika, tetapi
-            perlu dimanipulasi supaya variabel start dan finish bisa diubah.
-            """
-            # irange(1, 'a') -> irange('1', 'a')
-            # irange(1, '5') -> irange(1, 5)
-            # irange('1', 5) -> irange(1, 5)
-            # irange('a', 5) -> irange('a', '5')
-            #
-            # if start_str and finish_int:
-            #     # irange("a", 5) -> irange("a", "5")
-            #     finish = str(finish)
-            #     return (ord, chr)
-            #
-            # if start_int and finish_str:
-            #     # irange(1, "g") -> irange("1", "g")
-            #     start = str(start)
-            #     return (ord, chr)
-
-            raise Exception(
-                f"[{start} - {finish}] tidak dapat diidentifikasi kesamaannya"
-            )
-
-        counter_class, converter_class = casting_class()
-        start = counter_class(start)
-        finish = counter_class(finish)
-
-        step = 1 if is_empty(step) else int(step)
-
-        faktor = 1 if finish > start else -1
-        step *= faktor
-        finish += faktor
 
-        for i in range(start, finish, step):
-            yield converter_class(i)
+def sets_ordered(iterator):
+    """
+    Hanya mengambil nilai unik dari suatu list
 
-    @staticmethod
-    def sets_ordered(iterator):
-        """
-        Hanya mengambil nilai unik dari suatu list
+    ```python
+    array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]
+    print(sets_ordered(array))
+    print(list(sets_ordered(array)))
+    ```
+    """
+    for i in dict.fromkeys(iterator):
+        yield i
 
-        ```python
-        array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]
-        print(generator.sets_ordered(array))
-        print(sets_ordered(array))
-        ```
-        """
-        for i in dict.fromkeys(iterator):
-            yield i
+def filter_empty(iterable, zero_is_empty=True, str_strip=True):
+    for i in iterable:
+        if i == 0 and zero_is_empty:
+            continue
+        if isinstance(i, str) and str_strip:
+            i = i.strip()
+        if not is_iterable(i) and not to_str(i):
+            continue
+        yield i
 
-    @staticmethod
-    def filter_empty(iterable, zero_is_empty=True, str_strip=True):
-        for i in iterable:
-            if i == 0 and zero_is_empty:
-                continue
-            if isinstance(i, str) and str_strip:
-                i = i.strip()
-            if not is_iterable(i) and not to_str(i):
-                continue
-            yield i
+def batchmaker(text: str):
+    """
+    Alat Bantu untuk membuat teks yang berulang.
+    Gunakan {[start][separator][finish]([separator][step])}.
+    ```
+    [start] dan [finish]    -> bisa berupa huruf maupun angka
+    ([separator][step])     -> bersifat optional
+    [separator]             -> selain huruf dan angka
+    [step]                  -> berupa angka positif
+    ```
 
-    @staticmethod
-    def batchmaker(text: str):
-        """
-        Alat Bantu untuk membuat teks yang berulang.
-        Gunakan {[start][separator][finish]([separator][step])}.
-        ```
-        [start] dan [finish]    -> bisa berupa huruf maupun angka
-        ([separator][step])     -> bersifat optional
-        [separator]             -> selain huruf dan angka
-        [step]                  -> berupa angka positif
-        ```
-
-        ```python
-        s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."
-        print(generator.batchmaker(s))
-        print(batchmaker(s))
-        ```
-        """
-        s = __batchmaker__regex_compile__.search(text)
-        if s is None:
-            yield text
-            return
+    ```python
+    s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."
+    print(batchmaker(s))
+    print(list(batchmaker(s)))
+    ```
+    """
+    s = __batchmaker__regex_compile__.search(text)
+    if s is None:
+        yield text
+        return
 
-        find = s.group()
-        start, finish, step = s.groups()
+    find = s.group()
+    start, finish, step = s.groups()
 
-        for i in generator.irange(start, finish, step):
-            r = text.replace(find, i, 1)
-            yield from generator.batchmaker(r)
+    for i in irange(start, finish, step):
+        r = text.replace(find, i, 1)
+        yield from batchmaker(r)
 
 
 
 def datetime_now(timezone=None):
     """
     Memudahkan dalam membuat Datetime untuk suatu timezone tertentu
 
@@ -255,54 +140,28 @@
     ```
     """
     return datetime.datetime.fromisoformat(iso_string).replace(
         tzinfo=zoneinfo.ZoneInfo(timezone)
     )
 
 
-def sets_ordered(iterable):
-    return type(iterable)(generator.sets_ordered(iterable))
-
-
-def chunck_array(array, size, start=0):
-    return tuple(generator.chunck_array(array=array, size=size, start=start))
-
-
 def create_folder(folder_name):
     """
     Membuat folder.
     Membuat folder secara recursive dengan permission.
 
     ```py
     create_folder("contoh_membuat_folder")
     create_folder("contoh/membuat/folder/recursive")
     create_folder("./contoh_membuat_folder/secara/recursive")
     ```
     """
     pathlib.Path(folder_name).mkdir(parents=True, exist_ok=True)
 
 
-def iscandir(
-    folder_name=".",
-    glob_pattern="*",
-    recursive=True,
-    scan_file=True,
-    scan_folder=True,
-):
-    return tuple(
-        generator.iscandir(
-            folder_name=folder_name,
-            glob_pattern=glob_pattern,
-            recursive=recursive,
-            scan_file=scan_file,
-            scan_folder=scan_folder,
-        )
-    )
-
-
 def get_filesize(filename):
     """
     Mengambil informasi file size dalam bytes
 
     ```python
     print(get_filesize(__file__))
     ```
@@ -370,18 +229,14 @@
     """
     t = threading.Timer(interval=interval, function=func, args=args, kwargs=kwargs)
     t.start()
     # t.cancel() untuk menghentikan timer sebelum waktu habis
     return t
 
 
-def get_class_method(cls):
-    return tuple(generator.get_class_method(cls))
-
-
 class ComparePerformance:
     """
     Menjalankan seluruh method dalam class,
     Kemudian membandingkan waktu yg diperlukan.
     Nilai 100 berarti yang tercepat.
 
     ```python
@@ -613,109 +468,14 @@
     """
     for i in args:
         if not is_empty(i):
             return
     sys.exit()
 
 
-def implode(
-    iterable,
-    separator="",
-    start="",
-    end="",
-    remove_empty=False,
-    recursive=True,
-    recursive_flat=False,
-    str_strip=False,
-):
-    """
-    Simplify Python join functions like PHP function.
-    Iterable bisa berupa sets, tuple, list, dictionary.
-
-    ```python
-    arr = {'asd','dfs','weq','qweqw'}
-    print(implode(arr, ', '))
-
-    arr = '/ini/path/seperti/url/'.split('/')
-    print(implode(arr, ','))
-    print(implode(arr, ',', remove_empty=True))
-
-    arr = {'a':'satu', 'b':(12, 34, 56), 'c':'tiga', 'd':'empat'}
-    print(implode(arr, separator='</li>\\n<li>', start='<li>', end='</li>', recursive_flat=True))
-    print(implode(arr, separator='</div>\\n<div>', start='<div>', end='</div>'))
-    print(implode(10, ' '))
-    ```
-    """
-    if not is_iterable(iterable):
-        iterable = [iterable]
-
-    separator = to_str(separator)
-
-    if isinstance(iterable, dict):
-        iterable = iterable.values()
-
-    if remove_empty:
-        iterable = (i for i in generator.filter_empty(iterable))
-
-    if recursive:
-        rec_flat = dict(start=start, end=end)
-        if recursive_flat:
-            rec_flat = dict(start="", end="")
-        rec = lambda x: implode(
-            iterable=x,
-            separator=separator,
-            **rec_flat,
-            remove_empty=remove_empty,
-            recursive=recursive,
-            recursive_flat=recursive_flat,
-        )
-        iterable = ((rec(i) if is_iterable(i) else i) for i in iterable)
-
-    iterable = (str(i) for i in iterable)
-
-    if str_strip:
-        iterable = (i.strip() for i in iterable)
-
-    result = start
-
-    for index, value in enumerate(iterable):
-        if index:
-            result += separator
-        result += value
-
-    result += end
-
-    return result
-
-
-def strtr(
-    string: str,
-    replacements: dict,
-    flags=re.DOTALL | re.MULTILINE | re.IGNORECASE,
-):
-    """
-    STRing TRanslate mengubah string menggunakan kamus dari dict.
-    Replacement dapat berupa text biasa ataupun regex pattern.
-    Apabila replacement berupa regex, gunakan raw string `r"..."`
-    Untuk regex capturing gunakan `(...)`, dan untuk mengaksesnya gunakan `\\1`, `\\2`, .., dst.
-
-    ```python
-    text = 'aku ini mau ke sini'
-    replacements = {
-        "sini": "situ",
-        r"(ini)": r"itu dan \\1",
-    }
-    print(strtr(text, replacements))
-    ```
-    """
-    for i, v in replacements.items():
-        string = re.sub(i, v, string, flags=flags)
-    return string
-
-
 def is_iterable(var, str_is_iterable=False):
     """
     Mengecek apakah suatu variabel bisa dilakukan forloop atau tidak
 
     ```python
     s = 'ini string'
     print(is_iterable(s))
@@ -749,31 +509,14 @@
     try:
         iter(var)
         return True
     except:
         return False
 
 
-def irange(start, finish, step=1):
-    """
-    Improve python range() function untuk pengulangan menggunakan huruf
-
-    ```python
-    print(generator.irange('a', 'z'))
-    print(irange('H', 'a'))
-    print(irange('1', '5', 3))
-    print(irange('1', 5, 3))
-    # print(irange('a', 5, 3))
-    print(irange(-10, 4, 3))
-    print(irange(1, 5))
-    ```
-    """
-    return list(generator.irange(start, finish, step))
-
-
 def serialize(data, syntax="yaml", indent=4):
     """
     Mengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.
     String yang dihasilkan berbentuk syntax YAML/JSON/HTML.
 
     ```python
     data = {
@@ -831,28 +574,14 @@
     ```python
     print(dirname("/ini/nama/folder/ke/file.py"))
     ```
     """
     return os.path.dirname(path)
 
 
-def batchmaker(text: str):
-    return tuple(generator.batchmaker(text))
-
-
-def filter_empty(iterable, zero_is_empty=True, str_strip=True):
-    return type(iterable)(
-        generator.filter_empty(
-            iterable=iterable,
-            zero_is_empty=zero_is_empty,
-            str_strip=str_strip,
-        )
-    )
-
-
 def to_str(value):
     """
     Mengubah value menjadi string literal
 
     ```python
     print(to_str(5))
     print(to_str([]))
@@ -893,154 +622,27 @@
     """
     for e in empty:
         if variable == e:
             return True
     return False
 
 
-def explode(text, separator="", include_separator=False):
-    """
-    Memecah text menjadi list berdasarkan separator.
-
-    ```python
-    t = '/ini/contoh/path/'
-    print(explode(t, separator='/'))
-    ```
-    """
-    if include_separator:
-        separator = f"({separator})"
-
-    result = re.split(separator, text, flags=re.IGNORECASE | re.MULTILINE)
-
-    return result
-
-
-def calculate(teks):
-    """
-    Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
-    Mendukung perhitungan matematika dasar dengan satuan.
-
-    Return value:
-    - Berupa class Quantity dari modul pint
-
-    Format:
-    - f"{result:~P}"            -> pretty
-    - f"{result:~H}"            -> html
-    - result.to_base_units()    -> SI
-    - result.to_compact()       -> human readable
-
-    ```python
-    fx = "3 meter * 10 cm * 3 km"
-    res = calculate(fx)
-    print(res)
-    print(res.to_base_units())
-    print(res.to_compact())
-    print(f"{res:~P}")
-    print(f"{res:~H}")
-    ```
-    """
-    return __calculate__quantity__(teks)
-
-
 def is_valid_url(path):
     """
     Mengecek apakah path merupakan URL yang valid atau tidak.
     Cara ini merupakan cara yang paling efektif.
 
     ```python
     print(is_valid_url("https://chat.openai.com/?model=text-davinci-002-render-sha"))
     print(is_valid_url("https://chat.openai.com/?model/=text-dav/inci-002-render-sha"))
     ```
     """
     return bool(__is_valid_url__regex__.fullmatch(path))
 
 
-def iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False):
-    """
-    Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.
-
-    Baca File :
-    - Membaca seluruh file.
-    - Jika berhasil content dapat diparse dengan regex.
-    - Apabila File berupa html, dapat diparse dengan css atau xpath.
-
-    Tulis File :
-    - Menulis pada file.
-    - Jika file tidak ada maka akan dibuat.
-    - Jika file memiliki content maka akan di overwrite.
-
-    Membaca URL :
-    - Mengakses URL dan mengembalikan isi html nya berupa teks.
-    - Content dapat diparse dengan regex, css atau xpath.
-
-    Tulis URL :
-    - Mengirimkan data dengan metode POST ke url.
-    - Jika berhasil dan response memiliki content, maka dapat diparse dengan regex, css atau xpath.
-
-
-    ```python
-    # FILE
-    print(iopen("__iopen.txt", "mana aja"))
-    print(iopen("__iopen.txt", regex="(\w+)"))
-    # URL
-    print(iopen("https://www.google.com/", css_select="a"))
-    print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))
-    ```
-    """
-    path = to_str(path)
-    content = ""
-
-    if is_valid_url(path):
-        req = dict(
-            url=path,
-            headers={
-                "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Mobile Safari/537.36"
-            },
-        )
-
-        if data:
-            req["data"] = urllib.parse.urlencode(data).encode()
-
-        req = urllib.request.Request(**req)
-
-        # Connect to URL
-        try:
-            with urllib.request.urlopen(req) as url_open:
-                content = url_open.read().decode()
-        except Exception as e:
-            # print(f"An error occurred: {str(e)}")
-            return False
-
-    else:
-        # Write File
-        if data is not None:
-            mode = "a" if file_append else "w"
-            with open(path, mode, encoding="utf-8") as f:
-                content = f.write(data)
-        # Read File
-        else:
-            try:
-                with open(path, "r") as f:
-                    content = f.read()
-            except Exception as e:
-                # print(f"An error occurred: {str(e)}")
-                return False
-
-    """ Parse """
-    if regex:
-        return re.findall(regex, content)
-    if css_select:
-        return lxml.html.fromstring(content).cssselect(css_select)
-    if xpath:
-        return lxml.html.fromstring(content).xpath(xpath)
-
-    """ Return """
-    return content
-
-
 def serialize_html(data, indent=None):
     """
     Serialisasi python variabel menjadi HTML.
     ```
     List -> <ul>...</ul>
     Dict -> <table>...</table>
     ```
@@ -1210,15 +812,15 @@
         return result
 
     def text_content(e):
         """
         mengambil semua text dalam element secara recursive.
         karena tidak ditemukan data dalam element.
         """
-        return implode(e.itertext(), str_strip=True)
+        return ijoin(e.itertext(), str_strip=True)
 
     element, childs = xpath(
         html,
         "//*[self::ul | self::ol | self::dl | self::table][not(ancestor::ul | ancestor::ol | ancestor::dl | ancestor::table)]",
     )
     if childs:
         return tuple((parse(data) for data in childs))
```

### Comparing `pypipr-1.0.7/PKG-INFO` & `pypipr-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 1.0.7
+Version: 1.0.8
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

