# Comparing `tmp/hedgesql-1.0.tar.gz` & `tmp/hedgesql-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedgesql-1.0.tar", last modified: Sun Jun 18 17:47:55 2023, max compression
+gzip compressed data, was "hedgesql-1.1.tar", last modified: Sun Jun 18 18:39:40 2023, max compression
```

## Comparing `hedgesql-1.0.tar` & `hedgesql-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 17:47:55.077679 hedgesql-1.0/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.0/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      630 2023-06-18 17:47:55.077679 hedgesql-1.0/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1735 2023-06-14 17:26:48.000000 hedgesql-1.0/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 17:47:55.073679 hedgesql-1.0/hedgesql/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.0/hedgesql/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.0/hedgesql/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8985 2023-06-17 15:16:56.000000 hedgesql-1.0/hedgesql/hedge_sql.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 17:47:55.077679 hedgesql-1.0/hedgesql.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      630 2023-06-18 17:47:54.000000 hedgesql-1.0/hedgesql.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-18 17:47:54.000000 hedgesql-1.0/hedgesql.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-18 17:47:54.000000 hedgesql-1.0/hedgesql.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-18 17:47:54.000000 hedgesql-1.0/hedgesql.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-18 17:47:54.000000 hedgesql-1.0/hedgesql.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-18 17:47:55.077679 hedgesql-1.0/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      782 2023-06-18 17:45:33.000000 hedgesql-1.0/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 18:39:40.531112 hedgesql-1.1/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.1/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-18 18:39:40.531112 hedgesql-1.1/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1927 2023-06-18 18:28:20.000000 hedgesql-1.1/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 18:39:40.527111 hedgesql-1.1/hedgesql/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.1/hedgesql/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.1/hedgesql/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9001 2023-06-18 18:25:44.000000 hedgesql-1.1/hedgesql/hedge_sql.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-18 18:39:40.531112 hedgesql-1.1/hedgesql.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-18 18:39:40.000000 hedgesql-1.1/hedgesql.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-18 18:39:40.531112 hedgesql-1.1/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      759 2023-06-18 18:39:24.000000 hedgesql-1.1/setup.py
```

### Comparing `hedgesql-1.0/LICENSE` & `hedgesql-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hedgesql-1.0/PKG-INFO` & `hedgesql-1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.0
+Version: 1.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
-Author-email: frevod_dev@mail.ru
-License: GPLv3
+Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `hedgesql-1.0/README.md` & `hedgesql-1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-<h1 align="center">LiteSqlite
+<h1 align="center">HedgeSQL
 
 <h3 align="center">Теперь вам не нужно каждый раз устанавливать соединение, писать sql-запрос и закрывать соединение. Данная библиотека сделает это за вас
 
 Она поддерживает как синхронную, так и асинхронную работу
 
 </h3>
 
 Установка:
 ```python
-pip install litesqlite
+pip install hedgesql
 ```
 Теперь импортируем нужное:
 ```python
-from litesqlite import Sqlite, AioSqlite, DataTypes
+from hedgesql import Sqlite, AioSqlite, DataTypes
 ```
 Определяем экземпляр класса:
 ```python
 db = Sqlite(db_name='db.db')
 ```
 Открытие/закрытие соединения:
 ```python
 # Рекомендуется так:
 with db:
-    # пока код внутри блока, соединение открыто, затем оно закрывается
+# пока код внутри блока, соединение открыто, затем оно закрывается
 
 # но можно и вручную:
 db.open_conn()
 db.close_conn()
 ```
 Создание таблиц:
 ```python
@@ -35,17 +35,19 @@
 Добавление записей:
 ```python
 db.insert_data(table_name='users', data={'id': '123', 'name': 'Дмитрий'})
 ```
 Получение записей:
 ```python
 db.select_data(table_name='users', columns=['name'], where=[{'id': '123'}])
+# В columns по умолчанию: '*', то есть все столбцы
+# В where словари списка разделены "OR" (или), а данные словарей - "AND" (и)
 ```
 Обновление записей:
 ```python
-db.update_data(table_name='users', set_data={'name': 'Сергей'}, where={'id': '123'})
+db.update_data(table_name='users', set_data={'name': 'Сергей'}, where=[{'id': '123'}])
 ```
 Удаление записей:
 ```python
-db.delete_data(table_name='users', where={'id': '123'})
+db.delete_data(table_name='users', where=[{'id': '123'}])
 ```
 Ну а как сделать работу с бд асинхронной, думаю, знаете
```

### Comparing `hedgesql-1.0/hedgesql/datatypes.py` & `hedgesql-1.1/hedgesql/datatypes.py`

 * *Files identical despite different names*

### Comparing `hedgesql-1.0/hedgesql/hedge_sql.py` & `hedgesql-1.1/hedgesql/hedge_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                     order_by: Optional[str] = None,
                     limit: Optional[int] = None,
                     offset: Optional[int] = None,
                     fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         if columns != '*':
             columns = ', '.join(columns)
         if where:
-            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            where_clause = ' WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
         if order_by:
             order_by_clause = f"ORDER BY {order_by}"
         else:
@@ -76,33 +76,33 @@
         return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
                     where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
                     sign: Optional[str] = None) -> None:
+        values = tuple(set_data.values())
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
-            values = tuple(value for d in where for value in d.values())
+            values = (values + tuple(value for d in where for value in d.values()))
         else:
             where_clause = ''
-            values = tuple(set_data.values())
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
                     where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if where:
-            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
             values = tuple(where.values())
         else:
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
@@ -186,24 +186,24 @@
         return result
 
     async def update_data(self,
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
                           where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
                           sign: Optional[str] = None) -> None:
+        values = tuple(set_data.values())
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
-            values = tuple(value for d in where for value in d.values())
+            values = (values + tuple(value for d in where for value in d.values()))
         else:
             where_clause = ''
-            values = tuple(set_data.values())
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
                           where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
```

### Comparing `hedgesql-1.0/hedgesql.egg-info/PKG-INFO` & `hedgesql-1.1/hedgesql.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.0
+Version: 1.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
-Author-email: frevod_dev@mail.ru
-License: GPLv3
+Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `hedgesql-1.0/setup.py` & `hedgesql-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup
 
 setup(
     name='hedgesql',
-    version='1.0',
+    version='1.1',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/I-HedgeDev/litesqlite',
     author='HedgeDev',
-    author_email='frevod_dev@mail.ru',
-    license='GPLv3',
+    author_email='hedge_dev@mail.ru',
     packages=['hedgesql'],
     install_requires=[
         'aiosqlite'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

