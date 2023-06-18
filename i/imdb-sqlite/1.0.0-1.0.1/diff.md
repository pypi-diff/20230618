# Comparing `tmp/imdb-sqlite-1.0.0.tar.gz` & `tmp/imdb-sqlite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imdb-sqlite-1.0.0.tar", last modified: Sun Jan 15 17:40:55 2023, max compression
+gzip compressed data, was "imdb-sqlite-1.0.1.tar", last modified: Sun Jun 18 20:50:45 2023, max compression
```

## Comparing `imdb-sqlite-1.0.0.tar` & `imdb-sqlite-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:55.620113 imdb-sqlite-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-01-15 17:40:41.000000 imdb-sqlite-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-01-15 17:40:55.620113 imdb-sqlite-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-01-15 17:40:41.000000 imdb-sqlite-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:55.616113 imdb-sqlite-1.0.0/imdb_sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:41.000000 imdb-sqlite-1.0.0/imdb_sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-01-15 17:40:41.000000 imdb-sqlite-1.0.0/imdb_sqlite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:55.620113 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-01-15 17:40:55.000000 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-15 17:40:55.000000 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 17:40:55.000000 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-15 17:40:55.000000 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-15 17:40:55.000000 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-15 17:40:55.000000 imdb-sqlite-1.0.0/imdb_sqlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 17:40:55.620113 imdb-sqlite-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-15 17:40:41.000000 imdb-sqlite-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:50:45.957408 imdb-sqlite-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-18 20:50:31.000000 imdb-sqlite-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-18 20:50:45.957408 imdb-sqlite-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-18 20:50:31.000000 imdb-sqlite-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:50:45.957408 imdb-sqlite-1.0.1/imdb_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 20:50:31.000000 imdb-sqlite-1.0.1/imdb_sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-06-18 20:50:31.000000 imdb-sqlite-1.0.1/imdb_sqlite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:50:45.957408 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-18 20:50:45.000000 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 20:50:45.000000 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:50:45.000000 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 20:50:45.000000 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 20:50:45.000000 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 20:50:45.000000 imdb-sqlite-1.0.1/imdb_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:50:45.957408 imdb-sqlite-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-18 20:50:31.000000 imdb-sqlite-1.0.1/setup.py
```

### Comparing `imdb-sqlite-1.0.0/LICENSE` & `imdb-sqlite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imdb-sqlite-1.0.0/PKG-INFO` & `imdb-sqlite-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: imdb-sqlite
-Version: 1.0.0
-Summary: Imports IMDB TSV files into a SQLite database
-Home-page: https://github.com/jojje/imdb-sqlite
-Author: Jonas Tingeborn
-Author-email: tinjon+pip@gmail.com
-License: GNU GPL v2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # imdb-sqlite
 Imports IMDB TSV files into a SQLite database.
 
 It will fetch the [files][1] from IMDB unless you've already fetched them earlier.
 
 The program relies on the following IMDB tab separated files:
 
@@ -169,50 +154,23 @@
 production. The current set of crew categories are:
 ```
 { actor, actress, archive_footage, archive_sound, cinematographer, composer,
   director, editor, producer, production_designer, self, writer }
 ```
 
 ### Performance tips
-Many relations over a ten gigabyte database is where a relational
-DB really starts showing its limits. The above query takes quite a while to run.
-Optimally a graph DB would be used instead, since the query is more of that
-nature. Some things can still be done to get an _OK_ response time. If you use
-IDs instead of names, some joins can be eliminated. For example by using the
-IMDB IDs for Pacino and De Niro instead of searching for them by name, the above
-query is sped up by an order of magnitude or so, by eliminating the index search
-through two people tables.
-
-```sql
-SELECT t.title_id, t.type, t.primary_title, t.premiered, t.genres,
-       c1.characters AS 'Pacino played', c2.characters AS 'Deniro played'
-FROM crew c1
-INNER JOIN crew c2 ON ( c1.title_id = c2.title_id  )
-INNER JOIN titles t ON ( c2.title_id = t.title_id  )
-WHERE c1.person_id = 'nm0000199' -- Pacino
-AND   c2.person_id = 'nm0000134' -- De Niro
-AND   c1.category = 'actor' AND c2.category = 'actor'
-```
-
-Another thing to try is to further normalize the data. There is quite some
-duplication in the data, such at title types, crew categories etc. That
-duplication prevents the DB from efficiently joining tables. Even though a lot
-of indices are used, any collection of duplicates in a column forces the engine
-to essentially do brute force scans through all those duplicates. It's not much
-else it can do, and this takes time. Normalizing away such duplicates _will_
-mean more joins are required, but it should hopefully allow the engine to more
-quickly whittle down the dataset. I've not tried this, but it seems something
-plausible to invetigate if your queries are too slow for your taste.
-
-Finally, when in doubt. Prefix your query with the `EXPLAIN QUERY PLAN`. If you
-see `SCAN TABLE` in there, particularly in the beginning, it means the DB is
-doing a brute-force search through all the data in the column. This is _very_
-slow. You want the query plan to say `SEARCH` everywhere. Create an index for
-the column indicated as being scanned and rerun the query plan. Hopefully that
-resulted in orders of magnitude query speed improvement.
+Prefix your query with the `EXPLAIN QUERY PLAN`. If you see `SCAN TABLE` in
+there, particularly in the beginning, it means the DB is doing a brute-force
+search through all the data in the column. This is _very_ slow. You want the
+query plan to say `SEARCH` everywhere. If the query shows autoindex rather than
+using an explicit index, then that may also be the cause for slow joins. The
+tables are very large, which can result in a lot of I/O without explicit
+indices. To resolve, create an index for the column indicated as being scanned
+or using autoindex and rerun the query plan. Hopefully that results in a
+massive query speedup.
 
 For example `sqlite3 imdb.db "CREATE INDEX myindex ON <table-name> (<slow-column>)"`
 
 ## PyPI
 Current status of the project is:
 [![Build Status](https://github.com/jojje/imdb-sqlite/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jojje/imdb-sqlite/actions/workflows/python-publish.yml)
 
@@ -222,8 +180,8 @@
 the github source, upon any version tagged commit to the master branch.
 
 Click the status link and check out the logs if you're interested in the
 package lineage; meaning how the released pypi module was constructed from
 source.
 
 [1]: https://www.imdb.com/interfaces/
-[2]: https://pypi.org/project/imdb-sqlite/
+[2]: https://pypi.org/project/imdb-sqlite/
```

### Comparing `imdb-sqlite-1.0.0/README.md` & `imdb-sqlite-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: imdb-sqlite
+Version: 1.0.1
+Summary: Imports IMDB TSV files into a SQLite database
+Home-page: https://github.com/jojje/imdb-sqlite
+Author: Jonas Tingeborn
+Author-email: tinjon+pip@gmail.com
+License: GNU GPL v2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # imdb-sqlite
 Imports IMDB TSV files into a SQLite database.
 
 It will fetch the [files][1] from IMDB unless you've already fetched them earlier.
 
 The program relies on the following IMDB tab separated files:
 
@@ -154,50 +169,23 @@
 production. The current set of crew categories are:
 ```
 { actor, actress, archive_footage, archive_sound, cinematographer, composer,
   director, editor, producer, production_designer, self, writer }
 ```
 
 ### Performance tips
-Many relations over a ten gigabyte database is where a relational
-DB really starts showing its limits. The above query takes quite a while to run.
-Optimally a graph DB would be used instead, since the query is more of that
-nature. Some things can still be done to get an _OK_ response time. If you use
-IDs instead of names, some joins can be eliminated. For example by using the
-IMDB IDs for Pacino and De Niro instead of searching for them by name, the above
-query is sped up by an order of magnitude or so, by eliminating the index search
-through two people tables.
-
-```sql
-SELECT t.title_id, t.type, t.primary_title, t.premiered, t.genres,
-       c1.characters AS 'Pacino played', c2.characters AS 'Deniro played'
-FROM crew c1
-INNER JOIN crew c2 ON ( c1.title_id = c2.title_id  )
-INNER JOIN titles t ON ( c2.title_id = t.title_id  )
-WHERE c1.person_id = 'nm0000199' -- Pacino
-AND   c2.person_id = 'nm0000134' -- De Niro
-AND   c1.category = 'actor' AND c2.category = 'actor'
-```
-
-Another thing to try is to further normalize the data. There is quite some
-duplication in the data, such at title types, crew categories etc. That
-duplication prevents the DB from efficiently joining tables. Even though a lot
-of indices are used, any collection of duplicates in a column forces the engine
-to essentially do brute force scans through all those duplicates. It's not much
-else it can do, and this takes time. Normalizing away such duplicates _will_
-mean more joins are required, but it should hopefully allow the engine to more
-quickly whittle down the dataset. I've not tried this, but it seems something
-plausible to invetigate if your queries are too slow for your taste.
-
-Finally, when in doubt. Prefix your query with the `EXPLAIN QUERY PLAN`. If you
-see `SCAN TABLE` in there, particularly in the beginning, it means the DB is
-doing a brute-force search through all the data in the column. This is _very_
-slow. You want the query plan to say `SEARCH` everywhere. Create an index for
-the column indicated as being scanned and rerun the query plan. Hopefully that
-resulted in orders of magnitude query speed improvement.
+Prefix your query with the `EXPLAIN QUERY PLAN`. If you see `SCAN TABLE` in
+there, particularly in the beginning, it means the DB is doing a brute-force
+search through all the data in the column. This is _very_ slow. You want the
+query plan to say `SEARCH` everywhere. If the query shows autoindex rather than
+using an explicit index, then that may also be the cause for slow joins. The
+tables are very large, which can result in a lot of I/O without explicit
+indices. To resolve, create an index for the column indicated as being scanned
+or using autoindex and rerun the query plan. Hopefully that results in a
+massive query speedup.
 
 For example `sqlite3 imdb.db "CREATE INDEX myindex ON <table-name> (<slow-column>)"`
 
 ## PyPI
 Current status of the project is:
 [![Build Status](https://github.com/jojje/imdb-sqlite/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jojje/imdb-sqlite/actions/workflows/python-publish.yml)
 
@@ -207,8 +195,8 @@
 the github source, upon any version tagged commit to the master branch.
 
 Click the status link and check out the logs if you're interested in the
 package lineage; meaning how the released pypi module was constructed from
 source.
 
 [1]: https://www.imdb.com/interfaces/
-[2]: https://pypi.org/project/imdb-sqlite/
+[2]: https://pypi.org/project/imdb-sqlite/
```

### Comparing `imdb-sqlite-1.0.0/imdb_sqlite/__main__.py` & `imdb-sqlite-1.0.1/imdb_sqlite/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # database. The files are imported in order listed, and are obtained from:
 # https://www.imdb.com/interfaces/
 
 # <filename>: ( <table-name>, {<tsv-header>: column} )
 TSV_TABLE_MAP = OrderedDict([
     ('name.basics.tsv.gz',
         ('people', OrderedDict([
-            ('nconst',            Column(name='person_id', type='VARCHAR PRIMARY KEY')),
+            ('nconst',            Column(name='person_id', type='VARCHAR PRIMARY KEY', index=True)),
             ('primaryName',       Column(name='name', index=True)),
             ('birthYear',         Column(name='born', type='INTEGER')),
             ('deathYear',         Column(name='died', type='INTEGER')),
         ]))),
     ('title.basics.tsv.gz',
         ('titles', OrderedDict([
             ('tconst',            Column(name='title_id', type='VARCHAR PRIMARY KEY')),
@@ -134,17 +134,21 @@
         self.connection.executescript(sql)
 
     def create_indices(self):
         sqls = [self._create_index_sql(table, mapping.values())
                 for table, mapping in TSV_TABLE_MAP.values()]
         sql = '\n'.join([s for s in sqls if s])
         logger.debug(sql)
-        self.connection.executescript(sql)
+        for stmt in tqdm(sql.split('\n'), unit='index'):
+            self.connection.executescript(stmt)
         self.commit()
 
+    def analyze(self):
+        self.connection.executescript("ANALYZE;")
+
     def begin(self):
         logger.debug('TX BEGIN')
         return self.cursor.execute('BEGIN')
 
     def commit(self):
         logger.debug('TX COMMIT')
         self.connection.commit()
@@ -181,15 +185,15 @@
         return '\n'.join(lines) + '\n'
 
     @staticmethod
     def _create_index_sql(table_name, columns):
         lines = ['CREATE INDEX ix_{table}_{col} ON {table} ({col});'
                  .format(table=table_name, col=c.name)
                  for c in columns
-                 if c.index and not c.pk and not c.unique]
+                 if c.index]
         return '\n'.join(lines)
 
 
 def ensure_downloaded(files, cache_dir):
     """
     Download the collection of +files+ into cache_dir unless they already
     exist there.
@@ -313,14 +317,17 @@
         table, column_mapping = table_mapping
         import_file(db, os.path.join(opts.cache_dir, filename),
                     table, column_mapping)
 
     logger.info('Creating table indices ...')
     db.create_indices()
 
+    logger.info('Analyzing DB to generate statistic for query planner ...')
+    db.analyze()
+
     db.close()
     logger.info('Import successful')
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `imdb-sqlite-1.0.0/imdb_sqlite.egg-info/PKG-INFO` & `imdb-sqlite-1.0.1/imdb_sqlite.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imdb-sqlite
-Version: 1.0.0
+Version: 1.0.1
 Summary: Imports IMDB TSV files into a SQLite database
 Home-page: https://github.com/jojje/imdb-sqlite
 Author: Jonas Tingeborn
 Author-email: tinjon+pip@gmail.com
 License: GNU GPL v2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -169,50 +169,23 @@
 production. The current set of crew categories are:
 ```
 { actor, actress, archive_footage, archive_sound, cinematographer, composer,
   director, editor, producer, production_designer, self, writer }
 ```
 
 ### Performance tips
-Many relations over a ten gigabyte database is where a relational
-DB really starts showing its limits. The above query takes quite a while to run.
-Optimally a graph DB would be used instead, since the query is more of that
-nature. Some things can still be done to get an _OK_ response time. If you use
-IDs instead of names, some joins can be eliminated. For example by using the
-IMDB IDs for Pacino and De Niro instead of searching for them by name, the above
-query is sped up by an order of magnitude or so, by eliminating the index search
-through two people tables.
-
-```sql
-SELECT t.title_id, t.type, t.primary_title, t.premiered, t.genres,
-       c1.characters AS 'Pacino played', c2.characters AS 'Deniro played'
-FROM crew c1
-INNER JOIN crew c2 ON ( c1.title_id = c2.title_id  )
-INNER JOIN titles t ON ( c2.title_id = t.title_id  )
-WHERE c1.person_id = 'nm0000199' -- Pacino
-AND   c2.person_id = 'nm0000134' -- De Niro
-AND   c1.category = 'actor' AND c2.category = 'actor'
-```
-
-Another thing to try is to further normalize the data. There is quite some
-duplication in the data, such at title types, crew categories etc. That
-duplication prevents the DB from efficiently joining tables. Even though a lot
-of indices are used, any collection of duplicates in a column forces the engine
-to essentially do brute force scans through all those duplicates. It's not much
-else it can do, and this takes time. Normalizing away such duplicates _will_
-mean more joins are required, but it should hopefully allow the engine to more
-quickly whittle down the dataset. I've not tried this, but it seems something
-plausible to invetigate if your queries are too slow for your taste.
-
-Finally, when in doubt. Prefix your query with the `EXPLAIN QUERY PLAN`. If you
-see `SCAN TABLE` in there, particularly in the beginning, it means the DB is
-doing a brute-force search through all the data in the column. This is _very_
-slow. You want the query plan to say `SEARCH` everywhere. Create an index for
-the column indicated as being scanned and rerun the query plan. Hopefully that
-resulted in orders of magnitude query speed improvement.
+Prefix your query with the `EXPLAIN QUERY PLAN`. If you see `SCAN TABLE` in
+there, particularly in the beginning, it means the DB is doing a brute-force
+search through all the data in the column. This is _very_ slow. You want the
+query plan to say `SEARCH` everywhere. If the query shows autoindex rather than
+using an explicit index, then that may also be the cause for slow joins. The
+tables are very large, which can result in a lot of I/O without explicit
+indices. To resolve, create an index for the column indicated as being scanned
+or using autoindex and rerun the query plan. Hopefully that results in a
+massive query speedup.
 
 For example `sqlite3 imdb.db "CREATE INDEX myindex ON <table-name> (<slow-column>)"`
 
 ## PyPI
 Current status of the project is:
 [![Build Status](https://github.com/jojje/imdb-sqlite/actions/workflows/python-publish.yml/badge.svg)](https://github.com/jojje/imdb-sqlite/actions/workflows/python-publish.yml)
```

### Comparing `imdb-sqlite-1.0.0/setup.py` & `imdb-sqlite-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='imdb-sqlite',
-    version='1.0.0',
+    version='1.0.1',
     author='Jonas Tingeborn',
     author_email='tinjon+pip@gmail.com',
     description='Imports IMDB TSV files into a SQLite database',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jojje/imdb-sqlite',
     packages=setuptools.find_packages(),
```

