# Comparing `tmp/mysql_to_sqlite3-2.0.0.tar.gz` & `tmp/mysql_to_sqlite3-2.0.1.tar.gz`

## Comparing `mysql_to_sqlite3-2.0.0.tar` & `mysql_to_sqlite3-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/requirements_dev.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/__init__.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/cli.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/click_utils.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/debug_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/py.typed
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/sqlite_utils.py
--rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/transporter.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/database.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/factories.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/func/__init__.py
--rw-r--r--   0        0        0    47466 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/func/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    24408 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/unit/mysql_to_sqlite3_test.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/LICENSE
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/README.md
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/requirements_dev.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/__init__.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/cli.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/click_utils.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/debug_info.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/py.typed
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/sqlite_utils.py
+-rw-r--r--   0        0        0    28099 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/transporter.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/database.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/factories.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/func/__init__.py
+-rw-r--r--   0        0        0    47466 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/func/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0    25443 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/tests/unit/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/README.md
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.1/PKG-INFO
```

### Comparing `mysql_to_sqlite3-2.0.0/CODE-OF-CONDUCT.md` & `mysql_to_sqlite3-2.0.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/cli.py` & `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/click_utils.py` & `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/click_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/debug_info.py` & `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/debug_info.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/sqlite_utils.py` & `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/transporter.py` & `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/transporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import mysql.connector
 import typing_extensions as tx
 from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
 from mysql.connector.types import ToPythonOutputTypes
 from tqdm import tqdm, trange
 
+from mysql_to_sqlite3.mysql_utils import CHARSET_INTRODUCERS
 from mysql_to_sqlite3.sqlite_utils import (
     CollatingSequences,
     adapt_decimal,
     adapt_timedelta,
     convert_date,
     convert_decimal,
     convert_timedelta,
@@ -245,47 +246,109 @@
             return "DATETIME"
         if data_type == "JSON" and sqlite_json1_extension_enabled:
             return "JSON"
         return "TEXT"
 
     @classmethod
     def _translate_default_from_mysql_to_sqlite(
-        cls, column_default: t.Optional[t.Any] = None, column_type: t.Optional[str] = None
+        cls,
+        column_default: ToPythonOutputTypes = None,
+        column_type: t.Optional[str] = None,
+        column_extra: ToPythonOutputTypes = None,
     ) -> str:
+        is_binary: bool
+        is_hex: bool
         if isinstance(column_default, bytes):
             if column_type in {
                 "BIT",
                 "BINARY",
                 "BLOB",
                 "LONGBLOB",
                 "MEDIUMBLOB",
                 "TINYBLOB",
                 "VARBINARY",
             }:
+                if column_extra in {"DEFAULT_GENERATED", "default_generated"}:
+                    for charset_introducer in CHARSET_INTRODUCERS:
+                        if column_default.startswith(charset_introducer.encode()):
+                            is_binary = False
+                            is_hex = False
+                            for b_prefix in ("B", "b"):
+                                if column_default.startswith(rf"{charset_introducer} {b_prefix}\'".encode()):
+                                    is_binary = True
+                                    break
+                            for x_prefix in ("X", "x"):
+                                if column_default.startswith(rf"{charset_introducer} {x_prefix}\'".encode()):
+                                    is_hex = True
+                                    break
+                            column_default = (
+                                column_default.replace(charset_introducer.encode(), b"")
+                                .replace(rb"x\'", b"")
+                                .replace(rb"X\'", b"")
+                                .replace(rb"b\'", b"")
+                                .replace(rb"B\'", b"")
+                                .replace(rb"\'", b"")
+                                .replace(rb"'", b"")
+                                .strip()
+                            )
+                            if is_binary:
+                                return f"DEFAULT '{chr(int(column_default, 2))}'"
+                            if is_hex:
+                                return f"DEFAULT x'{column_default.decode()}'"
+                            break
                 return f"DEFAULT x'{column_default.hex()}'"
             try:
                 column_default = column_default.decode()
             except (UnicodeDecodeError, AttributeError):
                 pass
         if column_default is None:
             return ""
         if isinstance(column_default, bool):
             if column_type == "BOOLEAN" and sqlite3.sqlite_version >= "3.23.0":
                 if column_default:
                     return "DEFAULT(TRUE)"
                 return "DEFAULT(FALSE)"
             return f"DEFAULT '{int(column_default)}'"
         if isinstance(column_default, str):
-            if column_default.upper() in {
-                "CURRENT_TIME",
-                "CURRENT_DATE",
-                "CURRENT_TIMESTAMP",
-            }:
-                return f"DEFAULT {column_default.upper()}"
-        return f"DEFAULT '{str(column_default)}'"
+            if column_extra in {"DEFAULT_GENERATED", "default_generated"}:
+                if column_default.upper() in {
+                    "CURRENT_TIME",
+                    "CURRENT_DATE",
+                    "CURRENT_TIMESTAMP",
+                }:
+                    return f"DEFAULT {column_default.upper()}"
+                for charset_introducer in CHARSET_INTRODUCERS:
+                    if column_default.startswith(charset_introducer):
+                        is_binary = False
+                        is_hex = False
+                        for b_prefix in ("B", "b"):
+                            if column_default.startswith(rf"{charset_introducer} {b_prefix}\'"):
+                                is_binary = True
+                                break
+                        for x_prefix in ("X", "x"):
+                            if column_default.startswith(rf"{charset_introducer} {x_prefix}\'"):
+                                is_hex = True
+                                break
+                        column_default = (
+                            column_default.replace(charset_introducer, "")
+                            .replace(r"x\'", "")
+                            .replace(r"X\'", "")
+                            .replace(r"b\'", "")
+                            .replace(r"B\'", "")
+                            .replace(r"\'", "")
+                            .replace(r"'", "")
+                            .strip()
+                        )
+                        if is_binary:
+                            return f"DEFAULT '{chr(int(column_default, 2))}'"
+                        if is_hex:
+                            return f"DEFAULT x'{column_default}'"
+                        return f"DEFAULT '{column_default}'"
+            return "DEFAULT '{}'".format(column_default.replace(r"\'", r"''"))
+        return "DEFAULT '{}'".format(str(column_default).replace(r"\'", r"''"))
 
     @classmethod
     def _data_type_collation_sequence(
         cls, collation: str = CollatingSequences.BINARY, column_type: t.Optional[str] = None
     ) -> str:
         if column_type and collation != CollatingSequences.BINARY:
             if column_type.startswith(
@@ -320,15 +383,15 @@
                     column_type=row["Type"],  # type: ignore[arg-type]
                     sqlite_json1_extension_enabled=self._sqlite_json1_extension_enabled,
                 )
                 sql += '\n\t"{name}" {type} {notnull} {default} {collation},'.format(
                     name=row["Field"].decode() if isinstance(row["Field"], bytes) else row["Field"],
                     type=column_type,
                     notnull="NULL" if row["Null"] == "YES" else "NOT NULL",
-                    default=self._translate_default_from_mysql_to_sqlite(row["Default"], column_type),
+                    default=self._translate_default_from_mysql_to_sqlite(row["Default"], column_type, row["Extra"]),
                     collation=self._data_type_collation_sequence(self._collation, column_type),
                 )
 
         self._mysql_cur_dict.execute(
             """
             SELECT INDEX_NAME AS `name`,
                   IF (NON_UNIQUE = 0 AND INDEX_NAME = 'PRIMARY', 1, 0) AS `primary`,
```

### Comparing `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/types.py` & `mysql_to_sqlite3-2.0.1/mysql_to_sqlite3/types.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/conftest.py` & `mysql_to_sqlite3-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/database.py` & `mysql_to_sqlite3-2.0.1/tests/database.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/factories.py` & `mysql_to_sqlite3-2.0.1/tests/factories.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/models.py` & `mysql_to_sqlite3-2.0.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/func/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.1/tests/func/mysql_to_sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/func/test_cli.py` & `mysql_to_sqlite3-2.0.1/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/tests/unit/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.1/tests/unit/mysql_to_sqlite3_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,46 +94,65 @@
                     assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == column_type.replace(
                         " UNSIGNED", ""
                     )
             else:
                 assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == column_type
 
     @pytest.mark.parametrize(
-        "column_default, sqlite_default_translation",
+        "column_default, column_extra, sqlite_default_translation",
         [
-            pytest.param(None, "", id="None"),
-            pytest.param("", "DEFAULT ''", id='""'),
-            pytest.param("lorem", "DEFAULT 'lorem'", id='"lorem"'),
+            pytest.param(None, None, "", id="None"),
+            pytest.param("", None, "DEFAULT ''", id='""'),
+            pytest.param("lorem", None, "DEFAULT 'lorem'", id='"lorem"'),
             pytest.param(
                 "lorem ipsum dolor",
+                None,
                 "DEFAULT 'lorem ipsum dolor'",
                 id='"lorem ipsum dolor"',
             ),
-            pytest.param("CURRENT_TIME", "DEFAULT CURRENT_TIME", id='"CURRENT_TIME"'),
-            pytest.param("current_time", "DEFAULT CURRENT_TIME", id='"current_time"'),
-            pytest.param("CURRENT_DATE", "DEFAULT CURRENT_DATE", id='"CURRENT_DATE"'),
-            pytest.param("current_date", "DEFAULT CURRENT_DATE", id='"current_date"'),
+            pytest.param("CURRENT_TIME", "DEFAULT_GENERATED", "DEFAULT CURRENT_TIME", id='"CURRENT_TIME"'),
+            pytest.param("current_time", "DEFAULT_GENERATED", "DEFAULT CURRENT_TIME", id='"current_time"'),
+            pytest.param("CURRENT_DATE", "DEFAULT_GENERATED", "DEFAULT CURRENT_DATE", id='"CURRENT_DATE"'),
+            pytest.param("current_date", "DEFAULT_GENERATED", "DEFAULT CURRENT_DATE", id='"current_date"'),
             pytest.param(
                 "CURRENT_TIMESTAMP",
+                "DEFAULT_GENERATED",
                 "DEFAULT CURRENT_TIMESTAMP",
                 id='"CURRENT_TIMESTAMP"',
             ),
             pytest.param(
                 "current_timestamp",
+                "DEFAULT_GENERATED",
                 "DEFAULT CURRENT_TIMESTAMP",
                 id='"current_timestamp"',
             ),
+            pytest.param(r"""_utf8mb4\'[]\'""", "DEFAULT_GENERATED", "DEFAULT '[]'", id=r"""_utf8mb4\'[]\'"""),
+            pytest.param(r"""_latin1\'abc\'""", "DEFAULT_GENERATED", "DEFAULT 'abc'", id=r"""_latin1\'abc\'"""),
+            pytest.param(r"""_binary\'abc\'""", "DEFAULT_GENERATED", "DEFAULT 'abc'", id=r"""_binary\'abc\'"""),
+            pytest.param(
+                r"""_latin1 X\'4D7953514C\'""",
+                "DEFAULT_GENERATED",
+                "DEFAULT x'4D7953514C'",
+                id=r"""_latin1 X\'4D7953514C\'""",
+            ),
+            pytest.param(
+                r"""_latin1 b\'1000001\'""", "DEFAULT_GENERATED", "DEFAULT 'A'", id=r"""_latin1 b\'1000001\'"""
+            ),
         ],
     )
     def test_translate_default_from_mysql_to_sqlite(
         self,
-        column_default: str,
+        column_default: t.Optional[str],
+        column_extra: t.Optional[str],
         sqlite_default_translation: str,
     ) -> None:
-        assert MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default) == sqlite_default_translation
+        assert (
+            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default, column_extra=column_extra)
+            == sqlite_default_translation
+        )
 
     @pytest.mark.parametrize(
         "column_default, sqlite_default_translation, sqlite_version",
         [
             pytest.param(False, "DEFAULT(FALSE)", "3.23.0", id="False (NEW)"),
             pytest.param(True, "DEFAULT(TRUE)", "3.23.0", id="True (NEW)"),
             pytest.param(False, "DEFAULT '0'", "3.22.0", id="False (OLD)"),
```

### Comparing `mysql_to_sqlite3-2.0.0/.gitignore` & `mysql_to_sqlite3-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/LICENSE` & `mysql_to_sqlite3-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/README.md` & `mysql_to_sqlite3-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/pyproject.toml` & `mysql_to_sqlite3-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mysql_to_sqlite3-2.0.0/PKG-INFO` & `mysql_to_sqlite3-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
```

