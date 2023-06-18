# Comparing `tmp/sqlalchemy_celery_beat-0.4.7.tar.gz` & `tmp/sqlalchemy_celery_beat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.4.7.tar", last modified: Fri Jun 16 17:40:43 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.5.0.tar", last modified: Sun Jun 18 04:06:42 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.4.7.tar` & `sqlalchemy_celery_beat-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:40:43.968468 sqlalchemy_celery_beat-0.4.7/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.4.7/LICENSE
--rw-rw-rw-   0        0        0     9914 2023-06-16 17:40:43.967475 sqlalchemy_celery_beat-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     8955 2023-06-16 16:33:08.000000 sqlalchemy_celery_beat-0.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 17:40:43.968468 sqlalchemy_celery_beat-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     3138 2023-06-16 17:40:10.000000 sqlalchemy_celery_beat-0.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:40:43.936468 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      455 2023-06-16 17:40:14.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    13539 2023-06-16 17:39:12.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16955 2023-06-16 03:08:50.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     3708 2023-06-16 17:18:27.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:40:43.964473 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0     9914 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-16 17:40:43.000000 sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 04:06:42.776528 sqlalchemy_celery_beat-0.5.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    10523 2023-06-18 04:06:42.774526 sqlalchemy_celery_beat-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9554 2023-06-18 02:51:09.000000 sqlalchemy_celery_beat-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 04:06:42.776528 sqlalchemy_celery_beat-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3138 2023-06-18 04:05:34.000000 sqlalchemy_celery_beat-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:06:42.735526 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      455 2023-06-18 04:05:43.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    12321 2023-06-18 03:56:52.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16270 2023-06-18 03:12:47.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     4164 2023-06-18 03:49:29.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-18 04:06:42.772525 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0    10523 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-18 04:06:42.000000 sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.4.7/LICENSE` & `sqlalchemy_celery_beat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.7/PKG-INFO` & `sqlalchemy_celery_beat-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.4.7
+Version: 0.5.0
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlalchemy-celery-beat
 
 A Scheduler Based Sqlalchemy for Celery.
 
-> NOTE: This project was originally developed by [AngelLiang](https://github.com/AngelLiang/celery-sqlalchemy-scheduler) to use sqlalchemy as the database scheduler, like [django-celery-beat](https://github.com/celery/django-celery-beat) for django. I am trying to continue on his work and maintain a working solution.
+> NOTE: This project was originally developed by [AngelLiang](https://github.com/AngelLiang/celery-sqlalchemy-scheduler) to use sqlalchemy as the database scheduler for Flask or FastAPI, like [django-celery-beat](https://github.com/celery/django-celery-beat) for django. I am trying to continue on his work and maintain a working solution.
 
 
 ### Prerequisites
 
 - Python 3
 - celery >= 5.0
 - sqlalchemy >= 1.4
@@ -171,15 +171,15 @@
     then they should all point to the same schedule object.
 
 Now that we have defined the schedule object, we can create the periodic task
 entry:
 
 ```python
     >>> task = PeriodicTask(
-    ...     interval=schedule,                  # we created this above.
+    ...     schedule_model=schedule,            # we created this above.
     ...     name='Importing contacts',          # simply describes this periodic task.
     ...     task='proj.tasks.import_contacts',  # name of task.
     ... )
     >>> session.add(task)
     >>> session.commit()
 ```
 
@@ -190,15 +190,15 @@
 Here\'s an example specifying the arguments, note how JSON serialization
 is required:
 
     >>> import json
     >>> from datetime import datetime, timedelta
 
     >>> periodic_task = PeriodicTask(
-    ...     interval=schedule,                  # we created this above.
+    ...     schedule_model=schedule,                  # we created this above.
     ...     name='Importing contacts',          # simply describes this periodic task.
     ...     task='proj.tasks.import_contacts',  # name of task.
     ...     args=json.dumps(['arg1', 'arg2']),
     ...     kwargs=json.dumps({
     ...        'be_careful': True,
     ...     }),
     ...     expires=datetime.utcnow() + timedelta(seconds=30)
@@ -223,23 +223,31 @@
     ... )
 
 The crontab schedule is linked to a specific timezone using the
 'timezone' input parameter.
 
 Then to create a periodic task using this schedule, use the same
 approach as the interval-based periodic task earlier in this document,
-but instead of `interval=schedule`, specify `crontab=schedule`:
+the `schedule_model` is a generic foreign-key implementation which makes things very easy and efficient:
 
     >>> periodic_task = PeriodicTask(
-    ...     crontab=schedule,
+    ...     schedule_model=schedule,
     ...     name='Importing contacts',
     ...     task='proj.tasks.import_contacts',
     ... )
-    ... session.add(periodic_task)
-    ... session.commit()
+
+What the previous code actually do is this:
+
+    >>> periodic_task = PeriodicTask(
+    ...     schedule_id=schedule.id,
+    ...     discriminator=schedule.discriminator,
+    ...     name='Importing contacts',
+    ...     task='proj.tasks.import_contacts',
+    ... )
+So when you can use `discriminator` + `schedule_id` or use the convenient property `schedule_model` and it will populate them for you behind the scenes.
 
 ### Temporarily disable a periodic task
 
 You can use the `enabled` flag to temporarily disable a periodic task:
 
     >>> periodic_task.enabled = False
     >>> session.add(periodic_task)
@@ -251,19 +259,19 @@
 ``` python
 from sqlalchemy_celery_beat.models import PeriodicTaskChanged
 
 session = get_beat_session()
 
 stmt = update(PeriodicTask).where(PeriodicTask.name == 'task-123').values(enabled=False)
 
-session.execute(stmt)
-session.commit()  # changes are not in the database but the schduler has no idea
+session.execute(stmt)  # using execute causes no orm event to fire, changes are in the database but the schduler has no idea
+session.commit()
 
 PeriodicTaskChanged.update_from_session(session)
-# now schduler reloads the tasks and all is good
+# now scheduler reloads the tasks and all is good
 ```
 This is not needed when you are updating a specific object using `session.add(task)` because it will trigger the `after_update`, `after_delete` or `after_insert` events.
 
 ### Example running periodic tasks
 
 The periodic tasks still need 'workers' to execute them. So make sure
 the default **Celery** package is installed. (If not installed, please
@@ -280,19 +288,21 @@
     scheduler):
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
+- ✅ Implement a generic foreign key
 - More robust attribute validation on models
 - Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
-Any help is appreciated 🙂
+Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
 
 - [django-celery-beat](https://github.com/celery/django-celery-beat)
 - [celerybeatredis](https://github.com/liuliqiang/celerybeatredis)
 - [celery](https://github.com/celery/celery)
+- [SQLAlchemy](https://www.sqlalchemy.org)
```

### Comparing `sqlalchemy_celery_beat-0.4.7/README.md` & `sqlalchemy_celery_beat-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sqlalchemy-celery-beat
 
 A Scheduler Based Sqlalchemy for Celery.
 
-> NOTE: This project was originally developed by [AngelLiang](https://github.com/AngelLiang/celery-sqlalchemy-scheduler) to use sqlalchemy as the database scheduler, like [django-celery-beat](https://github.com/celery/django-celery-beat) for django. I am trying to continue on his work and maintain a working solution.
+> NOTE: This project was originally developed by [AngelLiang](https://github.com/AngelLiang/celery-sqlalchemy-scheduler) to use sqlalchemy as the database scheduler for Flask or FastAPI, like [django-celery-beat](https://github.com/celery/django-celery-beat) for django. I am trying to continue on his work and maintain a working solution.
 
 
 ### Prerequisites
 
 - Python 3
 - celery >= 5.0
 - sqlalchemy >= 1.4
@@ -152,15 +152,15 @@
     then they should all point to the same schedule object.
 
 Now that we have defined the schedule object, we can create the periodic task
 entry:
 
 ```python
     >>> task = PeriodicTask(
-    ...     interval=schedule,                  # we created this above.
+    ...     schedule_model=schedule,            # we created this above.
     ...     name='Importing contacts',          # simply describes this periodic task.
     ...     task='proj.tasks.import_contacts',  # name of task.
     ... )
     >>> session.add(task)
     >>> session.commit()
 ```
 
@@ -171,15 +171,15 @@
 Here\'s an example specifying the arguments, note how JSON serialization
 is required:
 
     >>> import json
     >>> from datetime import datetime, timedelta
 
     >>> periodic_task = PeriodicTask(
-    ...     interval=schedule,                  # we created this above.
+    ...     schedule_model=schedule,                  # we created this above.
     ...     name='Importing contacts',          # simply describes this periodic task.
     ...     task='proj.tasks.import_contacts',  # name of task.
     ...     args=json.dumps(['arg1', 'arg2']),
     ...     kwargs=json.dumps({
     ...        'be_careful': True,
     ...     }),
     ...     expires=datetime.utcnow() + timedelta(seconds=30)
@@ -204,23 +204,31 @@
     ... )
 
 The crontab schedule is linked to a specific timezone using the
 'timezone' input parameter.
 
 Then to create a periodic task using this schedule, use the same
 approach as the interval-based periodic task earlier in this document,
-but instead of `interval=schedule`, specify `crontab=schedule`:
+the `schedule_model` is a generic foreign-key implementation which makes things very easy and efficient:
 
     >>> periodic_task = PeriodicTask(
-    ...     crontab=schedule,
+    ...     schedule_model=schedule,
     ...     name='Importing contacts',
     ...     task='proj.tasks.import_contacts',
     ... )
-    ... session.add(periodic_task)
-    ... session.commit()
+
+What the previous code actually do is this:
+
+    >>> periodic_task = PeriodicTask(
+    ...     schedule_id=schedule.id,
+    ...     discriminator=schedule.discriminator,
+    ...     name='Importing contacts',
+    ...     task='proj.tasks.import_contacts',
+    ... )
+So when you can use `discriminator` + `schedule_id` or use the convenient property `schedule_model` and it will populate them for you behind the scenes.
 
 ### Temporarily disable a periodic task
 
 You can use the `enabled` flag to temporarily disable a periodic task:
 
     >>> periodic_task.enabled = False
     >>> session.add(periodic_task)
@@ -232,19 +240,19 @@
 ``` python
 from sqlalchemy_celery_beat.models import PeriodicTaskChanged
 
 session = get_beat_session()
 
 stmt = update(PeriodicTask).where(PeriodicTask.name == 'task-123').values(enabled=False)
 
-session.execute(stmt)
-session.commit()  # changes are not in the database but the schduler has no idea
+session.execute(stmt)  # using execute causes no orm event to fire, changes are in the database but the schduler has no idea
+session.commit()
 
 PeriodicTaskChanged.update_from_session(session)
-# now schduler reloads the tasks and all is good
+# now scheduler reloads the tasks and all is good
 ```
 This is not needed when you are updating a specific object using `session.add(task)` because it will trigger the `after_update`, `after_delete` or `after_insert` events.
 
 ### Example running periodic tasks
 
 The periodic tasks still need 'workers' to execute them. So make sure
 the default **Celery** package is installed. (If not installed, please
@@ -261,19 +269,21 @@
     scheduler):
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
+- ✅ Implement a generic foreign key
 - More robust attribute validation on models
 - Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
-Any help is appreciated 🙂
+Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
 
 - [django-celery-beat](https://github.com/celery/django-celery-beat)
 - [celerybeatredis](https://github.com/liuliqiang/celerybeatredis)
 - [celery](https://github.com/celery/celery)
+- [SQLAlchemy](https://www.sqlalchemy.org)
```

### Comparing `sqlalchemy_celery_beat-0.4.7/setup.py` & `sqlalchemy_celery_beat-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.4.7",
+    version="0.5.0",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # coding=utf-8
-
+# The generic foreign key is implemented after this example:
+# https://docs.sqlalchemy.org/en/20/_modules/examples/generic_associations/generic_fk.html
 import datetime as dt
+from typing import Any
 from zoneinfo import ZoneInfo
 
 import sqlalchemy as sa
 from celery import schedules
 from celery.utils.log import get_logger
-from sqlalchemy import func
-from sqlalchemy.event import listen
+from sqlalchemy import event, func
 from sqlalchemy.future import Connection
-from sqlalchemy.orm import Session, foreign, relationship, remote, validates
+from sqlalchemy.orm import (Session, backref, foreign, relationship, remote,
+                            validates)
 from sqlalchemy.sql import insert, select, update
 
 from .clockedschedule import clocked
 from .session import ModelBase
 from .tzcrontab import TzAwareCrontab
 
 logger = get_logger('sqlalchemy_celery_beat.models')
@@ -32,21 +34,189 @@
 
     def update(self, **kw):
         for attr, value in kw.items():
             setattr(self, attr, value)
         return self
 
 
-class IntervalSchedule(ModelBase, ModelMixin):
-    __tablename__ = 'celery_interval_schedule'
+class PeriodicTaskChanged(ModelBase, ModelMixin):
+    """Helper table for tracking updates to periodic tasks."""
     __table_args__ = {
-        'sqlite_autoincrement': True,
-        'schema': 'celery_schema'
+        'sqlite_autoincrement': False
     }
 
+    id = sa.Column(sa.Integer, primary_key=True)
+    last_update = sa.Column(
+        sa.DateTime(timezone=True), nullable=False, default=dt.datetime.now)
+
+    @classmethod
+    def changed(cls, mapper, connection, target):
+        """
+        :param mapper: the Mapper which is the target of this event
+        :param connection: the Connection being used
+        :param target: the mapped instance being persisted
+        """
+        if not target.no_changes:
+            cls.update_changed(mapper, connection, target)
+
+    @classmethod
+    def update_changed(cls, mapper, connection: Connection, target):
+        """
+        :param mapper: the Mapper which is the target of this event
+        :param connection: the Connection being used
+        :param target: the mapped instance being persisted
+        """
+        logger.info('Database last time set to now')
+        s = connection.execute(select(PeriodicTaskChanged).
+                               where(PeriodicTaskChanged.id == 1).limit(1))
+        if not s:
+            s = connection.execute(insert(PeriodicTaskChanged),
+                                   last_update=dt.datetime.now())
+        else:
+            s = connection.execute(update(PeriodicTaskChanged).
+                                   where(PeriodicTaskChanged.id == 1).
+                                   values(last_update=dt.datetime.now()))
+
+    @classmethod
+    def update_from_session(cls, session: Session, commit: bool = True):
+        """
+        :param session: the Session to use
+        :param commit: commit the session if set to true
+        """
+        connection = session.connection()
+        cls.update_changed(None, connection, None)
+        if commit:
+            connection.commit()
+
+    @classmethod
+    def last_change(cls, session):
+        periodic_tasks = session.query(PeriodicTaskChanged).get(1)
+        if periodic_tasks:
+            return periodic_tasks.last_update
+
+
+class PeriodicTask(ModelBase, ModelMixin):
+
+    id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
+    # name
+    name = sa.Column(sa.String(255), unique=True)
+    # task name
+    task = sa.Column(sa.String(255))
+
+    args = sa.Column(sa.Text(), default='[]')
+    kwargs = sa.Column(sa.Text(), default='{}')
+    # queue for celery
+    queue = sa.Column(sa.String(255))
+    # exchange for celery
+    exchange = sa.Column(sa.String(255))
+    # routing_key for celery
+    routing_key = sa.Column(sa.String(255))
+    priority = sa.Column(sa.Integer())
+    expires = sa.Column(sa.DateTime(timezone=True))
+
+    one_off = sa.Column(sa.Boolean(), default=False)
+    start_time = sa.Column(sa.DateTime(timezone=True))
+    enabled = sa.Column(sa.Boolean(), default=True)
+    last_run_at = sa.Column(sa.DateTime(timezone=True))
+    total_run_count = sa.Column(sa.Integer(), nullable=False, default=0)
+
+    date_changed = sa.Column(sa.DateTime(timezone=True),
+                             default=func.now(), onupdate=func.now())
+    description = sa.Column(sa.Text(), default='')
+
+    no_changes = False
+
+    discriminator = sa.Column(sa.String(50), nullable=False)
+    """Refers to the type of parent."""
+
+    schedule_id = sa.Column(sa.Integer(), nullable=False)
+    """Refers to the primary key of the parent.
+
+    This could refer to any table.
+    """
+    @property
+    def schedule_model(self):
+        """Provides in-Python access to the "parent" by choosing
+        the appropriate relationship.
+
+        """
+        return getattr(self, "model_%s" % self.discriminator)
+
+    @schedule_model.setter
+    def schedule_model(self, value):
+        if value is not None:
+            self.schedule_id = value.id
+            self.discriminator = value.discriminator
+            setattr(self, "model_%s" % value.discriminator, value)
+
+    @classmethod
+    def validate_before_insert(cls, mapper, connection, target):
+        if isinstance(target.schedule_model, ClockedSchedule) and not target.one_off:
+            raise ValueError("one_off must be True for clocked schedule")
+
+    def __repr__(self):
+        fmt = '{0.name}: {0.schedule_model}'
+        return fmt.format(self)
+
+    @property
+    def task_name(self):
+        return self.task
+
+    @task_name.setter
+    def task_name(self, value):
+        self.task = value
+
+    @property
+    def schedule(self):
+        if self.schedule_model:
+            return self.schedule_model.schedule
+        raise ValueError('{} schedule is None!'.format(self.name))
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+
+
+class ScheduleModel:
+    """ScheduleModel mixin, inherited by all schedule classes
+
+    """
+
+
+@event.listens_for(ScheduleModel, "mapper_configured", propagate=True)
+def setup_listener(mapper, class_):
+    name = class_.__name__
+    discriminator = name.lower()
+    class_.periodic_tasks = relationship(
+        PeriodicTask,
+        primaryjoin=sa.and_(
+            class_.id == foreign(remote(PeriodicTask.schedule_id)),
+            PeriodicTask.discriminator == discriminator,
+        ),
+        backref=backref(
+            "model_%s" % discriminator,
+            primaryjoin=remote(class_.id) == foreign(PeriodicTask.schedule_id),
+            viewonly=True
+        ),
+        overlaps='periodic_tasks',
+        cascade="all, delete-orphan"
+    )
+
+    @event.listens_for(class_.periodic_tasks, "append")
+    def append_periodic_tasks(target, value, initiator):
+        value.discriminator = discriminator
+
+    @property
+    def get_discriminator(self):
+        return self.__class__.__name__.lower()
+
+    class_.discriminator = get_discriminator
+
+
+class IntervalSchedule(ScheduleModel, ModelBase):
+
     DAYS = 'days'
     HOURS = 'hours'
     MINUTES = 'minutes'
     SECONDS = 'seconds'
     MICROSECONDS = 'microseconds'
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
@@ -79,20 +249,15 @@
         return model
 
     @property
     def period_singular(self):
         return self.period[:-1]
 
 
-class CrontabSchedule(ModelBase, ModelMixin):
-    __tablename__ = 'celery_crontab_schedule'
-    __table_args__ = {
-        'sqlite_autoincrement': True,
-        'schema': 'celery_schema'
-    }
+class CrontabSchedule(ScheduleModel, ModelBase):
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
     minute = sa.Column(sa.String(60 * 4), default='*')
     hour = sa.Column(sa.String(24 * 4), default='*')
     day_of_week = sa.Column(sa.String(64), default='*')
     day_of_month = sa.Column(sa.String(31 * 4), default='*')
     month_of_year = sa.Column(sa.String(64), default='*')
@@ -132,20 +297,15 @@
         if not model:
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
 
-class SolarSchedule(ModelBase, ModelMixin):
-    __tablename__ = 'celery_solar_schedule'
-    __table_args__ = {
-        'sqlite_autoincrement': True,
-        'schema': 'celery_schema'
-    }
+class SolarSchedule(ScheduleModel, ModelBase):
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
 
     event = sa.Column(sa.String(24))
     latitude = sa.Column(sa.Float())
     longitude = sa.Column(sa.Float())
 
@@ -176,20 +336,15 @@
         return '{0} ({1}, {2})'.format(
             self.event,
             self.latitude,
             self.longitude
         )
 
 
-class ClockedSchedule(ModelBase, ModelMixin):
-    __tablename__ = 'celery_clocked_schedule'
-    __table_args__ = {
-        'sqlite_autoincrement': True,
-        'schema': 'celery_schema'
-    }
+class ClockedSchedule(ScheduleModel, ModelBase):
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
     clocked_time = sa.Column(sa.DateTime(timezone=True))
 
     def __repr__(self):
         return f'{self.clocked_time}'
 
@@ -205,195 +360,13 @@
         if not model:
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
 
-class PeriodicTaskChanged(ModelBase, ModelMixin):
-    """Helper table for tracking updates to periodic tasks."""
-
-    __tablename__ = 'celery_periodic_task_changed'
-    __table_args__ = {'schema': 'celery_schema'}
-
-    id = sa.Column(sa.Integer, primary_key=True)
-    last_update = sa.Column(
-        sa.DateTime(timezone=True), nullable=False, default=dt.datetime.now)
-
-    @classmethod
-    def changed(cls, mapper, connection, target):
-        """
-        :param mapper: the Mapper which is the target of this event
-        :param connection: the Connection being used
-        :param target: the mapped instance being persisted
-        """
-        if not target.no_changes:
-            cls.update_changed(mapper, connection, target)
-
-    @classmethod
-    def update_changed(cls, mapper, connection: Connection, target):
-        """
-        :param mapper: the Mapper which is the target of this event
-        :param connection: the Connection being used
-        :param target: the mapped instance being persisted
-        """
-        logger.debug('Setting last_update time to now')
-        s = connection.execute(select(PeriodicTaskChanged).
-                               where(PeriodicTaskChanged.id == 1).limit(1))
-        if not s:
-            s = connection.execute(insert(PeriodicTaskChanged),
-                                   last_update=dt.datetime.now())
-        else:
-            s = connection.execute(update(PeriodicTaskChanged).
-                                   where(PeriodicTaskChanged.id == 1).
-                                   values(last_update=dt.datetime.now()))
-
-    @classmethod
-    def update_from_session(cls, session: Session, commit: bool = True):
-        """
-        :param session: the Session to use
-        :param commit: commit the session if set to true
-        """
-        connection = session.connection()
-        cls.update_changed(None, connection, None)
-        if commit:
-            connection.commit()
-
-    @classmethod
-    def last_change(cls, session):
-        periodic_tasks = session.query(PeriodicTaskChanged).get(1)
-        if periodic_tasks:
-            return periodic_tasks.last_update
-
-
-class PeriodicTask(ModelBase, ModelMixin):
-
-    __tablename__ = 'celery_periodic_task'
-    __table_args__ = {
-        'sqlite_autoincrement': True,
-        'schema': 'celery_schema'
-    }
-
-    id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
-    # name
-    name = sa.Column(sa.String(255), unique=True)
-    # task name
-    task = sa.Column(sa.String(255))
-
-    # not use ForeignKey
-    interval_id = sa.Column(sa.Integer)
-    interval = relationship(
-        IntervalSchedule,
-        uselist=False,
-        primaryjoin=foreign(interval_id) == remote(IntervalSchedule.id)
-    )
-
-    crontab_id = sa.Column(sa.Integer)
-    crontab = relationship(
-        CrontabSchedule,
-        uselist=False,
-        primaryjoin=foreign(crontab_id) == remote(CrontabSchedule.id)
-    )
-
-    solar_id = sa.Column(sa.Integer)
-    solar = relationship(
-        SolarSchedule,
-        uselist=False,
-        primaryjoin=foreign(solar_id) == remote(SolarSchedule.id)
-    )
-
-    clocked_id = sa.Column(sa.Integer)
-    clocked = relationship(
-        ClockedSchedule,
-        uselist=False,
-        primaryjoin=foreign(clocked_id) == remote(ClockedSchedule.id)
-    )
-
-    args = sa.Column(sa.Text(), default='[]')
-    kwargs = sa.Column(sa.Text(), default='{}')
-    # queue for celery
-    queue = sa.Column(sa.String(255))
-    # exchange for celery
-    exchange = sa.Column(sa.String(255))
-    # routing_key for celery
-    routing_key = sa.Column(sa.String(255))
-    priority = sa.Column(sa.Integer())
-    expires = sa.Column(sa.DateTime(timezone=True))
-
-    # 只执行一次
-    one_off = sa.Column(sa.Boolean(), default=False)
-    start_time = sa.Column(sa.DateTime(timezone=True))
-    enabled = sa.Column(sa.Boolean(), default=True)
-    last_run_at = sa.Column(sa.DateTime(timezone=True))
-    total_run_count = sa.Column(sa.Integer(), nullable=False, default=0)
-    # 修改时间
-    date_changed = sa.Column(sa.DateTime(timezone=True),
-                             default=func.now(), onupdate=func.now())
-    description = sa.Column(sa.Text(), default='')
-
-    no_changes = False
-
-    @classmethod
-    def validate_before_insert(cls, mapper, connection, target):
-        schedule_types = ['interval_id', 'crontab_id', 'solar_id', 'clocked_id']
-        selected_schedule_types = [s for s in schedule_types
-                                   if getattr(target, s)]
-        if len(selected_schedule_types) == 0:
-            raise ValueError(
-                'One of clocked, interval, crontab, or solar '
-                'must be set.'
-            )
-        elif len(selected_schedule_types) > 1:
-            raise ValueError('Only one of clocked, interval, crontab, '
-                             'or solar must be set')
-        if target.clocked_id and not target.one_off:
-            raise ValueError("one_off must be True for clocked schedule")
-
-    def __repr__(self):
-        fmt = '{0.name}: {{no schedule}}'
-        if self.interval:
-            fmt = '{0.name}: {0.interval}'
-        elif self.crontab:
-            fmt = '{0.name}: {0.crontab}'
-        elif self.solar:
-            fmt = '{0.name}: {0.solar}'
-        elif self.clocked:
-            fmt = '{0.name}: {0.clocked}'
-        return fmt.format(self)
-
-    @property
-    def task_name(self):
-        return self.task
-
-    @task_name.setter
-    def task_name(self, value):
-        self.task = value
-
-    @property
-    def schedule(self):
-        if self.interval:
-            return self.interval.schedule
-        elif self.crontab:
-            return self.crontab.schedule
-        elif self.solar:
-            return self.solar.schedule
-        elif self.clocked:
-            return self.clocked.schedule
-        raise ValueError('{} schedule is None!'.format(self.name))
-
-
-listen(PeriodicTask, 'after_insert', PeriodicTaskChanged.update_changed)
-listen(PeriodicTask, 'after_delete', PeriodicTaskChanged.update_changed)
-listen(PeriodicTask, 'after_update', PeriodicTaskChanged.changed)
-listen(PeriodicTask, 'before_insert', PeriodicTask.validate_before_insert)
-listen(IntervalSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
-listen(IntervalSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
-listen(IntervalSchedule, 'after_update', PeriodicTaskChanged.update_changed)
-listen(CrontabSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
-listen(CrontabSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
-listen(CrontabSchedule, 'after_update', PeriodicTaskChanged.update_changed)
-listen(SolarSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
-listen(SolarSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
-listen(SolarSchedule, 'after_update', PeriodicTaskChanged.update_changed)
-listen(ClockedSchedule, 'after_insert', PeriodicTaskChanged.update_changed)
-listen(ClockedSchedule, 'after_delete', PeriodicTaskChanged.update_changed)
-listen(ClockedSchedule, 'after_update', PeriodicTaskChanged.update_changed)
+event.listen(PeriodicTask, 'after_insert', PeriodicTaskChanged.update_changed)
+event.listen(PeriodicTask, 'after_delete', PeriodicTaskChanged.update_changed)
+event.listen(PeriodicTask, 'after_update', PeriodicTaskChanged.changed)
+event.listen(PeriodicTask, 'before_insert', PeriodicTask.validate_before_insert)
+event.listen(ScheduleModel, 'after_delete', PeriodicTaskChanged.update_changed, propagate=True)
+event.listen(ScheduleModel, 'after_update', PeriodicTaskChanged.update_changed, propagate=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/schedulers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # coding=utf-8
 
 import datetime as dt
 import logging
 import math
 from multiprocessing.util import Finalize
 
-import sqlalchemy
+import sqlalchemy as sa
 from celery import current_app, schedules
 from celery.beat import ScheduleEntry, Scheduler
 from celery.utils.log import get_logger
 from celery.utils.time import maybe_make_aware
 from kombu.utils.encoding import safe_repr, safe_str
 from kombu.utils.json import dumps, loads
 
 from .clockedschedule import clocked
 from .models import (ClockedSchedule, CrontabSchedule, IntervalSchedule,
                      PeriodicTask, PeriodicTaskChanged, SolarSchedule)
 from .session import SessionManager, session_cleanup
+from .time_utils import NEVER_CHECK_TIMEOUT
 
 # This scheduler must wake up more frequently than the
 # regular of 5 minutes because it needs to take external
 # changes to the schedule into account.
 DEFAULT_MAX_INTERVAL = 5  # seconds
 
 DEFAULT_BEAT_DBURI = 'sqlite:///schedule.db'
@@ -29,42 +30,38 @@
 
 ADD_ENTRY_ERROR = """\
 Cannot add entry %r to database schedule: %r. Contents: %r
 """
 
 
 session_manager = SessionManager()
-# session = session_manager()
 
 
 logger = get_logger('sqlalchemy_celery_beat.schedulers')
 
 
 class ModelEntry(ScheduleEntry):
     """Scheduler entry taken from database row."""
 
     model_schedules = (
-        # (schedule_type, model_type, model_field)
-        (schedules.crontab, CrontabSchedule, 'crontab'),
-        (schedules.schedule, IntervalSchedule, 'interval'),
-        (schedules.solar, SolarSchedule, 'solar'),
-        (clocked, ClockedSchedule, 'clocked'),
+        # (schedule_type, model_type)
+        (schedules.crontab, CrontabSchedule),
+        (schedules.schedule, IntervalSchedule),
+        (schedules.solar, SolarSchedule),
+        (clocked, ClockedSchedule),
     )
     save_fields = ['last_run_at', 'total_run_count', 'no_changes']
 
     def __init__(self, model, Session, app=None, **kw):
         """Initialize the model entry."""
         self.app = app or current_app._get_current_object()
-        self.session = kw.get('session')
         self.Session = Session
-
         self.model = model
         self.name = model.name
         self.task = model.task
-
         try:
             self.schedule = model.schedule
             logger.debug('schedule: {}'.format(self.schedule))
         except Exception as e:
             logger.error(e)
             logger.error(
                 'Disabling schedule %s that was removed from database',
@@ -101,38 +98,31 @@
             # and avoid the heap block.
             if self.model.start_time:
                 model.last_run_at = model.last_run_at \
                     - dt.timedelta(days=365 * 30)
 
         self.last_run_at = model.last_run_at
 
-        # 因为从数据库读取的 last_run_at 可能没有时区信息，所以这里必须加上时区信息
+        # Because the last_run_at read from the database may not have time zone information, 
+        # so time zone information must be added here
         self.last_run_at = self.last_run_at.replace(tzinfo=self.app.timezone)
 
-        # self.options['expires'] 同理
+        # self.options['expires']
         # if 'expires' in self.options:
         #     expires = self.options['expires']
         #     self.options['expires'] = expires.replace(tzinfo=self.app.timezone)
 
     def _disable(self, model):
         model.no_changes = True
         self.model.enabled = self.enabled = model.enabled = False
-        if self.session:
-            self.session.add(model)
-            self.session.commit()
-        else:
-            session = self.Session()
-            with session_cleanup(session):
-                session.add(model)
-                session.commit()
-
-            #     obj = session.query(PeriodicTask).get(model.id)
-            #     obj.enable = model.enabled
-            #     session.add(obj)
-            #     session.commit()
+        session = self.Session()
+        with session_cleanup(session):
+            session.add(model)
+            session.commit()
+            # session.refresh(model)
 
     def is_due(self):
         if not self.model.enabled:
             # 5 second delay for re-enable.
             return schedules.schedstate(False, 5.0)
 
         # START DATE: only run after the `start_time`, if one exists.
@@ -152,15 +142,15 @@
                 and self.model.total_run_count > 0:
             self.model.enabled = False  # disable
             self.model.total_run_count = 0  # Reset
             self.model.no_changes = False  # Mark the model entry as changed
             save_fields = ('enabled',)   # the additional fields to save
             self.save(save_fields)
 
-            return schedules.schedstate(False, None)  # Don't recheck
+            return schedules.schedstate(False, NEVER_CHECK_TIMEOUT)  # Don't recheck
 
         return self.schedule.is_due(self.last_run_at)
 
     def _default_now(self):
         now = self.app.now()
         # The PyTZ datetime must be localised for the Django-Celery-Beat
         # scheduler to work. Keep in mind that timezone arithmatic
@@ -176,15 +166,14 @@
         return self.__class__(self.model, Session=self.Session)
     next = __next__  # for 2to3
 
     def save(self, fields=tuple()):
         """
         :params fields: tuple, the additional fields to save
         """
-        # TODO:
         session = self.Session()
         with session_cleanup(session):
             # Object may not be synchronized, so only
             # change the fields we care about.
             obj = session.query(PeriodicTask).get(self.model.id)
 
             for field in self.save_fields:
@@ -192,21 +181,20 @@
             for field in fields:
                 setattr(obj, field, getattr(self.model, field))
             session.add(obj)
             session.commit()
 
     @classmethod
     def to_model_schedule(cls, session, schedule):
-        for schedule_type, model_type, model_field in cls.model_schedules:
+        for schedule_type, model_class in cls.model_schedules:
             # change to schedule
             schedule = schedules.maybe_schedule(schedule)
             if isinstance(schedule, schedule_type):
-                # TODO:
-                model_schedule = model_type.from_schedule(session, schedule)
-                return model_schedule, model_field
+                model_schedule = model_class.from_schedule(session, schedule)
+                return model_schedule
         raise ValueError(
             'Cannot convert schedule type {0!r} to model'.format(schedule))
 
     @classmethod
     def from_entry(cls, name, Session, app=None, **entry):
         """
 
@@ -217,28 +205,22 @@
              'options': {'expires': 43200}}
 
         """
         session = Session()
         with session_cleanup(session):
             periodic_task = session.query(
                 PeriodicTask).filter_by(name=name).first()
-            if not periodic_task:
-                periodic_task = PeriodicTask(name=name)
             temp = cls._unpack_fields(session, **entry)
-            periodic_task.update(**temp)
+            if not periodic_task:
+                periodic_task = PeriodicTask(name=name, **temp)
+            else:
+                periodic_task.update(**temp)
             session.add(periodic_task)
-            try:
-                session.commit()
-            except sqlalchemy.exc.IntegrityError as exc:
-                logger.error(exc)
-                session.rollback()
-            except Exception as exc:
-                logger.error(exc)
-                session.rollback()
-            res = cls(periodic_task, app=app, Session=Session, session=session)
+            session.commit()
+            res = cls(periodic_task, app=app, Session=Session)
             return res
 
     @classmethod
     def _unpack_fields(cls, session, schedule,
                        args=None, kwargs=None, relative=None, options=None,
                        **entry):
         """
@@ -246,18 +228,19 @@
         **entry sample:
 
             {'task': 'celery.backend_cleanup',
              'schedule': <crontab: 0 4 * * * (m/h/d/dM/MY)>,
              'options': {'expires': 43200}}
 
         """
-        model_schedule, model_field = cls.to_model_schedule(session, schedule)
+        model_schedule = cls.to_model_schedule(session, schedule)
         entry.update(
             # the model_id which to relationship
-            {model_field + '_id': model_schedule.id},
+            # {model_field + '_id': model_schedule.id},
+            {'schedule_model': model_schedule},
             args=dumps(args or []),
             kwargs=dumps(kwargs or {}),
             **cls._unpack_options(**options or {})
         )
         return entry
 
     @classmethod
@@ -318,27 +301,25 @@
     def setup_schedule(self):
         """override"""
         logger.info('setup_schedule')
         self.install_default_entries(self.schedule)
         self.update_from_dict(self.app.conf.beat_schedule)
 
     def all_as_schedule(self):
-        # TODO:
         session = self.Session()
         with session_cleanup(session):
             logger.debug('DatabaseScheduler: Fetching database schedule')
             # get all enabled PeriodicTask
             models = session.query(self.Model).filter_by(enabled=True).all()
             s = {}
             for model in models:
                 try:
                     s[model.name] = self.Entry(model,
                                                app=self.app,
-                                               Session=self.Session,
-                                               session=session)
+                                               Session=self.Session)
                 except ValueError:
                     pass
             return s
 
     def schedule_changed(self):
         session = self.Session()
         with session_cleanup(session):
@@ -380,25 +361,25 @@
                     self.schedule[name].save()  # save to database
                     logger.debug(
                         '{name} save to database'.format(name=name))
                     _tried.add(name)
                 except (KeyError) as exc:
                     logger.error(exc)
                     _failed.add(name)
-        except sqlalchemy.exc.IntegrityError as exc:
+        except sa.exc.IntegrityError as exc:
             logger.exception('Database error while sync: %r', exc)
         except Exception as exc:
             logger.exception(exc)
         finally:
             # retry later, only for the failed ones
             self._dirty |= _failed
 
-    def update_from_dict(self, mapping):
+    def update_from_dict(self, dict_):
         s = {}
-        for name, entry_fields in mapping.items():
+        for name, entry_fields in dict_.items():
             # {'task': 'celery.backend_cleanup',
             #  'schedule': schedules.crontab('0', '4', '*'),
             #  'options': {'expires': 43200}}
             try:
                 entry = self.Entry.from_entry(
                     name, Session=self.Session, app=self.app,
                     **entry_fields)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,42 @@
 """SQLAlchemy session."""
 
 import time
 from contextlib import contextmanager
 
 from celery.utils.time import get_exponential_backoff_interval
 from kombu.utils.compat import register_after_fork
-from sqlalchemy import DDL, create_engine
+from sqlalchemy import DDL, Column, Integer, create_engine
 from sqlalchemy.exc import DatabaseError
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.ext.declarative import declarative_base, declared_attr
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import NullPool
 
 # from sqlalchemy.schema import CreateSchema  # does not work for SA 1.4
 
 
-ModelBase = declarative_base()
+class Base:
+    """Base class which provides automated table name
+    and surrogate primary key column.
+
+    """
+
+    @declared_attr
+    def __tablename__(cls):
+        return f"{cls.__name__.lower()}"
+
+    id = Column(Integer, primary_key=True)
+
+    __table_args__ = {
+        'sqlite_autoincrement': True,
+        'schema': 'celery_schema'
+    }
+
+
+ModelBase = declarative_base(cls=Base)
 PREPARE_MODELS_MAX_RETRIES = 10
 
 
 @contextmanager
 def session_cleanup(session):
     try:
         yield
@@ -61,17 +79,17 @@
             return create_engine(dburi, poolclass=NullPool, **kwargs)
 
     def create_session(self, dburi, schema=None, short_lived_sessions=False, **kwargs):
         engine = self.get_engine(dburi, future=True, **kwargs)
         engine = engine.execution_options(schema_translate_map={'celery_schema': schema})
         if self.forked:
             if short_lived_sessions or dburi not in self._sessions:
-                self._sessions[dburi] = sessionmaker(bind=engine)
+                self._sessions[dburi] = sessionmaker(bind=engine, expire_on_commit=False)
             return engine, self._sessions[dburi]
-        return engine, sessionmaker(bind=engine)
+        return engine, sessionmaker(bind=engine, expire_on_commit=False)
 
     def prepare_models(self, engine, schema=None):
         if not self.prepared:
             # SQLAlchemy will check if the items exist before trying to
             # create them, which is a race condition. If it raises an error
             # in one iteration, the next may pass all the existence checks
             # and the call will succeed.
```

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.4.7
+Version: 0.5.0
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlalchemy-celery-beat
 
 A Scheduler Based Sqlalchemy for Celery.
 
-> NOTE: This project was originally developed by [AngelLiang](https://github.com/AngelLiang/celery-sqlalchemy-scheduler) to use sqlalchemy as the database scheduler, like [django-celery-beat](https://github.com/celery/django-celery-beat) for django. I am trying to continue on his work and maintain a working solution.
+> NOTE: This project was originally developed by [AngelLiang](https://github.com/AngelLiang/celery-sqlalchemy-scheduler) to use sqlalchemy as the database scheduler for Flask or FastAPI, like [django-celery-beat](https://github.com/celery/django-celery-beat) for django. I am trying to continue on his work and maintain a working solution.
 
 
 ### Prerequisites
 
 - Python 3
 - celery >= 5.0
 - sqlalchemy >= 1.4
@@ -171,15 +171,15 @@
     then they should all point to the same schedule object.
 
 Now that we have defined the schedule object, we can create the periodic task
 entry:
 
 ```python
     >>> task = PeriodicTask(
-    ...     interval=schedule,                  # we created this above.
+    ...     schedule_model=schedule,            # we created this above.
     ...     name='Importing contacts',          # simply describes this periodic task.
     ...     task='proj.tasks.import_contacts',  # name of task.
     ... )
     >>> session.add(task)
     >>> session.commit()
 ```
 
@@ -190,15 +190,15 @@
 Here\'s an example specifying the arguments, note how JSON serialization
 is required:
 
     >>> import json
     >>> from datetime import datetime, timedelta
 
     >>> periodic_task = PeriodicTask(
-    ...     interval=schedule,                  # we created this above.
+    ...     schedule_model=schedule,                  # we created this above.
     ...     name='Importing contacts',          # simply describes this periodic task.
     ...     task='proj.tasks.import_contacts',  # name of task.
     ...     args=json.dumps(['arg1', 'arg2']),
     ...     kwargs=json.dumps({
     ...        'be_careful': True,
     ...     }),
     ...     expires=datetime.utcnow() + timedelta(seconds=30)
@@ -223,23 +223,31 @@
     ... )
 
 The crontab schedule is linked to a specific timezone using the
 'timezone' input parameter.
 
 Then to create a periodic task using this schedule, use the same
 approach as the interval-based periodic task earlier in this document,
-but instead of `interval=schedule`, specify `crontab=schedule`:
+the `schedule_model` is a generic foreign-key implementation which makes things very easy and efficient:
 
     >>> periodic_task = PeriodicTask(
-    ...     crontab=schedule,
+    ...     schedule_model=schedule,
     ...     name='Importing contacts',
     ...     task='proj.tasks.import_contacts',
     ... )
-    ... session.add(periodic_task)
-    ... session.commit()
+
+What the previous code actually do is this:
+
+    >>> periodic_task = PeriodicTask(
+    ...     schedule_id=schedule.id,
+    ...     discriminator=schedule.discriminator,
+    ...     name='Importing contacts',
+    ...     task='proj.tasks.import_contacts',
+    ... )
+So when you can use `discriminator` + `schedule_id` or use the convenient property `schedule_model` and it will populate them for you behind the scenes.
 
 ### Temporarily disable a periodic task
 
 You can use the `enabled` flag to temporarily disable a periodic task:
 
     >>> periodic_task.enabled = False
     >>> session.add(periodic_task)
@@ -251,19 +259,19 @@
 ``` python
 from sqlalchemy_celery_beat.models import PeriodicTaskChanged
 
 session = get_beat_session()
 
 stmt = update(PeriodicTask).where(PeriodicTask.name == 'task-123').values(enabled=False)
 
-session.execute(stmt)
-session.commit()  # changes are not in the database but the schduler has no idea
+session.execute(stmt)  # using execute causes no orm event to fire, changes are in the database but the schduler has no idea
+session.commit()
 
 PeriodicTaskChanged.update_from_session(session)
-# now schduler reloads the tasks and all is good
+# now scheduler reloads the tasks and all is good
 ```
 This is not needed when you are updating a specific object using `session.add(task)` because it will trigger the `after_update`, `after_delete` or `after_insert` events.
 
 ### Example running periodic tasks
 
 The periodic tasks still need 'workers' to execute them. So make sure
 the default **Celery** package is installed. (If not installed, please
@@ -280,19 +288,21 @@
     scheduler):
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
+- ✅ Implement a generic foreign key
 - More robust attribute validation on models
 - Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
-Any help is appreciated 🙂
+Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
 
 - [django-celery-beat](https://github.com/celery/django-celery-beat)
 - [celerybeatredis](https://github.com/liuliqiang/celerybeatredis)
 - [celery](https://github.com/celery/celery)
+- [SQLAlchemy](https://www.sqlalchemy.org)
```

### Comparing `sqlalchemy_celery_beat-0.4.7/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.5.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

