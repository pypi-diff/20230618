# Comparing `tmp/django-formset-1.0.dev4.tar.gz` & `tmp/django-formset-1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formset-1.0.dev4.tar", last modified: Tue Jun 13 15:44:47 2023, max compression
+gzip compressed data, was "django-formset-1.0.dev5.tar", last modified: Tue Jun 13 21:48:08 2023, max compression
```

## Comparing `django-formset-1.0.dev4.tar` & `django-formset-1.0.dev5.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.719149 django-formset-1.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.675145 django-formset-1.0.dev4/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 15:44:47.000000 django-formset-1.0.dev4/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-13 15:44:39.000000 django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.679145 django-formset-1.0.dev4/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.683146 django-formset-1.0.dev4/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-13 15:44:35.000000 django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 15:44:35.000000 django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 15:44:36.000000 django-formset-1.0.dev4/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 15:44:36.000000 django-formset-1.0.dev4/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-13 15:44:37.000000 django-formset-1.0.dev4/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.683146 django-formset-1.0.dev4/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.687146 django-formset-1.0.dev4/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DateTimePicker-BBOUOZRC.js
--rw-r--r--   0 runner    (1001) docker     (123)    55693 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DjangoSelectize-OIQWF5I5.js
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DjangoSlug-226MVQ6E.js
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/DualSelector-2ALH4RIS.js
--rw-r--r--   0 runner    (1001) docker     (123)   316874 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/RichtextArea-XKK27UIM.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/SortableSelect-CEPX3LH6.js
--rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-APVD22ED.js
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-EJ4RWPXK.js
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-ISEEQP4V.js
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-KDP4ZIAK.js
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-MD4VW33H.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-NLMHZ7JJ.js
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/chunk-R2VNGMYE.js
--rw-r--r--   0 runner    (1001) docker     (123)   105257 2023-06-13 15:44:38.000000 django-formset-1.0.dev4/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.687146 django-formset-1.0.dev4/formset/static/formset/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/scss/bootstrap5-extra.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/static/formset/scss/collections.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.671145 django-formset-1.0.dev4/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.687146 django-formset-1.0.dev4/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.691146 django-formset-1.0.dev4/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.695147 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.695147 django-formset-1.0.dev4/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.695147 django-formset-1.0.dev4/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_separator.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/dialog_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/datetimepicker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.699147 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.711148 django-formset-1.0.dev4/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:44:47.715149 django-formset-1.0.dev4/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:44:47.719149 django-formset-1.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 15:43:49.000000 django-formset-1.0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:48:07.000000 django-formset-1.0.dev5/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.119449 django-formset-1.0.dev5/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.119449 django-formset-1.0.dev5/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.119449 django-formset-1.0.dev5/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-13 21:47:59.000000 django-formset-1.0.dev5/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DateTimePicker-TF2GNHHS.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55693 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DjangoSelectize-W4FTVNOW.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DjangoSlug-226MVQ6E.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DualSelector-ZVBIRYKG.js
+-rw-r--r--   0 runner    (1001) docker     (123)   316874 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/RichtextArea-YV4E7SHM.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/SortableSelect-MAAIASIY.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-APVD22ED.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-ISEEQP4V.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-KDP4ZIAK.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-MD4VW33H.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-NLMHZ7JJ.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-R2VNGMYE.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-USKSTMSP.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105257 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/static/formset/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/scss/bootstrap5-extra.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/scss/collections.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_separator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/dialog_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/datetimepicker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.143449 django-formset-1.0.dev5/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/setup.py
```

### Comparing `django-formset-1.0.dev4/LICENSE` & `django-formset-1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/PKG-INFO` & `django-formset-1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev4
+Version: 1.0.dev5
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev4/README.md` & `django-formset-1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/django_formset.egg-info/PKG-INFO` & `django-formset-1.0.dev5/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev4
+Version: 1.0.dev5
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django-formset-1.0.dev4/django_formset.egg-info/SOURCES.txt` & `django-formset-1.0.dev5/django_formset.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/DateTimePicker-BBOUOZRC.js
-formset/static/formset/js/DjangoSelectize-OIQWF5I5.js
+formset/static/formset/js/DateTimePicker-TF2GNHHS.js
+formset/static/formset/js/DjangoSelectize-W4FTVNOW.js
 formset/static/formset/js/DjangoSlug-226MVQ6E.js
-formset/static/formset/js/DualSelector-2ALH4RIS.js
-formset/static/formset/js/RichtextArea-XKK27UIM.js
-formset/static/formset/js/SortableSelect-CEPX3LH6.js
+formset/static/formset/js/DualSelector-ZVBIRYKG.js
+formset/static/formset/js/RichtextArea-YV4E7SHM.js
+formset/static/formset/js/SortableSelect-MAAIASIY.js
 formset/static/formset/js/chunk-APVD22ED.js
-formset/static/formset/js/chunk-EJ4RWPXK.js
 formset/static/formset/js/chunk-ISEEQP4V.js
 formset/static/formset/js/chunk-KDP4ZIAK.js
 formset/static/formset/js/chunk-MD4VW33H.js
 formset/static/formset/js/chunk-NLMHZ7JJ.js
 formset/static/formset/js/chunk-R2VNGMYE.js
+formset/static/formset/js/chunk-USKSTMSP.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/scss/bootstrap5-extra.scss
 formset/static/formset/scss/collections.scss
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
 formset/templates/calendar/months.html
 formset/templates/calendar/weeks.html
```

### Comparing `django-formset-1.0.dev4/formset/boundfield.py` & `django-formset-1.0.dev5/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/calendar.py` & `django-formset-1.0.dev5/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/collection.py` & `django-formset-1.0.dev5/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/fields.py` & `django-formset-1.0.dev5/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/fieldset.py` & `django-formset-1.0.dev5/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.mo` & `django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/locale/de/LC_MESSAGES/django.po` & `django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/renderers/bootstrap.py` & `django-formset-1.0.dev5/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/renderers/bulma.py` & `django-formset-1.0.dev5/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/renderers/default.py` & `django-formset-1.0.dev5/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/renderers/foundation.py` & `django-formset-1.0.dev5/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/renderers/tailwind.py` & `django-formset-1.0.dev5/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/renderers/uikit.py` & `django-formset-1.0.dev5/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/richtext/controls.py` & `django-formset-1.0.dev5/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/richtext/dialogs.py` & `django-formset-1.0.dev5/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/richtext/widgets.py` & `django-formset-1.0.dev5/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css` & `django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/css/bootstrap5-extra.css.map` & `django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/css/collections.css` & `django-formset-1.0.dev5/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/css/tailwind.css` & `django-formset-1.0.dev5/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-audio.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-empty.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-font.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-missing.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-pdf.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-picture.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-unknown.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-video.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/icons/file-zip.svg` & `django-formset-1.0.dev5/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/DateTimePicker-BBOUOZRC.js` & `django-formset-1.0.dev5/formset/static/formset/js/DateTimePicker-TF2GNHHS.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/DjangoSelectize-OIQWF5I5.js` & `django-formset-1.0.dev5/formset/static/formset/js/DjangoSelectize-W4FTVNOW.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/DjangoSlug-226MVQ6E.js` & `django-formset-1.0.dev5/formset/static/formset/js/DjangoSlug-226MVQ6E.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/DualSelector-2ALH4RIS.js` & `django-formset-1.0.dev5/formset/static/formset/js/DualSelector-ZVBIRYKG.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-MD4VW33H.js";
 import {
     a as u,
     b as p
-} from "./chunk-EJ4RWPXK.js";
+} from "./chunk-USKSTMSP.js";
 import "./chunk-APVD22ED.js";
 import {
     a as g
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as r
 } from "./chunk-R2VNGMYE.js";
```

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/RichtextArea-XKK27UIM.js` & `django-formset-1.0.dev5/formset/static/formset/js/RichtextArea-YV4E7SHM.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-APVD22ED.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-APVD22ED.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-EJ4RWPXK.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-USKSTMSP.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-ISEEQP4V.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-ISEEQP4V.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-KDP4ZIAK.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-KDP4ZIAK.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-MD4VW33H.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-MD4VW33H.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-NLMHZ7JJ.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-NLMHZ7JJ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/chunk-R2VNGMYE.js` & `django-formset-1.0.dev5/formset/static/formset/js/chunk-R2VNGMYE.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/js/django-formset.js` & `django-formset-1.0.dev5/formset/static/formset/js/django-formset.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3173,43 +3173,43 @@
 
     function n(s, u, f, d = void 0) {
         customElements.get(u) instanceof Function ? s() : (window.customElements.define(u, f, d), window.customElements.whenDefined(u).then(() => s()))
     }
 
     function i(s) {
         s.querySelector('select[is="django-selectize"]') && r.push(new Promise((u, f) => {
-            import("./DjangoSelectize-OIQWF5I5.js").then(({
+            import("./DjangoSelectize-W4FTVNOW.js").then(({
                 DjangoSelectizeElement: d
             }) => {
                 n(u, "django-selectize", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector("django-sortable-select") ? r.push(new Promise((u, f) => {
-            import("./SortableSelect-CEPX3LH6.js").then(({
+            import("./SortableSelect-MAAIASIY.js").then(({
                 SortableSelectElement: d
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-2ALH4RIS.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-ZVBIRYKG.js").then(({
                     DualSelectorElement: h
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? u() : (window.customElements.define("django-dual-selector", h, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => u()))
                 }).catch(h => f(h))
             }).catch(d => f(d))
         })) : s.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((u, f) => {
-            import("./DualSelector-2ALH4RIS.js").then(({
+            import("./DualSelector-ZVBIRYKG.js").then(({
                 DualSelectorElement: d
             }) => {
                 n(u, "django-dual-selector", d, {
                     extends: "select"
                 })
             }).catch(d => f(d))
         })), s.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((u, f) => {
-            import("./RichtextArea-XKK27UIM.js").then(({
+            import("./RichtextArea-YV4E7SHM.js").then(({
                 RichTextAreaElement: d
             }) => {
                 n(u, "django-richtext", d, {
                     extends: "textarea"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-slug"]') && r.push(new Promise((u, f) => {
@@ -3217,23 +3217,23 @@
                 DjangoSlugElement: d
             }) => {
                 n(u, "django-slug", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-BBOUOZRC.js").then(({
+            import("./DateTimePicker-TF2GNHHS.js").then(({
                 DatePickerElement: d
             }) => {
                 n(u, "django-datepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         })), s.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-BBOUOZRC.js").then(({
+            import("./DateTimePicker-TF2GNHHS.js").then(({
                 DateTimePickerElement: d
             }) => {
                 n(u, "django-datetimepicker", d, {
                     extends: "input"
                 })
             }).catch(d => f(d))
         }))
```

### Comparing `django-formset-1.0.dev4/formset/static/formset/scss/bootstrap5-extra.scss` & `django-formset-1.0.dev5/formset/static/formset/scss/bootstrap5-extra.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/static/formset/scss/collections.scss` & `django-formset-1.0.dev5/formset/static/formset/scss/collections.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/calendar/hours.html` & `django-formset-1.0.dev5/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/calendar/months.html` & `django-formset-1.0.dev5/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/calendar/weeks.html` & `django-formset-1.0.dev5/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/calendar/years.html` & `django-formset-1.0.dev5/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/bootstrap/widgets/file.html` & `django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/dual_selector.html` & `django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/bulma/widgets/file.html` & `django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_align.html` & `django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_align.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_color.html` & `django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_color.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/buttons/richtext_heading.html` & `django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_heading.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/collection.html` & `django-formset-1.0.dev5/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/dialog_form.html` & `django-formset-1.0.dev5/formset/templates/formset/default/dialog_form.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/fieldset.html` & `django-formset-1.0.dev5/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/widgets/dual_selector.html` & `django-formset-1.0.dev5/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/widgets/file.html` & `django-formset-1.0.dev5/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/default/widgets/selectize.html` & `django-formset-1.0.dev5/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/dual_selector.html` & `django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/foundation/widgets/file.html` & `django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/icons/blockquote.svg` & `django-formset-1.0.dev5/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/icons/letters.svg` & `django-formset-1.0.dev5/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/icons/placeholder.svg` & `django-formset-1.0.dev5/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/icons/questionmark.svg` & `django-formset-1.0.dev5/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/icons/subscript.svg` & `django-formset-1.0.dev5/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/icons/unlink.svg` & `django-formset-1.0.dev5/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/tailwind/widgets/file.html` & `django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templates/formset/uikit/widgets/file.html` & `django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templatetags/formsetify.py` & `django-formset-1.0.dev5/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/templatetags/richtext.py` & `django-formset-1.0.dev5/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/upload.py` & `django-formset-1.0.dev5/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/utils.py` & `django-formset-1.0.dev5/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/views.py` & `django-formset-1.0.dev5/formset/views.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev4/formset/widgets.py` & `django-formset-1.0.dev5/formset/widgets.py`

 * *Files 9% similar despite different names*

```diff
@@ -121,30 +121,32 @@
     def _optgroups_static_choice(self, name, values, attrs=None):
         optgroups = super().optgroups(name, values, attrs)
         return optgroups
 
     def _options_model_choice(self, name, values, attrs=None):
         values_list = [str(val) for val in values]
         optgroups, counter = [], 0
-        for counter, (val, label) in enumerate(self.choices, counter):
+        for val, label in self.choices:
             if counter == self.max_prefetch_choices:
                 break
             if not isinstance(val, ModelChoiceIteratorValue):
                 continue
             val = str(val)
             if selected := val in values_list:
                 values_list.remove(val)
             optgroups.append((None, [{'value': val, 'label': label, 'selected': selected}], counter))
-        for counter, val in enumerate(values_list, counter):
+            counter += 1
+        for val in values_list:
             try:
                 obj = self.choices.queryset.get(pk=val)
             except ObjectDoesNotExist:
                 continue
             label = self.choices.field.label_from_instance(obj)
             optgroups.append((None, [{'value': str(val), 'label': label, 'selected': True}], counter))
+            counter += 1
         return optgroups
 
     def _optgroups_model_choice(self, name, values, attrs=None):
         values_list = [str(val) for val in values]
         optgroups, prev_group_name, counter = [], '-', 0
         # first handle selected values
         for counter, val in enumerate(values_list, counter):
@@ -236,14 +238,38 @@
     """
     Render widget suitable for the <select is="django-dual-sortable-selector"> widget
     """
     def get_context(self, name, value, attrs):
         context = super().get_context(name, value, attrs)
         context['is_sortable'] = True
         return context
+    def _options_model_choice(self, name, values, attrs=None):
+        values_list = [str(val) for val in values]
+        optgroups, counter = [], 0
+        # first create options from values_list, otherwise order is lost
+        for val in values_list:
+            try:
+                obj = self.choices.queryset.get(pk=val)
+            except ObjectDoesNotExist:
+                continue
+            label = self.choices.field.label_from_instance(obj)
+            optgroups.append((None, [{'value': str(val), 'label': label, 'selected': True}], counter))
+            counter += 1
+        # then add remaining options up to max_prefetch_choices
+        for val, label in self.choices:
+            if counter >= self.max_prefetch_choices:
+                break
+            if not isinstance(val, ModelChoiceIteratorValue):
+                continue
+            val = str(val)
+            if val in values_list:
+                continue
+            optgroups.append((None, [{'value': val, 'label': label, 'selected': False}], counter))
+            counter += 1
+        return optgroups
 
 
 class SlugInput(TextInput):
     def __init__(self, populate_from, attrs=None):
         super().__init__(attrs)
         self.attrs.update({
             'is': 'django-slug',
```

### Comparing `django-formset-1.0.dev4/setup.py` & `django-formset-1.0.dev5/setup.py`

 * *Files identical despite different names*

