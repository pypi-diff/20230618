# Comparing `tmp/wizwad-0.4.0.tar.gz` & `tmp/wizwad-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizwad-0.4.0.tar", max compression
+gzip compressed data, was "wizwad-0.4.1.tar", max compression
```

## Comparing `wizwad-0.4.0.tar` & `wizwad-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2022-09-29 14:39:25.807825 wizwad-0.4.0/LICENSE
--rw-r--r--   0        0        0      541 2022-10-10 12:56:02.868384 wizwad-0.4.0/README.md
--rw-r--r--   0        0        0      487 2022-10-11 06:27:21.175797 wizwad-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       34 2022-09-29 14:53:48.341745 wizwad-0.4.0/wizwad/__init__.py
--rw-r--r--   0        0        0     2477 2022-10-11 06:27:08.675612 wizwad-0.4.0/wizwad/__main__.py
--rw-r--r--   0        0        0    10614 2022-10-11 06:22:13.131245 wizwad-0.4.0/wizwad/wad.py
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 wizwad-0.4.0/setup.py
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 wizwad-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-18 13:14:03.090020 wizwad-0.4.1/LICENSE
+-rw-r--r--   0        0        0      541 2023-06-18 13:14:03.090020 wizwad-0.4.1/README.md
+-rw-r--r--   0        0        0      597 2023-06-18 13:20:20.568849 wizwad-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-06-18 13:22:31.768216 wizwad-0.4.1/wizwad/__init__.py
+-rw-r--r--   0        0        0     2669 2023-06-18 13:47:17.002183 wizwad-0.4.1/wizwad/__main__.py
+-rw-r--r--   0        0        0    11161 2023-06-18 13:47:17.423190 wizwad-0.4.1/wizwad/wad.py
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 wizwad-0.4.1/PKG-INFO
```

### Comparing `wizwad-0.4.0/LICENSE` & `wizwad-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wizwad-0.4.0/README.md` & `wizwad-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wizwad-0.4.0/wizwad/__main__.py` & `wizwad-0.4.1/wizwad/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 import sys
 from pathlib import Path
 
 import click
 
 from .wad import Wad
 
+logging.getLogger("wizwad").addHandler(logging.StreamHandler())
+
 
 def _get_recommended_workers() -> int:
     if sys.platform == "win32":
         return 60
 
     return 100
 
@@ -18,63 +21,91 @@
     """
     wizwad
     """
     pass
 
 
 @main.command()
-@click.argument("input_wad", type=click.Path(exists=True, dir_okay=False, path_type=Path))
-@click.argument("output_dir", type=click.Path(file_okay=False, path_type=Path), default=".")
+@click.argument(
+    "input_wad", type=click.Path(exists=True, dir_okay=False, path_type=Path)
+)
+@click.argument(
+    "output_dir", type=click.Path(file_okay=False, path_type=Path), default="."
+)
 def extract(input_wad: Path, output_dir: Path):
     """
     Extract the content of a wad to <output_dir> which defaults to the current directory
     """
     wad = Wad(input_wad)
     click.echo("Extracting")
     wad.extract_all(output_dir)
 
 
 @main.command()
 @click.argument("target_wad", type=click.Path(path_type=Path))
 @click.argument("content_to_add", type=click.Path(path_type=Path, exists=True))
-@click.option("--overwrite", is_flag=True, default=False, help="overwrite a wad if there already is one")
+@click.option(
+    "--overwrite",
+    is_flag=True,
+    default=False,
+    help="overwrite a wad if there already is one",
+)
 @click.option("--wad-version", type=int, default=1, help="the wad version to use")
-@click.option("--workers", type=int, default=10, help="the number of workers to use; 100 is recommend on linux")
-@click.option("--compression-level", type=int, default=9, help="zlib compression level of the data blob")
+@click.option(
+    "--workers",
+    type=int,
+    default=10,
+    help="the number of workers to use; 100 is recommend on linux",
+)
+@click.option(
+    "--compression-level",
+    type=int,
+    default=9,
+    help="zlib compression level of the data blob",
+)
 def pack(
-        target_wad: Path,
-        content_to_add: Path,
-        overwrite: bool,
-        wad_version: int,
-        workers: int,
-        compression_level: int,
+    target_wad: Path,
+    content_to_add: Path,
+    overwrite: bool,
+    wad_version: int,
+    workers: int,
+    compression_level: int,
 ):
     """
     Pack a directory into <target_wad>
     """
     if wad_version == 1 and target_wad.name == "Root.wad":
         click.echo("You may wish to use --wad-version 2 for Root.wad")
 
     recommended_workers = _get_recommended_workers()
     if workers < recommended_workers:
-        click.echo(f"Using less than {recommended_workers} workers may make packing slower")
+        click.echo(
+            f"Using less than {recommended_workers} workers may make packing slower"
+        )
 
     if workers <= 0:
         click.echo("workers must be greater than 0")
         exit(1)
 
     if not 1 <= compression_level <= 9:
         click.echo("compression level must be 1-9")
         exit(1)
 
-    Wad.from_full_add(content_to_add, target_wad, overwrite=overwrite, compression_level=compression_level)
+    Wad.from_full_add(
+        content_to_add,
+        target_wad,
+        overwrite=overwrite,
+        compression_level=compression_level,
+    )
 
 
 @main.command(name="list")
-@click.argument("wad_to_list", type=click.Path(path_type=Path, exists=True, dir_okay=False))
+@click.argument(
+    "wad_to_list", type=click.Path(path_type=Path, exists=True, dir_okay=False)
+)
 def _list(wad_to_list: Path):
     """
     List the files in <wad_to_list>
     """
     wad = Wad(wad_to_list)
     # TODO: raise an error if it isn't a valid wad file
     click.echo("\n".join(wad.name_list()))
```

### Comparing `wizwad-0.4.0/wizwad/wad.py` & `wizwad-0.4.1/wizwad/wad.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+import concurrent.futures
+import logging
 import os
 import struct
 import zlib
-import concurrent.futures
 from dataclasses import dataclass
-from pathlib import Path
-from typing import Optional, Union, List
-from mmap import mmap, ACCESS_READ
 from io import BytesIO
+from mmap import ACCESS_READ, mmap
+from pathlib import Path
+from typing import Iterator, List, Optional, Union
 
 import more_itertools
 
-
 _NO_COMPRESS = frozenset(
     (
         ".mp3",
         ".ogg",
     )
 )
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class WadFileInfo:
     name: str
     offset: int
     size: int
     zipped_size: int
@@ -31,21 +33,21 @@
 
 class Wad:
     # TODO: allow for `file` that doesnt exist yet
     def __init__(self, file: Union[Path, str]):
         self.file_path = Path(file)
         self.name = self.file_path.stem
 
-        self._file_map = {}
+        self._file_map: dict[str, WadFileInfo] = {}
         self._file_pointer = None
-        self._mmap = None
+        self._mmap: mmap | None = None
 
         self._refreshed_once = False
 
-        self._size = None
+        self._size: None | int = None
 
     def __repr__(self):
         return f"<Wad {self.name=}>"
 
     def __enter__(self):
         self._open()
         return self
@@ -89,56 +91,64 @@
             raise RuntimeError("This Wad is already open")
 
         # noinspection PyTypeChecker
         self._file_pointer = open(self.file_path, "rb")
         self._mmap = mmap(self._file_pointer.fileno(), 0, access=ACCESS_READ)
         self._refresh_journal()
 
-    def open(self, file_name: str) -> BytesIO:
+    def open(self, file_name: str) -> BytesIO | None:
         data = self.read(file_name)
+
+        if data is None:
+            return None
+
         return BytesIO(data)
 
     def close(self):
+        if self._file_pointer is None:
+            raise ValueError("Wad must be opened before closing")
+
         self._file_pointer.close()
         self._file_pointer = None
 
     # fmt: off
     def _read(self, start: int, size: int) -> bytes:
-        return self._mmap[start: start + size]
+        # Note, must be sure _open is always called before _read
+        return self._mmap[start: start + size]  # type: ignore
     # fmt: on
 
     # fmt: off
     def _refresh_journal(self):
         if self._refreshed_once:
             return
 
         self._refreshed_once = True
 
         # WAD id string
         file_offset = 5
 
         version, file_num = struct.unpack(
-            "<ll", self._mmap[file_offset: file_offset + 8]
+            "<ll", self._mmap[file_offset: file_offset + 8] # type: ignore
         )
 
         file_offset += 8
 
         if version >= 2:
             file_offset += 1
 
         for _ in range(file_num):
             # no reason to use struct.calcsize
             offset, size, zipped_size, is_zip, crc, name_length = struct.unpack(
-                "<lll?Ll", self._mmap[file_offset: file_offset + 21]
+                "<lll?Ll", self._mmap[file_offset: file_offset + 21] # type: ignore
             )
 
             # 21 is the size of all the data we just read
             file_offset += 21
 
-            name = self._mmap[file_offset: file_offset + name_length].decode()
+            name = self._mmap[file_offset: file_offset + name_length].decode() # type: ignore
             name = name.rstrip("\x00")
 
             file_offset += name_length
 
             self._file_map[name] = WadFileInfo(
                 name, offset, size, zipped_size, is_zip, crc
             )
@@ -211,39 +221,40 @@
         with open(self.file_path, "rb") as fp:
             with mmap(fp.fileno(), 0, access=ACCESS_READ) as mm:
                 for file in self._file_map.values():
                     file_path = path / file.name
                     file_path.parent.mkdir(parents=True, exist_ok=True)
 
                     if file.is_zip:
-                        data = mm[file.offset: file.offset + file.zipped_size]
+                        data = mm[file.offset : file.offset + file.zipped_size]
 
                     else:
-                        data = mm[file.offset: file.offset + file.size]
+                        data = mm[file.offset : file.offset + file.size]
 
                     # unpatched file
                     if data[:4] == b"\x00\x00\x00\x00":
+                        logger.warning(f'Touching unpatched file "{file.name}"')
                         file_path.touch()
                         continue
 
                     if file.is_zip:
                         data = zlib.decompress(data)
 
                     file_path.write_bytes(data)
 
     @classmethod
     def from_full_add(
-            cls,
-            source_path: Path | str,
-            new_wad_name: Path | str,
-            *,
-            overwrite: bool = False,
-            wad_version: int = 1,
-            workers: int = 10,
-            compression_level: int = 9,
+        cls,
+        source_path: Path | str,
+        new_wad_name: Path | str,
+        *,
+        overwrite: bool = False,
+        wad_version: int = 1,
+        workers: int = 10,
+        compression_level: int = 9,
     ):
         if isinstance(source_path, str):
             source_path = Path(source_path)
 
         if not source_path.is_dir():
             if not source_path.exists():
                 raise FileNotFoundError(source_path)
@@ -252,15 +263,17 @@
 
         if isinstance(new_wad_name, str):
             new_wad_name = Path(new_wad_name)
 
         if not overwrite and new_wad_name.exists():
             raise FileExistsError(f"{new_wad_name} already exists.")
 
-        cls._insert_all_fast(source_path, new_wad_name, wad_version, workers, compression_level)
+        cls._insert_all_fast(
+            source_path, new_wad_name, wad_version, workers, compression_level
+        )
         return cls(new_wad_name)
 
     @staticmethod
     def _insert_all_fast(
         source_path: Path,
         output_path: Path,
         wad_version: int = 1,
@@ -269,15 +282,15 @@
     ):
         to_write = []
         source_path_string = str(source_path)
         for root, _, files in os.walk(source_path):
             if root == source_path_string:
                 directory_prefix = ""
             else:
-                directory_prefix = root[len(str(source_path)) + 1:] + "/"
+                directory_prefix = root[len(str(source_path)) + 1 :] + "/"
 
             for file in files:
                 to_write.append(Path(directory_prefix + file))
 
         # file names must be sorted
         to_write = sorted(to_write, key=lambda p: p.as_posix())
 
@@ -292,15 +305,19 @@
         if wad_version == 1:
             journal_size -= 1
 
         with concurrent.futures.ProcessPoolExecutor(max_workers=workers) as executor:
             futures = []
 
             for chunk in more_itertools.divide(workers, to_write):
-                futures.append(executor.submit(_calculate_chunk, chunk, 0, source_path, compression_level))
+                futures.append(
+                    executor.submit(
+                        _calculate_chunk, chunk, 0, source_path, compression_level
+                    )
+                )
 
             with open(output_path, "wb+") as fp:
                 data_block = BytesIO()
 
                 chunk_offset = journal_size
 
                 # magic bytes
@@ -338,18 +355,18 @@
 
                 data_block.seek(0)
                 fp.write(data_block.getvalue())
 
 
 # has to be defined here
 def _calculate_chunk(
-        files: list[Path],
-        start: int,
-        source: Path,
-        compression_level: int = 9,
+    files: Iterator[Path],
+    start: int,
+    source: Path,
+    compression_level: int = 9,
 ) -> tuple[int, BytesIO, list[WadFileInfo]]:
     """
     returns end offset, data block, and journal entries
     """
     current_offset = start
     data_buffer = BytesIO()
     journal_entries = []
```

### Comparing `wizwad-0.4.0/PKG-INFO` & `wizwad-0.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: wizwad
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/StarrFox/wizwad
 License: MIT
 Author: StarrFox
 Author-email: starrfox6312@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: more-itertools (>=8.14.0,<9.0.0)
+Requires-Dist: more-itertools (>=8.14,<10.0)
 Project-URL: Repository, https://github.com/StarrFox/wizwad
 Description-Content-Type: text/markdown
 
 # wizwad
 A fast extractor and packer for wizard101/pirate101 wad files
 
 ## install
```

