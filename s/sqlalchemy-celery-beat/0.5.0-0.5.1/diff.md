# Comparing `tmp/sqlalchemy_celery_beat-0.5.0.tar.gz` & `tmp/sqlalchemy_celery_beat-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.5.0.tar", last modified: Sun Jun 18 04:06:42 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.5.1.tar", last modified: Sun Jun 18 04:43:57 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.5.0.tar` & `sqlalchemy_celery_beat-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 04:06:42.776528 sqlalchemy_celery_beat-0.5.0/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.5.0/LICENSE
--rw-rw-rw-   0        0        0    10523 2023-06-18 04:06:42.774526 sqlalchemy_celery_beat-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     9554 2023-06-18 02:51:09.000000 sqlalchemy_celery_beat-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 04:06:42.776528 sqlalchemy_celery_beat-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     3138 2023-06-18 04:05:34.000000 sqlalchemy_celery_beat-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:06:42.735526 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      455 2023-06-18 04:05:43.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    12321 2023-06-18 03:56:52.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16270 2023-06-18 03:12:47.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     4164 2023-06-18 03:49:29.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:06:42.772525 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0    10523 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 04:43:57.417286 sqlalchemy_celery_beat-0.5.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    10573 2023-06-18 04:43:57.416284 sqlalchemy_celery_beat-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9602 2023-06-18 04:42:43.000000 sqlalchemy_celery_beat-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 04:43:57.417286 sqlalchemy_celery_beat-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     3138 2023-06-18 04:43:11.000000 sqlalchemy_celery_beat-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:43:57.380286 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      455 2023-06-18 04:43:14.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    12367 2023-06-18 04:28:22.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16270 2023-06-18 03:12:47.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     4171 2023-06-18 04:09:09.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:43:57.414284 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0    10573 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.5.0/LICENSE` & `sqlalchemy_celery_beat-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.0/PKG-INFO` & `sqlalchemy_celery_beat-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -70,14 +70,16 @@
    $ celery beat -A tasks -S sqlalchemy_celery_beat.schedulers:DatabaseScheduler -l info
    ```
     you can also use the shorthand argument `-S sqlalchemy`
 ## Description
 
 After the celery beat is started, by default it create a sqlite database(`schedule.db`) in current folder. You can use `SQLiteStudio.exe` to inspect it.
 
+Sample from the `PeriodicTask` model's table
+
 ![sqlite](screenshot/sqlite.png)
 
 When you want to update scheduler, you can update the data in `schedule.db`. But `sqlalchemy_celery_beat` don't update the scheduler immediately. Then you shoule be change the first column's `last_update` field in the `celery_periodic_task_changed` to now datetime. Finally the celery beat will update scheduler at next wake-up time.
 
 ### Database Configuration
 
 You can configure sqlalchemy db uri when you configure the celery, example as:
```

### Comparing `sqlalchemy_celery_beat-0.5.0/README.md` & `sqlalchemy_celery_beat-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
    $ celery beat -A tasks -S sqlalchemy_celery_beat.schedulers:DatabaseScheduler -l info
    ```
     you can also use the shorthand argument `-S sqlalchemy`
 ## Description
 
 After the celery beat is started, by default it create a sqlite database(`schedule.db`) in current folder. You can use `SQLiteStudio.exe` to inspect it.
 
+Sample from the `PeriodicTask` model's table
+
 ![sqlite](screenshot/sqlite.png)
 
 When you want to update scheduler, you can update the data in `schedule.db`. But `sqlalchemy_celery_beat` don't update the scheduler immediately. Then you shoule be change the first column's `last_update` field in the `celery_periodic_task_changed` to now datetime. Finally the celery beat will update scheduler at next wake-up time.
 
 ### Database Configuration
 
 You can configure sqlalchemy db uri when you configure the celery, example as:
```

### Comparing `sqlalchemy_celery_beat-0.5.0/setup.py` & `sqlalchemy_celery_beat-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.5.0",
+    version="0.5.1",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,16 @@
             setattr(self, attr, value)
         return self
 
 
 class PeriodicTaskChanged(ModelBase, ModelMixin):
     """Helper table for tracking updates to periodic tasks."""
     __table_args__ = {
-        'sqlite_autoincrement': False
+        'sqlite_autoincrement': False,
+        'schema': 'celery_schema'
     }
 
     id = sa.Column(sa.Integer, primary_key=True)
     last_update = sa.Column(
         sa.DateTime(timezone=True), nullable=False, default=dt.datetime.now)
 
     @classmethod
@@ -116,15 +117,15 @@
     one_off = sa.Column(sa.Boolean(), default=False)
     start_time = sa.Column(sa.DateTime(timezone=True))
     enabled = sa.Column(sa.Boolean(), default=True)
     last_run_at = sa.Column(sa.DateTime(timezone=True))
     total_run_count = sa.Column(sa.Integer(), nullable=False, default=0)
 
     date_changed = sa.Column(sa.DateTime(timezone=True),
-                             default=func.now(), onupdate=func.now())
+                             default=dt.datetime.now, onupdate=dt.datetime.now)
     description = sa.Column(sa.Text(), default='')
 
     no_changes = False
 
     discriminator = sa.Column(sa.String(50), nullable=False)
     """Refers to the type of parent."""
```

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/schedulers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """Base class which provides automated table name
     and surrogate primary key column.
 
     """
 
     @declared_attr
     def __tablename__(cls):
-        return f"{cls.__name__.lower()}"
+        return f"celery_{cls.__name__.lower()}"
 
     id = Column(Integer, primary_key=True)
 
     __table_args__ = {
         'sqlite_autoincrement': True,
         'schema': 'celery_schema'
     }
```

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -70,14 +70,16 @@
    $ celery beat -A tasks -S sqlalchemy_celery_beat.schedulers:DatabaseScheduler -l info
    ```
     you can also use the shorthand argument `-S sqlalchemy`
 ## Description
 
 After the celery beat is started, by default it create a sqlite database(`schedule.db`) in current folder. You can use `SQLiteStudio.exe` to inspect it.
 
+Sample from the `PeriodicTask` model's table
+
 ![sqlite](screenshot/sqlite.png)
 
 When you want to update scheduler, you can update the data in `schedule.db`. But `sqlalchemy_celery_beat` don't update the scheduler immediately. Then you shoule be change the first column's `last_update` field in the `celery_periodic_task_changed` to now datetime. Finally the celery beat will update scheduler at next wake-up time.
 
 ### Database Configuration
 
 You can configure sqlalchemy db uri when you configure the celery, example as:
```

### Comparing `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

