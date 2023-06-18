# Comparing `tmp/cruiz-1.3.2b1.tar.gz` & `tmp/cruiz-1.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruiz-1.3.2b1.tar", last modified: Mon Dec 12 13:26:12 2022, max compression
+gzip compressed data, was "cruiz-1.4.0a1.tar", last modified: Sun Jun 18 19:35:41 2023, max compression
```

## Comparing `cruiz-1.3.2b1.tar` & `cruiz-1.4.0a1.tar`

### file list

```diff
@@ -1,235 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.220954 cruiz-1.3.2b1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       76 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2022-12-12 13:26:12.220954 cruiz-1.3.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.196954 cruiz-1.3.2b1/cruiz/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz/RELEASE_VERSION.py
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/__main_pyside2__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1828 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/application.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.196954 cruiz-1.3.2b1/cruiz/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      303 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/conanconf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1677 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/conanenv.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6322 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/conaninvocation.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    25516 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/context.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1731 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/guardedlisttoflush.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2401 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/logdetails.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4289 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/messagereplyprocessor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5721 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/commands/metarequestconaninvocation.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/dumpobjecttypes.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3843 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/environ.py
--rw-r--r--   0 runner    (1001) docker     (122)      531 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.200954 cruiz-1.3.2b1/cruiz/interop/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13930 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/commandparameters.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/commonparameters.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/packagebinaryparameters.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/packageidparameters.py
--rw-r--r--   0 runner    (1001) docker     (122)      934 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/packagenode.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/packagerevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/pod.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/reciperevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (122)      547 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/interop/searchrecipesparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.200954 cruiz-1.3.2b1/cruiz/load_recipe/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4801 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/loadrecipewizard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.200954 cruiz-1.3.2b1/cruiz/load_recipe/pages/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/pages/initialprofilepage.py
--rw-r--r--   0 runner    (1001) docker     (122)      304 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/pages/intropage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/pages/localcachepage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5504 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/load_recipe/pages/packageversionpage.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    28316 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.200954 cruiz-1.3.2b1/cruiz/manage_local_cache/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    34333 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/managelocalcachesdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.200954 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      592 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2541 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2635 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2729 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/addremotedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      759 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/configpathorurl.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3862 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/installconfigdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1902 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/keyvaluetable.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8043 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7209 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1877 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1683 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/progressdialogs.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4933 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/remotestable.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1258 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2179 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/runconancommanddialog.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.200954 cruiz-1.3.2b1/cruiz/model/
--rw-r--r--   0 runner    (1001) docker     (122)       53 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/model/conanpackagetypeflags.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2494 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/model/graphaslistmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/pyside2/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/pyside2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/pyside6/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/pyside6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/recipe/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1755 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/dependencyview.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1352 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/expressioneditordialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1682 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/findtextdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/recipe/logs/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/logs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5904 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/logs/command.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2234 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    58572 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/recipewidget.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/recipe/toolbars/
--rw-r--r--   0 runner    (1001) docker     (122)       54 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/toolbars/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6267 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/toolbars/behaviour.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10253 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/toolbars/buildfeatures.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    30694 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/recipe/toolbars/command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/remote_browser/
--rw-r--r--   0 runner    (1001) docker     (122)       53 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.204954 cruiz-1.3.2b1/cruiz/remote_browser/pages/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15268 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/packagebinarypage.py
--rw-r--r--   0 runner    (1001) docker     (122)    17650 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/packageidpage.py
--rw-r--r--   0 runner    (1001) docker     (122)     6957 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/packagereferencepage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5298 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/packagerevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2617 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     5160 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/pages/reciperevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3178 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/remote_browser/remotebrowser.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2484 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resourcegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.212954 cruiz-1.3.2b1/cruiz/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/001-rubbish.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1392 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/002-null.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/003-chemistry.svg
--rw-r--r--   0 runner    (1001) docker     (122)      539 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/004-share.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2426 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/005-box.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1992 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/006-toolbox.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/007-book.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/008-cloud-computing.svg
--rw-r--r--   0 runner    (1001) docker     (122)      907 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/009-import.svg
--rw-r--r--   0 runner    (1001) docker     (122)      838 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/010-draw.svg
--rw-r--r--   0 runner    (1001) docker     (122)     6784 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/012-hammer.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1594 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/013-pencil.svg
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/014-code.svg
--rw-r--r--   0 runner    (1001) docker     (122)    17753 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/Cmake.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2174 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/about_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/cruise.png
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/cruizres.qrc
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/find_text_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (122)    53573 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/license-cruise.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    96863 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/license.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     4622 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/load_recipe_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_add_environment.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3515 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_add_profile_directory.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3407 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_add_remote.ui
--rw-r--r--   0 runner    (1001) docker     (122)     7174 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_install_config.ui
--rw-r--r--   0 runner    (1001) docker     (122)    26699 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_manage.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2356 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_move.ui
--rw-r--r--   0 runner    (1001) docker     (122)     9594 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_new_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_remove_environment.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/local_cache_run_command_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (122)    40925 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/preferences.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_cmake_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2068 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_compilercache_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_cpucores_frame.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4377 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_local_workflow_expression_editor.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_profile_frame.ui
--rw-r--r--   0 runner    (1001) docker     (122)    33767 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/recipe_window.ui
--rw-r--r--   0 runner    (1001) docker     (122)    28688 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/remote_browser.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/resources/remote_browser_fileview.ui
--rw-r--r--   0 runner    (1001) docker     (122)      364 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/restart.py
--rw-r--r--   0 runner    (1001) docker     (122)     3843 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/revealonfilesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.212954 cruiz-1.3.2b1/cruiz/settings/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      582 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/ensuredefaultlocalcache.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.212954 cruiz-1.3.2b1/cruiz/settings/managers/
--rw-r--r--   0 runner    (1001) docker     (122)     1223 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10185 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/basesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4871 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/cleansettings.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1728 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/cmakepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3244 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/compilercachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2499 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/conanpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2309 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/fontpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6803 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/generalpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1890 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/graphvizpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3903 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/localcachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14295 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/namedlocalcache.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1830 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/ninjapreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3681 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/recentconanconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3590 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/recentconanremotes.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3564 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/recentrecipes.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    18314 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      317 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/restoredefaults.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7928 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/shortcuts.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1149 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/valueclasses.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4187 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/managers/writermixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.216954 cruiz-1.3.2b1/cruiz/settings/models/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1419 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/models/recentconanconfigmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1345 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/models/recentconanremotesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2751 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/models/recipesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    53673 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/preferencesdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14342 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/settings/updatesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6070 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/svggraph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1838 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.216954 cruiz-1.3.2b1/cruiz/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      240 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      986 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/widgets/aboutcruizdialog.py
--rw-r--r--   0 runner    (1001) docker     (122)    12371 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/widgets/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1387 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/widgets/shortcutlineedit.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2031 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.220954 cruiz-1.3.2b1/cruiz/workers/
--rw-r--r--   0 runner    (1001) docker     (122)       53 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      974 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/arbitrary.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      962 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/build.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2215 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/cmakebuildtool.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1577 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/configinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1222 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/create.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      895 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/deletecmakecache.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      325 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/endmessagethread.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1439 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/exportpackage.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      815 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/imports.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1366 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/install.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4826 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/lockcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    15174 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/meta.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      968 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/package.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1704 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/packagebinary.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      798 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/packagedetails.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      761 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/packagerevisions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      756 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/reciperevisions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2169 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/remotesearch.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      696 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/removeallpackages.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      506 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/removelocks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      967 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/removepackage.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      781 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/source.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1092 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/testpackage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.220954 cruiz-1.3.2b1/cruiz/workers/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/colorarma_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     5586 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/conanapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/formatoptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1783 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/message.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8233 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/monkeypatch.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1588 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/qtlogger.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/text2html.py
--rw-r--r--   0 runner    (1001) docker     (122)     5993 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/cruiz/workers/utils/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 13:26:12.196954 cruiz-1.3.2b1/cruiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3789 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7235 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      205 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-12 13:26:12.000000 cruiz-1.3.2b1/cruiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      143 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      200 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-12 13:26:12.220954 cruiz-1.3.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4653 2022-12-12 13:24:46.000000 cruiz-1.3.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.170604 cruiz-1.4.0a1/cruiz/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz/RELEASE_VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1828 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.174605 cruiz-1.4.0a1/cruiz/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/conanconf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1677 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/conanenv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/conaninvocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25506 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/guardedlisttoflush.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/logdetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4289 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/messagereplyprocessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5721 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/commands/metarequestconaninvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/dumpobjecttypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3769 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.174605 cruiz-1.4.0a1/cruiz/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/commandparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/commonparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packagebinaryparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packageidparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packagenode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/packagerevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/reciperevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/interop/searchrecipesparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.174605 cruiz-1.4.0a1/cruiz/load_recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/loadrecipewizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.178604 cruiz-1.4.0a1/cruiz/load_recipe/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/initialprofilepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/intropage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/localcachepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/load_recipe/pages/packageversionpage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28384 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.178604 cruiz-1.4.0a1/cruiz/manage_local_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34261 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/managelocalcachesdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.178604 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addremotedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/configpathorurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3695 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/installconfigdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/keyvaluetable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7891 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/progressdialogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/remotestable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2062 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/runconancommanddialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/model/conanpackagetypeflags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/model/graphaslistmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/pyside6/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/pyside6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/dependencyview.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/expressioneditordialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/findtextdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/recipe/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/logs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6110 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/logs/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58859 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/recipewidget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.182604 cruiz-1.4.0a1/cruiz/recipe/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6096 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/behaviour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/buildfeatures.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30694 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/recipe/toolbars/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.186604 cruiz-1.4.0a1/cruiz/remote_browser/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.186604 cruiz-1.4.0a1/cruiz/remote_browser/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packagebinarypage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packageidpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packagereferencepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/packagerevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/pages/reciperevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/remote_browser/remotebrowser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resourcegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.194604 cruiz-1.4.0a1/cruiz/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/001-rubbish.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/002-null.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/003-chemistry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/004-share.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/005-box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/006-toolbox.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/007-book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/008-cloud-computing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/009-import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/010-draw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/012-hammer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/013-pencil.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/014-code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/Cmake.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/about_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/cruise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/cruizres.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/find_text_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/license-cruise.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/license.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/load_recipe_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_add_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_add_profile_directory.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_add_remote.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_install_config.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    26699 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_manage.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_move.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_new_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_remove_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/local_cache_run_command_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/preferences.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_cmake_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_compilercache_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_cpucores_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_local_workflow_expression_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_profile_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/recipe_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/remote_browser.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/resources/remote_browser_fileview.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/revealonfilesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.194604 cruiz-1.4.0a1/cruiz/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/ensuredefaultlocalcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.202604 cruiz-1.4.0a1/cruiz/settings/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/basesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/cleansettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/cmakepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/compilercachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/conanpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/fontpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/generalpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/graphvizpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/localcachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/namedlocalcache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/ninjapreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recentconanconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recentconanremotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recentrecipes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18314 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/restoredefaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/shortcuts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/valueclasses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4187 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/managers/writermixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.202604 cruiz-1.4.0a1/cruiz/settings/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/recentconanconfigmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/recentconanremotesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2727 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/models/recipesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53761 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/preferencesdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14331 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/settings/updatesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/svggraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.202604 cruiz-1.4.0a1/cruiz/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/aboutcruizdialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/shortcutlineedit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/cruiz/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/arbitrary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2148 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/cmakebuildtool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/configinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/deletecmakecache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      325 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/endmessagethread.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1439 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/exportpackage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4826 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/lockcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15302 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/meta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      968 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/package.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/packagebinary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1339 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/packagedetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/packagerevisions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/reciperevisions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2169 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/remotesearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/removeallpackages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/removelocks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/removepackage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1092 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/testpackage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/cruiz/workers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/colorarma_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/conanapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/formatoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/message.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7679 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/monkeypatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/qtlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/text2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/cruiz/workers/utils/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:35:41.170604 cruiz-1.4.0a1/cruiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 19:35:41.000000 cruiz-1.4.0a1/cruiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 19:35:41.214604 cruiz-1.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-18 19:35:17.000000 cruiz-1.4.0a1/setup.py
```

### Comparing `cruiz-1.3.2b1/LICENSE` & `cruiz-1.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/PKG-INFO` & `cruiz-1.4.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.3.2b1
+Version: 1.4.0a1
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # cruiz
 
 Conan recipe user interface
 
-Written by Mark Final, (c) 2020-2022.
+Written by Mark Final.
 
 ![main action workflow](https://github.com/markfinal/cruiz/actions/workflows/main.yml/badge.svg)
 
 
 ## Documentation
 See the documentation at [Read The Docs](https://cruiz.readthedocs.io/).
 
@@ -36,15 +37,15 @@
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
   - macOS (10.13+)
 - Apple Silicon platforms:
   - macOS (11.0+)
-- Python 3.7-3.10
+- Python 3.7-3.11
 - Conan 1.17.1+, but not 2.x (these are the versions tested)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
 ## Getting started
@@ -66,29 +67,14 @@
 
 4. Run from any directory
 
     - From your Python environment shell, `cruiz` or `python -m cruiz`
 
 Step 3 will need to be re-run when the Python dependencies, or the resource files used, change.
 
-## PySide versions
-PySide2 and PySide6 have been tested. PySide6 is the default, when running `cruiz`. PySide2 is only available on Intel x86_64 platforms.
-
-On Linux, PySide 6 from PyPI requires modern libstdc++. If you see a launch error indicating `CXXABI_1.3.9` then your distribution is likely too old.
-
-You can alter the default PySide versiont to use, in a number of ways:
-
-1. Use a different entry point
-
-    - `cruiz-pyside2` or `python -m cruiz-pyside2`
-
-2. Use an environment variable
-
-    - `QT_API=pyside2 cruiz`
-
 ## Linting
 Install linting dependencies with `pip install -r requirements_dev.txt`.
 
 cruiz uses [tox](https://tox.wiki/en/latest/) to automate linting. Use `tox -e lint`.
 
 [flake8](https://flake8.pycqa.org/en/latest/) is used for lint checks, specifically using [black](https://black.readthedocs.io/en/stable/) as the formatter.
```

### Comparing `cruiz-1.3.2b1/README.md` & `cruiz-1.4.0a1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # cruiz
 
 Conan recipe user interface
 
-Written by Mark Final, (c) 2020-2022.
+Written by Mark Final.
 
 ![main action workflow](https://github.com/markfinal/cruiz/actions/workflows/main.yml/badge.svg)
 
 
 ## Documentation
 See the documentation at [Read The Docs](https://cruiz.readthedocs.io/).
 
@@ -14,15 +14,15 @@
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
   - macOS (10.13+)
 - Apple Silicon platforms:
   - macOS (11.0+)
-- Python 3.7-3.10
+- Python 3.7-3.11
 - Conan 1.17.1+, but not 2.x (these are the versions tested)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
 ## Getting started
@@ -44,29 +44,14 @@
 
 4. Run from any directory
 
     - From your Python environment shell, `cruiz` or `python -m cruiz`
 
 Step 3 will need to be re-run when the Python dependencies, or the resource files used, change.
 
-## PySide versions
-PySide2 and PySide6 have been tested. PySide6 is the default, when running `cruiz`. PySide2 is only available on Intel x86_64 platforms.
-
-On Linux, PySide 6 from PyPI requires modern libstdc++. If you see a launch error indicating `CXXABI_1.3.9` then your distribution is likely too old.
-
-You can alter the default PySide versiont to use, in a number of ways:
-
-1. Use a different entry point
-
-    - `cruiz-pyside2` or `python -m cruiz-pyside2`
-
-2. Use an environment variable
-
-    - `QT_API=pyside2 cruiz`
-
 ## Linting
 Install linting dependencies with `pip install -r requirements_dev.txt`.
 
 cruiz uses [tox](https://tox.wiki/en/latest/) to automate linting. Use `tox -e lint`.
 
 [flake8](https://flake8.pycqa.org/en/latest/) is used for lint checks, specifically using [black](https://black.readthedocs.io/en/stable/) as the formatter.
```

### Comparing `cruiz-1.3.2b1/cruiz/application.py` & `cruiz-1.4.0a1/cruiz/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def on_preferences_updated(self) -> None:
         """
         Slot executed when preferences have reported an update.
         """
         with GeneralSettingsReader() as settings:
             use_dark_mode = settings.use_dark_mode.resolve()
         self.setStyleSheet(
-            qdarkstyle.load_stylesheet_pyside2() if use_dark_mode else ""
+            qdarkstyle.load_stylesheet_pyside6() if use_dark_mode else ""
         )
         with FontSettingsReader(FontUsage.UI) as settings:
             font_details = (settings.name.resolve(), settings.size.resolve())
         if font_details[0]:
             self.setFont(QtGui.QFont(*font_details))
         else:
             self.setFont(self.default_font)
```

### Comparing `cruiz-1.3.2b1/cruiz/commands/conanenv.py` & `cruiz-1.4.0a1/cruiz/commands/conanenv.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/commands/conaninvocation.py` & `cruiz-1.4.0a1/cruiz/commands/conaninvocation.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/commands/context.py` & `cruiz-1.4.0a1/cruiz/commands/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 """
 A context object wrapping the Conan API
 """
 
 from contextlib import contextmanager
 import logging
-import os
 import pathlib
 import typing
 
 from qtpy import QtCore, QtWidgets
 
 from cruiz.exceptions import RecipeInspectionError
 
@@ -225,21 +224,20 @@
         # from Explorer even though a cmd dir command does show what its linked to
         os.symlink(source, link)
     """
 
     @staticmethod
     def _make_hard_link(source: pathlib.Path, link: pathlib.Path) -> None:
         if link.exists():
-            if os.path.samefile(source, link):
+            if source.samefile(link):
                 return
             # the inode may have changed, so just remove the old link, and recreate
-            os.unlink(link)
-        if not link.parent.exists():
-            os.makedirs(link.parent)
-        os.link(source, link)
+            link.unlink()
+        link.parent.mkdir(parents=True, exist_ok=True)
+        link.hardlink_to(source)
 
     def editable_add(
         self,
         ref: str,
         recipe_path: pathlib.Path,
         config_subdir: str,
         continuation: typing.Optional[typing.Callable[[typing.Any, typing.Any], None]],
@@ -376,15 +374,15 @@
         continuation: typing.Optional[typing.Callable[[typing.Any, typing.Any], None]],
     ) -> None:
         """
         Perform one of the actions to get package details from a remote.
         """
         self._start_invocation(params, None, continuation)
 
-    def get_package_directory(self, pkgdata: PackageNode) -> str:
+    def get_package_directory(self, pkgdata: PackageNode) -> pathlib.Path:
         """
         Get the package directory for the specified package.
         """
         package_dir, exception = self._meta_invocation.request_data(
             "package_dir",
             {
                 "ref": pkgdata.reference,
@@ -395,15 +393,15 @@
         )
         if exception:
             if self.parent():
                 self.parent().record_exception(exception)
             else:
                 raise Exception("Get package directory failed") from exception
         else:
-            assert isinstance(package_dir, str)
+            assert isinstance(package_dir, pathlib.Path)
         return package_dir
 
     def cancel(self) -> None:
         """
         Cancel any current running worker thread.
         """
         if self._invocations:
@@ -434,15 +432,15 @@
         profiles_dir, exception = self._meta_invocation.request_data("profiles_dir")
         if exception:
             if self.parent():
                 self.parent().record_exception(exception)
             else:
                 raise Exception("Get profiles directory failed") from exception
         else:
-            assert isinstance(profiles_dir, str)
+            assert isinstance(profiles_dir, pathlib.Path)
         return pathlib.Path(profiles_dir)
 
     def all_profile_dirs(self) -> typing.List[pathlib.Path]:
         """
         Get a list of all profile directories inspected.
         """
         profile_dirs = [self.profiles_dir()]
```

### Comparing `cruiz-1.3.2b1/cruiz/commands/guardedlisttoflush.py` & `cruiz-1.4.0a1/cruiz/commands/guardedlisttoflush.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/commands/logdetails.py` & `cruiz-1.4.0a1/cruiz/commands/logdetails.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/commands/messagereplyprocessor.py` & `cruiz-1.4.0a1/cruiz/commands/messagereplyprocessor.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/commands/metarequestconaninvocation.py` & `cruiz-1.4.0a1/cruiz/commands/metarequestconaninvocation.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/constants.py` & `cruiz-1.4.0a1/cruiz/constants.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/dumpobjecttypes.py` & `cruiz-1.4.0a1/cruiz/dumpobjecttypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,15 @@
     if "CRUIZ_DUMP_OBJECT_TYPES_DETAIL" in os.environ:
         logger.log(loglevel, "%s%s%s (%s)", indent, prefix, type(obj), obj.__repr__)
     else:
         logger.log(loglevel, "%s%s%s", indent, prefix, type(obj))
     if isinstance(obj, (list, tuple)):
         for i, item in enumerate(obj):
             __examine(item, loglevel, depth + 1, f"{i}: ")
-    elif isinstance(obj, str):
-        pass
-    elif isinstance(obj, bool):
+    elif isinstance(obj, (str, bool)):
         pass
     elif isinstance(obj, dict):
         for key, value in obj.items():
             __examine(value, loglevel, depth + 1, f"{key}: ")
     elif obj is not None:
         try:
             dict_of_attribs = obj.__dict__
```

### Comparing `cruiz-1.3.2b1/cruiz/entrypoint.py` & `cruiz-1.4.0a1/cruiz/entrypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import importlib.util
 import logging
 import os
 import pathlib
 import platform
 import sys
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
 from cruiz.resourcegeneration import generate_resources
 
 
 logging.basicConfig(
     level=os.getenv("LOGLEVEL", "WARNING"),
     filename=os.getenv("LOGFILE", None),
@@ -23,18 +23,15 @@
 
 
 logger = logging.getLogger(__name__)
 
 # resource generation be invoked before resources and MainWindow are imported
 generate_resources()
 
-if PYSIDE2:
-    import cruiz.pyside2.resources  # noqa: F401
-else:
-    import cruiz.pyside6.resources  # noqa: F401
+import cruiz.pyside6.resources  # noqa: F401, E402
 
 from cruiz.application import Application  # noqa: E402
 from cruiz.mainwindow import MainWindow  # noqa: E402
 from cruiz.settings.updatesettings import (  # noqa: E402
     update_settings_to_current_version,
 )
```

### Comparing `cruiz-1.3.2b1/cruiz/environ.py` & `cruiz-1.4.0a1/cruiz/environ.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/exceptions.py` & `cruiz-1.4.0a1/cruiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/interop/commandparameters.py` & `cruiz-1.4.0a1/cruiz/interop/commandparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/interop/dependencygraph.py` & `cruiz-1.4.0a1/cruiz/interop/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/interop/packagenode.py` & `cruiz-1.4.0a1/cruiz/interop/packagenode.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/interop/pod.py` & `cruiz-1.4.0a1/cruiz/interop/pod.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Plain old data classes
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-import os
+import pathlib
 import typing
 
 
 # copied from distutils.url.strtobool and modified
 def _strtobool(val: str) -> bool:
     """Convert a string representation of truth to true (1) or false (0).
 
@@ -76,37 +76,37 @@
 
 @dataclass(frozen=True)
 class ConanHook:
     """
     Plain old data class representing a Conan hook
     """
 
-    path: str
+    path: pathlib.Path
     enabled: bool
 
-    def has_path(self, path: str) -> bool:
+    def has_path(self, path: pathlib.Path) -> bool:
         """
         Does the hook contain the specified path?
         """
-        return self.path in (path, os.path.splitext(path)[0])
+        return self.path in (path, path.stem)
 
     @classmethod
     def from_string(cls, string: str) -> ConanHook:
         """
         Convert a string to a ConanHook.
         """
         assert string.startswith("ConanHook(")
         assert string.endswith(")")
         string = string.replace("ConanHook(", "")
         string = string.replace(")", "")
         args = string.split(",")
         assert len(args) == 2
         path_arg = args[0].strip().split("=")
         enabled_arg = args[1].strip().split("=")
-        path = path_arg[1][1:-1]
+        path = pathlib.Path(path_arg[1][1:-1])
         enabled = _strtobool(enabled_arg[1])
         return cls(path, enabled)
 
 
 @dataclass(frozen=True)
 class ExtraProfileDirectory:
     """
```

### Comparing `cruiz-1.3.2b1/cruiz/interop/reciperevisionsparameters.py` & `cruiz-1.4.0a1/cruiz/interop/reciperevisionsparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/interop/searchrecipesparameters.py` & `cruiz-1.4.0a1/cruiz/interop/searchrecipesparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/load_recipe/loadrecipewizard.py` & `cruiz-1.4.0a1/cruiz/load_recipe/loadrecipewizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 """
 Wizard for loading a recipe
 """
 
 import pathlib
 import typing
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.load_recipe_wizard import Ui_LoadRecipeWizard
-else:
-    from cruiz.pyside6.load_recipe_wizard import Ui_LoadRecipeWizard
+from cruiz.pyside6.load_recipe_wizard import Ui_LoadRecipeWizard
 
 from cruiz.exceptions import RecipeDoesNotExistError, RecipeAlreadyOpenError
 from cruiz.settings.managers.recipe import RecipeSettings, RecipeSettingsReader
 from cruiz.recipe.recipewidget import Recipe
 
 from cruiz.commands.context import managed_conan_context
 from cruiz.commands.logdetails import LogDetails
@@ -131,10 +128,9 @@
 
     def validate(self) -> None:
         """
         Validate the recipe in the wizard.
         """
         if not self._path.exists():
             raise RecipeDoesNotExistError()
-        if self._uuid:
-            if cruiz.globals.get_main_window().is_recipe_active(self._uuid):
-                raise RecipeAlreadyOpenError()
+        if self._uuid and cruiz.globals.get_main_window().is_recipe_active(self._uuid):
+            raise RecipeAlreadyOpenError()
```

### Comparing `cruiz-1.3.2b1/cruiz/load_recipe/pages/initialprofilepage.py` & `cruiz-1.4.0a1/cruiz/load_recipe/pages/initialprofilepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/load_recipe/pages/localcachepage.py` & `cruiz-1.4.0a1/cruiz/load_recipe/pages/localcachepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/load_recipe/pages/packageversionpage.py` & `cruiz-1.4.0a1/cruiz/load_recipe/pages/packageversionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/mainwindow.py` & `cruiz-1.4.0a1/cruiz/mainwindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,71 +107,70 @@
             self._remote_browser_dock.on_local_cache_modified
         )
         self.addDockWidget(
             QtCore.Qt.RightDockWidgetArea,
             self._remote_browser_dock,
         )
 
-        open_recipe_action = QAction("Open recipe...", self)
+        open_recipe_action = QtGui.QAction("Open recipe...", self)
         open_recipe_action.setShortcut(QtGui.QKeySequence("Ctrl+O"))
         open_recipe_action.triggered.connect(self._open_recipe)
 
-        self._recent_recipe_menu = QtWidgets.QMenu("Recent recipes", self)
-
-        exit_action = QAction("&Quit", self)
-        exit_action.setMenuRole(QAction.QuitRole)
+        exit_action = QtGui.QAction("&Quit", self)
+        exit_action.setMenuRole(QtGui.QAction.QuitRole)
         exit_action.setShortcut(QtGui.QKeySequence("Ctrl+Q"))
         exit_action.setStatusTip("Quit application")
         exit_action.triggered.connect(
             qApp.closeAllWindows,  # type: ignore # noqa: F821
             QtCore.Qt.QueuedConnection,
         )
 
         # need a clone of the exit action without the menu role to
         # appear on the systrayicon
-        systray_exit_icon = QAction("&Quit", self)
+        systray_exit_icon = QtGui.QAction("&Quit", self)
         systray_exit_icon.setShortcut(QtGui.QKeySequence("Ctrl+Q"))
         systray_exit_icon.setStatusTip("Quit application")
         systray_exit_icon.triggered.connect(
             qApp.closeAllWindows,  # type: ignore # noqa: F821
             QtCore.Qt.QueuedConnection,
         )
         if QtWidgets.QSystemTrayIcon.isSystemTrayAvailable():
             self._app_menu.addAction(systray_exit_icon)
 
         menubar = self.menuBar()
         file_menu = menubar.addMenu("&File")
+        self._recent_recipe_menu = QtWidgets.QMenu("Recent recipes", file_menu)
         file_menu.aboutToShow.connect(self._rebuild_recent_recipe_menu)
         file_menu.addAction(open_recipe_action)
         file_menu.addMenu(self._recent_recipe_menu)
         file_menu.addSeparator()
         file_menu.addAction(exit_action)
 
         edit_menu = menubar.addMenu("&Edit")
-        edit_preferences_action = QAction("Preferences...", self)
-        edit_preferences_action.setMenuRole(QAction.PreferencesRole)
+        edit_preferences_action = QtGui.QAction("Preferences...", self)
+        edit_preferences_action.setMenuRole(QtGui.QAction.PreferencesRole)
         edit_preferences_action.triggered.connect(self._edit_preferences_new)
         edit_menu.addAction(edit_preferences_action)
-        manage_local_caches_action = QAction("Manage local caches...", self)
+        manage_local_caches_action = QtGui.QAction("Manage local caches...", self)
         manage_local_caches_action.triggered.connect(self._manage_local_caches)
         edit_menu.addAction(manage_local_caches_action)
 
         view_menu = menubar.addMenu("&View")
         view_menu.addAction(self._remote_browser_dock.toggleViewAction())
 
         help_menu = menubar.addMenu("&Help")
-        about_cruiz_action = QAction("About cruiz...", self)
-        about_cruiz_action.setMenuRole(QAction.AboutRole)
+        about_cruiz_action = QtGui.QAction("About cruiz...", self)
+        about_cruiz_action.setMenuRole(QtGui.QAction.AboutRole)
         about_cruiz_action.triggered.connect(self._about_cruiz)
         help_menu.addAction(about_cruiz_action)
-        about_qt_action = QAction("About Qt...", self)
-        about_qt_action.setMenuRole(QAction.AboutQtRole)
+        about_qt_action = QtGui.QAction("About Qt...", self)
+        about_qt_action.setMenuRole(QtGui.QAction.AboutQtRole)
         about_qt_action.triggered.connect(QtWidgets.QApplication.aboutQt)
         help_menu.addAction(about_qt_action)
-        icon_license_action = QAction("Icon licenses...", self)
+        icon_license_action = QtGui.QAction("Icon licenses...", self)
         icon_license_action.triggered.connect(self._icon_license)
         help_menu.addAction(icon_license_action)
 
         self._ccache_label: QtWidgets.QLabel = QtWidgets.QLabel()
         self._ccache_label.setFrameStyle(
             QtWidgets.QFrame.Panel | QtWidgets.QFrame.Sunken
         )
@@ -247,15 +246,15 @@
         )
 
         self.setWindowTitle(qApp.applicationName())  # type: ignore # noqa: F821
 
         cruiz.globals.CRUIZ_MAINWINDOW = self
 
     def _on_warning_label_menu(self, position: QtCore.QPoint) -> None:
-        action = QAction("Dismiss", self)
+        action = QtGui.QAction("Dismiss", self)
         action.triggered.connect(self._on_warning_label_dismiss)
         menu = QtWidgets.QMenu(self)
         menu.addAction(action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_warning_label_dismiss(self) -> None:
         self._warning_label.setToolTip("")
@@ -339,15 +338,15 @@
                     # can drop through even though the path doesn't exist
                 attributes = settings.attribute_overrides.resolve()
             label = (
                 f"{recipe_path} [v{attributes['version']}]"
                 if "version" in attributes
                 else str(recipe_path)
             )
-            recent_recipe_action = QAction(label, self)
+            recent_recipe_action = QtGui.QAction(label, self)
             recent_recipe_action.triggered.connect(
                 partial(self.load_recipe, recipe_path, uuid)
             )
             self._recent_recipe_menu.addAction(recent_recipe_action)
             recent_recipe_action.setEnabled(not self.is_recipe_active(uuid))
             all_uuids_with_settings.remove(uuid)
         self._recent_recipe_menu.setEnabled(len(uuids) > 0)
@@ -681,11 +680,11 @@
             )
 
     def is_recipe_active(self, uuid: QtCore.QUuid) -> bool:
         """
         Is the recipe with the given UUID active (i.e. has an open tab)?
         """
         mdi_area = self.centralWidget()
-        for subwindow in mdi_area.subWindowList():
-            if subwindow.widget().recipe.uuid == uuid:
-                return True
-        return False
+        return any(
+            subwindow.widget().recipe.uuid == uuid
+            for subwindow in mdi_area.subWindowList()
+        )
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/managelocalcachesdialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/managelocalcachesdialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 """
 Dialog for managing local caches
 """
 
 from enum import IntEnum
 import os
+import pathlib
 import platform
 import shutil
 import stat
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 from cruiz.commands.logdetails import LogDetails
 
 from cruiz.interop.pod import ConanHook
 from cruiz.settings.managers.namedlocalcache import (
     NamedLocalCacheSettings,
     NamedLocalCacheSettingsReader,
     NamedLocalCacheSettingsWriter,
@@ -29,22 +30,15 @@
 )
 from cruiz.widgets.util import BlockSignals
 from cruiz.commands.context import ConanContext, ConanConfigBoolean
 
 from cruiz.revealonfilesystem import reveal_on_filesystem
 from cruiz.constants import DEFAULT_CACHE_NAME
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_manage import Ui_ManageLocalCaches
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_manage import Ui_ManageLocalCaches
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_manage import Ui_ManageLocalCaches
 
 from .widgets import (
     NewLocalCacheWizard,
     InstallConfigDialog,
     MoveLocalCacheDialog,
     AddRemoteDialog,
     RemoveLocksDialog,
@@ -85,22 +79,22 @@
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Apply).setEnabled(False)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Apply).clicked.connect(
             self._save_modifications
         )
         # locations
         dir_icon = self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon)
         self._ui.conan_user_home.setReadOnly(True)
-        open_user_home_action = QAction(dir_icon, "", self)
+        open_user_home_action = QtGui.QAction(dir_icon, "", self)
         open_user_home_action.triggered.connect(self._open_conan_user_home)
         self._ui.conan_user_home.addAction(
             open_user_home_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.conan_user_home_short.setReadOnly(True)
-        open_short_user_home_action = QAction(dir_icon, "", self)
+        open_short_user_home_action = QtGui.QAction(dir_icon, "", self)
         open_short_user_home_action.triggered.connect(self._open_conan_user_home_short)
         self._ui.conan_user_home_short.addAction(
             open_short_user_home_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # extra profiles
         self._ui.profilesTableButtons.button(QtWidgets.QDialogButtonBox.Open).setText(
@@ -198,41 +192,40 @@
         self._log_details.logging.connect(self._ui.localCacheLog.show)
         self._context = ConanContext(DEFAULT_CACHE_NAME, self._log_details)
         self._populate_cache_names(cache_name_to_open)
         self._modifications: typing.Dict[str, typing.Any] = {}
         self._modified.connect(self._on_modification)
 
     def _open_conan_user_home(self) -> None:
-        reveal_on_filesystem(self._ui.conan_user_home.text())
+        reveal_on_filesystem(pathlib.Path(self._ui.conan_user_home.text()))
 
     def _open_conan_user_home_short(self) -> None:
-        reveal_on_filesystem(self._ui.conan_user_home_short.text())
+        reveal_on_filesystem(pathlib.Path(self._ui.conan_user_home_short.text()))
 
     def _on_modification(self) -> None:
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Apply).setEnabled(
             bool(self._modifications)
         )
 
     def accept(self) -> None:
         if self._modifications:
             self._save_modifications()
         self._context.close()
         super().accept()
 
     def reject(self) -> None:
-        if self._modifications:
-            if (
-                QtWidgets.QMessageBox.question(
-                    self,
-                    "Local cache modifications",
-                    "Do you want to lose unsaved changes to the local cache?",
-                )
-                == QtWidgets.QMessageBox.StandardButton.No
-            ):
-                return
+        if self._modifications and (
+            QtWidgets.QMessageBox.question(
+                self,
+                "Local cache modifications",
+                "Do you want to lose unsaved changes to the local cache?",
+            )
+            == QtWidgets.QMessageBox.StandardButton.No
+        ):
+            return
         self._context.close()
         super().reject()
 
     def _populate_cache_names(
         self, cache_name_to_select: typing.Optional[str] = None
     ) -> None:
         combo = self._ui.local_cache_names
@@ -344,15 +337,15 @@
                 QtCore.Qt.ItemIsEnabled  # type: ignore
                 | QtCore.Qt.ItemIsSelectable
                 | QtCore.Qt.ItemIsUserCheckable
             )
             enabled_item.setCheckState(
                 QtCore.Qt.Checked if hook.enabled else QtCore.Qt.Unchecked
             )
-            name_item = QtWidgets.QTableWidgetItem(hook.path)
+            name_item = QtWidgets.QTableWidgetItem(os.fspath(hook.path))
             name_item.setFlags(
                 QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsSelectable  # type: ignore
             )
             with BlockSignals(self._ui.hooksTable) as blocked_widget:
                 blocked_widget.setItem(
                     i,
                     ManageLocalCachesDialog._HooksTableColumnIndex.ENABLED,
@@ -458,24 +451,24 @@
             )
             if index >= 0:
                 del self._modifications["Remotes"]["Add"][index]
                 if not self._modifications["Remotes"]["Add"]:
                     del self._modifications["Remotes"]["Add"]
                 if not self._modifications["Remotes"]:
                     del self._modifications["Remotes"]
+                # has the removal of the addition now put the
+                # table back into it's original order?
                 if (
                     "Remotes" in self._modifications
                     and "Reordered" in self._modifications["Remotes"]
+                    and self._ui.remotesTable.same(self._context.get_remotes_list())
                 ):
-                    # has the removal of the addition now put the
-                    # table back into it's original order?
-                    if self._ui.remotesTable.same(self._context.get_remotes_list()):
-                        del self._modifications["Remotes"]["Reordered"]
-                        if not self._modifications["Remotes"]:
-                            del self._modifications["Remotes"]
+                    del self._modifications["Remotes"]["Reordered"]
+                    if not self._modifications["Remotes"]:
+                        del self._modifications["Remotes"]
         else:
             if "Remove" not in self._modifications["Remotes"]:
                 self._modifications["Remotes"]["Remove"] = []
             self._modifications["Remotes"]["Remove"].append(remote_removed.name)
         self._modified.emit()
 
     def _remotes_selection(self) -> None:
@@ -524,15 +517,15 @@
         self._modified.emit()
 
     def _hooks_item_changed(self, item: QtWidgets.QTableWidgetItem) -> None:
         if item.column() == ManageLocalCachesDialog._HooksTableColumnIndex.ENABLED:
             path_item = self._ui.hooksTable.item(
                 item.row(), ManageLocalCachesDialog._HooksTableColumnIndex.PATH
             )
-            hook_path = path_item.text().strip()
+            hook_path = pathlib.Path(path_item.text().strip())
             item_enabled = bool(item.checkState())
             hooks = self._context.get_hooks_list()
             hook = next(item for item in hooks if item.has_path(hook_path))
             assert hook
             if item_enabled == hook.enabled:
                 hook_unchanged = next(
                     item
@@ -573,23 +566,24 @@
         if (
             MoveLocalCacheDialog(self._context, self).exec_()
             == QtWidgets.QDialog.Accepted
         ):
             self._update_cache_details(self._context.cache_name)
 
     @staticmethod
-    def _delete_tree_with_readonly_files(dir_path: str) -> None:
-        if not os.path.isdir(dir_path):
+    def _delete_tree_with_readonly_files(dir_path: pathlib.Path) -> None:
+        if not dir_path.is_dir():
             return
 
         def make_writeable(action: typing.Any, name: str, exc: typing.Any) -> None:
             # pylint: disable=unused-argument
             if exc[0] is PermissionError:
-                os.chmod(name, stat.S_IWRITE)
-                os.remove(name)
+                name_path = pathlib.Path(name)
+                name_path.chmod(stat.S_IWRITE)
+                name_path.unlink()
             else:
                 raise exc[1]
 
         shutil.rmtree(dir_path, onerror=make_writeable)
 
     def _operations_delete_cache(self) -> None:
         cache_name = self._context.cache_name
@@ -597,19 +591,19 @@
             self,
             "Local cache deletion",
             f"Are you sure you want to delete the local cache {cache_name}?",
         )
         if result == QtWidgets.QMessageBox.StandardButton.No:
             return
         with NamedLocalCacheSettingsReader(cache_name) as settings:
-            home_dir = settings.home_dir.resolve()
-            short_home_dir = settings.short_home_dir.resolve()
+            home_dir = pathlib.Path(settings.home_dir.resolve())
+            short_home_dir = pathlib.Path(settings.short_home_dir.resolve())
 
         assert home_dir  # because it's non-default
-        conan_home_dir = os.path.join(home_dir, ".conan")
+        conan_home_dir = home_dir / ".conan"
         # since this is destructive, check again
         result = QtWidgets.QMessageBox.question(
             self,
             "Local cache deletion",
             f"Please confirm you want to delete the directories {conan_home_dir} and "
             f"{short_home_dir}?"
             if short_home_dir
@@ -778,15 +772,15 @@
         assert isinstance(self._modifications["Env"], _EnvChangeManagement)
         self._modifications["Env"].key_never_required(key)
         self._modified.emit()
 
     def _log_context_menu(self, position: QtCore.QPoint) -> None:
         menu = self.sender().createStandardContextMenu(position)
         menu.addSeparator()
-        clear_action = QAction("Clear", self)
+        clear_action = QtGui.QAction("Clear", self)
         clear_action.triggered.connect(self._clear_log)
         menu.addAction(clear_action)
         menu.exec_(self.sender().viewport().mapToGlobal(position))
 
     def _clear_log(self) -> None:
         self._ui.localCacheLog.clear()
         self._ui.localCacheLog.hide()
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/__init__.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/addenvironmentdialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addenvironmentdialog.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,19 @@
 
 """
 Dialog for adding an environment variable
 """
 
 from dataclasses import dataclass
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.commands.context import ConanContext
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_add_environment import Ui_AddEnvironmentDialog
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_add_environment import Ui_AddEnvironmentDialog
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_add_environment import Ui_AddEnvironmentDialog
 
 
 @dataclass
 class KeyValuePair:
     """
     Representation of a key-value pair
     """
@@ -38,20 +31,20 @@
     def __init__(self, context: ConanContext, parent: QtWidgets.QWidget) -> None:
         super().__init__(parent)
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose, True)
         self._ui = Ui_AddEnvironmentDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         conan_environment_menu = QtWidgets.QMenu("Conan environment variables", self)
         for key, _ in context.get_conan_config_environment_variables().items():
-            key_action = QAction(key, self)
+            key_action = QtGui.QAction(key, self)
             key_action.triggered.connect(self._set_name)
             conan_environment_menu.addAction(key_action)
         conan_environment_menu.addSeparator()
         # TODO: CONAN_V2_MODE is obsolete
-        conan_v2_mode_action = QAction("CONAN_V2_MODE", self)
+        conan_v2_mode_action = QtGui.QAction("CONAN_V2_MODE", self)
         conan_v2_mode_action.triggered.connect(self._set_name)  # type: ignore
         conan_environment_menu.addAction(conan_v2_mode_action)
         self._ui.name.set_custom_menu(conan_environment_menu)
         self._ui.name.textChanged.connect(self._updated)
         self._ui.value.textChanged.connect(self._updated)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
         self._name: str = ""
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,22 @@
 
 """
 Dialog for adding extra profile directories
 """
 
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.interop.pod import ExtraProfileDirectory
 from cruiz.widgets.util import search_for_dir_options
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_add_profile_directory import (
-        Ui_AddExtraProfileDirectoryDialog,
-    )
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_add_profile_directory import (
-        Ui_AddExtraProfileDirectoryDialog,
-    )
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_add_profile_directory import (
+    Ui_AddExtraProfileDirectoryDialog,
+)
 
 
 class AddExtraProfileDirectoryDialog(QtWidgets.QDialog):
     """
     Dialog for adding an extra profile directory.
     """
 
@@ -36,15 +27,15 @@
         self._ui = Ui_AddExtraProfileDirectoryDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
         self._ui.buttonBox.accepted.connect(self.accept)
         self._ui.buttonBox.rejected.connect(self.reject)
         self._ui.name.textChanged.connect(self._updated)
         self._ui.directory.textChanged.connect(self._updated)
-        browse_for_profile_dir_action = QAction(
+        browse_for_profile_dir_action = QtGui.QAction(
             self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon), "", self
         )
         browse_for_profile_dir_action.triggered.connect(self._browse_for_profile_dir)
         self._ui.directory.addAction(
             browse_for_profile_dir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/addremotedialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/addremotedialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,23 @@
 """
 Dialog for adding a new remote.
 """
 
 from functools import partial
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 import validators
 
 from cruiz.interop.pod import ConanRemote
 
 from cruiz.settings.managers.recentconanremotes import RecentConanRemotesSettingsReader
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_add_remote import Ui_AddRemoteDialog
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_add_remote import Ui_AddRemoteDialog
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_add_remote import Ui_AddRemoteDialog
 
 
 class AddRemoteDialog(QtWidgets.QDialog):
     """
     Dialog for adding a new remote.
     """
 
@@ -36,15 +29,15 @@
         self._ui = Ui_AddRemoteDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         recent_remotes_menu = QtWidgets.QMenu("Recent remotes", self)
         with RecentConanRemotesSettingsReader() as settings:
             recent_remote_urls = settings.urls.resolve()
         if recent_remote_urls:
             for remote in recent_remote_urls:
-                remote_action = QAction(remote, self)
+                remote_action = QtGui.QAction(remote, self)
                 remote_action.triggered.connect(partial(self._set_remote_url, remote))
                 recent_remotes_menu.addAction(remote_action)
         else:
             recent_remotes_menu.setEnabled(False)
         self._ui.url.set_custom_menu(recent_remotes_menu)
         self._ui.url.textChanged.connect(self._updated)
         self._ui.name.textChanged.connect(self._updated)
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/configpathorurl.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/configpathorurl.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,9 +19,10 @@
         # pylint: disable=attribute-defined-outside-init
         self._custom_menu = menu
 
     def contextMenuEvent(self, event: QtGui.QContextMenuEvent) -> None:
         menu = self.createStandardContextMenu()
         if self._custom_menu:
             menu.addSeparator()
+            self._custom_menu.setParent(menu)
             menu.addMenu(self._custom_menu)
         menu.exec_(event.globalPos())
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/installconfigdialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/installconfigdialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,20 @@
 """
 Dialog for installing a new Conan config
 """
 
 from functools import partial
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.commands.context import ConanContext
 from cruiz.interop.commandparameters import CommandParameters
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_install_config import Ui_InstallConfigDialog
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_install_config import Ui_InstallConfigDialog
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_install_config import Ui_InstallConfigDialog
 
 from cruiz.settings.managers.recentconanconfigs import (
     RecentConanConfigSettingsReader,
     RecentConanConfigSettings,
     RecentConanConfigSettingsWriter,
 )
 import cruiz.workers
@@ -41,15 +34,15 @@
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         self._context = context
         recent_config_paths_menu = QtWidgets.QMenu("Recent config paths", self)
         with RecentConanConfigSettingsReader() as settings:
             config_paths = settings.paths.resolve()
         if config_paths:
             for path in config_paths:
-                path_action = QAction(path, self)
+                path_action = QtGui.QAction(path, self)
                 path_action.triggered.connect(partial(self._set_url, path))
                 recent_config_paths_menu.addAction(path_action)
         else:
             recent_config_paths_menu.setEnabled(False)
         self._ui.pathOrUrl.set_custom_menu(recent_config_paths_menu)
         self._ui.pathOrUrl.textChanged.connect(self._path_updated)
         self._ui.installButton.setEnabled(False)
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/keyvaluetable.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/keyvaluetable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/movelocalcachedialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/movelocalcachedialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,32 +5,25 @@
 """
 
 import pathlib
 import platform
 import shutil
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.commands.context import ConanContext
 
 from cruiz.settings.managers.namedlocalcache import (
     NamedLocalCacheSettings,
     NamedLocalCacheSettingsReader,
     NamedLocalCacheSettingsWriter,
 )
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_move import Ui_LocalCacheMove
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_move import Ui_LocalCacheMove
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_move import Ui_LocalCacheMove
 
 from cruiz.widgets.util import search_for_dir_options
 
 
 class MoveLocalCacheDialog(QtWidgets.QDialog):
     """
     Dialog for moving a non-default local cache.
@@ -43,15 +36,15 @@
         self._ui = Ui_LocalCacheMove()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         with NamedLocalCacheSettingsReader(context.cache_name) as settings:
             self._ui.currentUserHome.setText(settings.home_dir.resolve())
             self._ui.currentUserHomeShort.setText(settings.short_home_dir.resolve())
         self._ui.buttonBox.accepted.connect(self.accept)
         self._ui.buttonBox.rejected.connect(self.reject)
-        home_dir_browse_action = QAction(
+        home_dir_browse_action = QtGui.QAction(
             self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon), "", self
         )
         home_dir_browse_action.triggered.connect(self._home_dir_browse)
         self._ui.newUserHome.addAction(
             home_dir_browse_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/newlocalcachewizard.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,34 +3,27 @@
 """
 Wizard for creating new Conan local caches
 """
 
 import platform
 import typing
 
-from qtpy import QtGui, QtWidgets, PYSIDE2
+from qtpy import QtGui, QtWidgets
 
 from cruiz.commands.context import ConanContext
 from cruiz.interop.commandparameters import CommandParameters
 from cruiz.commands.logdetails import LogDetails
 from cruiz.settings.managers.localcachepreferences import LocalCacheSettingsReader
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheCreator
 from cruiz.widgets.util import search_for_dir_options
 from cruiz.constants import DEFAULT_CACHE_NAME
 
 import cruiz.workers
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_new_wizard import Ui_NewLocalCacheWizard
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.local_cache_new_wizard import Ui_NewLocalCacheWizard
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.local_cache_new_wizard import Ui_NewLocalCacheWizard
 
 
 class NewLocalCacheWizard(QtWidgets.QWizard):
     """
     Wizard for creating new local caches
     """
 
@@ -42,21 +35,21 @@
         self._context = ConanContext(DEFAULT_CACHE_NAME, self._log_details)
         self._ui.new_cache_name.textChanged.connect(self._ui.namePage.completeChanged)
         self._ui.userHome.textChanged.connect(self._ui.locationsPage.completeChanged)
         self._ui.userHomeShort.textChanged.connect(
             self._ui.locationsPage.completeChanged
         )
         dir_icon: QtGui.QIcon = self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon)
-        browse_home_dir_action = QAction(dir_icon, "", self)
+        browse_home_dir_action = QtGui.QAction(dir_icon, "", self)
         browse_home_dir_action.triggered.connect(self._browse_for_home_dir)
         self._ui.userHome.addAction(
             browse_home_dir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
-        browse_short_home_dir_action = QAction(dir_icon, "", self)
+        browse_short_home_dir_action = QtGui.QAction(dir_icon, "", self)
         browse_short_home_dir_action.triggered.connect(self._browse_for_short_home_dir)
         self._ui.userHomeShort.addAction(
             browse_short_home_dir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         with LocalCacheSettingsReader() as settings:
             new_config_url = settings.new_configuration_install.resolve()
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/progressdialogs.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/progressdialogs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/remotestable.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/remotestable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 #!/usr/bin/env python3
 
 """
 Dialog for removing an environment variable
 """
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_remove_environment import Ui_RemoveEnvironmentDialog
-else:
-    from cruiz.pyside6.local_cache_remove_environment import Ui_RemoveEnvironmentDialog
+from cruiz.pyside6.local_cache_remove_environment import Ui_RemoveEnvironmentDialog
 
 
 class RemoveEnvironmentDialog(QtWidgets.QDialog):
     """
     Dialog for removing an environment variable from the collection used to run
     Conan commands
     """
```

### Comparing `cruiz-1.3.2b1/cruiz/manage_local_cache/widgets/runconancommanddialog.py` & `cruiz-1.4.0a1/cruiz/manage_local_cache/widgets/runconancommanddialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 
 """
 Dialog for running a Conan command in a local cache.
 """
 
 import typing
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
 from cruiz.commands.context import ConanContext, LogDetails
 from cruiz.interop.commandparameters import CommandParameters
 
-if PYSIDE2:
-    from cruiz.pyside2.local_cache_run_command_dialog import Ui_RunConanCommandDialog
-else:
-    from cruiz.pyside6.local_cache_run_command_dialog import Ui_RunConanCommandDialog
+from cruiz.pyside6.local_cache_run_command_dialog import Ui_RunConanCommandDialog
 
 import cruiz.workers.arbitrary
 
 
 class RunConanCommandDialog(QtWidgets.QDialog):
     """
     Dialog for adding an environment key-value pair to the local cache.
```

### Comparing `cruiz-1.3.2b1/cruiz/model/graphaslistmodel.py` & `cruiz-1.4.0a1/cruiz/model/graphaslistmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/recipe/dependencyview.py` & `cruiz-1.4.0a1/cruiz/recipe/dependencyview.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,16 @@
 
 """
 Conan dependency view
 """
 
 import typing
 
-from qtpy import QtWidgets, QtSvg, PYSIDE2
-
-if PYSIDE2:
-    QGraphicsSvgItem = QtSvg.QGraphicsSvgItem
-else:
-    # module not present in qtpy at the time of writing
-    from PySide6 import QtSvgWidgets
-
-    QGraphicsSvgItem = QtSvgWidgets.QGraphicsSvgItem
+# TODO: note, change, as QtSvgWidgets wasn't available here previously
+from qtpy import QtWidgets, QtSvg, QtSvgWidgets
 
 from cruiz.interop.dependencygraph import DependencyGraph
 from cruiz.svggraph import DependenciesToDigraph, DigraphToSVG, SVGScene
 
 
 class DependencyView(QtWidgets.QGraphicsView):
     def clear(self) -> None:
@@ -44,14 +37,14 @@
         super().__init__(parent)
         self.setWindowTitle(f"What uses {depgraph.root.name}")
 
         # TODO: should this be in cruiz.svggraph to isolate the SVG code?
         digraph = DependenciesToDigraph(depgraph, "LR", flipped_edges=True)
         svg = DigraphToSVG(digraph)
         self._renderer = QtSvg.QSvgRenderer(svg.svg)
-        item = QGraphicsSvgItem()
+        item = QtSvgWidgets.QGraphicsSvgItem()
         item.setSharedRenderer(self._renderer)
         self._scene = QtWidgets.QGraphicsScene()
         self._scene.addItem(item)
         view = QtWidgets.QGraphicsView(self._scene)
 
         QtWidgets.QVBoxLayout(self).addWidget(view)
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/expressioneditordialog.py` & `cruiz-1.4.0a1/cruiz/recipe/expressioneditordialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 #!/usr/bin/env python3
 
 """
 Local workflow folder expression editor dialog
 """
 
-from qtpy import QtWidgets, PYSIDE2
+from qtpy import QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.recipe_local_workflow_expression_editor import (
-        Ui_ExpressionEditor,
-    )
-else:
-    from cruiz.pyside6.recipe_local_workflow_expression_editor import (
-        Ui_ExpressionEditor,
-    )
+from cruiz.pyside6.recipe_local_workflow_expression_editor import (
+    Ui_ExpressionEditor,
+)
 
 
 class ExpressionEditorDialog(QtWidgets.QDialog):
     """
     Dialog for editing expressions for local workflow folders
     """
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/findtextdialog.py` & `cruiz-1.4.0a1/cruiz/recipe/findtextdialog.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 #!/usr/bin/env python3
 
 """
 Conan recipe find text dialog
 """
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.find_text_dialog import Ui_FindTextDialog
-else:
-    from cruiz.pyside6.find_text_dialog import Ui_FindTextDialog
+from cruiz.pyside6.find_text_dialog import Ui_FindTextDialog
 
 
 class FindTextDialog(QtWidgets.QDialog):
     """
     Widget representing a Find dialog
     """
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/logs/command.py` & `cruiz-1.4.0a1/cruiz/recipe/logs/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """
 Recipe command log window
 """
 
-import os
+import pathlib
 import stat
 import typing
 
 from qtpy import QtCore, QtGui, QtWidgets, PYSIDE6
 
 from cruiz.interop.commandparameters import CommandParameters
 
@@ -41,29 +41,29 @@
     QListWidget representing a history of Conan commands
     """
 
     def __init__(self, parent: typing.Optional[QtWidgets.QWidget] = None) -> None:
         super().__init__(parent)
         self.customContextMenuRequested.connect(self._show_context_menu)
         self.itemSelectionChanged.connect(self._selection_changed)
-        self._export_bash_action = QAction("Export to file...", self)
+        self._export_bash_action = QtGui.QAction("Export to file...", self)
         self._export_bash_action.triggered.connect(self._export_bash)
-        self._export_zsh_action = QAction("Export to file...", self)
+        self._export_zsh_action = QtGui.QAction("Export to file...", self)
         self._export_zsh_action.triggered.connect(self._export_zsh)
-        self._export_cmd_action = QAction("Export to file...", self)
+        self._export_cmd_action = QtGui.QAction("Export to file...", self)
         self._export_cmd_action.triggered.connect(self._export_cmd)
-        self._copy_bash_to_clipboard_action = QAction("Copy to clipboard", self)
+        self._copy_bash_to_clipboard_action = QtGui.QAction("Copy to clipboard", self)
         self._copy_bash_to_clipboard_action.triggered.connect(
             self._copy_bash_to_clipboard
         )
-        self._copy_zsh_to_clipboard_action = QAction("Copy to clipboard", self)
+        self._copy_zsh_to_clipboard_action = QtGui.QAction("Copy to clipboard", self)
         self._copy_zsh_to_clipboard_action.triggered.connect(
             self._copy_zsh_to_clipboard
         )
-        self._copy_cmd_to_clipboard_action = QAction("Copy to clipboard", self)
+        self._copy_cmd_to_clipboard_action = QtGui.QAction("Copy to clipboard", self)
         self._copy_cmd_to_clipboard_action.triggered.connect(
             self._copy_cmd_to_clipboard
         )
         self._menu = QtWidgets.QMenu()
         self._menu.setEnabled(False)
         bash_menu = self._menu.addMenu("bash")
         bash_menu.insertAction(None, self._export_bash_action)  # type: ignore[arg-type]
@@ -97,49 +97,52 @@
             "",
             "Shell script (*.sh)",
         )
         if not filename:
             return
         item = self.selectedItems()[0]
         parameters = item.data(0x0100)
-        with open(filename, "wt", encoding="utf-8") as shell_script:
+        filename_path = pathlib.Path(filename)
+        with filename_path.open("wt", encoding="utf-8") as shell_script:
             shell_script.write("#!/usr/bin/env bash\n")
             shell_script.write(f"{parameters.bash_expression.getvalue()}\n")
-        os.chmod(filename, os.stat(filename).st_mode | stat.S_IEXEC)
+        filename_path.chmod(filename_path.stat().st_mode | stat.S_IEXEC)
 
     def _export_zsh(self) -> None:
         filename, _ = QtWidgets.QFileDialog.getSaveFileName(
             self,
             "Export Conan command as zsh shell script",
             "",
             "Shell script (*.sh)",
         )
         if not filename:
             return
         item = self.selectedItems()[0]
         parameters = item.data(0x0100)
-        with open(filename, "wt", encoding="utf-8") as shell_script:
+        filename_path = pathlib.Path(filename)
+        with filename_path.open("wt", encoding="utf-8") as shell_script:
             shell_script.write("#!/usr/bin/env zsh\n")
             shell_script.write(f"{parameters.zsh_expression.getvalue()}\n")
-        os.chmod(filename, os.stat(filename).st_mode | stat.S_IEXEC)
+        filename_path.chmod(filename_path.stat().st_mode | stat.S_IEXEC)
 
     def _export_cmd(self) -> None:
         filename, _ = QtWidgets.QFileDialog.getSaveFileName(
             self,
             "Export Conan command as CMD Batch shell script",
             "",
             "Batch script (*.bat)",
         )
         if not filename:
             return
         item = self.selectedItems()[0]
         parameters = item.data(0x0100)
-        with open(filename, "wt", encoding="utf-8") as shell_script:
+        filename_path = pathlib.Path(filename)
+        with filename_path.open("wt", encoding="utf-8") as shell_script:
             shell_script.write(f"{parameters.cmd_expression.getvalue()}\n")
-        os.chmod(filename, os.stat(filename).st_mode | stat.S_IEXEC)
+        filename_path.chmod(filename_path.stat().st_mode | stat.S_IEXEC)
 
     def _copy_bash_to_clipboard(self) -> None:
         item = self.selectedItems()[0]
         parameters = item.data(0x0100)
         qApp.clipboard().setText(  # type: ignore  # noqa: F821
             parameters.bash_expression.getvalue()
         )
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/recipe.py` & `cruiz-1.4.0a1/cruiz/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/recipe/recipewidget.py` & `cruiz-1.4.0a1/cruiz/recipe/recipewidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 
 import logging
 import os
 import pathlib
 import re
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2, PYSIDE6
-import git
+from qtpy import QtCore, QtGui, QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.recipe_window import Ui_RecipeWindow
+try:
+    import git
+except ImportError as exc:
+    print(exc)
 
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.recipe_window import Ui_RecipeWindow
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.recipe_window import Ui_RecipeWindow
 
 from cruiz.commands.context import ConanContext
 from cruiz.interop.commandparameters import CommandParameters
 from cruiz.interop.dependencygraph import dependencygraph_from_node_dependees
 from cruiz.commands.logdetails import LogDetails
 from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
 from cruiz.settings.managers.recipe import WorkflowCwd
@@ -48,19 +45,14 @@
 from .findtextdialog import FindTextDialog
 from .expressioneditordialog import ExpressionEditorDialog
 from .dependencyview import InverseDependencyViewDialog
 
 
 logger = logging.getLogger(__name__)
 
-if PYSIDE6:
-    QShortcut = QtGui.QShortcut
-else:
-    QShortcut = QtWidgets.QShortcut
-
 
 # copied from distutils.url.strtobool and modified
 def _strtobool(val: str) -> bool:
     """Convert a string representation of truth to true (1) or false (0).
 
     True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
     are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
@@ -92,26 +84,28 @@
         super().__init__(parent)
         self._ui = Ui_RecipeWindow()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         try:
             self._git_repository: typing.Optional[git.Repo] = git.Repo(
                 path, search_parent_directories=True
             )
+        except NameError:
+            self._git_repository = None
         except git.exc.InvalidGitRepositoryError:  # type: ignore
             self._git_repository = None
         self._ui.paneSplitter.setStretchFactor(0, 4)
         self._ui.paneSplitter.setStretchFactor(1, 1)
         self._ui.outputPane.customContextMenuRequested.connect(self._pane_context_menu)
         self._ui.errorPane.customContextMenuRequested.connect(self._pane_context_menu)
         self._empty_widget = QtWidgets.QWidget(self)
         self._empty_widget.setFixedSize(0, 0)
         self._disable_delete_on_default_output_tab()
         self._ui.pane_tabs.tabCloseRequested.connect(self._on_tab_close_request)
 
-        self._find_shortcut = QShortcut(QtGui.QKeySequence("Ctrl+F"), self)
+        self._find_shortcut = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+F"), self)
         self._find_shortcut.setContext(QtCore.Qt.WidgetWithChildrenShortcut)
         self._find_shortcut.activated.connect(self._open_find_dialog)
         with GeneralSettingsReader() as settings:
             combine_panes = settings.combine_panes.resolve()
             use_batching = settings.use_stdout_batching.resolve()
         self.combined_output_and_error_logs = combine_panes
         if self.combined_output_and_error_logs:
@@ -147,93 +141,107 @@
         # as the connected slots are so heavy weight that
         # user responsiveness on typing to the widgets is very bad
         # common subdir
         self._ui.localWorkflowCommonSubdir.editingFinished.connect(
             self._local_workflow_update_common_subdir
         )
         trash_icon = self.style().standardIcon(QtWidgets.QStyle.SP_TrashIcon)
-        self._local_workflow_common_subdir_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_common_subdir_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_common_subdir_trash_action.setToolTip("Delete folder")
         self._local_workflow_common_subdir_trash_action.triggered.connect(
             self._local_workflow_on_delete_common_subdir
         )
         self._ui.localWorkflowCommonSubdir.addAction(
             self._local_workflow_common_subdir_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # install command
         self._ui.localWorkflowInstallFolder.editingFinished.connect(
             self._local_workflow_update_install_folder
         )
-        self._local_workflow_install_folder_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_install_folder_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_install_folder_trash_action.setToolTip("Delete folder")
         self._local_workflow_install_folder_trash_action.triggered.connect(
             self._local_workflow_on_delete_install_folder
         )
         self._ui.localWorkflowInstallFolder.addAction(
             self._local_workflow_install_folder_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # imports command
         self._ui.localWorkflowImportsFolder.editingFinished.connect(
             self._local_workflow_update_imports_folder
         )
-        self._local_workflow_imports_folder_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_imports_folder_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_imports_folder_trash_action.setToolTip("Delete folder")
         self._local_workflow_imports_folder_trash_action.triggered.connect(
             self._local_workflow_on_delete_imports_folder
         )
         self._ui.localWorkflowImportsFolder.addAction(
             self._local_workflow_imports_folder_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # source command
         self._ui.localWorkflowSourceFolder.editingFinished.connect(
             self._local_workflow_update_source_folder
         )
-        self._local_workflow_source_folder_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_source_folder_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_source_folder_trash_action.setToolTip("Delete folder")
         self._local_workflow_source_folder_trash_action.triggered.connect(
             self._local_workflow_on_delete_source_folder
         )
         self._ui.localWorkflowSourceFolder.addAction(
             self._local_workflow_source_folder_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # build command
         self._ui.localWorkflowBuildFolder.editingFinished.connect(
             self._local_workflow_update_build_folder
         )
-        self._local_workflow_build_folder_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_build_folder_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_build_folder_trash_action.setToolTip("Delete folder")
         self._local_workflow_build_folder_trash_action.triggered.connect(
             self._local_workflow_on_delete_build_folder
         )
         self._ui.localWorkflowBuildFolder.addAction(
             self._local_workflow_build_folder_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # package command
         self._ui.localWorkflowPackageFolder.editingFinished.connect(
             self._local_workflow_update_package_folder
         )
-        self._local_workflow_package_folder_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_package_folder_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_package_folder_trash_action.setToolTip("Delete folder")
         self._local_workflow_package_folder_trash_action.triggered.connect(
             self._local_workflow_on_delete_package_folder
         )
         self._ui.localWorkflowPackageFolder.addAction(
             self._local_workflow_package_folder_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         # test command
         self._ui.localWorkflowTestFolder.editingFinished.connect(
             self._local_workflow_update_test_folder
         )
-        self._local_workflow_test_folder_trash_action = QAction(trash_icon, "", self)
+        self._local_workflow_test_folder_trash_action = QtGui.QAction(
+            trash_icon, "", self
+        )
         self._local_workflow_test_folder_trash_action.setToolTip("Delete folder")
         self._local_workflow_test_folder_trash_action.triggered.connect(
             self._local_workflow_on_delete_test_folder
         )
         self._ui.localWorkflowTestFolder.addAction(
             self._local_workflow_test_folder_trash_action,
             QtWidgets.QLineEdit.TrailingPosition,
@@ -372,15 +380,15 @@
         return self.recipe.context.inspect_recipe(
             self.recipe.path, propagate_errors=True
         )
 
     def _get_options_from_recipe(
         self, attrs: typing.Dict[str, str]
     ) -> typing.List[typing.Tuple[str, typing.List[typing.Any], typing.Any]]:
-        options = attrs.get("options", None)
+        options = attrs.get("options")
         if not options:
             return []
         default_options = attrs["default_options"]
         if isinstance(default_options, (tuple, list)):
             as_dict = {}
             for entry in default_options:
                 key, value = entry.split("=")
@@ -451,15 +459,16 @@
         """
         Get a dict of tokens usable in expressions
         """
         recipe_attributes = self.get_recipe_attributes()
         with RecipeSettingsReader.from_recipe(self.recipe) as settings_recipe:
             profile = settings_recipe.profile.resolve()
         profile_meta = self.recipe.context.get_profile_meta(profile)
-        if os.path.isabs(profile):
+        profile_path = pathlib.Path(profile)
+        if profile_path.is_absolute():
             with NamedLocalCacheSettingsReader(
                 self.recipe.context.cache_name
             ) as settings_localcache:
                 extra_profile_dirs = (
                     settings_localcache.extra_profile_directories.resolve()
                 )
             extra_profile_dir_name = [
@@ -475,15 +484,15 @@
             profile_prefix = ""
 
         tokens = {
             "name": recipe_attributes["name"],
             # version is either in the attributes, or for version agnostic recipes,
             # check the recipe object
             "version": recipe_attributes["version"] or self.recipe.version,
-            "profile": f"{profile_prefix}{os.path.basename(profile)}",
+            "profile": f"{profile_prefix}{profile_path.name}",
             "build_type": profile_meta["settings"]["build_type"],
             "build_type_lc": profile_meta["settings"]["build_type"].lower(),
         }
         return tokens, r"(\${(.*?)})"
 
     def resolve_expression(
         self, expression: typing.Optional[str]
@@ -501,19 +510,19 @@
             else:
                 raise RuntimeError(
                     f"Unrecognised macro '{token}' found in '{expression}'"
                 )
         return expression
 
     def _update_window_title(self, attributes: typing.Dict[str, str]) -> None:
-        version_in_recipe = attributes.get("version", None)
+        version_in_recipe = attributes.get("version")
         if version_in_recipe is not None:
             self._ui.actionOpen_another_version.setEnabled(False)
         version = version_in_recipe or self.recipe.version
-        name = attributes.get("name", None)
+        name = attributes.get("name")
         if self.recipe.user:
             package = f"{name}/{version}@{self.recipe.user}/{self.recipe.channel}"
         else:
             package = f"{name}/{version}"
         self.setWindowTitle(
             f"Package: {package} - Local cache: {self.recipe.context.cache_name}"
         )
@@ -573,15 +582,15 @@
 
             self._git_workspace_label.setText(message)
             if tooltip:
                 self._git_workspace_label.setToolTip(tooltip)
 
     def _on_git_context_menu(self, position: QtCore.QPoint) -> None:
         menu = QtWidgets.QMenu(self)
-        fetch_action = QAction("Fetch", self)
+        fetch_action = QtGui.QAction("Fetch", self)
         fetch_action.triggered.connect(self._fetch_git_repository)
         menu.addAction(fetch_action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _fetch_git_repository(self) -> None:
         assert self._git_repository
         for remote in self._git_repository.remotes:
@@ -977,15 +986,15 @@
         # Note: this does appear to get called twice, which also appears to be a bug
         # https://stackoverflow.com/questions/26782211/qlineedit-editingfinished-signal-twice-when-changing-focus
         text = self.sender().text()
         settings = RecipeSettings()
         if text:
             regex = self.sender().validator().regularExpression()
             matches = regex.match(text)
-            assert 3 == matches.lastCapturedIndex()
+            assert matches.lastCapturedIndex() == 3
             user = matches.captured(2)
             channel = matches.captured(3)
             settings.append_attribute(
                 {"user": user, "channel": channel}  # type: ignore
             )
         else:
             settings.append_attribute({"user": None, "channel": None})  # type: ignore
@@ -1000,15 +1009,15 @@
             script_args = [str(self.recipe.path)]
             QtCore.QProcess.execute(recipe_editor, script_args)
         else:
             url = QtCore.QUrl.fromLocalFile(str(self.recipe.path))
             QtGui.QDesktopServices.openUrl(url)
 
     def _open_recipe_folder(self) -> None:
-        reveal_on_filesystem(str(self.recipe.folder))
+        reveal_on_filesystem(self.recipe.folder)
 
     def _copy_recipe_folder_to_clipboard(self) -> None:
         QtWidgets.QApplication.clipboard().setText(str(self.recipe.folder))
 
     def _open_another_version(self) -> None:
         # TODO: note the last argument to this is the wrong type
         cruiz.globals.get_main_window().load_recipe(self.recipe.path, None, self)
@@ -1029,15 +1038,15 @@
         self._ui.configurePackageId.setText("Calculating...")
         # https://stackoverflow.com/questions/46630185/qt-remove-model-from-view
         self._ui.dependenciesPackageList.setModel(None)  # type: ignore[arg-type]
         self._ui.dependencyView.clear()
         # calculate lock file
         params = CommandParameters("lock create", cruiz.workers.lockcreate.invoke)
         params.recipe_path = self.recipe.path
-        params.name = recipe_attributes.get("name", None)
+        params.name = recipe_attributes.get("name")
         params.version = self.recipe.version
         params.user = self.recipe.user
         params.channel = self.recipe.channel
         with RecipeSettingsReader.from_recipe(self.recipe) as settings:
             params.profile = settings.profile.resolve()
             for key, value in settings.options.resolve().items():
                 # TODO: is this the most efficient algorithm?
@@ -1058,26 +1067,29 @@
                 self._visualise_dependencies(self._ui.dependency_rankdir.currentIndex())
             except FileNotFoundError as exc:
                 exception = exc
                 # fall through
         if exception:
             if payload is None:
                 self._ui.configurePackageId.setText("Failed")
+                self._dependency_graph = None
             lines = str(exception).splitlines()
             html = ""
             for line in lines:
                 stripped_line = line.lstrip()
                 num_leading_spaces = len(line) - len(stripped_line)
                 html += "&nbsp;" * num_leading_spaces + stripped_line + "<br>"
             self._dependency_generate_log.stderr(
                 f"Exception raised from running command:<br>"
                 f"<font color='red'>{html}</font><br>"
             )
 
     def _visualise_dependencies(self, rank_dir_index: int) -> None:
+        if self._dependency_graph is None:
+            return
         # list visualisation of dependencies
         self._dependencies_list_model = DependenciesListModel(self._dependency_graph)
         self._ui.dependenciesPackageList.setModel(self._dependencies_list_model)
         # tree visualisation of dependencies (DISABLED)
         self._dependencies_tree_model = DependenciesTreeModel(self._dependency_graph)
         self._ui.dependenciesPackageTree.setModel(self._dependencies_tree_model)
         # graphical visualisation of dependencies
@@ -1128,33 +1140,33 @@
         self._ui.conanLocalWorkflowDock.setEnabled(True)
         self._ui.behaviourToolbar.setEnabled(True)
         self._ui.buildFeaturesToolbar.setEnabled(True)
 
     def _pane_context_menu(self, position: QtCore.QPoint) -> None:
         menu = self.sender().createStandardContextMenu(position)
         menu.addSeparator()
-        find_action = QAction("Find...", self)
+        find_action = QtGui.QAction("Find...", self)
         find_action.setShortcut(self._find_shortcut.key())
         find_action.setShortcutVisibleInContextMenu(True)
         find_action.setData(self.sender())
         find_action.triggered.connect(self._open_find_dialog)
         menu.addAction(find_action)
         menu.addSeparator()
-        clear_action = QAction("Clear", self)
+        clear_action = QtGui.QAction("Clear", self)
         clear_action.triggered.connect(self.sender().clear)
         menu.addAction(clear_action)
         menu.addSeparator()
-        pin_action = QAction("Pin to tab", self)
+        pin_action = QtGui.QAction("Pin to tab", self)
         pin_action.triggered.connect(self._pin_current_output)
         pin_action.setEnabled(self._ui.pane_tabs.count() == 1)
         menu.addAction(pin_action)
         menu.exec_(self.sender().viewport().mapToGlobal(position))
 
     def _open_find_dialog(self) -> None:
-        if isinstance(self.sender(), QShortcut):
+        if isinstance(self.sender(), QtGui.QShortcut):
             pane = QtWidgets.QApplication.focusWidget()
         else:
             pane = self.sender().data()
         if isinstance(pane, QtWidgets.QPlainTextEdit):
             dialog = FindTextDialog(pane)
             dialog.search_forwards.connect(self._find_next)
             dialog.search_backwards.connect(self._find_prev)
@@ -1188,55 +1200,57 @@
         result = pane.find(pattern, flags)
         if not result and wrap_around:
             pane.moveCursor(QtGui.QTextCursor.End)
             result = pane.find(pattern, flags)
 
     def _dependency_list_context_menu(self, position: QtCore.QPoint) -> None:
         menu = QtWidgets.QMenu(self)
-        open_package_dir_action = QAction("Open package directory", self)
+        open_package_dir_action = QtGui.QAction("Open package directory", self)
         open_package_dir_action.triggered.connect(self._open_package_directory)
         menu.addAction(open_package_dir_action)
-        copy_package_dir_action = QAction("Copy package directory to clipboard", self)
+        copy_package_dir_action = QtGui.QAction(
+            "Copy package directory to clipboard", self
+        )
         copy_package_dir_action.triggered.connect(self._copy_package_directory)
         menu.addAction(copy_package_dir_action)
-        what_uses_this_action = QAction("What uses this?...", self)
+        what_uses_this_action = QtGui.QAction("What uses this?...", self)
         what_uses_this_action.triggered.connect(self._on_what_uses_this)
         menu.addAction(what_uses_this_action)
         menu.exec_(self._ui.dependenciesPackageList.mapToGlobal(position))
 
-    def _get_package_directory_of_current_dependency(self) -> str:
+    def _get_package_directory_of_current_dependency(self) -> pathlib.Path:
         index = self._ui.dependenciesPackageList.currentIndex()
         node = index.data(QtCore.Qt.UserRole)
         return self.recipe.context.get_package_directory(node)
 
     def _open_package_directory(self) -> None:
         directory = self._get_package_directory_of_current_dependency()
-        if os.path.isdir(directory):
+        if directory.is_dir():
             cruiz.revealonfilesystem.reveal_on_filesystem(directory)
         else:
             QtWidgets.QMessageBox.critical(
                 self,
                 "No such package directory",
                 f"Package directory '{directory}' does not exist",
             )
 
     def _copy_package_directory(self) -> None:
         directory = self._get_package_directory_of_current_dependency()
-        QtWidgets.QApplication.clipboard().setText(directory)
+        QtWidgets.QApplication.clipboard().setText(os.fspath(directory))
 
     def _on_what_uses_this(self) -> None:
         index = self._ui.dependenciesPackageList.currentIndex()
         node = index.data(QtCore.Qt.UserRole)
         new_graph = dependencygraph_from_node_dependees(node)
         InverseDependencyViewDialog(new_graph).exec_()
 
     def _dependents_log_context_menu(self, position: QtCore.QPoint) -> None:
         menu = self.sender().createStandardContextMenu(position)
         menu.addSeparator()
-        clear_action = QAction("Clear", self)
+        clear_action = QtGui.QAction("Clear", self)
         clear_action.triggered.connect(self._clear_dependents_log)
         menu.addAction(clear_action)
         menu.exec_(self.sender().viewport().mapToGlobal(position))
 
     def _clear_dependents_log(self) -> None:
         self._ui.dependentsLog.clear()
         self._ui.dependentsLog.hide()
@@ -1320,15 +1334,15 @@
         can be updated
         """
         if cache_name != self.recipe.context.cache_name:
             return
         self._ui.behaviourToolbar.refresh_content()
 
     def _on_configure_packageid_context_menu(self, position: QtCore.QPoint) -> None:
-        action = QAction("Copy to clipboard", self)
+        action = QtGui.QAction("Copy to clipboard", self)
         action.triggered.connect(self._on_configure_package_id_copy)
         menu = QtWidgets.QMenu(self)
         menu.addAction(action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_configure_package_id_copy(self) -> None:
         QtWidgets.QApplication.clipboard().setText(self._ui.configurePackageId.text())
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/toolbars/behaviour.py` & `cruiz-1.4.0a1/cruiz/recipe/toolbars/behaviour.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 """
 Recipe behaviour toolbar
 """
 
 import os
 import pathlib
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.recipe_profile_frame import Ui_profileFrame
-    from cruiz.pyside2.recipe_cpucores_frame import Ui_cpuCoresFrame
-else:
-    from cruiz.pyside6.recipe_profile_frame import Ui_profileFrame
-    from cruiz.pyside6.recipe_cpucores_frame import Ui_cpuCoresFrame
+from cruiz.pyside6.recipe_profile_frame import Ui_profileFrame
+from cruiz.pyside6.recipe_cpucores_frame import Ui_cpuCoresFrame
 
 from cruiz.widgets.util import BlockSignals
 
 from cruiz.settings.managers.recipe import (
     RecipeSettings,
     RecipeSettingsReader,
     RecipeSettingsWriter,
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/toolbars/buildfeatures.py` & `cruiz-1.4.0a1/cruiz/recipe/toolbars/buildfeatures.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,34 @@
 
 """
 Build features toolbar
 """
 
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.constants import CompilerCacheTypes
 
 from cruiz.settings.managers.recipe import (
     RecipeSettingsReader,
     RecipeSettings,
     RecipeSettingsWriter,
 )
 from cruiz.settings.managers.compilercachepreferences import CompilerCacheSettingsReader
 
 from cruiz.widgets.util import BlockSignals
 
-if PYSIDE2:
-    from cruiz.pyside2.recipe_cmake_features_frame import Ui_cmakeFeaturesFrame
-    from cruiz.pyside2.recipe_compilercache_features_frame import (
-        Ui_compilerCacheFrame,
-    )
-    from cruiz.pyside2.recipe_compiler_cache_configuration_dialog import (
-        Ui_CompilerCacheConfigurationDialog,
-    )
-else:
-    from cruiz.pyside6.recipe_cmake_features_frame import Ui_cmakeFeaturesFrame
-    from cruiz.pyside6.recipe_compilercache_features_frame import (
-        Ui_compilerCacheFrame,
-    )
-    from cruiz.pyside6.recipe_compiler_cache_configuration_dialog import (
-        Ui_CompilerCacheConfigurationDialog,
-    )
+from cruiz.pyside6.recipe_cmake_features_frame import Ui_cmakeFeaturesFrame
+from cruiz.pyside6.recipe_compilercache_features_frame import (
+    Ui_compilerCacheFrame,
+)
+from cruiz.pyside6.recipe_compiler_cache_configuration_dialog import (
+    Ui_CompilerCacheConfigurationDialog,
+)
 
 
 class _CMakeFeaturesFrame(QtWidgets.QFrame):
     def __init__(self, parent: typing.Optional[QtWidgets.QWidget] = None) -> None:
         super().__init__(parent)
         self._ui = Ui_cmakeFeaturesFrame()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
```

### Comparing `cruiz-1.3.2b1/cruiz/recipe/toolbars/command.py` & `cruiz-1.4.0a1/cruiz/recipe/toolbars/command.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/pages/packagebinarypage.py` & `cruiz-1.4.0a1/cruiz/remote_browser/pages/packagebinarypage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,21 @@
 import html
 import pathlib
 import shutil
 import tarfile
 import tempfile
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
-if PYSIDE2:
-    from qtpy import QtWebEngineWidgets
-
-    QAction = QtWidgets.QAction
-else:
-    from qtpy import QtWebEngineCore
-
-    QAction = QtGui.QAction
+from qtpy import QtWebEngineCore
 
 from cruiz.interop.packagebinaryparameters import PackageBinaryParameters
 
-if PYSIDE2:
-    from cruiz.pyside2.remote_browser_fileview import Ui_remote_browser_fileview
-else:
-    from cruiz.pyside6.remote_browser_fileview import Ui_remote_browser_fileview
+from cruiz.pyside6.remote_browser_fileview import Ui_remote_browser_fileview
 
 from cruiz.settings.managers.generalpreferences import GeneralSettingsReader
 
 from .page import Page
 
 
 class _FileNode:
@@ -155,39 +145,43 @@
         if not parent.isValid():
             return super().createIndex(row, column, self._root)
         parent_node = parent.internalPointer()
         node = parent_node.children[row]
         return super().createIndex(row, column, node)
 
     def headerData(self, section, orientation, role):  # type: ignore
-        if role == QtCore.Qt.DisplayRole and orientation == QtCore.Qt.Horizontal:
-            if section == 0:
-                return "Path"
+        if (
+            role == QtCore.Qt.DisplayRole
+            and orientation == QtCore.Qt.Horizontal
+            and section == 0
+        ):
+            return "Path"
         return None
 
     def data(self, index, role):  # type: ignore
         node = index.internalPointer()
-        if role == QtCore.Qt.DisplayRole:
-            if index.column() == 0:
-                return pathlib.Path(node.path).name
-        if role == QtCore.Qt.ToolTipRole:
-            if index.column() == 0:
-                if node.is_file and node.link_target:
-                    return f"Symbolic link to {node.link_target}"
-        if role == QtCore.Qt.DecorationRole:
-            if index.column() == 0:
-                if node.is_file:
-                    if node.link_target:
-                        return self._parent_object.style().standardIcon(
-                            QtWidgets.QStyle.SP_FileLinkIcon
-                        )
-                else:
-                    return QtWidgets.QFileIconProvider().icon(
-                        QtWidgets.QFileIconProvider.Folder
+        if role == QtCore.Qt.DisplayRole and index.column() == 0:
+            return pathlib.Path(node.path).name
+        if (
+            role == QtCore.Qt.ToolTipRole
+            and index.column() == 0
+            and node.is_file
+            and node.link_target
+        ):
+            return f"Symbolic link to {node.link_target}"
+        if role == QtCore.Qt.DecorationRole and index.column() == 0:
+            if node.is_file:
+                if node.link_target:
+                    return self._parent_object.style().standardIcon(
+                        QtWidgets.QStyle.SP_FileLinkIcon
                     )
+            else:
+                return QtWidgets.QFileIconProvider().icon(
+                    QtWidgets.QFileIconProvider.Folder
+                )
         return None
 
     def flags(self, index):  # type: ignore
         default_flags = super().flags(index)
         node = index.internalPointer()
         if node.link_target:
             return default_flags & ~QtCore.Qt.ItemIsEnabled  # type: ignore[operator]
@@ -201,23 +195,17 @@
         path: pathlib.Path,
         container: pathlib.Path,
         parent: typing.Optional[QtWidgets.QWidget] = None,
     ) -> None:
         super().__init__(parent)
         self._ui = Ui_remote_browser_fileview()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
-        if PYSIDE2:
-            self._ui.fileview.page().settings().setAttribute(
-                QtWebEngineWidgets.QWebEngineSettings.LocalContentCanAccessRemoteUrls,
-                True,
-            )
-        else:
-            self._ui.fileview.page().settings().setAttribute(
-                QtWebEngineCore.QWebEngineSettings.LocalContentCanAccessRemoteUrls, True
-            )
+        self._ui.fileview.page().settings().setAttribute(
+            QtWebEngineCore.QWebEngineSettings.LocalContentCanAccessRemoteUrls, True
+        )
         if container:
             html_path = _FileViewer._write_html(path, root / container)
             self.setWindowTitle(f"{path} in {container}")
         else:
             html_path = _FileViewer._write_html(root / path, None)
             self.setWindowTitle(str(path))
         self._ui.fileview.load(QtCore.QUrl.fromLocalFile(str(html_path)))
@@ -225,26 +213,26 @@
     @staticmethod
     def _write_html(
         path: pathlib.PurePath, archive: typing.Optional[pathlib.Path]
     ) -> pathlib.Path:
         if archive:
             with tarfile.open(archive, "r") as tar:
                 tar.extract(str(path), path=archive.parent)
-            with open(archive.parent / path, "rt", encoding="utf-8") as data_file:
+            with (archive.parent / path).open("rt", encoding="utf-8") as data_file:
                 contents = data_file.readlines()
             html_path = archive.parent / path
             html_path = html_path.with_suffix(".html")
         else:
-            with open(path, "rt", encoding="utf-8") as data_file:
+            with path.open("rt", encoding="utf-8") as data_file:
                 contents = data_file.readlines()
             html_path = pathlib.Path(path.with_suffix(".html"))
         html_path.parent.mkdir(parents=True, exist_ok=True)
         with GeneralSettingsReader() as settings:
             use_dark_mode = settings.use_dark_mode.resolve()
-        with open(html_path, "wt", encoding="utf-8") as html_file:
+        with html_path.open("wt", encoding="utf-8") as html_file:
             url_start = "https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.4.0"
             html_file.write("<html>")
             html_file.write("<head>")
             if use_dark_mode:
                 html_file.write(
                     f'<link rel="stylesheet" href="{url_start}/styles/dark.min.css">'
                 )
@@ -369,36 +357,37 @@
         self._open_start()
 
     def _on_copy_pkgref_to_clip(self) -> None:
         QtWidgets.QApplication.clipboard().setText(self._ui.pbinary_pkgref.text())
 
     def _on_file_menu(self, position: QtCore.QPoint) -> None:
         selection = self._ui.package_binary.selectedIndexes()
-        assert 1 == len(selection)
+        assert len(selection) == 1
         node = selection[0].internalPointer()
         if not node.is_file:
             return
         if node.link_target:
             return
         menu = QtWidgets.QMenu(self)
-        save_action = QAction("Save ...", self)
+        save_action = QtGui.QAction("Save ...", self)
         save_action.triggered.connect(self._on_file_save)
         menu.addAction(save_action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_file_save(self) -> None:
         selection = self._ui.package_binary.selectedIndexes()
-        assert 1 == len(selection)
+        assert len(selection) == 1
         node = selection[0].internalPointer()
         new_path, _ = QtWidgets.QFileDialog.getSaveFileName(
             self, f"Save {node.path} from package", "", ""
         )
         if not new_path:
             return
         if node.container:
             with tarfile.open(self._artifact_folder / node.container, "r") as tar:
                 contents_object = tar.extractfile(node.tar_info)
                 assert contents_object
-                with open(new_path, "wb") as writer:
+                new_path_path = pathlib.Path(new_path)
+                with new_path_path.open("wb") as writer:
                     writer.write(contents_object.read())
         else:
             shutil.copyfile(self._artifact_folder / node.path, new_path)
```

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/pages/packageidpage.py` & `cruiz-1.4.0a1/cruiz/remote_browser/pages/packageidpage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 
 """
 Remote browser page
 """
 
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
-
-if PYSIDE2:
-    QAction = QtWidgets.QAction
-else:
-    QAction = QtGui.QAction
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.interop.packageidparameters import PackageIdParameters
 from cruiz.widgets.util import BlockSignals
 
 from .page import Page
 
 
@@ -174,15 +169,15 @@
     def data(self, index, role):  # type: ignore
         if role == QtCore.Qt.DisplayRole:
             return self._filters[index.row()][index.column() + 1]
         return None
 
     def headerData(self, section, orientation, role):  # type: ignore
         if role == QtCore.Qt.DisplayRole and orientation == QtCore.Qt.Horizontal:
-            if 0 == section:
+            if section == 0:
                 return "Key"
             return "Value"
         return None
 
 
 class _PackageIdSortFilterProxyModel(QtCore.QSortFilterProxyModel):
     def __init__(self, model: _PackageIdModel, filtering: _FilteringModel) -> None:
@@ -359,48 +354,48 @@
         QtWidgets.QApplication.clipboard().setText(self._ui.pid_pkgref.text())
 
     def _on_package_id_header_menu(self, position: QtCore.QPoint) -> None:
         menu = QtWidgets.QMenu(self)
         offset = 1
         assert self._model._settings
         for i, s in enumerate(self._model._settings):
-            action = QAction(s, self)
+            action = QtGui.QAction(s, self)
             action.setCheckable(True)
             action.setData(i + offset)
             action.setChecked(not self._ui.package_ids.isColumnHidden(i + offset))
             action.toggled.connect(self._on_toggle_hide_column)
             menu.addAction(action)
         menu.addSeparator()
         offset = 1 + len(self._model._settings)
         assert self._model._options
         for i, o in enumerate(self._model._options):
-            action = QAction(o, self)
+            action = QtGui.QAction(o, self)
             action.setData(i + offset)
             action.setCheckable(True)
             action.setChecked(not self._ui.package_ids.isColumnHidden(i + offset))
             action.toggled.connect(self._on_toggle_hide_column)
             menu.addAction(action)
         menu.addSeparator()
         offset = 1 + len(self._model._settings) + len(self._model._options)
-        action = QAction("Requires", self)
+        action = QtGui.QAction("Requires", self)
         action.setData(offset)
         action.setCheckable(True)
         action.setChecked(not self._ui.package_ids.isColumnHidden(offset))
         action.toggled.connect(self._on_toggle_hide_column)
         menu.addAction(action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_toggle_hide_column(self, checked: bool) -> None:
         action = self.sender()
         self._ui.package_ids.setColumnHidden(action.data(), not checked)
 
     def _on_pid_filter_changed(self, text: str) -> None:
         self._ui.pid_filter_value.setEnabled(True)
         assert self._model._settings
-        if 0 == self.sender().currentIndex():
+        if self.sender().currentIndex() == 0:
             with BlockSignals(self._ui.pid_filter_value) as blocked_widget:
                 blocked_widget.clear()
                 assert self._model._pids
                 for pid in self._model._pids:
                     blocked_widget.addItem(pid["id"])
                 blocked_widget.setCurrentIndex(-1)
         elif self.sender().currentIndex() < len(self._model._settings) + 1:
@@ -428,15 +423,15 @@
         self._sorting_model.invalidateFilter()
         self._populate_settings_options_filter()
 
     def _on_pid_filter_menu(self, position: QtCore.QPoint) -> None:
         if not self.sender().selectionModel().selectedRows():
             return
         menu = QtWidgets.QMenu(self)
-        remove_action = QAction("Remove", self)
+        remove_action = QtGui.QAction("Remove", self)
         remove_action.triggered.connect(self._on_pid_filter_remove)
         menu.addAction(remove_action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_pid_filter_remove(self) -> None:
         selected_row_index = (
             self._ui.pid_filterTable.selectionModel().selectedRows()[0].row()
```

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/pages/packagereferencepage.py` & `cruiz-1.4.0a1/cruiz/remote_browser/pages/packagereferencepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
     @property
     def package_reference(self) -> str:
         """
         Get the package reference selected on this page
         """
         selection = self._ui.package_references.selectedIndexes()
-        assert 1 == len(selection)
+        assert len(selection) == 1
         return self._model.data(selection[0], QtCore.Qt.DisplayRole)
 
     def on_local_cache_change(self, text: str) -> None:
         """
         Called when which local cache has been selected has changed
         """
         self._context.change_cache(text)
```

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/pages/packagerevisionpage.py` & `cruiz-1.4.0a1/cruiz/remote_browser/pages/packagerevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/pages/page.py` & `cruiz-1.4.0a1/cruiz/remote_browser/pages/page.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 
 """
 Remote browser page
 """
 
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
-
-if PYSIDE2:
-    QAction = QtWidgets.QAction
-else:
-    QAction = QtGui.QAction
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.commands.context import ConanContext
 from cruiz.commands.logdetails import LogDetails
 
 
 class Page(QtWidgets.QWidget):
     """
@@ -44,22 +39,22 @@
     def _revisions_enabled(self) -> bool:
         stacked_widget = self.parent()
         pkgref_page = stacked_widget.widget(0)
         return pkgref_page._revs_enabled
 
     def _on_pkgref_menu(self, position: QtCore.QPoint) -> None:
         menu = QtWidgets.QMenu(self)
-        copy_action = QAction("Copy to clipboard", self)
+        copy_action = QtGui.QAction("Copy to clipboard", self)
         copy_action.triggered.connect(self._on_copy_pkgref_to_clip)
         menu.addAction(copy_action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_selected_pkgref_menu(self, position: QtCore.QPoint) -> None:
         menu = QtWidgets.QMenu(self)
-        copy_action = QAction("Copy to clipboard", self)
+        copy_action = QtGui.QAction("Copy to clipboard", self)
         copy_action.triggered.connect(self._on_copy_selected_pkgref_to_clip)
         menu.addAction(copy_action)
         menu.exec_(self.sender().mapToGlobal(position))
 
     def _on_copy_selected_pkgref_to_clip(self) -> None:
         QtWidgets.QApplication.clipboard().setText(self.package_reference)
```

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/pages/reciperevisionpage.py` & `cruiz-1.4.0a1/cruiz/remote_browser/pages/reciperevisionpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     @property
     def package_reference(self) -> str:
         """
         Get the package reference for the selection on this page
         """
         selection = self._ui.recipe_revisions.selectedIndexes()
-        assert 2 == len(selection)  # num columns in row
+        assert len(selection) == 2  # num columns in row
         rrev = self._model.data(selection[0], QtCore.Qt.DisplayRole)
         return f"{self._previous_pkgref}#{rrev}"
 
     def _enable_progress(self, enable: bool) -> None:
         self._ui.rrev_progress.setMaximum(0 if enable else 1)
         self._ui.rrev_buttons.setEnabled(not enable)
         self._ui.rrev_cancel.setEnabled(enable)
```

### Comparing `cruiz-1.3.2b1/cruiz/remote_browser/remotebrowser.py` & `cruiz-1.4.0a1/cruiz/remote_browser/remotebrowser.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,17 @@
 """
 Remote browser
 """
 
 import logging
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
-if PYSIDE2:
-    from cruiz.pyside2.remote_browser import Ui_remotebrowser
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.remote_browser import Ui_remotebrowser
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.remote_browser import Ui_remotebrowser
 
 from cruiz.commands.context import ConanContext
 from cruiz.commands.logdetails import LogDetails
 from cruiz.constants import DEFAULT_CACHE_NAME
 
 logger = logging.getLogger(__name__)
 
@@ -81,15 +74,15 @@
             self._ui.pkgref.on_local_cache_change(cache_name)
             self._ui.stackedWidget.setCurrentWidget(self._ui.pkgref)
             self._clear_log()
 
     def _log_context_menu(self, position: QtCore.QPoint) -> None:
         menu = self.sender().createStandardContextMenu(position)
         menu.addSeparator()
-        clear_action = QAction("Clear", self)
+        clear_action = QtGui.QAction("Clear", self)
         clear_action.triggered.connect(self._clear_log)
         menu.addAction(clear_action)
         menu.exec_(self.sender().viewport().mapToGlobal(position))
 
     def _clear_log(self) -> None:
         self._ui.log.clear()
         self._ui.log.hide()
```

### Comparing `cruiz-1.3.2b1/cruiz/resourcegeneration.py` & `cruiz-1.4.0a1/cruiz/resourcegeneration.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 import logging
 import os
 import pathlib
 import platform
 import subprocess
 import typing
 
-from qtpy import PYSIDE2
-
-if PYSIDE2:
-    SUBDIR = "pyside2"
-    RCC = "pyside2-rcc"
-    UIC = "pyside2-uic"
-else:
-    SUBDIR = "pyside6"
-    RCC = "pyside6-rcc"
-    UIC = "pyside6-uic"
+SUBDIR = "pyside6"
+RCC = "pyside6-rcc"
+UIC = "pyside6-uic"
 
 
 logger = logging.getLogger(__name__)
 
 
 def _run_command_if_out_of_date(
     input: pathlib.Path, output: pathlib.Path, cmd_args: typing.List[str]
```

### Comparing `cruiz-1.3.2b1/cruiz/resources/001-rubbish.svg` & `cruiz-1.4.0a1/cruiz/resources/001-rubbish.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/002-null.svg` & `cruiz-1.4.0a1/cruiz/resources/002-null.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/003-chemistry.svg` & `cruiz-1.4.0a1/cruiz/resources/003-chemistry.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/004-share.svg` & `cruiz-1.4.0a1/cruiz/resources/004-share.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/005-box.svg` & `cruiz-1.4.0a1/cruiz/resources/005-box.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/006-toolbox.svg` & `cruiz-1.4.0a1/cruiz/resources/006-toolbox.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/007-book.svg` & `cruiz-1.4.0a1/cruiz/resources/007-book.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/008-cloud-computing.svg` & `cruiz-1.4.0a1/cruiz/resources/008-cloud-computing.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/009-import.svg` & `cruiz-1.4.0a1/cruiz/resources/009-import.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/010-draw.svg` & `cruiz-1.4.0a1/cruiz/resources/010-draw.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/012-hammer.svg` & `cruiz-1.4.0a1/cruiz/resources/012-hammer.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/013-pencil.svg` & `cruiz-1.4.0a1/cruiz/resources/013-pencil.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/014-code.svg` & `cruiz-1.4.0a1/cruiz/resources/014-code.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/Cmake.svg` & `cruiz-1.4.0a1/cruiz/resources/Cmake.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/about_dialog.ui` & `cruiz-1.4.0a1/cruiz/resources/about_dialog.ui`

 * *Files 8% similar despite different names*

#### Comparing `cruiz-1.3.2b1/cruiz/resources/about_dialog.ui` & `cruiz-1.4.0a1/cruiz/resources/about_dialog.ui`

```diff
@@ -19,50 +19,50 @@
     <layout class="QGridLayout" name="gridLayout">
       <property name="sizeConstraint">
         <enum>QLayout::SetFixedSize</enum>
       </property>
       <item row="2" column="1">
         <widget class="QLabel" name="label_4">
           <property name="text">
-            <string>Author: Mark Final (c) 2020-2022</string>
+            <string>Author: Mark Final (c) 2020-2023</string>
           </property>
         </widget>
       </item>
       <item row="0" column="1">
         <widget class="QLabel" name="label_2">
           <property name="text">
             <string>cruiz: Conan recipe user interface</string>
           </property>
         </widget>
       </item>
       <item row="3" column="1">
         <widget class="QLabel" name="python">
           <property name="text">
-            <string>Python executable:</string>
+            <string>Python executable: unknown</string>
           </property>
         </widget>
       </item>
       <item row="1" column="1">
         <widget class="QLabel" name="version">
           <property name="text">
-            <string>Version:</string>
+            <string>Version: unknown</string>
           </property>
         </widget>
       </item>
       <item row="4" column="1">
         <widget class="QLabel" name="python_version">
           <property name="text">
-            <string>Python version:</string>
+            <string>Python version: unknown</string>
           </property>
         </widget>
       </item>
       <item row="5" column="1">
         <widget class="QLabel" name="pyside_version">
           <property name="text">
-            <string>PySide2 version:</string>
+            <string>PySide version: unknown</string>
           </property>
         </widget>
       </item>
       <item row="0" column="0" rowspan="6">
         <widget class="QLabel" name="cruiz">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
```

### Comparing `cruiz-1.3.2b1/cruiz/resources/cruise.png` & `cruiz-1.4.0a1/cruiz/resources/cruise.png`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/cruizres.qrc` & `cruiz-1.4.0a1/cruiz/resources/cruizres.qrc`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/find_text_dialog.ui` & `cruiz-1.4.0a1/cruiz/resources/find_text_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/license-cruise.pdf` & `cruiz-1.4.0a1/cruiz/resources/license-cruise.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/license.pdf` & `cruiz-1.4.0a1/cruiz/resources/license.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/load_recipe_wizard.ui` & `cruiz-1.4.0a1/cruiz/resources/load_recipe_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_add_environment.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_add_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_add_profile_directory.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_add_profile_directory.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_add_remote.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_add_remote.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_install_config.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_install_config.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_manage.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_manage.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_move.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_move.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_new_wizard.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_new_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_remove_environment.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_remove_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/local_cache_run_command_dialog.ui` & `cruiz-1.4.0a1/cruiz/resources/local_cache_run_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/preferences.ui` & `cruiz-1.4.0a1/cruiz/resources/preferences.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_cmake_features_frame.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_cmake_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_compilercache_features_frame.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_compilercache_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_cpucores_frame.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_cpucores_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_local_workflow_expression_editor.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_local_workflow_expression_editor.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_profile_frame.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_profile_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/recipe_window.ui` & `cruiz-1.4.0a1/cruiz/resources/recipe_window.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/remote_browser.ui` & `cruiz-1.4.0a1/cruiz/resources/remote_browser.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/resources/remote_browser_fileview.ui` & `cruiz-1.4.0a1/cruiz/resources/remote_browser_fileview.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/revealonfilesystem.py` & `cruiz-1.4.0a1/cruiz/revealonfilesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Based on the C++ code in
 https://github.com/qt-creator/qt-creator/blob/master/src/plugins/coreplugin/fileutils.cpp, # noqa: E501
 FileUtils::showInGraphicalShell
 """
 
 import os
+import pathlib
 import platform
 
 from qtpy import QtCore, QtWidgets
 
 
 def _run_apple_script(command: str) -> None:
     script_args = ["-e", command]
@@ -47,25 +48,24 @@
             "Unable to find the path to xdg-open",
         )
         return
     script_args = [file_info.canonicalFilePath()]
     QtCore.QProcess.startDetached(xdg_open_path, script_args)
 
 
-# TODO: pathlib instead?
-def reveal_on_filesystem(path: str) -> None:
+def reveal_on_filesystem(path: pathlib.Path) -> None:
     """
     Reveal the path in a filesystem GUI
     """
-    file_info = QtCore.QFileInfo(path)
-    if not file_info.exists():
+    if not path.exists():
         QtWidgets.QMessageBox.critical(
             None, "Cannot reveal path", f"Path '{path}' does not exist"  # type: ignore
         )
         return
+    file_info = QtCore.QFileInfo(path)
     if platform.system() == "Darwin":
         _use_finder(file_info)
     elif platform.system() == "Windows":
         _use_explorer(file_info)
     elif platform.system() == "Linux":
         _use_xdg_open(file_info)
     else:
```

### Comparing `cruiz-1.3.2b1/cruiz/settings/ensuredefaultlocalcache.py` & `cruiz-1.4.0a1/cruiz/settings/ensuredefaultlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/__init__.py` & `cruiz-1.4.0a1/cruiz/settings/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/basesettings.py` & `cruiz-1.4.0a1/cruiz/settings/managers/basesettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/cleansettings.py` & `cruiz-1.4.0a1/cruiz/settings/managers/cleansettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/cmakepreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/cmakepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/compilercachepreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/compilercachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/conanpreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/conanpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/fontpreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/fontpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/generalpreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/generalpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/graphvizpreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/graphvizpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/localcachepreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/localcachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/namedlocalcache.py` & `cruiz-1.4.0a1/cruiz/settings/managers/namedlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/ninjapreferences.py` & `cruiz-1.4.0a1/cruiz/settings/managers/ninjapreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/recentconanconfigs.py` & `cruiz-1.4.0a1/cruiz/settings/managers/recentconanconfigs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/recentconanremotes.py` & `cruiz-1.4.0a1/cruiz/settings/managers/recentconanremotes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/recentrecipes.py` & `cruiz-1.4.0a1/cruiz/settings/managers/recentrecipes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/recipe.py` & `cruiz-1.4.0a1/cruiz/settings/managers/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/shortcuts.py` & `cruiz-1.4.0a1/cruiz/settings/managers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/valueclasses.py` & `cruiz-1.4.0a1/cruiz/settings/managers/valueclasses.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/managers/writermixin.py` & `cruiz-1.4.0a1/cruiz/settings/managers/writermixin.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/models/recentconanconfigmodel.py` & `cruiz-1.4.0a1/cruiz/settings/models/recentconanconfigmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/models/recentconanremotesmodel.py` & `cruiz-1.4.0a1/cruiz/settings/models/recentconanremotesmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/settings/models/recipesmodel.py` & `cruiz-1.4.0a1/cruiz/settings/models/recipesmodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,13 +78,12 @@
                     self._uuids[index.row()]
                 ) as settings:
                     return settings.local_cache_name.resolve()
         return None
 
     def flags(self, index):  # type: ignore
         def_flags = super().flags(index)
-        if self._uuids:
-            if cruiz.globals.get_main_window().is_recipe_active(
-                self._uuids[index.row()]
-            ):
-                return def_flags & ~QtCore.Qt.ItemIsEnabled  # type: ignore[operator]
+        if self._uuids and cruiz.globals.get_main_window().is_recipe_active(
+            self._uuids[index.row()]
+        ):
+            return def_flags & ~QtCore.Qt.ItemIsEnabled  # type: ignore[operator]
         return def_flags
```

### Comparing `cruiz-1.3.2b1/cruiz/settings/preferencesdialog.py` & `cruiz-1.4.0a1/cruiz/settings/preferencesdialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 #!/usr/bin/env python3
 
 """
 Application settings utilities
 """
 
 import json
+import pathlib
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.settings.managers.namedlocalcache import NamedLocalCacheSettingsReader
 
-if PYSIDE2:
-    from cruiz.pyside2.preferences import Ui_PreferencesDialog
-
-    QAction = QtWidgets.QAction
-else:
-    from cruiz.pyside6.preferences import Ui_PreferencesDialog
-
-    QAction = QtGui.QAction
+from cruiz.pyside6.preferences import Ui_PreferencesDialog
 
 from cruiz.settings.managers.generalpreferences import (
     GeneralSettings,
     GeneralSettingsReader,
     GeneralSettingsWriter,
 )
 from cruiz.settings.managers.fontpreferences import (
@@ -230,28 +224,28 @@
         self._ui.prefs_general_enable_darkmode.stateChanged.connect(
             self._general_darkmode
         )
         self._ui.prefs_general_enable_compact.stateChanged.connect(
             self._general_compactlook
         )
         dir_icon = self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon)
-        open_recipedir_action = QAction(dir_icon, "", self)
+        open_recipedir_action = QtGui.QAction(dir_icon, "", self)
         open_recipedir_action.triggered.connect(self._general_open_recipedir)
         self._ui.prefs_general_default_recipe_dir.addAction(
             open_recipedir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.prefs_general_default_recipe_dir.textChanged.connect(
             self._general_recipedir
         )
         self._ui.prefs_general_busy_colour.clicked.connect(self._general_busyiconcolour)
         self._ui.prefs_general_found_text_background_colour.clicked.connect(
             self._general_foundtextbgroundcolour
         )
-        open_recipe_in_editor_action = QAction(dir_icon, "", self)
+        open_recipe_in_editor_action = QtGui.QAction(dir_icon, "", self)
         open_recipe_in_editor_action.triggered.connect(self._general_open_recipe_editor)
         self._ui.prefs_general_recipe_editor.addAction(
             open_recipe_in_editor_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.prefs_general_recipe_editor.textChanged.connect(
             self._general_recipe_editor
@@ -295,15 +289,15 @@
         )
 
     def _setup_graphviz_toolbox(self) -> None:
         self._prefs_graphviz = GraphVizSettings()
         self._ui.prefs_graphviz_bin_directory.textChanged.connect(
             self._graphviz_bin_directory_changed
         )
-        open_graphviz_bindir_action = QAction(
+        open_graphviz_bindir_action = QtGui.QAction(
             self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon), "", self
         )
         open_graphviz_bindir_action.triggered.connect(self._graphviz_open_bindir)
         self._ui.prefs_graphviz_bin_directory.addAction(
             open_graphviz_bindir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
@@ -311,24 +305,24 @@
     def _setup_cmake_toolbox(self) -> None:
         self._prefs_cmake = CMakeSettings()
         self._prefs_ninja = NinjaSettings()
         self._ui.prefs_cmake_cmake_bin_directory.textChanged.connect(
             self._cmake_bin_directory_changed
         )
         dir_icon = self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon)
-        open_cmake_bindir_action = QAction(dir_icon, "", self)
+        open_cmake_bindir_action = QtGui.QAction(dir_icon, "", self)
         open_cmake_bindir_action.triggered.connect(self._cmake_open_bindir)
         self._ui.prefs_cmake_cmake_bin_directory.addAction(
             open_cmake_bindir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.prefs_cmake_ninja_bin_directory.textChanged.connect(
             self._ninja_bin_directory_changed
         )
-        open_ninja_bindir_action = QAction(dir_icon, "", self)
+        open_ninja_bindir_action = QtGui.QAction(dir_icon, "", self)
         open_ninja_bindir_action.triggered.connect(self._ninja_open_bindir)
         self._ui.prefs_cmake_ninja_bin_directory.addAction(
             open_ninja_bindir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
 
     def _setup_compilercache_toolbox(self) -> None:
@@ -336,37 +330,37 @@
         self._ui.prefs_compilercache_default.currentTextChanged.connect(
             self._compilercache_default_changed
         )
         self._ui.prefs_compilercache_ccache_location.textChanged.connect(
             self._compilercache_ccache_bin_directory_changed
         )
         dir_icon = self.style().standardIcon(QtWidgets.QStyle.SP_DirIcon)
-        open_ccache_bindir_action = QAction(dir_icon, "", self)
+        open_ccache_bindir_action = QtGui.QAction(dir_icon, "", self)
         open_ccache_bindir_action.triggered.connect(
             self._compilercache_open_ccache_bindir
         )
         self._ui.prefs_compilercache_ccache_location.addAction(
             open_ccache_bindir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.prefs_compilercache_sccache_location.textChanged.connect(
             self._compilercache_sccache_bin_directory_changed
         )
-        open_scache_bindir_action = QAction(dir_icon, "", self)
+        open_scache_bindir_action = QtGui.QAction(dir_icon, "", self)
         open_scache_bindir_action.triggered.connect(
             self._compilercache_open_sccache_bindir
         )
         self._ui.prefs_compilercache_sccache_location.addAction(
             open_scache_bindir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
         self._ui.prefs_compilercache_buildcache_location.textChanged.connect(
             self._compilercache_buildcache_bin_directory_changed
         )
-        open_buildcache_bindir_action = QAction(dir_icon, "", self)
+        open_buildcache_bindir_action = QtGui.QAction(dir_icon, "", self)
         open_buildcache_bindir_action.triggered.connect(
             self._compilercache_open_buildcache_bindir
         )
         self._ui.prefs_compilercache_buildcache_location.addAction(
             open_buildcache_bindir_action,
             QtWidgets.QLineEdit.TrailingPosition,
         )
@@ -1070,28 +1064,30 @@
         uuid = self._prefs_recipes_model.uuid(selected_index.row())
         menu = QtWidgets.QMenu(self)
         menu.addActions(self._ui.prefs_recipes_table.actions())
         forget_recipe_action = menu.actions()[0]
         forget_recipe_action.setData(uuid)
         forget_recipe_action.triggered.connect(self._recipes_forget_recipe)
         menu.addSeparator()
-        menu.addMenu(self._recipes_build_change_cache_menu(uuid)).setText(
+        menu.addMenu(self._recipes_build_change_cache_menu(uuid, menu)).setText(
             "Change local cache to"
         )
         menu.exec_(self._ui.prefs_recipes_table.viewport().mapToGlobal(position))
 
-    def _recipes_build_change_cache_menu(self, uuid: QtCore.QUuid) -> QtWidgets.QMenu:
-        menu = QtWidgets.QMenu(self)
+    def _recipes_build_change_cache_menu(
+        self, uuid: QtCore.QUuid, parent_menu: QtWidgets.QMenu
+    ) -> QtWidgets.QMenu:
+        menu = QtWidgets.QMenu(parent_menu)
         with RecipeSettingsReader.from_uuid(uuid) as settings:
             uuid_local_cache = settings.local_cache_name.resolve()
         with AllNamedLocalCacheSettingsReader() as cache_names:
             for name in cache_names:
                 if name == uuid_local_cache:
                     continue
-                action = QAction(name, self)
+                action = QtGui.QAction(name, self)
                 action.setData(uuid)
                 action.triggered.connect(self._recipes_change_cache)
                 menu.addAction(action)
         return menu
 
     def _recipes_change_cache(self) -> None:
         selected_rows = self._ui.prefs_recipes_table.selectionModel().selectedRows()
@@ -1201,15 +1197,16 @@
         prefix_path, _ = QtWidgets.QFileDialog.getOpenFileName(
             self,
             caption="Import preferences presets",
             filter="JSON (*.json)",
         )
         if not prefix_path:
             return
-        with open(prefix_path, "rt", encoding="utf-8") as preset_json_file:
+        prefix_path_path = pathlib.Path(prefix_path)
+        with prefix_path_path.open("rt", encoding="utf-8") as preset_json_file:
             presets = json.load(preset_json_file)
         if "cruiz_presets" not in presets:
             QtWidgets.QMessageBox.critical(
                 self,
                 "Preference presets",
                 f"{prefix_path} is an invalid preference presets file. "
                 "Aborting import.",
@@ -1224,15 +1221,16 @@
         )
         if not prefix_path:
             return
         presets: typing.Dict[str, str] = {}
         with LocalCacheSettingsReader() as settings:
             presets.update(settings.presets())  # type: ignore
         if presets:
-            with open(prefix_path, "wt", encoding="utf-8") as preset_json_file:
+            prefix_path_path = pathlib.Path(prefix_path)
+            with prefix_path_path.open("wt", encoding="utf-8") as preset_json_file:
                 json.dump({"cruiz_presets": presets}, preset_json_file, indent=4)
 
     def _clean_preferences(self) -> None:
         sanitise_settings(self)
 
     def _restore_defaults(self) -> None:
         result = QtWidgets.QMessageBox.question(
```

### Comparing `cruiz-1.3.2b1/cruiz/settings/updatesettings.py` & `cruiz-1.4.0a1/cruiz/settings/updatesettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,20 +249,21 @@
                 keys = settings.allKeys()
                 for key in keys:
                     per_editable_settings[key] = settings.value(key)
                 editable_data[uuid_str].append(per_editable_settings)
         settings.remove(editable_group)
     for editable_uuid_str, editable_array in editable_data.items():
         group = f"Recipe/{editable_uuid_str}"
-        with SettingsGroup(settings, group):
-            with SettingsWriteArray(settings, "Editables", len(editable_array)):
-                for i, editable_dict in enumerate(editable_array):
-                    settings.setArrayIndex(i)
-                    for key, value in editable_dict.items():
-                        settings.setValue(key, value)
+        with SettingsGroup(settings, group), SettingsWriteArray(
+            settings, "Editables", len(editable_array)
+        ):
+            for i, editable_dict in enumerate(editable_array):
+                settings.setArrayIndex(i)
+                for key, value in editable_dict.items():
+                    settings.setValue(key, value)
 
 
 def _patch_settings_from_v0(settings: QtCore.QSettings) -> None:
     # pylint: disable=too-many-locals, too-many-branches
     """
     This patch:
     1) Removes the %General group
```

### Comparing `cruiz-1.3.2b1/cruiz/svggraph.py` & `cruiz-1.4.0a1/cruiz/svggraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,15 @@
 Utilities for generating SVGs from Conan dependency graphs
 """
 
 import os
 import typing
 
 import graphviz
-from qtpy import QtCore, QtGui, QtSvg, QtWidgets, PYSIDE2
-
-if PYSIDE2:
-    QGraphicsSvgItem = QtSvg.QGraphicsSvgItem
-    QAction = QtWidgets.QAction
-else:
-    # module not present in qtpy at the time of writing
-    from PySide6 import QtSvgWidgets
-
-    QGraphicsSvgItem = QtSvgWidgets.QGraphicsSvgItem
-    QAction = QtGui.QAction
+from qtpy import QtCore, QtGui, QtSvg, QtWidgets, QtSvgWidgets
 
 from cruiz.settings.managers.graphvizpreferences import GraphVizSettingsReader
 from cruiz.environ import EnvironSaver
 from cruiz.interop.packagenode import PackageNode
 from cruiz.interop.dependencygraph import DependencyGraph
 
 
@@ -102,15 +92,15 @@
 class _SVGDialog(QtWidgets.QDialog):
     def __init__(self, renderer: QtSvg.QSvgRenderer) -> None:
         super().__init__()
         self.setWindowTitle("Package dependency graph view")
         self.setContextMenuPolicy(QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
         self.customContextMenuRequested.connect(self._context_menu)
         self._renderer = renderer
-        item = QGraphicsSvgItem()
+        item = QtSvgWidgets.QGraphicsSvgItem()
         item.setSharedRenderer(renderer)
         self._scene = QtWidgets.QGraphicsScene()
         self._scene.addItem(item)
         self._view = QtWidgets.QGraphicsView(self._scene)
         layout = QtWidgets.QVBoxLayout(self)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(self._view)
@@ -121,15 +111,15 @@
 
     def resizeEvent(self, event: QtGui.QResizeEvent) -> None:
         self._view.fitInView(self._scene.sceneRect(), QtCore.Qt.KeepAspectRatio)
         super().resizeEvent(event)
 
     def _context_menu(self, position: QtCore.QPoint) -> None:
         menu = QtWidgets.QMenu(self)
-        save_action = QAction("Save...", self)
+        save_action = QtGui.QAction("Save...", self)
         save_action.triggered.connect(self._on_save)
         menu.addAction(save_action)
         menu.exec_(self.mapToGlobal(position))
 
     def _on_save(self) -> None:
         new_path, _ = QtWidgets.QFileDialog.getSaveFileName(
             self, "Save SVG", "", "SVG files (*.svg)"
@@ -151,17 +141,17 @@
     """
     Wrapper around an SVG scene
     """
 
     def __init__(self, renderer: QtSvg.QSvgRenderer) -> None:
         super().__init__()
         self._renderer = renderer
-        item = QGraphicsSvgItem()
+        item = QtSvgWidgets.QGraphicsSvgItem()
         item.setSharedRenderer(renderer)
         self.addItem(item)
 
     def mouseDoubleClickEvent(self, event: QtWidgets.QGraphicsSceneMouseEvent) -> None:
         item = self.itemAt(event.scenePos(), QtGui.QTransform())
-        if item and isinstance(item, QGraphicsSvgItem):
+        if item and isinstance(item, QtSvgWidgets.QGraphicsSvgItem):
             _SVGDialog(self._renderer).exec_()
             event.setAccepted(True)
         return super().mouseDoubleClickEvent(event)
```

### Comparing `cruiz-1.3.2b1/cruiz/version.py` & `cruiz-1.4.0a1/cruiz/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,18 +16,19 @@
     """
     try:
         from .RELEASE_VERSION import __version__  # type: ignore[import]
 
         return __version__
     except ImportError:
         import os
+        import pathlib
         import subprocess
         import sys
 
-        def _describe(cwd: str) -> str:
+        def _describe(cwd: pathlib.Path) -> str:
             if (
                 "GITHUB_REF_TYPE" in os.environ
                 and os.environ["GITHUB_REF_TYPE"] == "tag"
             ):
                 # during GitHub actions, prefer to use the ref pushed
                 return os.environ["GITHUB_REF_NAME"]
             else:
@@ -35,20 +36,22 @@
                 return (
                     subprocess.check_output(["git", "describe", "--tags"], cwd=cwd)
                     .decode("utf-8")
                     .rstrip()
                 )
 
         try:
-            root_dir = os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
+            file_path = pathlib.Path(__file__)
+            root_dir = file_path.parent.parent.absolute()
         except NameError:
-            root_dir = os.path.dirname(sys.argv[0])
+            executable_path = pathlib.Path(sys.argv[0])
+            root_dir = executable_path.parent
         try:
             ref_description = _describe(root_dir)
-        except subprocess.CalledProcessError:
+        except (FileNotFoundError, subprocess.CalledProcessError):
             return "0.0.0"
         ref_split = ref_description.split("-")
         # drop the v prefix from the tag
         ref_tag = ref_split[0][1:]
         if len(ref_split) == 1:
             __version__ = ref_tag
         else:
```

### Comparing `cruiz-1.3.2b1/cruiz/widgets/aboutcruizdialog.py` & `cruiz-1.4.0a1/cruiz/widgets/aboutcruizdialog.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 """
 Dialog to show cruiz information
 """
 
 import sys
 import typing
 
-from qtpy import QtCore, QtGui, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtGui, QtWidgets
 
 from cruiz.version import get_version
 
-if PYSIDE2:
-    from cruiz.pyside2.about_dialog import Ui_AboutCruiz
-else:
-    from cruiz.pyside6.about_dialog import Ui_AboutCruiz
+from cruiz.pyside6.about_dialog import Ui_AboutCruiz
 
 
 class AboutDialog(QtWidgets.QDialog):
     def __init__(self, parent: typing.Optional[QtWidgets.QWidget] = None) -> None:
         super().__init__(parent)
         self._ui = Ui_AboutCruiz()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
```

### Comparing `cruiz-1.3.2b1/cruiz/widgets/debugging.py` & `cruiz-1.4.0a1/cruiz/widgets/debugging.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 Widget debugging
 """
 
 import logging
 
-from qtpy import QtCore, QtWidgets, PYSIDE2
+from qtpy import QtCore, QtWidgets
 
 
 def _widget_window_flags_to_string(widget: QtWidgets.QWidget) -> str:
     flags = widget.windowFlags()
     text = ""
     # window type
     window_type = flags & QtCore.Qt.WindowType_Mask
@@ -92,75 +92,56 @@
 
 def _widget_attributes_to_string(widget: QtWidgets.QWidget) -> str:
     text = "Attrs"
     if widget.testAttribute(QtCore.Qt.WA_AcceptDrops):
         text += ":WA_AcceptDrops"
     if widget.testAttribute(QtCore.Qt.WA_AlwaysShowToolTips):
         text += ":WA_AlwaysShowToolTips"
-    if PYSIDE2:
-        if widget.testAttribute(QtCore.Qt.WA_ContentsPropagated):
-            text += ":WA_ContentsPropagated"
     if widget.testAttribute(QtCore.Qt.WA_CustomWhatsThis):
         text += ":WA_CustomWhatsThis"
     if widget.testAttribute(QtCore.Qt.WA_DeleteOnClose):
         text += ":WA_DeleteOnClose"
     if widget.testAttribute(QtCore.Qt.WA_Disabled):
         text += ":WA_Disabled"
     if widget.testAttribute(QtCore.Qt.WA_DontShowOnScreen):
         text += ":WA_DontShowOnScreen"
     if widget.testAttribute(QtCore.Qt.WA_ForceDisabled):
         text += ":WA_ForceDisabled"
     if widget.testAttribute(QtCore.Qt.WA_ForceUpdatesDisabled):
         text += ":WA_ForceUpdatesDisabled"
-    if PYSIDE2:
-        if widget.testAttribute(QtCore.Qt.WA_GroupLeader):
-            text += ":WA_GroupLeader"
     if widget.testAttribute(QtCore.Qt.WA_Hover):
         text += ":WA_Hover"
     if widget.testAttribute(QtCore.Qt.WA_InputMethodEnabled):
         text += ":WA_InputMethodEnabled"
     if widget.testAttribute(QtCore.Qt.WA_KeyboardFocusChange):
         text += ":WA_KeyboardFocusChange"
     if widget.testAttribute(QtCore.Qt.WA_KeyCompression):
         text += ":WA_KeyCompression"
     if widget.testAttribute(QtCore.Qt.WA_LayoutOnEntireRect):
         text += ":WA_LayoutOnEntireRect"
     if widget.testAttribute(QtCore.Qt.WA_LayoutUsesWidgetRect):
         text += ":WA_LayoutUsesWidgetRect"
-    if PYSIDE2:
-        if widget.testAttribute(QtCore.Qt.WA_MacNoClickThrough):
-            text += ":WA_MacNoClickThrough"
     if widget.testAttribute(QtCore.Qt.WA_MacOpaqueSizeGrip):
         text += ":WA_MacOpaqueSizeGrip"
     if widget.testAttribute(QtCore.Qt.WA_MacShowFocusRect):
         text += ":WA_MacShowFocusRect"
     if widget.testAttribute(QtCore.Qt.WA_MacNormalSize):
         text += ":WA_MacNormalSize"
     if widget.testAttribute(QtCore.Qt.WA_MacSmallSize):
         text += ":WA_MacSmallSize"
     if widget.testAttribute(QtCore.Qt.WA_MacMiniSize):
         text += ":WA_MacMiniSize"
-    if PYSIDE2:
-        if widget.testAttribute(QtCore.Qt.WA_MacVariableSize):
-            text += ":WA_MacVariableSize"
-        if widget.testAttribute(QtCore.Qt.WA_MacBrushedMetal):
-            text += ":WA_MacBrushedMetal"
     if widget.testAttribute(QtCore.Qt.WA_Mapped):
         text += ":WA_Mapped"
     if widget.testAttribute(QtCore.Qt.WA_MouseNoMask):
         text += ":WA_MouseNoMask"
     if widget.testAttribute(QtCore.Qt.WA_MouseTracking):
         text += ":WA_MouseTracking"
     if widget.testAttribute(QtCore.Qt.WA_Moved):
         text += ":WA_Moved"
-    if PYSIDE2:
-        if widget.testAttribute(QtCore.Qt.WA_MSWindowsUseDirect3D):
-            text += ":WA_MSWindowsUseDirect3D"
-        if widget.testAttribute(QtCore.Qt.WA_NoBackground):
-            text += ":WA_NoBackground"
     if widget.testAttribute(QtCore.Qt.WA_NoChildEventsForParent):
         text += ":WA_NoChildEventsForParent"
     if widget.testAttribute(QtCore.Qt.WA_NoChildEventsFromChildren):
         text += ":WA_NoChildEventsFromChildren"
     if widget.testAttribute(QtCore.Qt.WA_NoMouseReplay):
         text += ":WA_NoMouseReplay"
     if widget.testAttribute(QtCore.Qt.WA_NoMousePropagation):
@@ -249,17 +230,14 @@
         text += ":WA_X11NetWmWindowTypeToolTip"
     if widget.testAttribute(QtCore.Qt.WA_X11NetWmWindowTypeNotification):
         text += ":WA_X11NetWmWindowTypeNotification"
     if widget.testAttribute(QtCore.Qt.WA_X11NetWmWindowTypeCombo):
         text += ":WA_X11NetWmWindowTypeCombo"
     if widget.testAttribute(QtCore.Qt.WA_X11NetWmWindowTypeDND):
         text += ":WA_X11NetWmWindowTypeDND"
-    if PYSIDE2:
-        if widget.testAttribute(QtCore.Qt.WA_MacFrameworkScaled):
-            text += ":WA_MacFrameworkScaled"
     if widget.testAttribute(QtCore.Qt.WA_AcceptTouchEvents):
         text += ":WA_AcceptTouchEvents"
     if widget.testAttribute(QtCore.Qt.WA_TouchPadAcceptSingleTouchEvents):
         text += ":WA_TouchPadAcceptSingleTouchEvents"
     if widget.testAttribute(QtCore.Qt.WA_X11DoNotAcceptFocus):
         text += ":WA_X11DoNotAcceptFocus"
     if widget.testAttribute(QtCore.Qt.WA_AlwaysStackOnTop):
```

### Comparing `cruiz-1.3.2b1/cruiz/widgets/shortcutlineedit.py` & `cruiz-1.4.0a1/cruiz/widgets/shortcutlineedit.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/widgets/util.py` & `cruiz-1.4.0a1/cruiz/widgets/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 
 import platform
 import typing
 
 from qtpy import QtCore, QtWidgets
 
 
-def search_for_dir_options() -> QtWidgets.QFileDialog.Options:
+def search_for_dir_options() -> QtWidgets.QFileDialog.Option:
     """
     Get standard file dialog options for directory searching.
     """
-    options = QtWidgets.QFileDialog.ShowDirsOnly
+    options = QtWidgets.QFileDialog.Option.ShowDirsOnly
     if platform.system() == "Darwin":
         # have to use the non-native dialog on macOS, otherwise cannot browse
         # into an application bundle
-        options = options | QtWidgets.QFileDialog.DontUseNativeDialog
+        options = options | QtWidgets.QFileDialog.Option.DontUseNativeDialog
     return options
 
 
-def search_for_file_options() -> QtWidgets.QFileDialog.Options:
+def search_for_file_options() -> QtWidgets.QFileDialog.Option:
     """
     Get standard file dialog options for file searching.
     """
-    options = QtWidgets.QFileDialog.Options()
+    options = QtWidgets.QFileDialog.Option(0)
     if platform.system() == "Darwin":
         # have to use the non-native dialog on macOS, otherwise cannot browse
         # into an application bundle
-        options = options | QtWidgets.QFileDialog.DontUseNativeDialog
+        options = options | QtWidgets.QFileDialog.Option.DontUseNativeDialog
     return options
 
 
 def clear_widgets_from_layout(layout: QtWidgets.QLayout) -> None:
     """
     Clear all widgets from a layout.
     Does not take child layouts into account.
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/build.py` & `cruiz-1.4.0a1/cruiz/workers/build.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/cmakebuildtool.py` & `cruiz-1.4.0a1/cruiz/workers/cmakebuildtool.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,29 @@
             "CONAN_MAKE_PROGRAM"
         ]
     if "CONAN_CMAKE_GENERATOR" in params.added_environment:
         params.added_environment["CMAKE_GENERATOR"] = params.added_environment[
             "CONAN_CMAKE_GENERATOR"
         ]
     if "verbose" in params.arguments:
-        if params.added_environment.get("CONAN_CMAKE_GENERATOR", None) == "Ninja":
+        if params.added_environment.get("CONAN_CMAKE_GENERATOR") == "Ninja":
             build_cmd.append("-v")
         else:
             params.added_environment["VERBOSE"] = "1"
     if "CONAN_CPU_COUNT" in params.added_environment:
         build_cmd.append(
             f"-j{params.added_environment['CONAN_CPU_COUNT']}"
         )  # suitable for both Make and Ninja
-    with worker.Worker(queue, params):
-        with subprocess.Popen(
-            build_cmd,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            cwd=params.cwd,
-        ) as process:
-            assert process.stdout
-            for line in iter(process.stdout.readline, b""):
-                queue.put(Stdout(line.decode("utf-8")))
-            assert process.stderr
-            for line in iter(process.stderr.readline, b""):
-                queue.put(Stderr(line.decode("utf-8")))
+    with worker.Worker(queue, params), subprocess.Popen(
+        build_cmd,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        cwd=params.cwd,
+    ) as process:
+        assert process.stdout
+        for line in iter(process.stdout.readline, b""):
+            queue.put(Stdout(line.decode("utf-8")))
+        assert process.stderr
+        for line in iter(process.stderr.readline, b""):
+            queue.put(Stderr(line.decode("utf-8")))
 
-            queue.put(Success(process.returncode))
+        queue.put(Success(process.returncode))
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/configinstall.py` & `cruiz-1.4.0a1/cruiz/workers/configinstall.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/create.py` & `cruiz-1.4.0a1/cruiz/workers/create.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/deletecmakecache.py` & `cruiz-1.4.0a1/cruiz/workers/deletecmakecache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/exportpackage.py` & `cruiz-1.4.0a1/cruiz/workers/exportpackage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/imports.py` & `cruiz-1.4.0a1/cruiz/workers/imports.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/install.py` & `cruiz-1.4.0a1/cruiz/workers/install.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/lockcreate.py` & `cruiz-1.4.0a1/cruiz/workers/lockcreate.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/meta.py` & `cruiz-1.4.0a1/cruiz/workers/meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Child process commands
 """
 
 from __future__ import annotations
 
 import multiprocessing
 import os
+import pathlib
 import urllib.parse
 import typing
 
 from cruiz.interop.commandparameters import CommandParameters
 from cruiz.interop.pod import ConanRemote, ConanHook
 from .utils import worker, message
 
@@ -53,25 +54,25 @@
         api.remote_remove(remote.name)
     for remote_str in remotes:
         remote = ConanRemote.from_string(remote_str)
         api.remote_add(remote.name, remote.url)
         api.remote_set_disabled_state(remote.name, not remote.enabled)
 
 
-def _profiles_dir(api: typing.Any) -> str:
+def _profiles_dir(api: typing.Any) -> pathlib.Path:
     # pylint: disable=pointless-statement
     try:
         # Conan 1.18+
-        profile_dir = api.app.cache.profiles_path
-        if not os.path.isdir(profile_dir):
+        profile_dir = pathlib.Path(api.app.cache.profiles_path)
+        if not profile_dir.is_dir():
             # this creates the default profile
             api.app.cache.default_profile
     except AttributeError:
-        profile_dir = api._cache.profiles_path
-        if not os.path.isdir(profile_dir):
+        profile_dir = pathlib.Path(api._cache.profiles_path)
+        if not profile_dir.is_dir():
             # this creates the default profile
             api._cache.default_profile
     return profile_dir
 
 
 def _default_profile_path(api: typing.Any) -> str:
     try:
@@ -116,21 +117,21 @@
 
 def _package_dir(
     api: typing.Any,
     reference: str,
     package_id: str,
     package_revision: str,
     short_paths: bool,
-) -> str:
+) -> pathlib.Path:
     from conans.model.ref import PackageReference
 
     layout, file_ref = _get_package_layout(api, reference, short_paths)
     pref = PackageReference(file_ref, package_id, package_revision)
     package_dir = layout.package(pref)
-    return package_dir
+    return pathlib.Path(package_dir)
 
 
 def _package_export_dir(api: typing.Any, reference: str, short_paths: bool) -> str:
     layout, _ = _get_package_layout(api, reference, short_paths)
     package_export_dir = layout.export()
     return package_export_dir
 
@@ -182,72 +183,72 @@
         # conan 1.18+
         result = api.app.cache.config.hooks
     except AttributeError:
         result = api._cache.config.hooks
     return result
 
 
-def _available_hooks(api: typing.Any) -> typing.List[str]:
+def _available_hooks(api: typing.Any) -> typing.List[pathlib.Path]:
     try:
         # conan 1.18+
-        hooks_dir = api.app.cache.hooks_path
+        hooks_dir = pathlib.Path(api.app.cache.hooks_path)
     except AttributeError:
-        hooks_dir = api._cache.hooks_path
-    if not hooks_dir or not os.path.isdir(hooks_dir):
+        hooks_dir = pathlib.Path(api._cache.hooks_path)
+    if not hooks_dir or not hooks_dir.is_dir():
         return []
-    hook_files = []
+    hook_files: typing.List[pathlib.Path] = []
     for root, dirs, files in os.walk(hooks_dir):
         if ".git" in dirs:
             # ignore .git folders
             dirs.remove(".git")
         for file in files:
             if file.endswith(".py"):
-                full_path = os.path.join(root, file)
-                stored_path = os.path.relpath(full_path, hooks_dir)
+                full_path = pathlib.Path(root) / file
+                stored_path = full_path.relative_to(hooks_dir)
                 hook_files.append(stored_path)
     return hook_files
 
 
 def _hooks_get(api: typing.Any) -> typing.List[ConanHook]:
     try:
         # conan 1.18+
-        hooks_dir = api.app.cache.hooks_path
+        hooks_dir = pathlib.Path(api.app.cache.hooks_path)
         enabled_hooks = api.app.cache.config.hooks
     except AttributeError:
-        hooks_dir = api._cache.hooks_path
+        hooks_dir = pathlib.Path(api._cache.hooks_path)
         enabled_hooks = api._cache.config.hooks
-    if not hooks_dir or not os.path.isdir(hooks_dir):
+    if not hooks_dir or not hooks_dir.is_dir():
         return []
     hook_files: typing.List[ConanHook] = []
     for root, dirs, files in os.walk(hooks_dir):
         if ".git" in dirs:
             # ignore .git folders
             dirs.remove(".git")
         for file in files:
             if file.endswith(".py"):
-                full_path = os.path.join(root, file)
-                stored_path = os.path.relpath(full_path, hooks_dir)
+                full_path = pathlib.Path(root) / file
+                stored_path = full_path.relative_to(hooks_dir)
                 hook_enabled = (
-                    file in enabled_hooks or os.path.splitext(file)[0] in enabled_hooks
+                    file in enabled_hooks or pathlib.Path(file).stem in enabled_hooks
                 )
                 hook_files.append(ConanHook(stored_path, hook_enabled))
     return hook_files
 
 
 def _hooks_sync(api: typing.Any, hook_changes: typing.List[str]) -> None:
     for change in hook_changes:
         hook = ConanHook.from_string(change)
         hook_config = f"hooks.{hook.path}"
         if hook.enabled:
             _set_config(api, hook_config, None)
         else:
-            if _has_config_option(api, "hooks", hook.path):
+            if _has_config_option(api, "hooks", os.fspath(hook.path)):
                 _rm_config(api, hook_config)
             else:
-                no_ext_path = os.path.splitext(hook.path)[0]
+                no_ext_path = hook.path.stem
                 hook_config = f"hooks.{no_ext_path}"
                 assert _has_config_option(api, "hooks", no_ext_path)
                 _rm_config(api, hook_config)
 
 
 def _enable_hook(api: typing.Any, hook: str, hook_enabled: bool) -> None:
     hook = f"hooks.{hook}"
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/package.py` & `cruiz-1.4.0a1/cruiz/workers/package.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/packagebinary.py` & `cruiz-1.4.0a1/cruiz/workers/packagebinary.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/packagedetails.py` & `cruiz-1.4.0a1/cruiz/workers/reciperevisions.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 Child process commands
 """
 
 from __future__ import annotations
 
 import multiprocessing
 
-from cruiz.interop.packageidparameters import PackageIdParameters
+from cruiz.interop.reciperevisionsparameters import RecipeRevisionsParameters
 
 from .utils import worker
 from .utils.message import Message, Success
 
 
-def invoke(queue: multiprocessing.Queue[Message], params: PackageIdParameters) -> None:
+def invoke(
+    queue: multiprocessing.Queue[Message], params: RecipeRevisionsParameters
+) -> None:
     """
     Equivalent to
 
-    'conan search -r <remote_name> <reference>'
+    'conan search -r <remote_name> <reference> -rev'
 
-    PackageIdParameters has dynamic attributes.
+    RecipeRevisionsParameters has dynamic attributes.
     """
     with worker.ConanWorker(queue, params) as api:
-        result = api.search_packages(
+        result = api.get_recipe_revisions(
             params.reference,  # type: ignore
             remote_name=params.remote_name,  # type: ignore
         )
-        results_list = result["results"][0]["items"][0]["packages"]
 
-        queue.put(Success(results_list or None))
+        queue.put(Success(result))
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/packagerevisions.py` & `cruiz-1.4.0a1/cruiz/workers/packagerevisions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/reciperevisions.py` & `cruiz-1.4.0a1/cruiz/workers/source.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 Child process commands
 """
 
 from __future__ import annotations
 
 import multiprocessing
 
-from cruiz.interop.reciperevisionsparameters import RecipeRevisionsParameters
-
+from cruiz.interop.commandparameters import CommandParameters
 from .utils import worker
 from .utils.message import Message, Success
 
 
-def invoke(
-    queue: multiprocessing.Queue[Message], params: RecipeRevisionsParameters
-) -> None:
+def invoke(queue: multiprocessing.Queue[Message], params: CommandParameters) -> None:
     """
-    Equivalent to
-
-    'conan search -r <remote_name> <reference> -rev'
-
-    RecipeRevisionsParameters has dynamic attributes.
+    Run 'conan source'
     """
     with worker.ConanWorker(queue, params) as api:
-        result = api.get_recipe_revisions(
-            params.reference,  # type: ignore
-            remote_name=params.remote_name,  # type: ignore
-        )
+        assert params.recipe_path
+        assert params.cwd
+        args = {}
+        if params.install_folder:
+            args["info_folder"] = params.install_folder
+        if params.source_folder:
+            args["source_folder"] = params.source_folder
 
+        result = api.source(str(params.recipe_path), **args)
         queue.put(Success(result))
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/remotesearch.py` & `cruiz-1.4.0a1/cruiz/workers/remotesearch.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/removeallpackages.py` & `cruiz-1.4.0a1/cruiz/workers/removeallpackages.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/removepackage.py` & `cruiz-1.4.0a1/cruiz/workers/removepackage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/source.py` & `cruiz-1.4.0a1/cruiz/workers/testpackage.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,28 +3,39 @@
 """
 Child process commands
 """
 
 from __future__ import annotations
 
 import multiprocessing
+import typing
 
 from cruiz.interop.commandparameters import CommandParameters
 from .utils import worker
+from .utils.formatoptions import format_options
 from .utils.message import Message, Success
 
 
 def invoke(queue: multiprocessing.Queue[Message], params: CommandParameters) -> None:
     """
-    Run 'conan source'
+    Run 'conan test'
     """
     with worker.ConanWorker(queue, params) as api:
         assert params.recipe_path
         assert params.cwd
-        args = {}
-        if params.install_folder:
-            args["info_folder"] = params.install_folder
-        if params.source_folder:
-            args["source_folder"] = params.source_folder
+        assert params.package_reference
+        assert params.profile
+        args: typing.Dict[str, typing.Union[str, typing.List[str]]] = {
+            "profile_names": [params.profile],
+        }
+        if params.options:
+            args["options"] = format_options(params.options)
+        if params.test_folder:
+            args["test_build_folder"] = str(params.test_folder)
+
+        result = api.test(
+            params.recipe_path,
+            params.package_reference,
+            **args,
+        )
 
-        result = api.source(str(params.recipe_path), **args)
         queue.put(Success(result))
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/colorarma_conversion.py` & `cruiz-1.4.0a1/cruiz/workers/utils/colorarma_conversion.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/conanapi.py` & `cruiz-1.4.0a1/cruiz/workers/utils/conanapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,33 +37,33 @@
     """
     # pylint: disable=no-member
     cruiz.workers.utils.qtlogger.QtLogger().set_queue(queue)
     stdout = QueuedStreamSix(queue, Stdout)
     stderr = QueuedStreamSix(queue, Stderr)
     newoutputter = output.ConanOutput(stream=stdout, stream_err=stderr, color=True)
     if isinstance(params, CommandParameters):
-        home_dir = params.added_environment.get(
-            "CONAN_USER_HOME", get_conan_user_home()
+        home_dir = pathlib.Path(
+            params.added_environment.get("CONAN_USER_HOME", get_conan_user_home())
         )
-        local_cache_dir = os.path.join(home_dir, ".conan")
+        local_cache_dir = home_dir / ".conan"
         cache = conan_api.ClientCache(local_cache_dir, stdout)
         print_commands_to_output = cache.config.print_commands_to_output
         if params.cwd:
             # TODO: this has some broken assumptions about pure paths
             if isinstance(params.cwd, pathlib.PurePosixPath):
                 path = pathlib.Path(params.cwd)
                 path.mkdir(parents=True, exist_ok=True)
             else:
                 params.cwd.mkdir(parents=True, exist_ok=True)
             os.chdir(params.cwd)
     elif isinstance(params, CommonParameters):
-        home_dir = params.added_environment.get(
-            "CONAN_USER_HOME", get_conan_user_home()
+        home_dir = pathlib.Path(
+            params.added_environment.get("CONAN_USER_HOME", get_conan_user_home())
         )
-        local_cache_dir = os.path.join(home_dir, ".conan")
+        local_cache_dir = home_dir / ".conan"
         cache = conan_api.ClientCache(local_cache_dir, stdout)
         print_commands_to_output = False
 
     newrunner = runner.ConanRunner(
         print_commands_to_output=print_commands_to_output, output=newoutputter
     )
 
@@ -98,24 +98,24 @@
     from conans.tools import set_global_instances
     from conans.client.conan_api import ConanAPIV1
     from conans.paths import get_conan_user_home
     import conans
 
     user_io = UserIO(out=out)
 
-    user_home = get_conan_user_home()
-    base_folder = os.path.join(user_home, ".conan")
+    user_home = pathlib.Path(get_conan_user_home())
+    base_folder = user_home / ".conan"
 
     cache = ClientCache(base_folder, out)
     # Migration system
     migrator = ClientMigrator(cache, Version(client_version), out)
     migrator.migrate()
 
     if base_folder:
-        sys.path.append(os.path.join(base_folder, "python"))
+        sys.path.append(os.fspath(base_folder / "python"))
 
     config = cache.config
     # Adjust CONAN_LOGGING_LEVEL with the env readed
     conans.util.log.logger = configure_logger(config.logging_level, config.logging_file)
     conans.util.log.logger.debug("INIT: Using config '%s'", cache.conan_conf_path)
 
     hook_manager = HookManager(cache.hooks_path, config.hooks, user_io.out)
```

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/env.py` & `cruiz-1.4.0a1/cruiz/workers/utils/env.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/message.py` & `cruiz-1.4.0a1/cruiz/workers/utils/message.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/qtlogger.py` & `cruiz-1.4.0a1/cruiz/workers/utils/qtlogger.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/stream.py` & `cruiz-1.4.0a1/cruiz/workers/utils/stream.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/text2html.py` & `cruiz-1.4.0a1/cruiz/workers/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.3.2b1/cruiz/workers/utils/worker.py` & `cruiz-1.4.0a1/cruiz/workers/utils/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Utils for worker context managers
 """
 
 from __future__ import annotations
 
+import contextlib
 import datetime
 import multiprocessing
 import os
 import traceback
 import typing
 
 from qtpy import QtCore
@@ -52,25 +53,21 @@
         else:
             # can occur for other types of *Parameters classes
             self._wall_clock = None
 
     def __enter__(self) -> None:
         multiprocessing.get_logger().debug("%i (child): %s", os.getpid(), self._params)
         clear_conan_env()
-        if isinstance(self._params, CommandParameters):
-            set_env(self._params.added_environment, self._params.removed_environment)
-        elif isinstance(self._params, CommonParameters):
+        if isinstance(self._params, (CommandParameters, CommonParameters)):
             set_env(self._params.added_environment, self._params.removed_environment)
         else:
-            try:
+            with contextlib.suppress(TypeError):
+                # can happen for other types of *Parameters classes
                 if "env" in self._params:
                     set_env(self._params["env"], [])
-            except TypeError:
-                # can happen for other types of *Parameters classes
-                pass
 
         if self._wall_clock is not None:
             self._wall_clock.start()
 
     def _exception_to_html(
         self, exc_type: typing.Any, value: typing.Any, exc_tb: typing.Any
     ) -> None:
@@ -149,22 +146,18 @@
         for package in installed["packages"]:
             try:
                 cpp_info = package["cpp_info"]
             except KeyError:
                 # no cpp_info, so abort further processing
                 continue
             cpp_info["version"] = str(cpp_info["version"])
-            try:
+            with contextlib.suppress(KeyError):
+                # ignore 'components' not being in cpp_info
                 for component_key in cpp_info["components"]:
                     component = cpp_info["components"][component_key]
                     component["version"] = str(component["version"])
-            except KeyError:
-                # ignore 'components' not being in cpp_info
-                pass
-            try:
+            with contextlib.suppress(KeyError):
+                # ignore 'build_modules' not being in cpp_info
                 build_modules: typing.Dict[str, str] = {}
                 for key, value in cpp_info["build_modules"].items():
                     build_modules[key] = value
                 cpp_info["build_modules"] = build_modules
-            except KeyError:
-                # ignore 'build_modules' not being in cpp_info
-                pass
```

### Comparing `cruiz-1.3.2b1/cruiz.egg-info/PKG-INFO` & `cruiz-1.4.0a1/cruiz.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.3.2b1
+Version: 1.4.0a1
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # cruiz
 
 Conan recipe user interface
 
-Written by Mark Final, (c) 2020-2022.
+Written by Mark Final.
 
 ![main action workflow](https://github.com/markfinal/cruiz/actions/workflows/main.yml/badge.svg)
 
 
 ## Documentation
 See the documentation at [Read The Docs](https://cruiz.readthedocs.io/).
 
@@ -36,15 +37,15 @@
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
   - macOS (10.13+)
 - Apple Silicon platforms:
   - macOS (11.0+)
-- Python 3.7-3.10
+- Python 3.7-3.11
 - Conan 1.17.1+, but not 2.x (these are the versions tested)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
 ## Getting started
@@ -66,29 +67,14 @@
 
 4. Run from any directory
 
     - From your Python environment shell, `cruiz` or `python -m cruiz`
 
 Step 3 will need to be re-run when the Python dependencies, or the resource files used, change.
 
-## PySide versions
-PySide2 and PySide6 have been tested. PySide6 is the default, when running `cruiz`. PySide2 is only available on Intel x86_64 platforms.
-
-On Linux, PySide 6 from PyPI requires modern libstdc++. If you see a launch error indicating `CXXABI_1.3.9` then your distribution is likely too old.
-
-You can alter the default PySide versiont to use, in a number of ways:
-
-1. Use a different entry point
-
-    - `cruiz-pyside2` or `python -m cruiz-pyside2`
-
-2. Use an environment variable
-
-    - `QT_API=pyside2 cruiz`
-
 ## Linting
 Install linting dependencies with `pip install -r requirements_dev.txt`.
 
 cruiz uses [tox](https://tox.wiki/en/latest/) to automate linting. Use `tox -e lint`.
 
 [flake8](https://flake8.pycqa.org/en/latest/) is used for lint checks, specifically using [black](https://black.readthedocs.io/en/stable/) as the formatter.
```

### Comparing `cruiz-1.3.2b1/cruiz.egg-info/SOURCES.txt` & `cruiz-1.4.0a1/cruiz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 setup.py
 cruiz/RELEASE_VERSION.py
 cruiz/__init__.py
 cruiz/__main__.py
-cruiz/__main_pyside2__.py
 cruiz/application.py
 cruiz/config.py
 cruiz/constants.py
 cruiz/dumpobjecttypes.py
 cruiz/entrypoint.py
 cruiz/environ.py
 cruiz/exceptions.py
@@ -72,15 +71,14 @@
 cruiz/manage_local_cache/widgets/progressdialogs.py
 cruiz/manage_local_cache/widgets/remotestable.py
 cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
 cruiz/manage_local_cache/widgets/runconancommanddialog.py
 cruiz/model/__init__.py
 cruiz/model/conanpackagetypeflags.py
 cruiz/model/graphaslistmodel.py
-cruiz/pyside2/__init__.py
 cruiz/pyside6/__init__.py
 cruiz/recipe/__init__.py
 cruiz/recipe/dependencyview.py
 cruiz/recipe/expressioneditordialog.py
 cruiz/recipe/findtextdialog.py
 cruiz/recipe/recipe.py
 cruiz/recipe/recipewidget.py
```

### Comparing `cruiz-1.3.2b1/setup.py` & `cruiz-1.4.0a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,21 +41,19 @@
                 dst_file,
                 "cruiz/resources/cruizres.qrc",
             ]
         )
         return dst_file
 
     paths_written.append(_compile_pyside_resources(6))
-    paths_written.append(_compile_pyside_resources(2))
 
 
 def _compile_uis(paths_written: typing.List[str]) -> None:
     ui_variants = {
         "pyside6": "pyside6-uic",
-        "pyside2": "pyside2-uic",
     }
     for ui_subdir, uic_tool in ui_variants.items():
         ui_dir = f"cruiz/{ui_subdir}"
         if not os.path.isdir(ui_dir):
             os.makedirs(ui_dir)
         ui_basenames = [
             os.path.splitext(ui_file)[0]
@@ -110,17 +108,15 @@
 )
 
 
 with open(requirements_path) as requirements_file:
     requires = requirements_file.readlines()
 
 
-readme_path = os.path.join(
-    os.path.dirname(os.path.realpath(__file__)), "README.md"
-)
+readme_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "README.md")
 
 
 with open(readme_path) as readme_file:
     readme = readme_file.read()
 
 
 setup(
@@ -128,35 +124,35 @@
         "build_py": _BuildPyCommand,
         "sdist": _SDistCommand,
     },
     name="cruiz",
     version=get_version(),
     description="Conan recipe user interface",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="Mark Final",
     author_email="markfinal@hotmail.com",
     url="https://github.com/markfinal/cruiz",
     packages=find_packages(),
     install_requires=requires,
     entry_points={
         "gui_scripts": [
             "cruiz = cruiz.__main__:main",
-            "cruiz-pyside2 = cruiz.__main_pyside2__:main",
         ],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7, <3.11",
+    python_requires=">=3.7, <3.12",
     project_urls={
-        'Documentation': 'https://cruiz.readthedocs.io/en/latest/',
-        'GitHub': 'https://github.com/markfinal/cruiz',
+        "Documentation": "https://cruiz.readthedocs.io/en/latest/",
+        "GitHub": "https://github.com/markfinal/cruiz",
     },
 )
```

