# Comparing `tmp/django-timezone-field-5.0.tar.gz` & `tmp/django_timezone_field-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-timezone-field-5.0.tar", max compression
+gzip compressed data, was "django_timezone_field-5.1.tar", max compression
```

## Comparing `django-timezone-field-5.0.tar` & `django_timezone_field-5.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1333 2021-12-15 23:09:11.452042 django-timezone-field-5.0/LICENSE.txt
--rw-r--r--   0        0        0     8914 2022-02-09 04:43:12.331560 django-timezone-field-5.0/README.md
--rw-r--r--   0        0        0     1669 2022-02-09 04:42:10.315074 django-timezone-field-5.0/pyproject.toml
--rw-r--r--   0        0        0      169 2022-02-09 04:42:10.318956 django-timezone-field-5.0/timezone_field/__init__.py
--rw-r--r--   0        0        0     1732 2022-02-09 04:42:10.319373 django-timezone-field-5.0/timezone_field/choices.py
--rw-r--r--   0        0        0      196 2022-02-09 04:42:10.319596 django-timezone-field-5.0/timezone_field/compat.py
--rw-r--r--   0        0        0     7025 2022-02-09 04:42:10.320012 django-timezone-field-5.0/timezone_field/fields.py
--rw-r--r--   0        0        0     1680 2022-02-09 04:42:10.320454 django-timezone-field-5.0/timezone_field/forms.py
--rw-r--r--   0        0        0       27 2022-02-02 00:50:42.689914 django-timezone-field-5.0/timezone_field/models.py
--rw-r--r--   0        0        0      997 2022-02-09 04:42:10.320689 django-timezone-field-5.0/timezone_field/rest_framework.py
--rw-r--r--   0        0        0      251 2022-02-09 04:42:10.320993 django-timezone-field-5.0/timezone_field/utils.py
--rw-r--r--   0        0        0     9993 2022-02-09 04:47:13.282881 django-timezone-field-5.0/setup.py
--rw-r--r--   0        0        0    10110 2022-02-09 04:47:13.283281 django-timezone-field-5.0/PKG-INFO
+-rw-r--r--   0        0        0     1333 2022-10-11 00:56:56.030619 django_timezone_field-5.1/LICENSE.txt
+-rw-r--r--   0        0        0     9891 2023-06-18 21:37:51.423764 django_timezone_field-5.1/README.md
+-rw-r--r--   0        0        0     1651 2023-06-18 21:53:21.933345 django_timezone_field-5.1/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-18 21:37:59.717777 django_timezone_field-5.1/timezone_field/__init__.py
+-rw-r--r--   0        0        0     1732 2022-10-11 00:56:56.033009 django_timezone_field-5.1/timezone_field/choices.py
+-rw-r--r--   0        0        0      196 2022-10-11 00:56:56.033107 django_timezone_field-5.1/timezone_field/compat.py
+-rw-r--r--   0        0        0     7580 2023-06-18 19:35:44.495576 django_timezone_field-5.1/timezone_field/fields.py
+-rw-r--r--   0        0        0     1680 2022-10-11 00:56:56.033358 django_timezone_field-5.1/timezone_field/forms.py
+-rw-r--r--   0        0        0       27 2022-10-11 00:56:56.033475 django_timezone_field-5.1/timezone_field/models.py
+-rw-r--r--   0        0        0     1076 2023-06-18 20:50:54.942962 django_timezone_field-5.1/timezone_field/rest_framework.py
+-rw-r--r--   0        0        0      251 2022-10-11 00:56:56.033721 django_timezone_field-5.1/timezone_field/utils.py
+-rw-r--r--   0        0        0    11268 1970-01-01 00:00:00.000000 django_timezone_field-5.1/PKG-INFO
```

### Comparing `django-timezone-field-5.0/LICENSE.txt` & `django_timezone_field-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-timezone-field-5.0/README.md` & `django_timezone_field-5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,31 @@
 - Django == 4.X: `use_pytz` defaults to the value of
   [`django.conf.settings.USE_DEPRECATED_PYTZ`](https://docs.djangoproject.com/en/4.0/ref/settings/#use-deprecated-pytz),
   which itself defaults to `False`
 - Django >= 5.X: django plans to
   [drop support for `pytz` altogether](https://docs.djangoproject.com/en/4.0/releases/4.0/#zoneinfo-default-timezone-implementation),
   and this app will likely do the same.
 
-When switching between `pytz` and `zoneinfo`, in general a
-[data migration](https://docs.djangoproject.com/en/4.0/topics/migrations/#data-migrations) is _not_ needed, as both
-libraries recognize the same set of strings as valid timezones. Exceptions to that include if your local system has an
-unusual set of time zones installed, or if you are using the `Factory` timezone which `zoneinfo` recognizes but `pytz`
-does not.
+### Differences in recognized timezones between `pytz` and `zoneinfo`
+
+`pytz` and `zoneinfo` search for timezone data differently.
+
+- `pytz` bundles and searches within its own copy of the [IANA timezone DB](https://www.iana.org/time-zones)
+- `zoneinfo` first searches the local system's timezone DB for a match. If no match is found, it then searches within
+  the [`tzdata`](https://pypi.org/project/tzdata/) package if it is installed. The `tzdata` package contains a copy of
+  the IANA timezone DB.
+
+If the local system's timezone DB doesn't cover the entire IANA timezone DB and the `tzdata` package is not installed,
+you may run across errors like `ZoneInfoNotFoundError: 'No time zone found with key Pacific/Kanton'` for seemingly valid
+timezones when transitioning from `pytz` to `zoneinfo`. The easy fix is to add `tzdata` to your project with
+`poetry add tzdata` or `pip install tzdata`.
+
+Assuming you have the `tzdata` package installed if needed, no
+[data migration](https://docs.djangoproject.com/en/4.0/topics/migrations/#data-migrations) should be necessary when
+switching from `pytz` to `zoneinfo`.
 
 ## Examples
 
 ### Database Field
 
 ```python
 import zoneinfo
@@ -115,19 +127,26 @@
 ```bash
 poetry install
 poetry run pytest
 ```
 
 ## Changelog
 
+#### 5.1 (2023-06-18)
+
+- Add django as a dependency of this package, with correct version constraints
+  ([#90](https://github.com/mfogel/django-timezone-field/issues/90))
+- Add support for django 4.1, 4.2
+- Add support for python 3.11
+
 #### 5.0 (2022-02-08)
 
 - Add support for `zoneinfo` objects ([#79](https://github.com/mfogel/django-timezone-field/issues/79))
 - Add support for django 4.0
-- Remove `display_GMT_offset` kwarg (use `choices_display` instead)
+- Remove `timezone_field.utils.add_gmt_offset_to_choices`, `display_GMT_offset` kwarg (use `choices_display` instead)
 - Drop support for django 3.0, 3.1
 - Drop support for python 3.5, 3.6
 
 #### 4.2.3 (2022-01-13)
 
 - Fix sdist installs ([#78](https://github.com/mfogel/django-timezone-field/issues/78))
 - Officially support python 3.10
```

### Comparing `django-timezone-field-5.0/pyproject.toml` & `django_timezone_field-5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,57 +10,56 @@
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.poetry]
 name = "django-timezone-field"
-version = "5.0"
+version = "5.1"
 description = "A Django app providing DB, form, and REST framework fields for zoneinfo and pytz timezone objects."
 license = "BSD-2-Clause"
 authors = ["Mike Fogel <mike@fogel.ca>"]
 readme = "README.md"
 repository = "https://github.com/mfogel/django-timezone-field/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 packages = [
     { include = "timezone_field" },
 ]
 
 [tool.poetry.dependencies]
+Django = ">=2.2,<5.0,!=3.0.*,!=3.1.*"
 python = "^3.7"
 pytz = "*"
 "backports.zoneinfo" = { version = "^0.2.1", python = "<3.9" }
 
 [tool.poetry.dev-dependencies]
 coverage = {extras = ["toml"], version = "^6.2"}
-Django = [
-    { version = "^2.2 || ^3.2", python = "~3.7" },
-    { version = "^2.2 || ^3.2 || ^4.0", python = "^3.8" },
-]
 djangorestframework = "^3.13.1"
-flake8 = "^4.0.1"
+flake8 = "^5.0.4"
 psycopg2-binary = "^2.9.3"
 pytest = "^6.2.5"
 pytest-django = "^4.5.2"
 pytest-pythonpath = "^0.7.3"
 pytest-lazy-fixture = "^0.6.3"
 pytest-cov = "^3.0.0"
-black = "^21.12b0"
-isort = "^5.10.1"
-pylint = "^2.12.2"
+black = "^23.3.0"
+isort = "^5.11.5"
+pylint = "^2.13.9"
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 120
 disable = "C, R, redefined-outer-name"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.settings"
```

### Comparing `django-timezone-field-5.0/timezone_field/choices.py` & `django_timezone_field-5.1/timezone_field/choices.py`

 * *Files identical despite different names*

### Comparing `django-timezone-field-5.0/timezone_field/fields.py` & `django_timezone_field-5.1/timezone_field/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,41 @@
     """
 
     description = "A timezone object"
 
     # NOTE: these defaults are excluded from migrations. If these are changed,
     #       existing migration files will need to be accomodated.
     default_max_length = 63
-    default_pytz_tzs = [pytz.timezone(tz) for tz in pytz.common_timezones]
-    default_zoneinfo_tzs = [ZoneInfo(tz) for tz in pytz.common_timezones]
+
+    @staticmethod
+    def get_default_pytz_tzs():
+        return [pytz.timezone(tz) for tz in pytz.common_timezones]
+
+    @staticmethod
+    def get_default_zoneinfo_tzs():
+        default_zoneinfo_tzs = []
+        for tz in pytz.common_timezones:
+            try:
+                default_zoneinfo_tzs.append(ZoneInfo(tz))
+            except ZoneInfoNotFoundError:
+                # ZoneInfo does not yet exist for this timezone
+                pass
+        return default_zoneinfo_tzs
 
     def __init__(self, *args, **kwargs):
         # allow some use of positional args up until the args we customize
         # https://github.com/mfogel/django-timezone-field/issues/42
         # https://github.com/django/django/blob/1.11.11/django/db/models/fields/__init__.py#L145
         if len(args) > 3:
             raise ValueError("Cannot specify max_length by positional arg")
         kwargs.setdefault("max_length", self.default_max_length)
 
         self.use_pytz_explicit = kwargs.pop("use_pytz", None)
         self.use_pytz = self.use_pytz_explicit if self.use_pytz_explicit is not None else use_pytz_default()
-        self.default_tzs = self.default_pytz_tzs if self.use_pytz else self.default_zoneinfo_tzs
+        self.default_tzs = self.get_default_pytz_tzs() if self.use_pytz else self.get_default_zoneinfo_tzs()
 
         if "choices" in kwargs:
             values, displays = zip(*kwargs["choices"])
             # Choices can be specified in two forms: either
             # [<pytz.timezone>, <str>] or [<str>, <str>]
             #
             # The [<pytz.timezone>, <str>] format is the one we actually
@@ -99,29 +112,32 @@
 
         if self.use_pytz_explicit is not None:
             kwargs["use_pytz"] = self.use_pytz_explicit
 
         if self.choices_display is not None:
             kwargs["choices_display"] = self.choices_display
 
-        choices = kwargs["choices"]
-        if self.choices_display is None:
-            if choices == standard(self.default_tzs):
-                kwargs.pop("choices")
-        else:
-            values, _ = zip(*choices)
-            if sorted(values, key=str) == sorted(self.default_tzs, key=str):
-                kwargs.pop("choices")
+        # don't assume super().deconstruct() will pass us back our kwargs["choices"]
+        # https://github.com/mfogel/django-timezone-field/issues/96
+        if "choices" in kwargs:
+            if self.choices_display is None:
+                if kwargs["choices"] == standard(self.default_tzs):
+                    kwargs.pop("choices")
             else:
-                kwargs["choices"] = [(value, "") for value in values]
+                values, _ = zip(*kwargs["choices"])
+                if sorted(values, key=str) == sorted(self.default_tzs, key=str):
+                    kwargs.pop("choices")
+                else:
+                    kwargs["choices"] = [(value, "") for value in values]
 
         # django can't decontruct pytz objects, so transform choices
         # to [<str>, <str>] format for writing out to the migration
         if "choices" in kwargs:
             kwargs["choices"] = [(str(tz), n) for tz, n in kwargs["choices"]]
+
         return name, path, args, kwargs
 
     def get_internal_type(self):
         return "CharField"
 
     def get_default(self):
         # allow defaults to be still specified as strings. Allows for easy
```

### Comparing `django-timezone-field-5.0/timezone_field/forms.py` & `django_timezone_field-5.1/timezone_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-timezone-field-5.0/timezone_field/rest_framework.py` & `django_timezone_field-5.1/timezone_field/rest_framework.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,23 @@
     }
 
     def __init__(self, *args, **kwargs):
         self.use_pytz = kwargs.pop("use_pytz", use_pytz_default())
         super().__init__(*args, **kwargs)
 
     def to_internal_value(self, data):
+        data_str = force_str(data)
         if self.use_pytz:
             try:
-                return pytz.timezone(force_str(data))
+                return pytz.timezone(data_str)
             except pytz.UnknownTimeZoneError:
                 self.fail("invalid")
         else:
-            try:
-                return ZoneInfo(force_str(data))
-            except ZoneInfoNotFoundError:
-                self.fail("invalid")
+            if data_str:
+                try:
+                    return ZoneInfo(data_str)
+                except ZoneInfoNotFoundError:
+                    pass
+            self.fail("invalid")
 
     def to_representation(self, value):
         return str(value)
```

### Comparing `django-timezone-field-5.0/setup.py` & `django_timezone_field-5.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,273 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-timezone-field
+Version: 5.1
+Summary: A Django app providing DB, form, and REST framework fields for zoneinfo and pytz timezone objects.
+Home-page: https://github.com/mfogel/django-timezone-field/
+License: BSD-2-Clause
+Author: Mike Fogel
+Author-email: mike@fogel.ca
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: Django (>=2.2,<5.0,!=3.0.*,!=3.1.*)
+Requires-Dist: backports.zoneinfo (>=0.2.1,<0.3.0) ; python_version < "3.9"
+Requires-Dist: pytz
+Project-URL: Repository, https://github.com/mfogel/django-timezone-field/
+Description-Content-Type: text/markdown
 
-packages = \
-['timezone_field']
+# django-timezone-field
 
-package_data = \
-{'': ['*']}
+[![CI](https://github.com/mfogel/django-timezone-field/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/mfogel/django-timezone-field/actions)
+[![codecov](https://codecov.io/gh/mfogel/django-timezone-field/branch/main/graph/badge.svg?token=Rwekzmim3l)](https://codecov.io/gh/mfogel/django-timezone-field)
+[![pypi downloads](https://img.shields.io/pypi/dm/django-timezone-field.svg)](https://pypi.python.org/pypi/django-timezone-field/)
+[![pypi python support](https://img.shields.io/pypi/pyversions/django-timezone-field.svg)](https://pypi.python.org/pypi/django-timezone-field/)
+[![pypi django support](https://img.shields.io/pypi/djversions/django-timezone-field.svg)](https://pypi.python.org/pypi/django-timezone-field/)
 
-install_requires = \
-['pytz']
-
-extras_require = \
-{':python_version < "3.9"': ['backports.zoneinfo>=0.2.1,<0.3.0']}
-
-setup_kwargs = {
-    'name': 'django-timezone-field',
-    'version': '5.0',
-    'description': 'A Django app providing DB, form, and REST framework fields for zoneinfo and pytz timezone objects.',
-    'long_description': '# django-timezone-field\n\n[![CI](https://github.com/mfogel/django-timezone-field/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/mfogel/django-timezone-field/actions)\n[![codecov](https://codecov.io/gh/mfogel/django-timezone-field/branch/main/graph/badge.svg?token=Rwekzmim3l)](https://codecov.io/gh/mfogel/django-timezone-field)\n[![pypi downloads](https://img.shields.io/pypi/dm/django-timezone-field.svg)](https://pypi.python.org/pypi/django-timezone-field/)\n[![pypi python support](https://img.shields.io/pypi/pyversions/django-timezone-field.svg)](https://pypi.python.org/pypi/django-timezone-field/)\n[![pypi django support](https://img.shields.io/pypi/djversions/django-timezone-field.svg)](https://pypi.python.org/pypi/django-timezone-field/)\n\nA Django app providing DB, form, and REST framework fields for\n[`zoneinfo`](https://docs.python.org/3/library/zoneinfo.html) and [`pytz`](http://pypi.python.org/pypi/pytz/) timezone\nobjects.\n\n## The transition from `pytz` to `zoneinfo`\n\nLike Django, this app supports both `pytz` and `zoneinfo` objects while the community transitions away from `pytz` to\n`zoneinfo`. All exposed fields and functions that return a timezone object accept an optional boolean kwarg `use_pytz`.\n\nIf not explicitly specified, the default value used for `use_pytz` matches Django\'s behavior:\n\n- Django <= 3.X: `use_pytz` defaults to `True`\n- Django == 4.X: `use_pytz` defaults to the value of\n  [`django.conf.settings.USE_DEPRECATED_PYTZ`](https://docs.djangoproject.com/en/4.0/ref/settings/#use-deprecated-pytz),\n  which itself defaults to `False`\n- Django >= 5.X: django plans to\n  [drop support for `pytz` altogether](https://docs.djangoproject.com/en/4.0/releases/4.0/#zoneinfo-default-timezone-implementation),\n  and this app will likely do the same.\n\nWhen switching between `pytz` and `zoneinfo`, in general a\n[data migration](https://docs.djangoproject.com/en/4.0/topics/migrations/#data-migrations) is _not_ needed, as both\nlibraries recognize the same set of strings as valid timezones. Exceptions to that include if your local system has an\nunusual set of time zones installed, or if you are using the `Factory` timezone which `zoneinfo` recognizes but `pytz`\ndoes not.\n\n## Examples\n\n### Database Field\n\n```python\nimport zoneinfo\nimport pytz\nfrom django.db import models\nfrom timezone_field import TimeZoneField\n\nclass MyModel(models.Model):\n    tz1 = TimeZoneField(default="Asia/Dubai")               # defaults supported, in ModelForm renders like "Asia/Dubai"\n    tz2 = TimeZoneField(choices_display="WITH_GMT_OFFSET")  # in ModelForm renders like "GMT+04:00 Asia/Dubai"\n    tz3 = TimeZoneField(use_pytz=True)                      # returns pytz timezone objects\n    tz4 = TimeZoneField(use_pytz=False)                     # returns zoneinfo objects\n\nmy_model = MyModel(\n    tz2="America/Vancouver",                     # assignment of a string\n    tz3=pytz.timezone("America/Vancouver"),      # assignment of a pytz timezone\n    tz4=zoneinfo.ZoneInfo("America/Vancouver"),  # assignment of a zoneinfo\n)\nmy_model.full_clean() # validates against pytz.common_timezones by default\nmy_model.save()       # values stored in DB as strings\nmy_model.tz3          # value returned as pytz timezone: <DstTzInfo \'America/Vancouver\' LMT-1 day, 15:48:00 STD>\nmy_model.tz4          # value returned as zoneinfo: zoneinfo.ZoneInfo(key=\'America/Vancouver\')\n```\n\n### Form Field\n\n```python\nfrom django import forms\nfrom timezone_field import TimeZoneFormField\n\nclass MyForm(forms.Form):\n    tz1 = TimeZoneFormField()                                   # renders like "Asia/Dubai"\n    tz2 = TimeZoneFormField(choices_display="WITH_GMT_OFFSET")  # renders like "GMT+04:00 Asia/Dubai"\n    tz3 = TimeZoneFormField(use_pytz=True)                      # returns pytz timezone objects\n    tz4 = TimeZoneFormField(use_pytz=False)                     # returns zoneinfo objects\n\nmy_form = MyForm({"tz3": "Europe/Berlin", "tz4": "Europe/Berlin"})\nmy_form.full_clean()         # validates against pytz.common_timezones by default\nmy_form.cleaned_data["tz3"]  # value returned as pytz timezone: <DstTzInfo \'Europe/Berlin\' LMT+0:53:00 STD>\nmy_form.cleaned_data["tz4"]  # value returned as zoneinfo: zoneinfo.ZoneInfo(key=\'Europe/Berlin\')\n```\n\n### REST Framework Serializer Field\n\n```python\nfrom rest_framework import serializers\nfrom timezone_field.rest_framework import TimeZoneSerializerField\n\nclass MySerializer(serializers.Serializer):\n    tz1 = TimeZoneSerializerField(use_pytz=True)\n    tz2 = TimeZoneSerializerField(use_pytz=False)\n\nmy_serializer = MySerializer(data={\n    "tz1": "America/Argentina/Buenos_Aires",\n    "tz2": "America/Argentina/Buenos_Aires",\n})\nmy_serializer.is_valid()\nmy_serializer.validated_data["tz1"]  # <DstTzInfo \'America/Argentina/Buenos_Aires\' LMT-1 day, 20:06:00 STD>\nmy_serializer.validated_data["tz2"]  # zoneinfo.ZoneInfo(key=\'America/Argentina/Buenos_Aires\')\n```\n\n## Installation\n\nReleases are hosted on [`pypi`](https://pypi.org/project/django-timezone-field/) and can be installed using various\npython packaging tools.\n\n```bash\n# with poetry\npoetry add django-timezone-field\n\n# with pip\npip install django-timezone-field\n```\n\n## Running the tests\n\nFrom the repository root, with [`poetry`](https://python-poetry.org/):\n\n```bash\npoetry install\npoetry run pytest\n```\n\n## Changelog\n\n#### 5.0 (2022-02-08)\n\n- Add support for `zoneinfo` objects ([#79](https://github.com/mfogel/django-timezone-field/issues/79))\n- Add support for django 4.0\n- Remove `display_GMT_offset` kwarg (use `choices_display` instead)\n- Drop support for django 3.0, 3.1\n- Drop support for python 3.5, 3.6\n\n#### 4.2.3 (2022-01-13)\n\n- Fix sdist installs ([#78](https://github.com/mfogel/django-timezone-field/issues/78))\n- Officially support python 3.10\n\n#### 4.2.1 (2021-07-07)\n\n- Reinstate `TimeZoneField.default_choices` ([#76](https://github.com/mfogel/django-timezone-field/issues/76))\n\n#### 4.2 (2021-07-07)\n\n- Officially support django 3.2, python 3.9\n- Fix bug with field deconstruction ([#74](https://github.com/mfogel/django-timezone-field/issues/74))\n- Housekeeping: use poetry, github actions, pytest\n\n#### 4.1.2 (2021-03-17)\n\n- Avoid `NonExistentTimeError` during DST transition ([#70](https://github.com/mfogel/django-timezone-field/issues/70))\n\n#### 4.1.1 (2020-11-28)\n\n- Don\'t import `rest_framework` from package root ([#67](https://github.com/mfogel/django-timezone-field/issues/67))\n\n#### 4.1 (2020-11-28)\n\n- Add Django REST Framework serializer field\n- Add new `choices_display` kwarg with supported values `WITH_GMT_OFFSET` and `STANDARD`\n- Deprecate `display_GMT_offset` kwarg\n\n#### 4.0 (2019-12-03)\n\n- Add support for django 3.0, python 3.8\n- Drop support for django 1.11, 2.0, 2.1, python 2.7, 3.4\n\n#### 3.1 (2019-10-02)\n\n- Officially support django 2.2 (already worked)\n- Add option to display TZ offsets in form field ([#46](https://github.com/mfogel/django-timezone-field/issues/46))\n\n#### 3.0 (2018-09-15)\n\n- Support django 1.11, 2.0, 2.1\n- Add support for python 3.7\n- Change default human-readable timezone names to exclude underscores\n  ([#32](https://github.com/mfogel/django-timezone-field/issues/32) &\n  [#37](https://github.com/mfogel/django-timezone-field/issues/37))\n\n#### 2.1 (2018-03-01)\n\n- Add support for django 1.10, 1.11\n- Add support for python 3.6\n- Add wheel support\n- Support bytes in DB fields ([#38](https://github.com/mfogel/django-timezone-field/issues/38) &\n  [#39](https://github.com/mfogel/django-timezone-field/issues/39))\n\n#### 2.0 (2016-01-31)\n\n- Drop support for django 1.7, add support for django 1.9\n- Drop support for python 3.2, 3.3, add support for python 3.5\n- Remove tests from source distribution\n\n#### 1.3 (2015-10-12)\n\n- Drop support for django 1.6, add support for django 1.8\n- Various [bug fixes](https://github.com/mfogel/django-timezone-field/issues?q=milestone%3A1.3)\n\n#### 1.2 (2015-02-05)\n\n- For form field, changed default list of accepted timezones from `pytz.all_timezones` to `pytz.common_timezones`, to\n  match DB field behavior.\n\n#### 1.1 (2014-10-05)\n\n- Django 1.7 compatibility\n- Added support for formatting `choices` kwarg as `[[<str>, <str>], ...]`, in addition to previous format of\n  `[[<pytz.timezone>, <str>], ...]`.\n- Changed default list of accepted timezones from `pytz.all_timezones` to `pytz.common_timezones`. If you have timezones\n  in your DB that are in `pytz.all_timezones` but not in `pytz.common_timezones`, this is a backward-incompatible\n  change. Old behavior can be restored by specifying `choices=[(tz, tz) for tz in pytz.all_timezones]` in your model\n  definition.\n\n#### 1.0 (2013-08-04)\n\n- Initial release as `timezone_field`.\n\n## Credits\n\nOriginally adapted from [Brian Rosner\'s django-timezones](https://github.com/brosner/django-timezones).\n\nMade possible thanks to the work of the\n[contributors](https://github.com/mfogel/django-timezone-field/graphs/contributors).\n',
-    'author': 'Mike Fogel',
-    'author_email': 'mike@fogel.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mfogel/django-timezone-field/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+A Django app providing DB, form, and REST framework fields for
+[`zoneinfo`](https://docs.python.org/3/library/zoneinfo.html) and [`pytz`](http://pypi.python.org/pypi/pytz/) timezone
+objects.
 
+## The transition from `pytz` to `zoneinfo`
+
+Like Django, this app supports both `pytz` and `zoneinfo` objects while the community transitions away from `pytz` to
+`zoneinfo`. All exposed fields and functions that return a timezone object accept an optional boolean kwarg `use_pytz`.
+
+If not explicitly specified, the default value used for `use_pytz` matches Django's behavior:
+
+- Django <= 3.X: `use_pytz` defaults to `True`
+- Django == 4.X: `use_pytz` defaults to the value of
+  [`django.conf.settings.USE_DEPRECATED_PYTZ`](https://docs.djangoproject.com/en/4.0/ref/settings/#use-deprecated-pytz),
+  which itself defaults to `False`
+- Django >= 5.X: django plans to
+  [drop support for `pytz` altogether](https://docs.djangoproject.com/en/4.0/releases/4.0/#zoneinfo-default-timezone-implementation),
+  and this app will likely do the same.
+
+### Differences in recognized timezones between `pytz` and `zoneinfo`
+
+`pytz` and `zoneinfo` search for timezone data differently.
+
+- `pytz` bundles and searches within its own copy of the [IANA timezone DB](https://www.iana.org/time-zones)
+- `zoneinfo` first searches the local system's timezone DB for a match. If no match is found, it then searches within
+  the [`tzdata`](https://pypi.org/project/tzdata/) package if it is installed. The `tzdata` package contains a copy of
+  the IANA timezone DB.
+
+If the local system's timezone DB doesn't cover the entire IANA timezone DB and the `tzdata` package is not installed,
+you may run across errors like `ZoneInfoNotFoundError: 'No time zone found with key Pacific/Kanton'` for seemingly valid
+timezones when transitioning from `pytz` to `zoneinfo`. The easy fix is to add `tzdata` to your project with
+`poetry add tzdata` or `pip install tzdata`.
+
+Assuming you have the `tzdata` package installed if needed, no
+[data migration](https://docs.djangoproject.com/en/4.0/topics/migrations/#data-migrations) should be necessary when
+switching from `pytz` to `zoneinfo`.
+
+## Examples
+
+### Database Field
+
+```python
+import zoneinfo
+import pytz
+from django.db import models
+from timezone_field import TimeZoneField
+
+class MyModel(models.Model):
+    tz1 = TimeZoneField(default="Asia/Dubai")               # defaults supported, in ModelForm renders like "Asia/Dubai"
+    tz2 = TimeZoneField(choices_display="WITH_GMT_OFFSET")  # in ModelForm renders like "GMT+04:00 Asia/Dubai"
+    tz3 = TimeZoneField(use_pytz=True)                      # returns pytz timezone objects
+    tz4 = TimeZoneField(use_pytz=False)                     # returns zoneinfo objects
+
+my_model = MyModel(
+    tz2="America/Vancouver",                     # assignment of a string
+    tz3=pytz.timezone("America/Vancouver"),      # assignment of a pytz timezone
+    tz4=zoneinfo.ZoneInfo("America/Vancouver"),  # assignment of a zoneinfo
+)
+my_model.full_clean() # validates against pytz.common_timezones by default
+my_model.save()       # values stored in DB as strings
+my_model.tz3          # value returned as pytz timezone: <DstTzInfo 'America/Vancouver' LMT-1 day, 15:48:00 STD>
+my_model.tz4          # value returned as zoneinfo: zoneinfo.ZoneInfo(key='America/Vancouver')
+```
+
+### Form Field
+
+```python
+from django import forms
+from timezone_field import TimeZoneFormField
+
+class MyForm(forms.Form):
+    tz1 = TimeZoneFormField()                                   # renders like "Asia/Dubai"
+    tz2 = TimeZoneFormField(choices_display="WITH_GMT_OFFSET")  # renders like "GMT+04:00 Asia/Dubai"
+    tz3 = TimeZoneFormField(use_pytz=True)                      # returns pytz timezone objects
+    tz4 = TimeZoneFormField(use_pytz=False)                     # returns zoneinfo objects
+
+my_form = MyForm({"tz3": "Europe/Berlin", "tz4": "Europe/Berlin"})
+my_form.full_clean()         # validates against pytz.common_timezones by default
+my_form.cleaned_data["tz3"]  # value returned as pytz timezone: <DstTzInfo 'Europe/Berlin' LMT+0:53:00 STD>
+my_form.cleaned_data["tz4"]  # value returned as zoneinfo: zoneinfo.ZoneInfo(key='Europe/Berlin')
+```
+
+### REST Framework Serializer Field
+
+```python
+from rest_framework import serializers
+from timezone_field.rest_framework import TimeZoneSerializerField
+
+class MySerializer(serializers.Serializer):
+    tz1 = TimeZoneSerializerField(use_pytz=True)
+    tz2 = TimeZoneSerializerField(use_pytz=False)
+
+my_serializer = MySerializer(data={
+    "tz1": "America/Argentina/Buenos_Aires",
+    "tz2": "America/Argentina/Buenos_Aires",
+})
+my_serializer.is_valid()
+my_serializer.validated_data["tz1"]  # <DstTzInfo 'America/Argentina/Buenos_Aires' LMT-1 day, 20:06:00 STD>
+my_serializer.validated_data["tz2"]  # zoneinfo.ZoneInfo(key='America/Argentina/Buenos_Aires')
+```
+
+## Installation
+
+Releases are hosted on [`pypi`](https://pypi.org/project/django-timezone-field/) and can be installed using various
+python packaging tools.
+
+```bash
+# with poetry
+poetry add django-timezone-field
+
+# with pip
+pip install django-timezone-field
+```
+
+## Running the tests
+
+From the repository root, with [`poetry`](https://python-poetry.org/):
+
+```bash
+poetry install
+poetry run pytest
+```
+
+## Changelog
+
+#### 5.1 (2023-06-18)
+
+- Add django as a dependency of this package, with correct version constraints
+  ([#90](https://github.com/mfogel/django-timezone-field/issues/90))
+- Add support for django 4.1, 4.2
+- Add support for python 3.11
+
+#### 5.0 (2022-02-08)
+
+- Add support for `zoneinfo` objects ([#79](https://github.com/mfogel/django-timezone-field/issues/79))
+- Add support for django 4.0
+- Remove `timezone_field.utils.add_gmt_offset_to_choices`, `display_GMT_offset` kwarg (use `choices_display` instead)
+- Drop support for django 3.0, 3.1
+- Drop support for python 3.5, 3.6
+
+#### 4.2.3 (2022-01-13)
+
+- Fix sdist installs ([#78](https://github.com/mfogel/django-timezone-field/issues/78))
+- Officially support python 3.10
+
+#### 4.2.1 (2021-07-07)
+
+- Reinstate `TimeZoneField.default_choices` ([#76](https://github.com/mfogel/django-timezone-field/issues/76))
+
+#### 4.2 (2021-07-07)
+
+- Officially support django 3.2, python 3.9
+- Fix bug with field deconstruction ([#74](https://github.com/mfogel/django-timezone-field/issues/74))
+- Housekeeping: use poetry, github actions, pytest
+
+#### 4.1.2 (2021-03-17)
+
+- Avoid `NonExistentTimeError` during DST transition ([#70](https://github.com/mfogel/django-timezone-field/issues/70))
+
+#### 4.1.1 (2020-11-28)
+
+- Don't import `rest_framework` from package root ([#67](https://github.com/mfogel/django-timezone-field/issues/67))
+
+#### 4.1 (2020-11-28)
+
+- Add Django REST Framework serializer field
+- Add new `choices_display` kwarg with supported values `WITH_GMT_OFFSET` and `STANDARD`
+- Deprecate `display_GMT_offset` kwarg
+
+#### 4.0 (2019-12-03)
+
+- Add support for django 3.0, python 3.8
+- Drop support for django 1.11, 2.0, 2.1, python 2.7, 3.4
+
+#### 3.1 (2019-10-02)
+
+- Officially support django 2.2 (already worked)
+- Add option to display TZ offsets in form field ([#46](https://github.com/mfogel/django-timezone-field/issues/46))
+
+#### 3.0 (2018-09-15)
+
+- Support django 1.11, 2.0, 2.1
+- Add support for python 3.7
+- Change default human-readable timezone names to exclude underscores
+  ([#32](https://github.com/mfogel/django-timezone-field/issues/32) &
+  [#37](https://github.com/mfogel/django-timezone-field/issues/37))
+
+#### 2.1 (2018-03-01)
+
+- Add support for django 1.10, 1.11
+- Add support for python 3.6
+- Add wheel support
+- Support bytes in DB fields ([#38](https://github.com/mfogel/django-timezone-field/issues/38) &
+  [#39](https://github.com/mfogel/django-timezone-field/issues/39))
+
+#### 2.0 (2016-01-31)
+
+- Drop support for django 1.7, add support for django 1.9
+- Drop support for python 3.2, 3.3, add support for python 3.5
+- Remove tests from source distribution
+
+#### 1.3 (2015-10-12)
+
+- Drop support for django 1.6, add support for django 1.8
+- Various [bug fixes](https://github.com/mfogel/django-timezone-field/issues?q=milestone%3A1.3)
+
+#### 1.2 (2015-02-05)
+
+- For form field, changed default list of accepted timezones from `pytz.all_timezones` to `pytz.common_timezones`, to
+  match DB field behavior.
+
+#### 1.1 (2014-10-05)
+
+- Django 1.7 compatibility
+- Added support for formatting `choices` kwarg as `[[<str>, <str>], ...]`, in addition to previous format of
+  `[[<pytz.timezone>, <str>], ...]`.
+- Changed default list of accepted timezones from `pytz.all_timezones` to `pytz.common_timezones`. If you have timezones
+  in your DB that are in `pytz.all_timezones` but not in `pytz.common_timezones`, this is a backward-incompatible
+  change. Old behavior can be restored by specifying `choices=[(tz, tz) for tz in pytz.all_timezones]` in your model
+  definition.
+
+#### 1.0 (2013-08-04)
+
+- Initial release as `timezone_field`.
+
+## Credits
+
+Originally adapted from [Brian Rosner's django-timezones](https://github.com/brosner/django-timezones).
+
+Made possible thanks to the work of the
+[contributors](https://github.com/mfogel/django-timezone-field/graphs/contributors).
 
-setup(**setup_kwargs)
```

