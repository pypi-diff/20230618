# Comparing `tmp/osxphotos-0.60.2.tar.gz` & `tmp/osxphotos-0.60.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.2.tar", last modified: Sat Jun 17 14:16:34 2023, max compression
+gzip compressed data, was "osxphotos-0.60.3.tar", last modified: Sun Jun 18 16:54:53 2023, max compression
```

## Comparing `osxphotos-0.60.2.tar` & `osxphotos-0.60.3.tar`

### file list

```diff
@@ -1,232 +1,233 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.568291 osxphotos-0.60.2/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.2/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.2/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-17 14:16:34.568103 osxphotos-0.60.2/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   224169 2023-06-17 14:16:23.000000 osxphotos-0.60.2/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.2/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.542224 osxphotos-0.60.2/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.2/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 15:00:00.000000 osxphotos-0.60.2/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-17 14:16:19.000000 osxphotos-0.60.2/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.2/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.2/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.550678 osxphotos-0.60.2/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.2/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    26594 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.2/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      713 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   106908 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.2/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     7833 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.2/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.2/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.2/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.2/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.551104 osxphotos-0.60.2/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.2/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1467985 2023-06-17 14:16:30.000000 osxphotos-0.60.2/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.2/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.2/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.2/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-06-17 04:33:59.000000 osxphotos-0.60.2/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.2/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    91520 2023-06-17 14:14:35.000000 osxphotos-0.60.2/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    81384 2023-06-17 14:14:35.000000 osxphotos-0.60.2/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5542 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.553485 osxphotos-0.60.2/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149146 2023-06-17 01:41:30.000000 osxphotos-0.60.2/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.2/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.2/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-17 14:16:22.000000 osxphotos-0.60.2/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.2/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.2/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.554480 osxphotos-0.60.2/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.2/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.2/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.2/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.2/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.2/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.2/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.2/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.555271 osxphotos-0.60.2/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.2/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.2/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.2/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.2/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-06-16 15:10:56.000000 osxphotos-0.60.2/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-06-17 14:12:56.000000 osxphotos-0.60.2/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.543048 osxphotos-0.60.2/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6344 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-17 14:16:34.000000 osxphotos-0.60.2/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-17 14:16:34.568332 osxphotos-0.60.2/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.2/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.567603 osxphotos-0.60.2/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-17 14:16:34.567873 osxphotos-0.60.2/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.2/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.2/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-06-16 16:22:37.000000 osxphotos-0.60.2/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.2/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.2/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.2/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.2/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.2/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.2/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.2/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.2/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.2/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.2/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.2/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.2/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.2/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.2/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.2/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.2/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.2/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.2/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.2/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.2/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.2/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.2/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.2/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-06-16 15:10:52.000000 osxphotos-0.60.2/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.512133 osxphotos-0.60.3/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.3/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.3/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 16:54:53.511935 osxphotos-0.60.3/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   225512 2023-06-18 16:54:41.000000 osxphotos-0.60.3/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.3/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.459861 osxphotos-0.60.3/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.3/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 15:00:00.000000 osxphotos-0.60.3/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-18 16:54:37.000000 osxphotos-0.60.3/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.3/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.3/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.468156 osxphotos-0.60.3/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.3/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27384 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.3/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      713 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   107273 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.3/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8754 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.3/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.3/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.3/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.3/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.476263 osxphotos-0.60.3/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.3/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1471429 2023-06-18 16:54:49.000000 osxphotos-0.60.3/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.3/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.3/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.3/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-06-17 04:33:59.000000 osxphotos-0.60.3/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.3/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    91520 2023-06-17 14:14:35.000000 osxphotos-0.60.3/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    84832 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5719 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.478990 osxphotos-0.60.3/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7576 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149944 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.3/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.3/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-18 16:54:41.000000 osxphotos-0.60.3/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.3/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.3/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.480338 osxphotos-0.60.3/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.3/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.3/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.3/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.3/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.3/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.3/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.481510 osxphotos-0.60.3/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.3/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-06-17 14:12:56.000000 osxphotos-0.60.3/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.460691 osxphotos-0.60.3/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6400 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-18 16:54:53.512168 osxphotos-0.60.3/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.3/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.511520 osxphotos-0.60.3/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.511747 osxphotos-0.60.3/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.3/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.3/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-06-16 16:22:37.000000 osxphotos-0.60.3/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.3/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.3/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.3/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.3/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.3/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.3/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.3/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.3/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.3/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.3/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.3/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.3/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.3/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.3/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.3/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.3/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.3/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.3/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.3/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.3/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.3/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.2/LICENSE` & `osxphotos-0.60.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/PKG-INFO` & `osxphotos-0.60.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.2
+Version: 0.60.3
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.2/README.md` & `osxphotos-0.60.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osxphotos)
 [![Downloads](https://static.pepy.tech/personalized-badge/osxphotos?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/osxphotos)
 [![subreddit](https://img.shields.io/reddit/subreddit-subscribers/osxphotos?style=social)](https://www.reddit.com/r/osxphotos/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-59-orange.svg?style=flat)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-61-orange.svg?style=flat)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 OSXPhotos provides the ability to interact with and query Apple's Photos.app library on macOS and Linux. You can query the Photos library database — for example, file name, file path, and metadata such as keywords/tags, persons/faces, albums, etc. You can also easily export both the original and edited photos.
 
 <p align="center"><img src="docs/screencast/demo.gif?raw=true" width="713" height="430"/></p>
 
 # Table of Contents
@@ -865,14 +865,24 @@
                                   library
   --not-cloudasset                Search for photos that are not part of an
                                   iCloud library
   --incloud                       Search for photos that are in iCloud (have
                                   been synched)
   --not-incloud                   Search for photos that are not in iCloud (have
                                   not been synched)
+  --syndicated                    Search for photos that have been shared via
+                                  syndication ('Shared with You' album via
+                                  Messages, etc.)
+  --not-syndicated                Search for photos that have not been shared
+                                  via syndication ('Shared with You' album via
+                                  Messages, etc.)
+  --saved-to-library              Search for syndicated photos that have saved
+                                  to the library
+  --not-saved-to-library          Search for syndicated photos that have not
+                                  saved to the library
   --regex REGEX TEMPLATE          Search for photos where TEMPLATE matches
                                   regular expression REGEX. For example, to find
                                   photos in an album that begins with 'Beach': '
                                   --regex "^Beach" "{album}"'. You may specify
                                   more than one regular expression match by
                                   repeating '--regex' with different arguments.
   --selected                      Filter for photos that are currently selected
@@ -2095,15 +2105,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.2'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.3'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2582,15 +2592,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.2'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.3'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2709,14 +2719,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pekingduck"><img src="https://avatars.githubusercontent.com/u/2597142?v=4?s=75" width="75px;" alt="Peking Duck"/><br /><sub><b>Peking Duck</b></sub></a><br /><a href="#ideas-pekingduck" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Apekingduck" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.patreon.com/cclauss"><img src="https://avatars.githubusercontent.com/u/3709715?v=4?s=75" width="75px;" alt="Christian Clauss"/><br /><sub><b>Christian Clauss</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=cclauss" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dvdkon"><img src="https://avatars.githubusercontent.com/u/3526303?v=4?s=75" width="75px;" alt="dvdkon"/><br /><sub><b>dvdkon</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dvdkon" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/wernerzj"><img src="https://avatars.githubusercontent.com/u/130370930?v=4?s=75" width="75px;" alt="wernerzj"/><br /><sub><b>wernerzj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Awernerzj" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/rajscode"><img src="https://avatars.githubusercontent.com/u/99123253?v=4?s=75" width="75px;" alt="rajscode"/><br /><sub><b>rajscode</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Arajscode" title="Bug reports">🐛</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=rajscode" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MaxLyt"><img src="https://avatars.githubusercontent.com/u/136200430?v=4?s=75" width="75px;" alt="MaxLyt"/><br /><sub><b>MaxLyt</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3AMaxLyt" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ces3001"><img src="https://avatars.githubusercontent.com/u/23762610?v=4?s=75" width="75px;" alt="ces3001"/><br /><sub><b>ces3001</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aces3001" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `osxphotos-0.60.2/README.rst` & `osxphotos-0.60.3/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/__init__.py` & `osxphotos-0.60.3/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/_constants.py` & `osxphotos-0.60.3/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.3/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/albuminfo.py` & `osxphotos-0.60.3/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/__init__.py` & `osxphotos-0.60.3/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/about.py` & `osxphotos-0.60.3/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/add_locations.py` & `osxphotos-0.60.3/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/albums.py` & `osxphotos-0.60.3/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.3/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/cli.py` & `osxphotos-0.60.3/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.3/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/cli_params.py` & `osxphotos-0.60.3/osxphotos/cli/cli_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,14 +586,34 @@
         help="Search for photos that are in iCloud (have been synched)",
     ),
     "--not-incloud": click.Option(
         ["--not-incloud"],
         is_flag=True,
         help="Search for photos that are not in iCloud (have not been synched)",
     ),
+    "--syndicated": click.Option(
+        ["--syndicated"],
+        is_flag=True,
+        help="Search for photos that have been shared via syndication ('Shared with You' album via Messages, etc.)",
+    ),
+    "--not-syndicated": click.Option(
+        ["--not-syndicated"],
+        is_flag=True,
+        help="Search for photos that have not been shared via syndication ('Shared with You' album via Messages, etc.)",
+    ),
+    "--saved-to-library": click.Option(
+        ["--saved-to-library"],
+        is_flag=True,
+        help="Search for syndicated photos that have saved to the library",
+    ),
+    "--not-saved-to-library": click.Option(
+        ["--not-saved-to-library"],
+        is_flag=True,
+        help="Search for syndicated photos that have not saved to the library",
+    ),
     "--regex": click.Option(
         ["--regex"],
         metavar="REGEX TEMPLATE",
         nargs=2,
         multiple=True,
         help="Search for photos where TEMPLATE matches regular expression REGEX. "
         "For example, to find photos in an album that begins with 'Beach': '--regex \"^Beach\" \"{album}\"'. "
```

### Comparing `osxphotos-0.60.2/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.3/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/color_themes.py` & `osxphotos-0.60.3/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/common.py` & `osxphotos-0.60.3/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/darkmode.py` & `osxphotos-0.60.3/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.3/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/docs.py` & `osxphotos-0.60.3/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/dump.py` & `osxphotos-0.60.3/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.3/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/export.py` & `osxphotos-0.60.3/osxphotos/cli/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -882,14 +882,18 @@
     use_photos_export,
     uti,
     uuid,
     uuid_from_file,
     verbose_flag,
     xattr_template,
     year,
+    syndicated,
+    not_syndicated,
+    saved_to_library,
+    not_saved_to_library,
     selected=False,  # Isn't provided on unsupported platforms
     # debug,  # debug, watch, breakpoint handled in cli/__init__.py
     # watch,
     # breakpoint,
 ):
     """Export photos from the Photos database.
     Export path DEST is required.
@@ -1103,14 +1107,19 @@
         uti = cfg.uti
         uuid = cfg.uuid
         uuid_from_file = cfg.uuid_from_file
         # this is the one option that is named differently in the config file than the variable passed by --verbose (verbose_flag)
         verbose_flag = cfg.verbose
         xattr_template = cfg.xattr_template
         year = cfg.year
+        syndicated = cfg.syndicated
+        not_syndicated = cfg.not_syndicated
+        saved_to_library = cfg.saved_to_library
+        not_saved_to_library = cfg.not_saved_to_library
+
         # config file might have changed verbose
         verbose = verbose_print(verbose=verbose_flag, timestamp=timestamp, theme=theme)
         verbose(f"Loaded options from file [filepath]{load_config}")
 
         set_crash_data("cfg", cfg.asdict())
 
     verbose(f"osxphotos version: {__version__}")
@@ -1151,14 +1160,16 @@
         ("screenshot", "not_screenshot"),
         ("selfie", "not_selfie"),
         ("shared", "not_shared"),
         ("skip_edited", "skip_original_if_edited"),
         ("slow_mo", "not_slow_mo"),
         ("time_lapse", "not_time_lapse"),
         ("title", "no_title"),
+        ("syndicated", "not_syndicated"),
+        ("saved_to_library", "not_saved_to_library"),
     ]
     dependent_options = [
         ("append", ("report")),
         ("exiftool_merge_keywords", ("exiftool", "sidecar")),
         ("exiftool_merge_persons", ("exiftool", "sidecar")),
         ("exiftool_option", ("exiftool")),
         ("favorite_rating", ("exiftool", "sidecar")),
```

### Comparing `osxphotos-0.60.2/osxphotos/cli/exportdb.py` & `osxphotos-0.60.3/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/grep.py` & `osxphotos-0.60.3/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/help.py` & `osxphotos-0.60.3/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/import_cli.py` & `osxphotos-0.60.3/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/info.py` & `osxphotos-0.60.3/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.3/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/keywords.py` & `osxphotos-0.60.3/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/kvstore.py` & `osxphotos-0.60.3/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/labels.py` & `osxphotos-0.60.3/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/list.py` & `osxphotos-0.60.3/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/orphans.py` & `osxphotos-0.60.3/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/param_types.py` & `osxphotos-0.60.3/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/persons.py` & `osxphotos-0.60.3/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.3/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/places.py` & `osxphotos-0.60.3/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.3/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/query.py` & `osxphotos-0.60.3/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/repl.py` & `osxphotos-0.60.3/osxphotos/cli/repl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """repl command for osxphotos CLI"""
 from __future__ import annotations
 
 import os
 import os.path
 import pathlib
 import re
+import shlex
+import subprocess
 import sys
 import time
+from functools import partial
 from typing import List
 
 import click
 from rich import pretty, print
 
 import osxphotos
 from osxphotos._constants import _PHOTOS_4_VERSION
@@ -96,14 +99,15 @@
     toc = time.perf_counter()
     tictoc = toc - tic
 
     # shortcut for helper functions
     get_photo = photosdb.get_photo
     show = _show_photo
     spotlight = _spotlight_photo
+    find = partial(_find_in_library, photosdb)
     get_selected = _get_selected(photosdb)
     try:
         selected = get_selected()
     except Exception:
         # get_selected sometimes fails
         selected = []
 
@@ -125,36 +129,39 @@
         f"- all_photos: list of PhotoInfo objects for all photos in photosdb, including those in the trash (len={len(all_photos)})"
     )
     print(
         f"- selected: list of PhotoInfo objects for any photos selected in Photos (len={len(selected)})"
     )
     print(f"\nThe following functions may be helpful:")
     print(
-        f"- get_photo(uuid): return a PhotoInfo object for photo with uuid; e.g. get_photo('B13F4485-94E0-41CD-AF71-913095D62E31')"
+        "- get_photo(uuid): return a PhotoInfo object for photo with uuid; e.g. get_photo('B13F4485-94E0-41CD-AF71-913095D62E31')"
     )
     print(
-        f"- get_selected(); return list of PhotoInfo objects for photos selected in Photos"
+        "- get_selected(); return list of PhotoInfo objects for photos selected in Photos"
     )
     print(
-        f"- show(photo): open a photo object in the default viewer; e.g. show(selected[0])"
+        "- show(photo): open a photo object in the default viewer; e.g. show(selected[0])"
     )
     print(
-        f"- show(path): open a file at path in the default viewer; e.g. show('/path/to/photo.jpg')"
+        "- show(path): open a file at path in the default viewer; e.g. show('/path/to/photo.jpg')"
     )
-    print(f"- spotlight(photo): open a photo and spotlight it in Photos")
+    print("- spotlight(photo): open a photo and spotlight it in Photos")
     # print(
     #     f"- help(object): print help text including list of methods for object; for example, help(PhotosDB)"
     # )
     print(
-        f"- inspect(object): print information about an object; e.g. inspect(PhotoInfo)"
+        "- inspect(object): print information about an object; e.g. inspect(PhotoInfo)"
     )
     print(
-        f"- explore(object): interactively explore an object with objexplore; e.g. explore(PhotoInfo)"
+        "- explore(object): interactively explore an object with objexplore; e.g. explore(PhotoInfo)"
     )
-    print(f"- q, quit, quit(), exit, exit(): exit this interactive shell\n")
+    print(
+        "- find(text): search for files matching text in Photos library; e.g. find('B13F4485')"
+    )
+    print("- q, quit, quit(), exit, exit(): exit this interactive shell\n")
 
     embed_repl(
         globals=globals(),
         locals=locals(),
         history_filename=str(pathlib.Path.home() / ".osxphotos_repl_history"),
         quit_words=["q", "quit", "exit"],
         vi_mode=not emacs,
@@ -229,7 +236,24 @@
             raise ValueError(e) from e
         msg = str(e).split(":")[1]
         raise click.BadOptionUsage(
             "query_eval", f"Invalid query-eval CRITERIA: {msg}"
         ) from e
 
     return photos
+
+
+def _find_in_library(photosdb: PhotosDB, search_str: str) -> list[str]:
+    """Find files in Photos library matching search_str using find command"""
+    # this is a quick and dirty way to find files in the Photos library
+    # e.g. those matching a UUID or a filename
+    library_path = photosdb.library_path
+    if not library_path:
+        raise ValueError("Could not find Photos library")
+
+    search_str = shlex.quote(search_str)
+    library_path = shlex.quote(library_path)
+    cmd = f"find {library_path} | grep {search_str}"
+    output = subprocess.check_output(cmd, shell=True, universal_newlines=True)
+
+    # Split the output into lines and return as a list
+    return output.strip().split("\n")
```

### Comparing `osxphotos-0.60.2/osxphotos/cli/report_writer.py` & `osxphotos-0.60.3/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.3/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/show_command.py` & `osxphotos-0.60.3/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.3/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/sync.py` & `osxphotos-0.60.3/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/sync_results.py` & `osxphotos-0.60.3/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/theme.py` & `osxphotos-0.60.3/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/timewarp.py` & `osxphotos-0.60.3/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/tutorial.py` & `osxphotos-0.60.3/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/uuid.py` & `osxphotos-0.60.3/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/verbose.py` & `osxphotos-0.60.3/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/cli/version.py` & `osxphotos-0.60.3/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/compare_exif.py` & `osxphotos-0.60.3/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/configoptions.py` & `osxphotos-0.60.3/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/crash_reporter.py` & `osxphotos-0.60.3/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/datetime_formatter.py` & `osxphotos-0.60.3/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/datetime_utils.py` & `osxphotos-0.60.3/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/debug.py` & `osxphotos-0.60.3/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/docs/docs.zip` & `osxphotos-0.60.3/osxphotos/docs/docs.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1467985 bytes, number of entries: 99
+Zip file size: 1471429 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jun-17 14:16 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jun-18 16:54 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
 -rw-r--r--  3.0 unx   324766 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   201027 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
 -rw-r--r--  3.0 unx    52325 tx defN 23-May-07 14:38 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   302896 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx   313861 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29240 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   523106 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photosdb/photosdb.html
--rw-r--r--  3.0 unx    36244 tx defN 23-May-07 14:38 docs/_modules/osxphotos/photosalbum.html
+-rw-r--r--  3.0 unx   526422 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx    37347 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/photosalbum.html
 -rw-r--r--  3.0 unx    92802 tx defN 23-May-07 14:38 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
--rw-r--r--  3.0 unx    59723 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/queryoptions.html
+-rw-r--r--  3.0 unx    61579 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
 -rw-r--r--  3.0 unx    61850 tx defN 23-May-14 15:28 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jun-17 14:16 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jun-18 16:54 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jun-17 14:16 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jun-18 16:54 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jun-17 14:16 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jun-18 16:54 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jun-17 14:16 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jun-18 16:54 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jun-17 14:16 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jun-18 16:54 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jun-17 14:16 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jun-18 16:54 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   414459 tx defN 23-Jun-17 14:16 docs/cli.html
+-rw-r--r--  3.0 unx   423685 tx defN 23-Jun-18 16:54 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   243869 tx defN 23-Jun-17 14:16 docs/genindex.html
--rw-r--r--  3.0 unx   103976 tx defN 23-Jun-17 14:16 docs/index.html
+-rw-r--r--  3.0 unx   249535 tx defN 23-Jun-18 16:54 docs/genindex.html
+-rw-r--r--  3.0 unx   105318 tx defN 23-Jun-18 16:54 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9396 bx stor 23-Jun-17 14:16 docs/objects.inv
+-rw-r--r--  3.0 unx     9610 bx stor 23-Jun-18 16:54 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jun-17 14:16 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jun-17 14:16 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jun-17 14:16 docs/py-modindex.html
--rw-r--r--  3.0 unx   438608 tx defN 23-Jun-17 14:16 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jun-18 16:54 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jun-18 16:54 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jun-18 16:54 docs/py-modindex.html
+-rw-r--r--  3.0 unx   446001 tx defN 23-Jun-18 16:54 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jun-17 14:16 docs/search.html
--rw-r--r--  3.0 unx   215976 tx defN 23-Jun-17 14:16 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jun-17 14:16 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jun-17 14:16 docs/tutorial.html
-99 files, 6913241 bytes uncompressed, 1449253 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jun-18 16:54 docs/search.html
+-rw-r--r--  3.0 unx   220592 tx defN 23-Jun-18 16:54 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jun-18 16:54 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jun-18 16:54 docs/tutorial.html
+99 files, 6958938 bytes uncompressed, 1452697 bytes compressed:  79.1%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.2 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.60.2 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -258,18 +258,19 @@
 <span class="kn">from</span> <span class="nn">.phototables</span> <span class="kn">import</span> <span class="n">PhotoTables</span>
 <span class="kn">from</span> <span class="nn">.phototemplate</span> <span class="kn">import</span> <span class="n">PhotoTemplate</span><span class="p">,</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">.placeinfo</span> <span class="kn">import</span> <span class="n">PlaceInfo4</span><span class="p">,</span> <span class="n">PlaceInfo5</span>
 <span class="kn">from</span> <span class="nn">.query_builder</span> <span class="kn">import</span> <span class="n">get_query</span>
 <span class="kn">from</span> <span class="nn">.scoreinfo</span> <span class="kn">import</span> <span class="n">ScoreInfo</span>
 <span class="kn">from</span> <span class="nn">.searchinfo</span> <span class="kn">import</span> <span class="n">SearchInfo</span>
 <span class="kn">from</span> <span class="nn">.uti</span> <span class="kn">import</span> <span class="n">get_preferred_uti_extension</span><span class="p">,</span> <span class="n">get_uti_for_extension</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">_get_resource_loc</span><span class="p">,</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">is_macos</span><span class="p">,</span> <span class="n">hexdigest</span><span class="p">,</span> <span class="n">list_directory</span>
+<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">_get_resource_loc</span><span class="p">,</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">hexdigest</span><span class="p">,</span> <span class="n">is_macos</span><span class="p">,</span> <span class="n">list_directory</span>
 
 <span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
     <span class="kn">from</span> <span class="nn">osxmetadata</span> <span class="kn">import</span> <span class="n">OSXMetaData</span>
+
     <span class="kn">from</span> <span class="nn">.text_detection</span> <span class="kn">import</span> <span class="n">detect_text</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotoInfo&quot;</span><span class="p">,</span> <span class="s2">&quot;PhotoInfoNone&quot;</span><span class="p">,</span> <span class="s2">&quot;frozen_photoinfo_factory&quot;</span><span class="p">]</span>
 
 <span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;osxphotos&quot;</span><span class="p">)</span>
 
 
@@ -327,16 +328,15 @@
         <span class="c1"># Photos &lt;= 4 provides no way to get date of adjustment and will update</span>
         <span class="c1"># lastmodifieddate anytime photo database record is updated (e.g. adding tags)</span>
         <span class="c1"># only report lastmodified date for Photos &lt;=4 if photo is edited;</span>
         <span class="c1"># even in this case, the date could be incorrect</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">hasadjustments</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
-        <span class="n">imagedate</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;lastmodifieddate&quot;</span><span class="p">]</span>
-        <span class="k">if</span> <span class="n">imagedate</span><span class="p">:</span>
+        <span class="k">if</span> <span class="n">imagedate</span> <span class="o">:=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;lastmodifieddate&quot;</span><span class="p">]:</span>
             <span class="n">seconds</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;imageTimeZoneOffsetSeconds&quot;</span><span class="p">]</span> <span class="ow">or</span> <span class="mi">0</span>
             <span class="n">delta</span> <span class="o">=</span> <span class="n">timedelta</span><span class="p">(</span><span class="n">seconds</span><span class="o">=</span><span class="n">seconds</span><span class="p">)</span>
             <span class="n">tz</span> <span class="o">=</span> <span class="n">timezone</span><span class="p">(</span><span class="n">delta</span><span class="p">)</span>
             <span class="k">return</span> <span class="n">imagedate</span><span class="o">.</span><span class="n">astimezone</span><span class="p">(</span><span class="n">tz</span><span class="o">=</span><span class="n">tz</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
@@ -365,14 +365,17 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_path</span> <span class="o">=</span> <span class="n">photopath</span>
             <span class="k">return</span> <span class="n">photopath</span>
 
     <span class="k">def</span> <span class="nf">_path_5</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns candidate path for original photo on Photos &gt;= version 5&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;shared&quot;</span><span class="p">]:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_5_shared</span><span class="p">()</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
+            <span class="c1"># path for &quot;shared with you&quot; syndicated photos that have not yet been saved to the library</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_syndication</span><span class="p">()</span>
         <span class="k">return</span> <span class="p">(</span>
             <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">],</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;filename&quot;</span><span class="p">])</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span>
             <span class="k">else</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_masters_path</span><span class="p">,</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">],</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;filename&quot;</span><span class="p">],</span>
@@ -404,14 +407,29 @@
         <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">shared_path</span><span class="p">,</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">],</span>
             <span class="n">filename</span><span class="p">,</span>
         <span class="p">)</span>
 
+    <span class="k">def</span> <span class="nf">_path_syndication</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return path for syndicated photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 8+ stores syndicated photos in a separate directory</span>
+        <span class="c1"># in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID.ext</span>
+        <span class="c1"># where X is first digit of UUID</span>
+        <span class="n">syndication_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/syndication/originals&quot;</span>
+        <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+        <span class="n">path</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
+            <span class="n">syndication_path</span><span class="p">,</span>
+            <span class="n">uuid_dir</span><span class="p">,</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">,</span>
+        <span class="p">)</span>
+        <span class="k">return</span> <span class="n">path</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
+
     <span class="k">def</span> <span class="nf">_path_4</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns candidate path for original photo on Photos &lt;= version 4&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;has_raw&quot;</span><span class="p">]:</span>
             <span class="c1"># return the path to JPEG even if RAW is original</span>
             <span class="n">vol</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbvolumes</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;raw_pair_info&quot;</span><span class="p">][</span><span class="s2">&quot;volumeId&quot;</span><span class="p">]]</span>
                 <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;raw_pair_info&quot;</span><span class="p">][</span><span class="s2">&quot;volumeId&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span>
@@ -1074,14 +1092,18 @@
 
         <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_4</span><span class="p">()</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">path</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_shared_5</span><span class="p">()</span>
+            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
+                <span class="c1"># syndicated (&quot;Shared with you&quot;) photos not yet saved to library</span>
+                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_syndicated</span><span class="p">()</span>
+
             <span class="n">filename</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="n">filename</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">photopath</span><span class="p">)</span>
             <span class="k">if</span> <span class="ow">not</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">photopath</span><span class="p">):</span>
                 <span class="c1"># In testing, I&#39;ve seen occasional missing movie for live photo</span>
                 <span class="c1"># these appear to be valid -- e.g. video component not yet downloaded from iCloud</span>
                 <span class="c1"># TODO: should this be a warning or debug?</span>
@@ -1131,42 +1153,70 @@
                     <span class="c1"># or could do the actual check with &quot;isfile&quot;</span>
                     <span class="c1"># TODO: should this be a warning or debug?</span>
                     <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">return</span> <span class="n">photopath</span>
 
+    <span class="k">def</span> <span class="nf">_path_live_syndicated</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return path for live syndicated photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 8+ stores live syndicated photos in a separate directory</span>
+        <span class="c1"># in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID_3.mov</span>
+        <span class="c1"># where X is first digit of UUID</span>
+        <span class="n">syndication_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/syndication/originals&quot;</span>
+        <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+        <span class="n">filename</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span>
+        <span class="n">live_photo</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
+            <span class="n">syndication_path</span><span class="p">,</span>
+            <span class="n">uuid_dir</span><span class="p">,</span>
+            <span class="n">filename</span><span class="p">,</span>
+        <span class="p">)</span>
+        <span class="k">return</span> <span class="n">live_photo</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">live_photo</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
+
     <span class="nd">@cached_property</span>
-    <span class="k">def</span> <span class="nf">path_derivatives</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+    <span class="k">def</span> <span class="nf">path_derivatives</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
         <span class="sd">&quot;&quot;&quot;Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_4</span><span class="p">()</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_5_shared</span><span class="p">()</span>
 
         <span class="n">directory</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>  <span class="c1"># first char of uuid</span>
-        <span class="n">derivative_path</span> <span class="o">=</span> <span class="p">(</span>
-            <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span> <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;resources/derivatives/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">&quot;</span>
-        <span class="p">)</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
+            <span class="c1"># syndicated (&quot;Shared with you&quot;) photos not yet saved to library</span>
+            <span class="n">derivative_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/syndication/resources/derivatives&quot;</span>
+            <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">derivative_path</span><span class="si">}</span><span class="s2">/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
+            <span class="p">)</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="n">derivative_path</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;resources/derivatives/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">&quot;</span>
+            <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;resources/derivatives/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
+            <span class="p">)</span>
+
+        <span class="n">derivative_path</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="n">derivative_path</span><span class="p">)</span>
+        <span class="n">thumb_path</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="n">thumb_path</span><span class="p">)</span>
+
+        <span class="c1"># find all files that start with uuid in derivative path</span>
         <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">derivative_path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">*.*&quot;</span><span class="p">))</span>
 
         <span class="c1"># previews may be missing from derivatives path</span>
         <span class="c1"># there are what appear to be low res thumbnails in the &quot;masters&quot; subfolder</span>
-        <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
-            <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span>
-            <span class="o">/</span> <span class="sa">f</span><span class="s2">&quot;resources/derivatives/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
-        <span class="p">)</span>
         <span class="k">if</span> <span class="n">thumb_path</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
             <span class="n">files</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">thumb_path</span><span class="p">)</span>
 
+        <span class="c1"># sort by file size, largest first</span>
         <span class="n">files</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">files</span><span class="p">,</span> <span class="n">reverse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">f</span><span class="p">:</span> <span class="n">f</span><span class="o">.</span><span class="n">stat</span><span class="p">()</span><span class="o">.</span><span class="n">st_size</span><span class="p">)</span>
+
         <span class="c1"># return list of filename but skip .THM files (these are actually low-res thumbnails in JPEG format but with .THM extension)</span>
         <span class="n">derivatives</span> <span class="o">=</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span> <span class="k">for</span> <span class="n">filename</span> <span class="ow">in</span> <span class="n">files</span> <span class="k">if</span> <span class="n">filename</span><span class="o">.</span><span class="n">suffix</span> <span class="o">!=</span> <span class="s2">&quot;.THM&quot;</span><span class="p">]</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">isphoto</span> <span class="ow">and</span> <span class="nb">len</span><span class="p">(</span><span class="n">derivatives</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">derivatives</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s2">&quot;.mov&quot;</span><span class="p">):</span>
+            <span class="c1"># ensure .mov is first in list as poster image could be larger than the movie preview</span>
             <span class="n">derivatives</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">derivatives</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">=</span> <span class="n">derivatives</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">derivatives</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
 
         <span class="k">return</span> <span class="n">derivatives</span>
 
     <span class="k">def</span> <span class="nf">_path_derivatives_4</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Return paths to all derivative (preview) files for Photos &lt;= 4&quot;&quot;&quot;</span>
         <span class="n">modelid</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;modelID&quot;</span><span class="p">]</span>
@@ -1477,14 +1527,46 @@
         <span class="c1"># memoize SearchInfo object</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_search_info_normalized</span>
         <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_search_info_normalized</span> <span class="o">=</span> <span class="n">SearchInfo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">normalized</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_search_info_normalized</span>
 
+    <span class="nd">@cached_property</span>
+    <span class="k">def</span> <span class="nf">syndicated</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Return true if photo was shared via syndication (e.g. via Messages, etc.);</span>
+<span class="sd">        these are photos that appear in &quot;Shared with you&quot; album.</span>
+<span class="sd">        Photos 8+ only; returns None if not Photos 8+.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&lt;</span> <span class="mi">8</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">None</span>
+
+        <span class="k">try</span><span class="p">:</span>
+            <span class="k">return</span> <span class="p">(</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_syndication_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;syndication_identifier&quot;</span><span class="p">]</span>
+                <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span>
+            <span class="p">)</span>
+        <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">False</span>
+
+    <span class="nd">@cached_property</span>
+    <span class="k">def</span> <span class="nf">saved_to_library</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span> <span class="o">|</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Return True if syndicated photo has been saved to library;</span>
+<span class="sd">        returns False if photo is not syndicated or has not been saved to the library.</span>
+<span class="sd">        Returns None if not Photos 8+.</span>
+<span class="sd">        Syndicated photos are photos that appear in &quot;Shared with you&quot; album; Photos 8+ only.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&lt;</span> <span class="mi">8</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">None</span>
+
+        <span class="k">try</span><span class="p">:</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_syndication_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;syndication_history&quot;</span><span class="p">]</span> <span class="o">!=</span> <span class="mi">0</span>
+        <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">False</span>
+
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">labels</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;returns list of labels applied to photo by Photos image categorization</span>
 <span class="sd">        only valid on Photos 5, on older libraries returns empty list</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="p">[]</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -100,19 +100,20 @@
 from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate, RenderOptions
 from .placeinfo import PlaceInfo4, PlaceInfo5
 from .query_builder import get_query
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
 from .uti import get_preferred_uti_extension, get_uti_for_extension
-from .utils import _get_resource_loc, assert_macos, is_macos, hexdigest,
+from .utils import _get_resource_loc, assert_macos, hexdigest, is_macos,
 list_directory
 
 if is_macos:
     from osxmetadata import OSXMetaData
+
     from .text_detection import detect_text
 
 __all__ = ["PhotoInfo", "PhotoInfoNone", "frozen_photoinfo_factory"]
 
 logger = logging.getLogger("osxphotos")
 
 
@@ -173,16 +174,15 @@
 adding tags)
         # only report lastmodified date for Photos <=4 if photo is edited;
         # even in this case, the date could be incorrect
         if not self.hasadjustments and self._db._db_version <=
 _PHOTOS_4_VERSION:
             return None
 
-        imagedate = self._info["lastmodifieddate"]
-        if imagedate:
+        if imagedate := self._info["lastmodifieddate"]:
             seconds = self._info["imageTimeZoneOffsetSeconds"] or 0
             delta = timedelta(seconds=seconds)
             tz = timezone(delta)
             return imagedate.astimezone(tz=tz)
         else:
             return None
 
@@ -211,14 +211,18 @@
             self._path = photopath
             return photopath
 
     def _path_5(self):
         """Returns candidate path for original photo on Photos >= version 5"""
         if self._info["shared"]:
             return self._path_5_shared()
+        if self.syndicated and not self.saved_to_library:
+            # path for "shared with you" syndicated photos that have not yet
+been saved to the library
+            return self._path_syndication()
         return (
             os.path.join(self._info["directory"], self._info["filename"])
             if self._info["directory"].startswith("/")
             else os.path.join(
                 self._db._masters_path,
                 self._info["directory"],
                 self._info["filename"],
@@ -250,14 +254,30 @@
         return os.path.join(
             self._db._library_path,
             shared_path,
             self._info["directory"],
             filename,
         )
 
+    def _path_syndication(self):
+        """Return path for syndicated photo on Photos >= version 8"""
+        # Photos 8+ stores syndicated photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/
+UUID.ext
+        # where X is first digit of UUID
+        syndication_path = "scopes/syndication/originals"
+        uuid_dir = self.uuid[0]
+        path = os.path.join(
+            self._db._library_path,
+            syndication_path,
+            uuid_dir,
+            self.filename,
+        )
+        return path if os.path.isfile(path) else None
+
     def _path_4(self):
         """Returns candidate path for original photo on Photos <= version 4"""
         if self._info["has_raw"]:
             # return the path to JPEG even if RAW is original
             vol = (
                 self._db._dbvolumes[self._info["raw_pair_info"]["volumeId"]]
                 if self._info["raw_pair_info"]["volumeId"] is not None
@@ -973,14 +993,19 @@
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
             if self.shared:
                 return self._path_live_photo_shared_5()
+            if self.syndicated and not self.saved_to_library:
+                # syndicated ("Shared with you") photos not yet saved to
+library
+                return self._path_live_syndicated()
+
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
             photopath = str(photopath)
             if not os.path.isfile(photopath):
                 # In testing, I've seen occasional missing movie for live photo
                 # these appear to be valid -- e.g. video component not yet
 downloaded from iCloud
@@ -1033,49 +1058,80 @@
                     # or could do the actual check with "isfile"
                     # TODO: should this be a warning or debug?
                     photopath = None
         else:
             photopath = None
         return photopath
 
+    def _path_live_syndicated(self):
+        """Return path for live syndicated photo on Photos >= version 8"""
+        # Photos 8+ stores live syndicated photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/
+UUID_3.mov
+        # where X is first digit of UUID
+        syndication_path = "scopes/syndication/originals"
+        uuid_dir = self.uuid[0]
+        filename = f"{pathlib.Path(self.filename).stem}_3.mov"
+        live_photo = os.path.join(
+            self._db._library_path,
+            syndication_path,
+            uuid_dir,
+            filename,
+        )
+        return live_photo if os.path.isfile(live_photo) else None
+
     @cached_property
-    def path_derivatives(self):
+    def path_derivatives(self) -> list[str]:
         """Return any derivative (preview) images associated with the photo as
 a list of paths, sorted by file size (largest first)"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
             return self._path_derivatives_5_shared()
 
         directory = self._uuid[0]  # first char of uuid
-        derivative_path = (
-            pathlib.Path(self._db._library_path) / f"resources/derivatives/
-{directory}"
-        )
+        if self.syndicated and not self.saved_to_library:
+            # syndicated ("Shared with you") photos not yet saved to library
+            derivative_path = "scopes/syndication/resources/derivatives"
+            thumb_path = (
+                f"{derivative_path}/masters/{directory}/
+{self.uuid}_4_5005_c.jpeg"
+            )
+        else:
+            derivative_path = f"resources/derivatives/{directory}"
+            thumb_path = (
+                f"resources/derivatives/masters/{directory}/
+{self.uuid}_4_5005_c.jpeg"
+            )
+
+        derivative_path = pathlib.Path(self._db._library_path).joinpath
+(derivative_path)
+        thumb_path = pathlib.Path(self._db._library_path).joinpath(thumb_path)
+
+        # find all files that start with uuid in derivative path
         files = list(derivative_path.glob(f"{self.uuid}*.*"))
 
         # previews may be missing from derivatives path
         # there are what appear to be low res thumbnails in the "masters"
 subfolder
-        thumb_path = (
-            pathlib.Path(self._db._library_path)
-            / f"resources/derivatives/masters/{directory}/
-{self.uuid}_4_5005_c.jpeg"
-        )
         if thumb_path.exists():
             files.append(thumb_path)
 
+        # sort by file size, largest first
         files = sorted(files, reverse=True, key=lambda f: f.stat().st_size)
+
         # return list of filename but skip .THM files (these are actually low-
 res thumbnails in JPEG format but with .THM extension)
         derivatives = [str(filename) for filename in files if filename.suffix
 != ".THM"]
         if self.isphoto and len(derivatives) > 1 and derivatives[0].endswith
 (".mov"):
+            # ensure .mov is first in list as poster image could be larger than
+the movie preview
             derivatives[1], derivatives[0] = derivatives[0], derivatives[1]
 
         return derivatives
 
     def _path_derivatives_4(self):
         """Return paths to all derivative (preview) files for Photos <= 4"""
         modelid = self._info["modelID"]
@@ -1406,14 +1462,51 @@
         # memoize SearchInfo object
         try:
             return self._search_info_normalized
         except AttributeError:
             self._search_info_normalized = SearchInfo(self, normalized=True)
             return self._search_info_normalized
 
+    @cached_property
+    def syndicated(self) -> bool | None:
+        """Return true if photo was shared via syndication (e.g. via Messages,
+etc.);
+        these are photos that appear in "Shared with you" album.
+        Photos 8+ only; returns None if not Photos 8+.
+        """
+        if self._db.photos_version < 8:
+            return None
+
+        try:
+            return (
+                self._db._db_syndication_uuid[self.uuid]
+["syndication_identifier"]
+                is not None
+            )
+        except KeyError:
+            return False
+
+    @cached_property
+    def saved_to_library(self) -> bool | None:
+        """Return True if syndicated photo has been saved to library;
+        returns False if photo is not syndicated or has not been saved to the
+library.
+        Returns None if not Photos 8+.
+        Syndicated photos are photos that appear in "Shared with you" album;
+Photos 8+ only.
+        """
+        if self._db.photos_version < 8:
+            return None
+
+        try:
+            return self._db._db_syndication_uuid[self.uuid]
+["syndication_history"] != 0
+        except KeyError:
+            return False
+
     @property
     def labels(self):
         """returns list of labels applied to photo by Photos image
 categorization
         only valid on Photos 5, on older libraries returns empty list
         """
         if self._db._db_version <= _PHOTOS_4_VERSION:
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.2 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -289,14 +289,15 @@
     <span class="kn">from</span> <span class="nn">._photosdb_process_searchinfo</span> <span class="kn">import</span> <span class="p">(</span>
         <span class="n">_process_searchinfo</span><span class="p">,</span>
         <span class="n">labels</span><span class="p">,</span>
         <span class="n">labels_as_dict</span><span class="p">,</span>
         <span class="n">labels_normalized</span><span class="p">,</span>
         <span class="n">labels_normalized_as_dict</span><span class="p">,</span>
     <span class="p">)</span>
+    <span class="kn">from</span> <span class="nn">._photosdb_process_syndicationinfo</span> <span class="kn">import</span> <span class="n">_process_syndicationinfo</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
         <span class="bp">self</span><span class="p">,</span>
         <span class="n">dbfile</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">verbose</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">exiftool</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
         <span class="n">rich</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
@@ -483,14 +484,18 @@
         <span class="c1"># Dict to hold information on moments (Photos 5+)</span>
         <span class="c1"># key is Z_PK of ZMOMENT table and values are the moment info</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_db_moment_pk</span> <span class="o">=</span> <span class="p">{}</span>
 
         <span class="c1"># Dict to hold data on imports for Photos &lt;= 4</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_db_import_group</span> <span class="o">=</span> <span class="p">{}</span>
 
+        <span class="c1"># Dict to hold syndication info for Photos &gt;= 8</span>
+        <span class="c1"># key is UUID and value is dict of syndication info</span>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_db_syndication_uuid</span> <span class="o">=</span> <span class="p">{}</span>
+
         <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;dbfile = </span><span class="si">{</span><span class="n">dbfile</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">dbfile</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">dbfile</span> <span class="o">=</span> <span class="n">get_last_library_path</span><span class="p">()</span>
             <span class="k">if</span> <span class="n">dbfile</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
                 <span class="c1"># get_last_library_path must have failed to find library</span>
                 <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="s2">&quot;Could not get path to photo library database&quot;</span><span class="p">)</span>
@@ -2710,14 +2715,18 @@
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing comments and likes for shared photos.&quot;</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_process_comments</span><span class="p">()</span>
 
         <span class="c1"># process moments</span>
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing moments.&quot;</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_process_moments</span><span class="p">()</span>
 
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos_version</span> <span class="o">&gt;=</span> <span class="mi">8</span><span class="p">:</span>
+            <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing syndication info.&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_process_syndicationinfo</span><span class="p">()</span>
+
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Done processing details from Photos library.&quot;</span><span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">_process_moments</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Process data from ZMOMENT table&quot;&quot;&quot;</span>
         <span class="c1"># _db_moment_pk is dict in form {pk: {moment info}} by ZMOMENT.Z_PK</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
@@ -3709,14 +3718,24 @@
             <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">date_added</span> <span class="ow">and</span> <span class="n">p</span><span class="o">.</span><span class="n">date_added</span> <span class="o">&lt;</span> <span class="n">added_before</span><span class="p">]</span>
 
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">added_in_last</span><span class="p">:</span>
             <span class="n">added_after</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">now</span><span class="p">()</span> <span class="o">-</span> <span class="n">options</span><span class="o">.</span><span class="n">added_in_last</span>
             <span class="n">added_after</span> <span class="o">=</span> <span class="n">datetime_naive_to_local</span><span class="p">(</span><span class="n">added_after</span><span class="p">)</span>
             <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">date_added</span> <span class="ow">and</span> <span class="n">p</span><span class="o">.</span><span class="n">date_added</span> <span class="o">&gt;</span> <span class="n">added_after</span><span class="p">]</span>
 
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">syndicated</span><span class="p">:</span>
+            <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span><span class="p">]</span>
+        <span class="k">elif</span> <span class="n">options</span><span class="o">.</span><span class="n">not_syndicated</span><span class="p">:</span>
+            <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span><span class="p">]</span>
+
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
+            <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="n">p</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">]</span>
+        <span class="k">elif</span> <span class="n">options</span><span class="o">.</span><span class="n">not_saved_to_library</span><span class="p">:</span>
+            <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">p</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">]</span>
+
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">function</span><span class="p">:</span>
             <span class="k">for</span> <span class="n">function</span> <span class="ow">in</span> <span class="n">options</span><span class="o">.</span><span class="n">function</span><span class="p">:</span>
                 <span class="n">photos</span> <span class="o">=</span> <span class="n">function</span><span class="p">[</span><span class="mi">0</span><span class="p">](</span><span class="n">photos</span><span class="p">)</span>
 
         <span class="c1"># burst should be checked last, ref #640</span>
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">:</span>
             <span class="c1"># add the burst_photos to the export set</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -131,14 +131,15 @@
     from ._photosdb_process_searchinfo import (
         _process_searchinfo,
         labels,
         labels_as_dict,
         labels_normalized,
         labels_normalized_as_dict,
     )
+    from ._photosdb_process_syndicationinfo import _process_syndicationinfo
 
     def __init__(
         self,
         dbfile=None,
         verbose=None,
         exiftool=None,
         rich=None,
@@ -354,14 +355,18 @@
         # Dict to hold information on moments (Photos 5+)
         # key is Z_PK of ZMOMENT table and values are the moment info
         self._db_moment_pk = {}
 
         # Dict to hold data on imports for Photos <= 4
         self._db_import_group = {}
 
+        # Dict to hold syndication info for Photos >= 8
+        # key is UUID and value is dict of syndication info
+        self._db_syndication_uuid = {}
+
         logger.debug(f"dbfile = {dbfile}")
 
         if dbfile is None:
             dbfile = get_last_library_path()
             if dbfile is None:
                 # get_last_library_path must have failed to find library
                 raise FileNotFoundError("Could not get path to photo library
@@ -2737,14 +2742,18 @@
         verbose("Processing comments and likes for shared photos.")
         self._process_comments()
 
         # process moments
         verbose("Processing moments.")
         self._process_moments()
 
+        if self.photos_version >= 8:
+            verbose("Processing syndication info.")
+            self._process_syndicationinfo()
+
         verbose("Done processing details from Photos library.")
 
     def _process_moments(self):
         """Process data from ZMOMENT table"""
         # _db_moment_pk is dict in form {pk: {moment info}} by ZMOMENT.Z_PK
 
         if self._db_version <= _PHOTOS_4_VERSION:
@@ -3816,14 +3825,25 @@
 
         if options.added_in_last:
             added_after = datetime.now() - options.added_in_last
             added_after = datetime_naive_to_local(added_after)
             photos = [p for p in photos if p.date_added and p.date_added >
 added_after]
 
+        if options.syndicated:
+            photos = [p for p in photos if p.syndicated]
+        elif options.not_syndicated:
+            photos = [p for p in photos if not p.syndicated]
+
+        if options.saved_to_library:
+            photos = [p for p in photos if p.syndicated and p.saved_to_library]
+        elif options.not_saved_to_library:
+            photos = [p for p in photos if p.syndicated and not
+p.saved_to_library]
+
         if options.function:
             for function in options.function:
                 photos = function[0](photos)
 
         # burst should be checked last, ref #640
         if options.burst_photos:
             # add the burst_photos to the export set
```

#### docs/_modules/osxphotos/photosalbum.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosalbum - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.photosalbum - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -294,18 +294,21 @@
 
     <span class="k">def</span> <span class="nf">add_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">photo_list</span><span class="p">:</span> <span class="n">List</span><span class="p">[</span><span class="n">PhotoInfo</span><span class="p">]):</span>
         <span class="n">photos</span> <span class="o">=</span> <span class="p">[]</span>
         <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photo_list</span><span class="p">:</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="n">photos</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">photoscript</span><span class="o">.</span><span class="n">Photo</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span><span class="p">))</span>
             <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error creating Photo object for photo </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_uuid</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span><span class="p">)</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">verbose</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;Error creating Photo object for photo </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_uuid</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span><span class="p">)</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span>
                 <span class="p">)</span>
+        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;photos: </span><span class="si">{</span><span class="n">photos</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">for</span> <span class="n">photolist</span> <span class="ow">in</span> <span class="n">chunked</span><span class="p">(</span><span class="n">photos</span><span class="p">,</span> <span class="mi">10</span><span class="p">):</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;photolist: </span><span class="si">{</span><span class="n">photolist</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">photolist</span><span class="p">)</span>
         <span class="n">photo_len</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">photo_list</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">verbose</span><span class="p">(</span>
             <span class="sa">f</span><span class="s2">&quot;Added </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_num</span><span class="p">(</span><span class="n">photo_len</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">pluralize</span><span class="p">(</span><span class="n">photo_len</span><span class="p">,</span> <span class="s1">&#39;photo&#39;</span><span class="p">,</span> <span class="s1">&#39;photos&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2"> to album </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_album</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">photos</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -142,19 +142,23 @@
 
     def add_list(self, photo_list: List[PhotoInfo]):
         photos = []
         for p in photo_list:
             try:
                 photos.append(photoscript.Photo(p.uuid))
             except Exception as e:
+                print(f"Error creating Photo object for photo
+{self._format_uuid(p.uuid)}: {e}")
                 self.verbose(
                     f"Error creating Photo object for photo {self._format_uuid
 (p.uuid)}: {e}"
                 )
+        print(f"photos: {photos}")
         for photolist in chunked(photos, 10):
+            print(f"photolist: {photolist}")
             self.album.add(photolist)
         photo_len = len(photo_list)
         self.verbose(
             f"Added {self._format_num(photo_len)} {pluralize(photo_len,
 'photo', 'photos')} to album {self._format_album(self.name)}"
         )
```

#### docs/_modules/osxphotos/queryoptions.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.queryoptions - osxphotos 0.58.1 documentation</title>
+        <title>osxphotos.queryoptions - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.58.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.58.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -301,14 +301,18 @@
 <span class="sd">        slow_mo: search for slow-mo photos</span>
 <span class="sd">        time_lapse: search for time-lapse photos</span>
 <span class="sd">        title: list of titles to search for</span>
 <span class="sd">        to_date: search for photos taken on or before this date</span>
 <span class="sd">        uti: list of UTIs to search for</span>
 <span class="sd">        uuid: list of uuids to search for</span>
 <span class="sd">        year: search for photos taken in a given year</span>
+<span class="sd">        syndicated: search for photos that have been shared via syndication (&quot;Shared with You&quot; album via Messages, etc.)</span>
+<span class="sd">        not_syndicated: search for photos that have not been shared via syndication (&quot;Shared with You&quot; album via Messages, etc.)</span>
+<span class="sd">        saved_to_library: search for syndicated photos that have been saved to the Photos library</span>
+<span class="sd">        not_saved_to_library: search for syndicated photos that have not been saved to the Photos library</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
     <span class="n">added_after</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">added_before</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">added_in_last</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">timedelta</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">album</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">burst_photos</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
@@ -385,14 +389,18 @@
     <span class="n">time_lapse</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">title</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">to_date</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">to_time</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">time</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">uti</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">uuid</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">year</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">int</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">syndicated</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">not_syndicated</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">saved_to_library</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">not_saved_to_library</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
 
     <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="k">return</span> <span class="n">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span></div>
 
 
 <span class="k">def</span> <span class="nf">query_options_from_kwargs</span><span class="p">(</span><span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">QueryOptions</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;Validate query options and create a QueryOptions instance.</span>
@@ -454,14 +462,16 @@
         <span class="p">(</span><span class="s2">&quot;selfie&quot;</span><span class="p">,</span> <span class="s2">&quot;not_selfie&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;shared&quot;</span><span class="p">,</span> <span class="s2">&quot;not_shared&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;slow_mo&quot;</span><span class="p">,</span> <span class="s2">&quot;not_slow_mo&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;time_lapse&quot;</span><span class="p">,</span> <span class="s2">&quot;not_time_lapse&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;deleted&quot;</span><span class="p">,</span> <span class="s2">&quot;not_deleted&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;deleted&quot;</span><span class="p">,</span> <span class="s2">&quot;deleted_only&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;deleted_only&quot;</span><span class="p">,</span> <span class="s2">&quot;not_deleted&quot;</span><span class="p">),</span>
+        <span class="p">(</span><span class="s2">&quot;syndicated&quot;</span><span class="p">,</span> <span class="s2">&quot;not_syndicated&quot;</span><span class="p">),</span>
+        <span class="p">(</span><span class="s2">&quot;saved_to_library&quot;</span><span class="p">,</span> <span class="s2">&quot;not_saved_to_library&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="c1"># TODO: add option to validate requiring at least one query arg</span>
     <span class="k">for</span> <span class="n">arg</span><span class="p">,</span> <span class="n">not_arg</span> <span class="ow">in</span> <span class="n">exclusive</span><span class="p">:</span>
         <span class="k">if</span> <span class="n">kwargs</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span> <span class="ow">and</span> <span class="n">kwargs</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">not_arg</span><span class="p">):</span>
             <span class="n">arg</span> <span class="o">=</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;_&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">)</span>
             <span class="n">not_arg</span> <span class="o">=</span> <span class="n">not_arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;_&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">)</span>
             <span class="k">raise</span> <span class="n">IncompatibleQueryOptions</span><span class="p">(</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.58.1_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.58.1_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -148,14 +148,22 @@
         slow_mo: search for slow-mo photos
         time_lapse: search for time-lapse photos
         title: list of titles to search for
         to_date: search for photos taken on or before this date
         uti: list of UTIs to search for
         uuid: list of uuids to search for
         year: search for photos taken in a given year
+        syndicated: search for photos that have been shared via syndication
+("Shared with You" album via Messages, etc.)
+        not_syndicated: search for photos that have not been shared via
+syndication ("Shared with You" album via Messages, etc.)
+        saved_to_library: search for syndicated photos that have been saved to
+the Photos library
+        not_saved_to_library: search for syndicated photos that have not been
+saved to the Photos library
     """
 
     added_after: Optional[datetime.datetime] = None
     added_before: Optional[datetime.datetime] = None
     added_in_last: Optional[datetime.timedelta] = None
     album: Optional[Iterable[str]] = None
     burst_photos: Optional[bool] = None
@@ -232,14 +240,18 @@
     time_lapse: Optional[bool] = None
     title: Optional[Iterable[str]] = None
     to_date: Optional[datetime.datetime] = None
     to_time: Optional[datetime.time] = None
     uti: Optional[Iterable[str]] = None
     uuid: Optional[Iterable[str]] = None
     year: Optional[Iterable[int]] = None
+    syndicated: Optional[bool] = None
+    not_syndicated: Optional[bool] = None
+    saved_to_library: Optional[bool] = None
+    not_saved_to_library: Optional[bool] = None
 
     def asdict(self):
         return asdict(self)
 
 
 
 def query_options_from_kwargs(**kwargs) -> QueryOptions:
@@ -302,14 +314,16 @@
         ("selfie", "not_selfie"),
         ("shared", "not_shared"),
         ("slow_mo", "not_slow_mo"),
         ("time_lapse", "not_time_lapse"),
         ("deleted", "not_deleted"),
         ("deleted", "deleted_only"),
         ("deleted_only", "not_deleted"),
+        ("syndicated", "not_syndicated"),
+        ("saved_to_library", "not_saved_to_library"),
     ]
     # TODO: add option to validate requiring at least one query arg
     for arg, not_arg in exclusive:
         if kwargs.get(arg) and kwargs.get(not_arg):
             arg = arg.replace("_", "-")
             not_arg = not_arg.replace("_", "-")
             raise IncompatibleQueryOptions(
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.2'
+     - The osxphotos version, e.g. '0.60.3'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.2',
+    VERSION: '0.60.3',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.2 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -725,14 +725,38 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-not-incloud">
 <span class="sig-name descname"><span class="pre">--not-incloud</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-not-incloud" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos that are not in iCloud (have not been synched)</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-syndicated">
+<span class="sig-name descname"><span class="pre">--syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-not-syndicated">
+<span class="sig-name descname"><span class="pre">--not-syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-not-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have not been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-saved-to-library">
+<span class="sig-name descname"><span class="pre">--saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-not-saved-to-library">
+<span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-not-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have not saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-selected">
@@ -1656,14 +1680,38 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-not-incloud">
 <span class="sig-name descname"><span class="pre">--not-incloud</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-not-incloud" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos that are not in iCloud (have not been synched)</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-syndicated">
+<span class="sig-name descname"><span class="pre">--syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-not-syndicated">
+<span class="sig-name descname"><span class="pre">--not-syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-not-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have not been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-saved-to-library">
+<span class="sig-name descname"><span class="pre">--saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-not-saved-to-library">
+<span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-not-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have not saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-export-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-selected">
@@ -3222,14 +3270,38 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-not-incloud">
 <span class="sig-name descname"><span class="pre">--not-incloud</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-not-incloud" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos that are not in iCloud (have not been synched)</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-syndicated">
+<span class="sig-name descname"><span class="pre">--syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-not-syndicated">
+<span class="sig-name descname"><span class="pre">--not-syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-not-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have not been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-saved-to-library">
+<span class="sig-name descname"><span class="pre">--saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-not-saved-to-library">
+<span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-not-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have not saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-query-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-selected">
@@ -3759,14 +3831,38 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-repl-not-incloud">
 <span class="sig-name descname"><span class="pre">--not-incloud</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-not-incloud" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos that are not in iCloud (have not been synched)</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-repl-syndicated">
+<span class="sig-name descname"><span class="pre">--syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-repl-not-syndicated">
+<span class="sig-name descname"><span class="pre">--not-syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-not-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have not been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-repl-saved-to-library">
+<span class="sig-name descname"><span class="pre">--saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-repl-not-saved-to-library">
+<span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-not-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have not saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-repl-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-repl-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-repl-selected">
@@ -4418,14 +4514,38 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-sync-not-incloud">
 <span class="sig-name descname"><span class="pre">--not-incloud</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-not-incloud" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos that are not in iCloud (have not been synched)</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-sync-syndicated">
+<span class="sig-name descname"><span class="pre">--syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-sync-not-syndicated">
+<span class="sig-name descname"><span class="pre">--not-syndicated</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-not-syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that have not been shared via syndication (‘Shared with You’ album via Messages, etc.)</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-sync-saved-to-library">
+<span class="sig-name descname"><span class="pre">--saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-sync-not-saved-to-library">
+<span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-not-saved-to-library" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for syndicated photos that have not saved to the library</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-sync-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-sync-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-sync-selected">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -280,14 +280,24 @@
       Search for photos that are part of an iCloud library
   --not-cloudasset#
       Search for photos that are not part of an iCloud library
   --incloud#
       Search for photos that are in iCloud (have been synched)
   --not-incloud#
       Search for photos that are not in iCloud (have not been synched)
+  --syndicated#
+      Search for photos that have been shared via syndication (âShared with
+      Youâ album via Messages, etc.)
+  --not-syndicated#
+      Search for photos that have not been shared via syndication (âShared
+      with Youâ album via Messages, etc.)
+  --saved-to-library#
+      Search for syndicated photos that have saved to the library
+  --not-saved-to-library#
+      Search for syndicated photos that have not saved to the library
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -787,14 +797,24 @@
       Search for photos that are part of an iCloud library
   --not-cloudasset#
       Search for photos that are not part of an iCloud library
   --incloud#
       Search for photos that are in iCloud (have been synched)
   --not-incloud#
       Search for photos that are not in iCloud (have not been synched)
+  --syndicated#
+      Search for photos that have been shared via syndication (âShared with
+      Youâ album via Messages, etc.)
+  --not-syndicated#
+      Search for photos that have not been shared via syndication (âShared
+      with Youâ album via Messages, etc.)
+  --saved-to-library#
+      Search for syndicated photos that have saved to the library
+  --not-saved-to-library#
+      Search for syndicated photos that have not saved to the library
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -1788,14 +1808,24 @@
       Search for photos that are part of an iCloud library
   --not-cloudasset#
       Search for photos that are not part of an iCloud library
   --incloud#
       Search for photos that are in iCloud (have been synched)
   --not-incloud#
       Search for photos that are not in iCloud (have not been synched)
+  --syndicated#
+      Search for photos that have been shared via syndication (âShared with
+      Youâ album via Messages, etc.)
+  --not-syndicated#
+      Search for photos that have not been shared via syndication (âShared
+      with Youâ album via Messages, etc.)
+  --saved-to-library#
+      Search for syndicated photos that have saved to the library
+  --not-saved-to-library#
+      Search for syndicated photos that have not saved to the library
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -2052,14 +2082,24 @@
       Search for photos that are part of an iCloud library
   --not-cloudasset#
       Search for photos that are not part of an iCloud library
   --incloud#
       Search for photos that are in iCloud (have been synched)
   --not-incloud#
       Search for photos that are not in iCloud (have not been synched)
+  --syndicated#
+      Search for photos that have been shared via syndication (âShared with
+      Youâ album via Messages, etc.)
+  --not-syndicated#
+      Search for photos that have not been shared via syndication (âShared
+      with Youâ album via Messages, etc.)
+  --saved-to-library#
+      Search for syndicated photos that have saved to the library
+  --not-saved-to-library#
+      Search for syndicated photos that have not saved to the library
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -2422,14 +2462,24 @@
       Search for photos that are part of an iCloud library
   --not-cloudasset#
       Search for photos that are not part of an iCloud library
   --incloud#
       Search for photos that are in iCloud (have been synched)
   --not-incloud#
       Search for photos that are not in iCloud (have not been synched)
+  --syndicated#
+      Search for photos that have been shared via syndication (âShared with
+      Youâ album via Messages, etc.)
+  --not-syndicated#
+      Search for photos that have not been shared via syndication (âShared
+      with Youâ album via Messages, etc.)
+  --saved-to-library#
+      Search for syndicated photos that have saved to the library
+  --not-saved-to-library#
+      Search for syndicated photos that have not saved to the library
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.2 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.3 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1559,16 +1559,14 @@
           <li><a href="cli.html#cmdoption-osxphotos-query-not-cloudasset">osxphotos-query command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-cloudasset">osxphotos-repl command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-cloudasset">osxphotos-sync command line option</a>
 </li>
         </ul></li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     --not-edited
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-edited">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-edited">osxphotos-export command line option</a>
@@ -1591,14 +1589,16 @@
           <li><a href="cli.html#cmdoption-osxphotos-query-not-favorite">osxphotos-query command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-favorite">osxphotos-repl command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-favorite">osxphotos-sync command line option</a>
 </li>
         </ul></li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     --not-hdr
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-hdr">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-hdr">osxphotos-export command line option</a>
@@ -1727,14 +1727,29 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-reference">osxphotos-repl command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-reference">osxphotos-sync command line option</a>
 </li>
         </ul></li>
         <li>
+    --not-saved-to-library
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-saved-to-library">osxphotos-add-locations command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-not-saved-to-library">osxphotos-export command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-not-saved-to-library">osxphotos-query command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-not-saved-to-library">osxphotos-repl command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-not-saved-to-library">osxphotos-sync command line option</a>
+</li>
+        </ul></li>
+        <li>
     --not-screenshot
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-screenshot">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-screenshot">osxphotos-export command line option</a>
 </li>
@@ -1785,14 +1800,29 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-slow-mo">osxphotos-repl command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-slow-mo">osxphotos-sync command line option</a>
 </li>
         </ul></li>
         <li>
+    --not-syndicated
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-syndicated">osxphotos-add-locations command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-not-syndicated">osxphotos-export command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-not-syndicated">osxphotos-query command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-not-syndicated">osxphotos-repl command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-not-syndicated">osxphotos-sync command line option</a>
+</li>
+        </ul></li>
+        <li>
     --not-time-lapse
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-time-lapse">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-time-lapse">osxphotos-export command line option</a>
 </li>
@@ -2131,14 +2161,29 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-save-config">osxphotos-export command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-exportdb-save-config">osxphotos-exportdb command line option</a>
 </li>
         </ul></li>
         <li>
+    --saved-to-library
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-saved-to-library">osxphotos-add-locations command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-saved-to-library">osxphotos-export command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-saved-to-library">osxphotos-query command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-saved-to-library">osxphotos-repl command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-saved-to-library">osxphotos-sync command line option</a>
+</li>
+        </ul></li>
+        <li>
     --screenshot
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-screenshot">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-screenshot">osxphotos-export command line option</a>
 </li>
@@ -2302,14 +2347,29 @@
     --style
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-diff-s">osxphotos-diff command line option</a>
 </li>
         </ul></li>
         <li>
+    --syndicated
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-syndicated">osxphotos-add-locations command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-syndicated">osxphotos-export command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-syndicated">osxphotos-query command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-syndicated">osxphotos-repl command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-syndicated">osxphotos-sync command line option</a>
+</li>
+        </ul></li>
+        <li>
     --template
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-inspect-T">osxphotos-inspect command line option</a>
 </li>
         </ul></li>
         <li>
@@ -3660,18 +3720,18 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_cloudasset">not_cloudasset (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_edited">not_edited (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_favorite">not_favorite (osxphotos.QueryOptions attribute)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.QueryOptions.not_hdr">not_hdr (osxphotos.QueryOptions attribute)</a>
 </li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.QueryOptions.not_hidden">not_hidden (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_in_album">not_in_album (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_incloud">not_incloud (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_live">not_live (osxphotos.QueryOptions attribute)</a>
@@ -3680,22 +3740,26 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_panorama">not_panorama (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_portrait">not_portrait (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_reference">not_reference (osxphotos.QueryOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.QueryOptions.not_saved_to_library">not_saved_to_library (osxphotos.QueryOptions attribute)</a>
+</li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_screenshot">not_screenshot (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_selfie">not_selfie (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_shared">not_shared (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_slow_mo">not_slow_mo (osxphotos.QueryOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.QueryOptions.not_syndicated">not_syndicated (osxphotos.QueryOptions attribute)</a>
+</li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_time_lapse">not_time_lapse (osxphotos.QueryOptions attribute)</a>
 </li>
     </ul></td>
   </tr></table>
 </section>
 
 <section id="O" class="genindex-section">
@@ -3842,22 +3906,26 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-panorama">--not-panorama</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-portrait">--not-portrait</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-reference">--not-reference</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-saved-to-library">--not-saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-shared">--not-shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-slow-mo">--not-slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-syndicated">--not-syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-only-movies">--only-movies</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-only-photos">--only-photos</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-panorama">--panorama</a>
@@ -3870,24 +3938,28 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-query-eval">--query-eval</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-query-function">--query-function</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-regex">--regex</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-saved-to-library">--saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-screenshot">--screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-shared">--shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-slow-mo">--slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-syndicated">--syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-theme">--theme</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-timestamp">--timestamp</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-title">--title</a>
@@ -4246,22 +4318,26 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-panorama">--not-panorama</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-portrait">--not-portrait</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-reference">--not-reference</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-not-saved-to-library">--not-saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-shared">--not-shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-slow-mo">--not-slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-not-syndicated">--not-syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-only-movies">--only-movies</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-only-new">--only-new</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-only-photos">--only-photos</a>
@@ -4304,14 +4380,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-report">--report</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-retry">--retry</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-save-config">--save-config</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-saved-to-library">--saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-screenshot">--screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-shared">--shared</a>
@@ -4334,14 +4412,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-uuid-from-file">--skip-uuid-from-file</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-slow-mo">--slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-strip">--strip</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-syndicated">--syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-theme">--theme</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-timestamp">--timestamp</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-title">--title</a>
@@ -4783,22 +4863,26 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-panorama">--not-panorama</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-portrait">--not-portrait</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-reference">--not-reference</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-not-saved-to-library">--not-saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-shared">--not-shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-slow-mo">--not-slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-not-syndicated">--not-syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-only-movies">--only-movies</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-only-photos">--only-photos</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-panorama">--panorama</a>
@@ -4815,24 +4899,28 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-query-function">--query-function</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-quiet">--quiet</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-regex">--regex</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-saved-to-library">--saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-screenshot">--screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-shared">--shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-slow-mo">--slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-syndicated">--syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-title">--title</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-to-date">--to-date</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-to-time">--to-time</a>
@@ -4966,22 +5054,26 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-panorama">--not-panorama</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-portrait">--not-portrait</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-reference">--not-reference</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-not-saved-to-library">--not-saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-shared">--not-shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-slow-mo">--not-slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-not-syndicated">--not-syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-only-movies">--only-movies</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-only-photos">--only-photos</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-panorama">--panorama</a>
@@ -4994,24 +5086,28 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-query-eval">--query-eval</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-query-function">--query-function</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-regex">--regex</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-saved-to-library">--saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-screenshot">--screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-shared">--shared</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-slow-mo">--slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-syndicated">--syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-title">--title</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-to-date">--to-date</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-to-time">--to-time</a>
@@ -5178,20 +5274,24 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-panorama">--not-panorama</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-portrait">--not-portrait</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-reference">--not-reference</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-not-saved-to-library">--not-saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-slow-mo">--not-slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-not-syndicated">--not-syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-only-movies">--only-movies</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-only-photos">--only-photos</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-panorama">--panorama</a>
@@ -5206,24 +5306,28 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-query-function">--query-function</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-regex">--regex</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-R">--report</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-saved-to-library">--saved-to-library</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-screenshot">--screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-s">--set</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-slow-mo">--slow-mo</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-syndicated">--syndicated</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-theme">--theme</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-timestamp">--timestamp</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-title">--title</a>
@@ -5616,14 +5720,20 @@
   </tr></table>
 </section>
 
 <section id="S" class="genindex-section">
   <h2>S</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.PhotoInfo.saved_to_library">saved_to_library (osxphotos.PhotoInfo property)</a>
+
+        <ul>
+          <li><a href="reference.html#osxphotos.QueryOptions.saved_to_library">(osxphotos.QueryOptions attribute)</a>
+</li>
+        </ul></li>
         <li><a href="reference.html#osxphotos.PhotoInfo.score">score (osxphotos.PhotoInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.ScoreInfo">ScoreInfo (class in osxphotos)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.screenshot">screenshot (osxphotos.PhotoInfo property)</a>
 
         <ul>
@@ -5699,14 +5809,20 @@
         <li>
     SUBTOPIC
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-help-arg-SUBTOPIC">osxphotos-help command line option</a>
 </li>
         </ul></li>
+        <li><a href="reference.html#osxphotos.PhotoInfo.syndicated">syndicated (osxphotos.PhotoInfo property)</a>
+
+        <ul>
+          <li><a href="reference.html#osxphotos.QueryOptions.syndicated">(osxphotos.QueryOptions attribute)</a>
+</li>
+        </ul></li>
     </ul></td>
   </tr></table>
 </section>
 
 <section id="T" class="genindex-section">
   <h2>T</h2>
   <table style="width: 100%" class="indextable genindextable"><tr>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -42,167 +42,167 @@
 
 ***** Symbols *****
     * --add-exported-to-album
           o osxphotos-export_command
             line_option
     * --add-missing-to-album
           o osxphotos-export_command
-            line_option                     * --not-edited
+            line_option                     * --not-hdr
     * --add-skipped-to-album                      o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
     * --add-to-album                                line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-timewarp_command            o osxphotos-repl_command_line
             line_option                             option
     * --added-after                               o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-favorite
+            command_line_option             * --not-hidden
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
     * --added-before                              o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-hdr
+            command_line_option             * --not-in-album
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
     * --added-in-last                             o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-hidden
+            command_line_option             * --not-incloud
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
     * --album                                     o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-in-album
+            command_line_option             * --not-live
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-import_command              o osxphotos-export_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
           o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option
-    * --album-keyword                       * --not-incloud
+    * --album-keyword                       * --not-missing
           o osxphotos-exiftool_command            o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
     * --alt-copy                                  o osxphotos-query_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-repl_command_line
     * --append                                      option
           o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-export_command        * --not-live
+          o osxphotos-export_command        * --not-panorama
             line_option                           o osxphotos-add-locations
           o osxphotos-exportdb_command              command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-import_command                line_option
             line_option                           o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
     * --burst                                       option
           o osxphotos-add-locations               o osxphotos-sync_command_line
             command_line_option                     option
-          o osxphotos-export_command        * --not-missing
+          o osxphotos-export_command        * --not-portrait
             line_option                           o osxphotos-add-locations
           o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
     * --check-signatures                            option
           o osxphotos-exportdb_command            o osxphotos-sync_command_line
             line_option                             option
-    * --check-templates                     * --not-panorama
+    * --check-templates                     * --not-reference
           o osxphotos-import_command              o osxphotos-add-locations
             line_option                             command_line_option
     * --cleanup                                   o osxphotos-export_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
     * --clear-location                              line_option
           o osxphotos-import_command              o osxphotos-repl_command_line
             line_option                             option
     * --clear-metadata                            o osxphotos-sync_command_line
           o osxphotos-import_command                option
-            line_option                     * --not-portrait
+            line_option                     * --not-saved-to-library
     * --clone                                     o osxphotos-add-locations
           o osxphotos-theme_command                 command_line_option
             line_option                           o osxphotos-export_command
     * --cloudasset                                  line_option
           o osxphotos-add-locations               o osxphotos-query_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-query_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * --not-reference
+          o osxphotos-repl_command_line     * --not-screenshot
             option                                o osxphotos-add-locations
           o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-export_command
     * --compare-exif                                line_option
           o osxphotos-timewarp_command            o osxphotos-query_command
             line_option                             line_option
     * --config                                    o osxphotos-repl_command_line
           o osxphotos-theme_command                 option
             line_option                           o osxphotos-sync_command_line
     * --config-only                                 option
-          o osxphotos-export_command        * --not-screenshot
+          o osxphotos-export_command        * --not-selfie
             line_option                           o osxphotos-add-locations
     * --convert-to-jpeg                             command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
     * --current-name                              o osxphotos-query_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-repl_command_line
     * --date                                        option
           o osxphotos-timewarp_command            o osxphotos-sync_command_line
             line_option                             option
-    * --date-added                          * --not-selfie
+    * --date-added                          * --not-shared
           o osxphotos-timewarp_command            o osxphotos-add-locations
             line_option                             command_line_option
     * --date-added-from-photo                     o osxphotos-export_command
           o osxphotos-timewarp_command              line_option
             line_option                           o osxphotos-query_command
     * --date-delta                                  line_option
           o osxphotos-timewarp_command            o osxphotos-repl_command_line
             line_option                             option
-    * --db                                        o osxphotos-sync_command_line
-          o osxphotos_command_line                  option
-            option                          * --not-shared
-          o osxphotos-albums_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-batch-edit                  o osxphotos-export_command
+    * --db                                  * --not-slow-mo
+          o osxphotos_command_line                o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-albums_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-batch-edit                  o osxphotos-query_command
             command_line_option                     line_option
-          o osxphotos-diff_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-dump_command_line           o osxphotos-repl_command_line
+          o osxphotos-diff_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-dump_command_line           o osxphotos-sync_command_line
             option                                  option
-          o osxphotos-exiftool_command      * --not-slow-mo
+          o osxphotos-exiftool_command      * --not-syndicated
             line_option                           o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-info_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-inspect_command               line_option
             line_option                           o osxphotos-repl_command_line
@@ -415,495 +415,517 @@
             line_option                     * --save-config
           o osxphotos-query_command               o osxphotos-exiftool_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-exportdb_command
             option                                  line_option
-    * --favorite-rating                     * --screenshot
+    * --favorite-rating                     * --saved-to-library
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
     * --field                                     o osxphotos-export_command
           o osxphotos-dump_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
     * --filename                                    option
           o osxphotos-export_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-uuid_command_line     * --selected
+          o osxphotos-uuid_command_line     * --screenshot
             option                                o osxphotos-add-locations
     * --finder-tag-keywords                         command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
     * --finder-tag-template                       o osxphotos-query_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-repl_command_line
     * --folder                                      option
           o osxphotos-add-locations               o osxphotos-sync_command_line
             command_line_option                     option
-          o osxphotos-export_command        * --selfie
+          o osxphotos-export_command        * --selected
             line_option                           o osxphotos-add-locations
           o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
     * --force                                       option
           o osxphotos-timewarp_command            o osxphotos-sync_command_line
             line_option                             option
-    * --force-update                        * --set
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-    * --from-date                           * --shared
+    * --force-update                        * --selfie
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+    * --from-date                                 o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-query_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line             option
+            option                          * --set
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --from-time                           * --shared
           o osxphotos-add-locations               o osxphotos-add-locations
             command_line_option                     command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
           o osxphotos-sync_command_line     * --sidecar
             option                                o osxphotos-export_command
-    * --from-time                                   line_option
-          o osxphotos-add-locations         * --sidecar-drop-ext
+    * --function                                    line_option
+          o osxphotos-timewarp_command      * --sidecar-drop-ext
+            line_option                           o osxphotos-export_command
+    * --glob                                        line_option
+          o osxphotos-import_command        * --skip-bursts
+            line_option                           o osxphotos-export_command
+    * --has-comment                                 line_option
+          o osxphotos-add-locations         * --skip-edited
             command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                     * --skip-bursts
+            line_option                     * --skip-live
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --skip-edited
+          o osxphotos-repl_command_line     * --skip-original-if-edited
             option                                o osxphotos-export_command
           o osxphotos-sync_command_line             line_option
-            option                          * --skip-live
-    * --function                                  o osxphotos-export_command
-          o osxphotos-timewarp_command              line_option
-            line_option                     * --skip-original-if-edited
-    * --glob                                      o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                     * --skip-raw
-    * --has-comment                               o osxphotos-export_command
+            option                          * --skip-raw
+    * --has-likes                                 o osxphotos-export_command
           o osxphotos-add-locations                 line_option
             command_line_option             * --skip-uuid
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
           o osxphotos-query_command         * --skip-uuid-from-file
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
             option                          * --slow-mo
           o osxphotos-sync_command_line           o osxphotos-add-locations
             option                                  command_line_option
-    * --has-likes                                 o osxphotos-export_command
+    * --has-raw                                   o osxphotos-export_command
           o osxphotos-add-locations                 line_option
             command_line_option                   o osxphotos-query_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-repl_command_line
           o osxphotos-query_command                 option
             line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
             option                          * --split-folder
           o osxphotos-sync_command_line           o osxphotos-import_command
             option                                  line_option
-    * --has-raw                             * --sql
+    * --hdr                                 * --sql
           o osxphotos-add-locations               o osxphotos-exportdb_command
             command_line_option                     line_option
           o osxphotos-export_command        * --strip
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
             line_option                     * --style
           o osxphotos-repl_command_line           o osxphotos-diff_command_line
             option                                  option
-          o osxphotos-sync_command_line     * --template
-            option                                o osxphotos-inspect_command
-    * --hdr                                         line_option
-          o osxphotos-add-locations         * --theme
-            command_line_option                   o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-batch-edit
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-exiftool_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-exportdb_command
-    * --help                                        line_option
-          o osxphotos-run_command_line            o osxphotos-import_command
+          o osxphotos-sync_command_line     * --syndicated
+            option                                o osxphotos-add-locations
+    * --help                                        command_line_option
+          o osxphotos-run_command_line            o osxphotos-export_command
             option                                  line_option
-    * --hidden                                    o osxphotos-inspect_command
+    * --hidden                                    o osxphotos-query_command
           o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-orphans_command
-          o osxphotos-export_command                line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-export_command                option
             line_option                           o osxphotos-sync_command_line
           o osxphotos-query_command                 option
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --time
+            line_option                     * --template
+          o osxphotos-repl_command_line           o osxphotos-inspect_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --theme
+            option                                o osxphotos-add-locations
+    * --ignore-case                                 command_line_option
+          o osxphotos-add-locations               o osxphotos-batch-edit
+            command_line_option                     command_line_option
+          o osxphotos-export_command              o osxphotos-exiftool_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-exportdb_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-import_command
+            option                                  line_option
+    * --ignore-date-modified                      o osxphotos-inspect_command
+          o osxphotos-exiftool_command              line_option
+            line_option                           o osxphotos-orphans_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-sync_command_line
+    * --ignore-signature                            option
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option
+    * --import                              * --time
           o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --ignore-case                         * --time-delta
+    * --in-album                            * --time-delta
           o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
           o osxphotos-export_command        * --time-lapse
             line_option                           o osxphotos-add-locations
           o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
-    * --ignore-date-modified                        option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
-            line_option                             option
+    * --incloud                                     option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
           o osxphotos-export_command        * --timestamp
             line_option                           o osxphotos-add-locations
-    * --ignore-signature                            command_line_option
-          o osxphotos-export_command              o osxphotos-batch-edit
-            line_option                             command_line_option
-    * --import                                    o osxphotos-diff_command_line
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-batch-edit
+          o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-diff_command_line
           o osxphotos-sync_command_line             option
             option                                o osxphotos-exiftool_command
-    * --in-album                                    line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
+    * --info                                        line_option
+          o osxphotos-exportdb_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-import_command
+    * --inspect                                   o osxphotos-exportdb_command
+          o osxphotos-timewarp_command              line_option
+            line_option                           o osxphotos-import_command
+    * --is-reference                                line_option
+          o osxphotos-add-locations               o osxphotos-orphans_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command               o osxphotos-timewarp_command
+            line_option                             line_option, [1]
+          o osxphotos-repl_command_line     * --timezone
+            option                                o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --title
+    * --jpeg-ext                                  o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-batch-edit
+    * --jpeg-quality                                command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-orphans_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --incloud                                   o osxphotos-timewarp_command
-          o osxphotos-add-locations                 line_option, [1]
-            command_line_option             * --timezone
-          o osxphotos-export_command              o osxphotos-timewarp_command
+    * --json                                      o osxphotos-import_command
+          o osxphotos_command_line                  line_option
+            option                                o osxphotos-query_command
+          o osxphotos-albums_command                line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-dump_command_line             option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-info_command_line             option
+            option                          * --tmpdir
+          o osxphotos-keywords_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --title
+          o osxphotos-labels_command        * --to-date
             line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-batch-edit
-          o osxphotos-sync_command_line             command_line_option
+          o osxphotos-list_command_line             command_line_option
             option                                o osxphotos-export_command
-    * --info                                        line_option
-          o osxphotos-exportdb_command            o osxphotos-import_command
-            line_option                             line_option
-    * --inspect                                   o osxphotos-query_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-repl_command_line
-    * --is-reference                                option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * --tmpdir
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --to-date
-          o osxphotos-repl_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-sync_command_line           o osxphotos-export_command
-            option                                  line_option
-    * --jpeg-ext                                  o osxphotos-query_command
-          o osxphotos-export_command                line_option
+          o osxphotos-persons_command               line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-places_command                line_option
             line_option                           o osxphotos-repl_command_line
-    * --jpeg-quality                                option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
+    * --keep                                        option
+          o osxphotos-export_command        * --to-time
+            line_option                           o osxphotos-add-locations
+    * --keyword                                     command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-batch-edit                  o osxphotos-query_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-    * --json                                * --to-time
-          o osxphotos_command_line                o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-albums_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-dump_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-info_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-keywords_command            o osxphotos-sync_command_line
+          o osxphotos-import_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-labels_command        * --touch-file
+          o osxphotos-query_command         * --touch-file
             line_option                           o osxphotos-export_command
-          o osxphotos-list_command_line             line_option
+          o osxphotos-repl_command_line             line_option
             option                                o osxphotos-exportdb_command
-          o osxphotos-persons_command               line_option
-            line_option                     * --undo
-          o osxphotos-places_command              o osxphotos-batch-edit
-            line_option                             command_line_option
-          o osxphotos-query_command         * --unmatched
-            line_option                           o osxphotos-sync_command_line
-    * --keep                                        option
-          o osxphotos-export_command        * --update
+          o osxphotos-sync_command_line             line_option
+            option                          * --undo
+    * --keyword-template                          o osxphotos-batch-edit
+          o osxphotos-exiftool_command              command_line_option
+            line_option                     * --unmatched
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --label                               * --update
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * --update-errors
             line_option                           o osxphotos-export_command
-    * --keyword                                     line_option
-          o osxphotos-add-locations         * --update-errors
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option             * --update-signatures
-          o osxphotos-export_command              o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-import_command        * --upgrade
-            line_option                           o osxphotos-install_command
           o osxphotos-query_command                 line_option
-            line_option                     * --use-file-time
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+            line_option                     * --update-signatures
+          o osxphotos-repl_command_line           o osxphotos-exportdb_command
             option                                  line_option
-          o osxphotos-sync_command_line     * --use-photokit
-            option                                o osxphotos-export_command
-    * --keyword-template                            line_option
-          o osxphotos-exiftool_command      * --use-photos-export
+          o osxphotos-sync_command_line     * --upgrade
+            option                                o osxphotos-install_command
+    * --last-errors                                 line_option
+          o osxphotos-exportdb_command      * --use-file-time
+            line_option                           o osxphotos-timewarp_command
+    * --last-run                                    line_option
+          o osxphotos-exportdb_command      * --use-photokit
             line_option                           o osxphotos-export_command
-          o osxphotos-export_command                line_option
+    * --library                                     line_option
+          o osxphotos_command_line          * --use-photos-export
+            option                                o osxphotos-export_command
+          o osxphotos-albums_command                line_option
             line_option                     * --uti
-    * --label                                     o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
+          o osxphotos-batch-edit                  o osxphotos-add-locations
+            command_line_option                     command_line_option
+          o osxphotos-diff_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-dump_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-exiftool_command            o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-info_command_line     * --uuid
+            option                                o osxphotos-add-locations
+          o osxphotos-inspect_command               command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-keywords_command              line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-labels_command                line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-repl_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                          * --uuid
-    * --last-errors                               o osxphotos-add-locations
-          o osxphotos-exportdb_command              command_line_option
-            line_option                           o osxphotos-export_command
-    * --last-run                                    line_option
-          o osxphotos-exportdb_command            o osxphotos-query_command
-            line_option                             line_option
-    * --library                                   o osxphotos-repl_command_line
-          o osxphotos_command_line                  option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-albums_command                option
+          o osxphotos-orphans_command               option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-persons_command               option
             line_option                     * --uuid-files
-          o osxphotos-batch-edit                  o osxphotos-exportdb_command
-            command_line_option                     line_option
-          o osxphotos-diff_command_line     * --uuid-from-file
-            option                                o osxphotos-add-locations
-          o osxphotos-dump_command_line             command_line_option
+          o osxphotos-places_command              o osxphotos-exportdb_command
+            line_option                             line_option
+          o osxphotos-query_command         * --uuid-from-file
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-export_command
-          o osxphotos-exiftool_command              line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-info_command_line             option
+          o osxphotos-show_command_line             line_option
+            option                                o osxphotos-query_command
+          o osxphotos-snap_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
             option                                o osxphotos-sync_command_line
-          o osxphotos-inspect_command               option
+          o osxphotos-timewarp_command              option
             line_option                     * --uuid-info
-          o osxphotos-keywords_command            o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-labels_command        * --vacuum
-            line_option                           o osxphotos-exportdb_command
-          o osxphotos-orphans_command               line_option
+    * --limit                                     o osxphotos-exportdb_command
+          o osxphotos-export_command                line_option
+            line_option                     * --vacuum
+    * --list                                      o osxphotos-exportdb_command
+          o osxphotos-theme_command                 line_option
             line_option                     * --verbose
-          o osxphotos-persons_command             o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-places_command              o osxphotos-batch-edit
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-diff_command_line
+    * --live                                      o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-batch-edit
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-diff_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-exiftool_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-exportdb_command
+    * --load-config                                 line_option
+          o osxphotos-exiftool_command            o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-export_command              o osxphotos-orphans_command
+            line_option                             line_option
+    * --location                                  o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option             * --version
+          o osxphotos-export_command              o osxphotos_command_line
             line_option                             option
-          o osxphotos-repl_command_line           o osxphotos-exiftool_command
-            option                                  line_option
-          o osxphotos-show_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-snap_command_line           o osxphotos-exportdb_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-          o osxphotos-timewarp_command            o osxphotos-orphans_command
+          o osxphotos-import_command              o osxphotos-exportdb_command
             line_option                             line_option
-    * --limit                                     o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                           o osxphotos-timewarp_command
-    * --list                                        line_option
-          o osxphotos-theme_command         * --version
-            line_option                           o osxphotos_command_line
-    * --live                                        option
-          o osxphotos-add-locations               o osxphotos-exportdb_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --walk
+          o osxphotos-query_command         * --walk
             line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --window
-          o osxphotos-repl_command_line           o osxphotos-add-locations
+          o osxphotos-repl_command_line             line_option
+            option                          * --window
+          o osxphotos-sync_command_line           o osxphotos-add-locations
             option                                  command_line_option
-          o osxphotos-sync_command_line     * --xattr-template
-            option                                o osxphotos-export_command
-    * --load-config                                 line_option
-          o osxphotos-exiftool_command      * --year
-            line_option                           o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --location                                    line_option
-          o osxphotos-add-locations               o osxphotos-query_command
-            command_line_option                     line_option
-          o osxphotos-batch-edit                  o osxphotos-repl_command_line
-            command_line_option                     option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+    * --match-time                          * --xattr-template
+          o osxphotos-timewarp_command            o osxphotos-export_command
+            line_option                             line_option
+    * --max-size                            * --year
+          o osxphotos-add-locations               o osxphotos-add-locations
+            command_line_option                     command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+    * --merge                               * --yes
+          o osxphotos-sync_command_line           o osxphotos-uninstall_command
+            option                                  line_option
+    * --merge-keywords                      * -A
+          o osxphotos-import_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-import_command        * --yes
-            line_option                           o osxphotos-uninstall_command
-          o osxphotos-query_command                 line_option
-            line_option                     * -A
+    * --migrate                             * -a
+          o osxphotos-exportdb_command            o osxphotos-import_command
+            line_option                             line_option
+    * --migrate-photos-library                    o osxphotos-timewarp_command
+          o osxphotos-exportdb_command              line_option
+            line_option                     * -C
+    * --min-size                                  o osxphotos-import_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -c
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-query_command         * -D
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -d
+    * --missing                                   o osxphotos-import_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * -e
+          o osxphotos-query_command               o osxphotos-import_command
+            line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-sync_command_line
             option                                  option
-          o osxphotos-sync_command_line     * -a
-            option                                o osxphotos-import_command
-    * --match-time                                  line_option
-          o osxphotos-timewarp_command            o osxphotos-timewarp_command
-            line_option                             line_option
-    * --max-size                            * -C
-          o osxphotos-add-locations               o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -c
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-query_command                 line_option
-            line_option                     * -D
-          o osxphotos-repl_command_line           o osxphotos-import_command
-            option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --merge                               * -d
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --merge-keywords                            o osxphotos-timewarp_command
-          o osxphotos-import_command                line_option
-            line_option                     * -e
-    * --migrate                                   o osxphotos-import_command
-          o osxphotos-exportdb_command              line_option
-            line_option                           o osxphotos-sync_command_line
-    * --migrate-photos-library                      option
-          o osxphotos-exportdb_command            o osxphotos-timewarp_command
-            line_option                             line_option
-    * --min-size                            * -F
+    * --name                                * -F
           o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
           o osxphotos-export_command        * -f
             line_option                           o osxphotos-dump_command_line
           o osxphotos-query_command                 option
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-timewarp_command
-    * --missing                                     line_option
+    * --no-comment                                  line_option
           o osxphotos-add-locations               o osxphotos-uuid_command_line
             command_line_option                     option
           o osxphotos-export_command        * -g
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                     * -h
           o osxphotos-repl_command_line           o osxphotos-run_command_line
             option                                  option
           o osxphotos-sync_command_line     * -i
             option                                o osxphotos-add-locations
-    * --name                                        command_line_option
+    * --no-description                              command_line_option
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-repl_command_line           o osxphotos-sync_command_line
             option                                  option, [1]
           o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --no-comment                          * -k
+    * --no-keyword                          * -k
           o osxphotos-add-locations               o osxphotos-import_command
             command_line_option                     line_option
           o osxphotos-export_command        * -L
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-timewarp_command
           o osxphotos-repl_command_line             line_option
             option                          * -l
           o osxphotos-sync_command_line           o osxphotos-import_command
             option                                  line_option
-    * --no-description                      * -M
+    * --no-likes                            * -M
           o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
           o osxphotos-export_command        * -m
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
             option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
             option                          * -P
-    * --no-keyword                                o osxphotos-import_command
+    * --no-location                               o osxphotos-import_command
           o osxphotos-add-locations                 line_option
             command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
             line_option                     * -p
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
           o osxphotos-sync_command_line     * -R
             option                                o osxphotos-import_command
-    * --no-likes                                    line_option
+    * --no-place                                    line_option
           o osxphotos-add-locations               o osxphotos-sync_command_line
             command_line_option                     option
           o osxphotos-export_command        * -r
             line_option                           o osxphotos-diff_command_line
           o osxphotos-query_command                 option
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
             option                          * -s
           o osxphotos-sync_command_line           o osxphotos-diff_command_line
             option                                  option
-    * --no-location                               o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * -T
-          o osxphotos-export_command              o osxphotos-inspect_command
+    * --no-progress                               o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * -T
+          o osxphotos-import_command              o osxphotos-inspect_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-timewarp_command
+    * --no-title                                  o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -t
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * -t
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-inspect_command
-    * --no-place                                    line_option
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -U
-            line_option                           o osxphotos-install_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-repl_command_line             option
-            option                          * -V
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --no-progress                               o osxphotos-batch-edit
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-diff_command_line
-          o osxphotos-import_command                option
-            line_option                           o osxphotos-exiftool_command
-    * --no-title                                    line_option
+          o osxphotos-query_command               o osxphotos-inspect_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * -U
+            option                                o osxphotos-install_command
+    * --not-burst                                   line_option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * -V
+            line_option                           o osxphotos-add-locations
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-batch-edit
+          o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-diff_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-exiftool_command
+    * --not-cloudasset                              line_option
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-exportdb_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-orphans_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option
-    * --not-burst                                 o osxphotos-timewarp_command
+    * --not-edited                                o osxphotos-timewarp_command
           o osxphotos-add-locations                 line_option
             command_line_option             * -v
           o osxphotos-export_command              o osxphotos_command_line
             line_option                             option
           o osxphotos-query_command         * -w
             line_option                           o osxphotos-add-locations
           o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
             option                          * -y
-    * --not-cloudasset                            o osxphotos-uninstall_command
+    * --not-favorite                              o osxphotos-uninstall_command
           o osxphotos-add-locations                 line_option
             command_line_option             * -z
           o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
           o osxphotos-query_command
             line_option
           o osxphotos-repl_command_line
@@ -1187,335 +1209,347 @@
       attribute)                             * movies_(osxphotos.QueryOptions
     * missing_(osxphotos.QueryOptions          attribute)
       attribute)
     * missing_bursts_
       (osxphotos.QueryOptions_attribute)
 
 ***** N *****
-                                            * not_hdr_(osxphotos.QueryOptions
-                                              attribute)
                                             * not_hidden_
+                                              (osxphotos.QueryOptions
+                                              attribute)
+                                            * not_in_album_
     * name_(osxphotos.QueryOptions            (osxphotos.QueryOptions
       attribute)                              attribute)
-    * neighborhoods_                        * not_in_album_
+    * neighborhoods_                        * not_incloud_
       (osxphotos.SearchInfo_property)         (osxphotos.QueryOptions
     * no_comment_                             attribute)
-      (osxphotos.QueryOptions               * not_incloud_
-      attribute)                              (osxphotos.QueryOptions
-    * no_description_                         attribute)
       (osxphotos.QueryOptions               * not_live_(osxphotos.QueryOptions
       attribute)                              attribute)
-    * no_keyword_                           * not_missing_
+    * no_description_                       * not_missing_
+      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
+      attribute)                              attribute)
+    * no_keyword_                           * not_panorama_
       (osxphotos.QueryOptions                 (osxphotos.QueryOptions
       attribute)                              attribute)
-    * no_likes_(osxphotos.QueryOptions      * not_panorama_
+    * no_likes_(osxphotos.QueryOptions      * not_portrait_
       attribute)                              (osxphotos.QueryOptions
     * no_location_                            attribute)
-      (osxphotos.QueryOptions               * not_portrait_
+      (osxphotos.QueryOptions               * not_reference_
       attribute)                              (osxphotos.QueryOptions
     * no_place_(osxphotos.QueryOptions        attribute)
-      attribute)                            * not_reference_
+      attribute)                            * not_saved_to_library_
     * no_title_(osxphotos.QueryOptions        (osxphotos.QueryOptions
       attribute)                              attribute)
     * not_burst_(osxphotos.QueryOptions     * not_screenshot_
       attribute)                              (osxphotos.QueryOptions
     * not_cloudasset_                         attribute)
       (osxphotos.QueryOptions               * not_selfie_
       attribute)                              (osxphotos.QueryOptions
     * not_edited_                             attribute)
       (osxphotos.QueryOptions               * not_shared_
       attribute)                              (osxphotos.QueryOptions
     * not_favorite_                           attribute)
       (osxphotos.QueryOptions               * not_slow_mo_
       attribute)                              (osxphotos.QueryOptions
+    * not_hdr_(osxphotos.QueryOptions         attribute)
+      attribute)                            * not_syndicated_
+                                              (osxphotos.QueryOptions
                                               attribute)
                                             * not_time_lapse_
                                               (osxphotos.QueryOptions
                                               attribute)
 
 ***** O *****
                                             * osxphotos-info command line
-    * orientation_(osxphotos.PhotoInfo        option
-      property)                                   o --db
-    * original_filename_                          o --json
-      (osxphotos.PhotoInfo_property)              o --library
-    * original_filesize_                          o PHOTOS_LIBRARY
+                                              option
+                                                  o --db
+    * orientation_(osxphotos.PhotoInfo            o --json
+      property)                                   o --library
+    * original_filename_                          o PHOTOS_LIBRARY
       (osxphotos.PhotoInfo_property)        * osxphotos-inspect command line
-    * original_height_                        option
+    * original_filesize_                      option
       (osxphotos.PhotoInfo_property)              o --db
-    * original_orientation_                       o --detect-text
+    * original_height_                            o --detect-text
       (osxphotos.PhotoInfo_property)              o --library
-    * original_width_                             o --template
+    * original_orientation_                       o --template
       (osxphotos.PhotoInfo_property)              o --theme
-    * osxphotos                                   o -t
-          o module                                o -T
-    * osxphotos command line option         * osxphotos-install command line
-          o --db                              option
-          o --json                                o --upgrade
-          o --library                             o -U
-          o --version                             o PACKAGES
-          o -v                              * osxphotos-keywords command line
-    * osxphotos-add-locations command         option
-      line option                                 o --db
-          o --added-after                         o --json
-          o --added-before                        o --library
-          o --added-in-last                       o PHOTOS_LIBRARY
-          o --album                         * osxphotos-labels command line
-          o --burst                           option
-          o --cloudasset                          o --db
-          o --description                         o --json
-          o --dry-run                             o --library
-          o --duplicate                           o PHOTOS_LIBRARY
-          o --edited                        * osxphotos-list command line
-          o --exif                            option
-          o --external-edit                       o --json
-          o --favorite                      * osxphotos-orphans command line
-          o --folder                          option
-          o --from-date                           o --db
-          o --from-time                           o --export
-          o --has-comment                         o --library
-          o --has-likes                           o --theme
-          o --has-raw                             o --timestamp
-          o --hdr                                 o --verbose
-          o --hidden                              o -V
-          o --ignore-case                   * osxphotos-persons command line
-          o --in-album                        option
-          o --incloud                             o --db
-          o --is-reference                        o --json
-          o --keyword                             o --library
-          o --label                               o PHOTOS_LIBRARY
-          o --live                          * osxphotos-places command line
-          o --location                        option
-          o --max-size                            o --db
-          o --min-size                            o --json
-          o --missing                             o --library
-          o --name                                o PHOTOS_LIBRARY
-          o --no-comment                    * osxphotos-query command line
-          o --no-description                  option
-          o --no-keyword                          o --add-to-album
-          o --no-likes                            o --added-after
-          o --no-location                         o --added-before
-          o --no-place                            o --added-in-last
-          o --no-title                            o --album
-          o --not-burst                           o --burst
-          o --not-cloudasset                      o --cloudasset
-          o --not-edited                          o --db
-          o --not-favorite                        o --deleted
-          o --not-hdr                             o --deleted-only
-          o --not-hidden                          o --description
-          o --not-in-album                        o --duplicate
-          o --not-incloud                         o --edited
-          o --not-live                            o --exif
-          o --not-missing                         o --external-edit
-          o --not-panorama                        o --favorite
-          o --not-portrait                        o --field
-          o --not-reference                       o --folder
-          o --not-screenshot                      o --from-date
-          o --not-selfie                          o --from-time
-          o --not-shared                          o --has-comment
-          o --not-slow-mo                         o --has-likes
-          o --not-time-lapse                      o --has-raw
-          o --only-movies                         o --hdr
-          o --only-photos                         o --hidden
-          o --panorama                            o --ignore-case
-          o --person                              o --in-album
-          o --place                               o --incloud
-          o --portrait                            o --is-reference
-          o --query-eval                          o --json
-          o --query-function                      o --keyword
-          o --regex                               o --label
-          o --screenshot                          o --library
-          o --selected                            o --live
-          o --selfie                              o --location
-          o --shared                              o --max-size
-          o --slow-mo                             o --min-size
-          o --theme                               o --missing
-          o --time-lapse                          o --name
-          o --timestamp                           o --no-comment
-          o --title                               o --no-description
-          o --to-date                             o --no-keyword
-          o --to-time                             o --no-likes
-          o --uti                                 o --no-location
-          o --uuid                                o --no-place
-          o --uuid-from-file                      o --no-title
-          o --verbose                             o --not-burst
-          o --window                              o --not-cloudasset
-          o --year                                o --not-edited
-          o -i                                    o --not-favorite
-          o -V                                    o --not-hdr
-          o -w                                    o --not-hidden
-    * osxphotos-albums command line               o --not-in-album
-      option                                      o --not-incloud
-          o --db                                  o --not-live
-          o --json                                o --not-missing
-          o --library                             o --not-panorama
-          o PHOTOS_LIBRARY                        o --not-portrait
-    * osxphotos-batch-edit command line           o --not-reference
-      option                                      o --not-screenshot
-          o --db                                  o --not-selfie
-          o --description                         o --not-shared
-          o --dry-run                             o --not-slow-mo
-          o --keyword                             o --not-time-lapse
-          o --library                             o --only-movies
-          o --location                            o --only-photos
-          o --replace-keywords                    o --panorama
-          o --theme                               o --person
-          o --timestamp                           o --place
-          o --title                               o --portrait
-          o --undo                                o --print
-          o --verbose                             o --query-eval
-          o -V                                    o --query-function
-    * osxphotos-diff command line                 o --quiet
-      option                                      o --regex
-          o --db                                  o --screenshot
-          o --library                             o --selected
-          o --raw-output                          o --selfie
-          o --style                               o --shared
-          o --timestamp                           o --slow-mo
-          o --verbose                             o --time-lapse
-          o -r                                    o --title
-          o -s                                    o --to-date
-          o -V                                    o --to-time
-          o DB2                                   o --uti
-    * osxphotos-dump command line                 o --uuid
-      option                                      o --uuid-from-file
-          o --db                                  o --year
-          o --deleted                             o -f
-          o --deleted-only                        o -i
-          o --field                               o PHOTOS_LIBRARY
-          o --json                          * osxphotos-repl command line
-          o --library                         option
-          o --print                               o --added-after
-          o -f                                    o --added-before
-          o PHOTOS_LIBRARY                        o --added-in-last
-    * osxphotos-exiftool command line             o --album
-      option                                      o --burst
-          o --album-keyword                       o --cloudasset
-          o --append                              o --db
-          o --db                                  o --deleted
-          o --db-config                           o --deleted-only
-          o --description-template                o --description
-          o --dry-run                             o --duplicate
-          o --exiftool-merge-keywords             o --edited
-          o --exiftool-merge-persons              o --emacs
-          o --exiftool-option                     o --exif
-          o --exiftool-path                       o --external-edit
-          o --exportdb                            o --favorite
-          o --ignore-date-modified                o --folder
-          o --keyword-template                    o --from-date
-          o --library                             o --from-time
-          o --load-config                         o --has-comment
-          o --person-keyword                      o --has-likes
-          o --replace-keywords                    o --has-raw
-          o --report                              o --hdr
-          o --save-config                         o --hidden
-          o --theme                               o --ignore-case
-          o --timestamp                           o --in-album
-          o --verbose                             o --incloud
-          o -V                                    o --is-reference
-          o EXPORT_DIRECTORY                      o --keyword
-    * osxphotos-export command line               o --label
-      option                                      o --library
-          o --add-exported-to-album               o --live
-          o --add-missing-to-album                o --location
-          o --add-skipped-to-album                o --max-size
-          o --added-after                         o --min-size
-          o --added-before                        o --missing
-          o --added-in-last                       o --name
-          o --album                               o --no-comment
-          o --album-keyword                       o --no-description
-          o --alt-copy                            o --no-keyword
-          o --append                              o --no-likes
-          o --burst                               o --no-location
-          o --cleanup                             o --no-place
-          o --cloudasset                          o --no-title
-          o --config-only                         o --not-burst
-          o --convert-to-jpeg                     o --not-cloudasset
-          o --current-name                        o --not-edited
-          o --db                                  o --not-favorite
-          o --deleted                             o --not-hdr
-          o --deleted-only                        o --not-hidden
-          o --description                         o --not-in-album
-          o --description-template                o --not-incloud
-          o --directory                           o --not-live
-          o --download-missing                    o --not-missing
-          o --dry-run                             o --not-panorama
-          o --duplicate                           o --not-portrait
-          o --edited                              o --not-reference
-          o --edited-suffix                       o --not-screenshot
-          o --exif                                o --not-selfie
-          o --exiftool                            o --not-shared
-          o --exiftool-merge-keywords             o --not-slow-mo
+    * original_width_                             o -t
+      (osxphotos.PhotoInfo_property)              o -T
+    * osxphotos                             * osxphotos-install command line
+          o module                            option
+    * osxphotos command line option               o --upgrade
+          o --db                                  o -U
+          o --json                                o PACKAGES
+          o --library                       * osxphotos-keywords command line
+          o --version                         option
+          o -v                                    o --db
+    * osxphotos-add-locations command             o --json
+      line option                                 o --library
+          o --added-after                         o PHOTOS_LIBRARY
+          o --added-before                  * osxphotos-labels command line
+          o --added-in-last                   option
+          o --album                               o --db
+          o --burst                               o --json
+          o --cloudasset                          o --library
+          o --description                         o PHOTOS_LIBRARY
+          o --dry-run                       * osxphotos-list command line
+          o --duplicate                       option
+          o --edited                              o --json
+          o --exif                          * osxphotos-orphans command line
+          o --external-edit                   option
+          o --favorite                            o --db
+          o --folder                              o --export
+          o --from-date                           o --library
+          o --from-time                           o --theme
+          o --has-comment                         o --timestamp
+          o --has-likes                           o --verbose
+          o --has-raw                             o -V
+          o --hdr                           * osxphotos-persons command line
+          o --hidden                          option
+          o --ignore-case                         o --db
+          o --in-album                            o --json
+          o --incloud                             o --library
+          o --is-reference                        o PHOTOS_LIBRARY
+          o --keyword                       * osxphotos-places command line
+          o --label                           option
+          o --live                                o --db
+          o --location                            o --json
+          o --max-size                            o --library
+          o --min-size                            o PHOTOS_LIBRARY
+          o --missing                       * osxphotos-query command line
+          o --name                            option
+          o --no-comment                          o --add-to-album
+          o --no-description                      o --added-after
+          o --no-keyword                          o --added-before
+          o --no-likes                            o --added-in-last
+          o --no-location                         o --album
+          o --no-place                            o --burst
+          o --no-title                            o --cloudasset
+          o --not-burst                           o --db
+          o --not-cloudasset                      o --deleted
+          o --not-edited                          o --deleted-only
+          o --not-favorite                        o --description
+          o --not-hdr                             o --duplicate
+          o --not-hidden                          o --edited
+          o --not-in-album                        o --exif
+          o --not-incloud                         o --external-edit
+          o --not-live                            o --favorite
+          o --not-missing                         o --field
+          o --not-panorama                        o --folder
+          o --not-portrait                        o --from-date
+          o --not-reference                       o --from-time
+          o --not-saved-to-library                o --has-comment
+          o --not-screenshot                      o --has-likes
+          o --not-selfie                          o --has-raw
+          o --not-shared                          o --hdr
+          o --not-slow-mo                         o --hidden
+          o --not-syndicated                      o --ignore-case
+          o --not-time-lapse                      o --in-album
+          o --only-movies                         o --incloud
+          o --only-photos                         o --is-reference
+          o --panorama                            o --json
+          o --person                              o --keyword
+          o --place                               o --label
+          o --portrait                            o --library
+          o --query-eval                          o --live
+          o --query-function                      o --location
+          o --regex                               o --max-size
+          o --saved-to-library                    o --min-size
+          o --screenshot                          o --missing
+          o --selected                            o --name
+          o --selfie                              o --no-comment
+          o --shared                              o --no-description
+          o --slow-mo                             o --no-keyword
+          o --syndicated                          o --no-likes
+          o --theme                               o --no-location
+          o --time-lapse                          o --no-place
+          o --timestamp                           o --no-title
+          o --title                               o --not-burst
+          o --to-date                             o --not-cloudasset
+          o --to-time                             o --not-edited
+          o --uti                                 o --not-favorite
+          o --uuid                                o --not-hdr
+          o --uuid-from-file                      o --not-hidden
+          o --verbose                             o --not-in-album
+          o --window                              o --not-incloud
+          o --year                                o --not-live
+          o -i                                    o --not-missing
+          o -V                                    o --not-panorama
+          o -w                                    o --not-portrait
+    * osxphotos-albums command line               o --not-reference
+      option                                      o --not-saved-to-library
+          o --db                                  o --not-screenshot
+          o --json                                o --not-selfie
+          o --library                             o --not-shared
+          o PHOTOS_LIBRARY                        o --not-slow-mo
+    * osxphotos-batch-edit command line           o --not-syndicated
+      option                                      o --not-time-lapse
+          o --db                                  o --only-movies
+          o --description                         o --only-photos
+          o --dry-run                             o --panorama
+          o --keyword                             o --person
+          o --library                             o --place
+          o --location                            o --portrait
+          o --replace-keywords                    o --print
+          o --theme                               o --query-eval
+          o --timestamp                           o --query-function
+          o --title                               o --quiet
+          o --undo                                o --regex
+          o --verbose                             o --saved-to-library
+          o -V                                    o --screenshot
+    * osxphotos-diff command line                 o --selected
+      option                                      o --selfie
+          o --db                                  o --shared
+          o --library                             o --slow-mo
+          o --raw-output                          o --syndicated
+          o --style                               o --time-lapse
+          o --timestamp                           o --title
+          o --verbose                             o --to-date
+          o -r                                    o --to-time
+          o -s                                    o --uti
+          o -V                                    o --uuid
+          o DB2                                   o --uuid-from-file
+    * osxphotos-dump command line                 o --year
+      option                                      o -f
+          o --db                                  o -i
+          o --deleted                             o PHOTOS_LIBRARY
+          o --deleted-only                  * osxphotos-repl command line
+          o --field                           option
+          o --json                                o --added-after
+          o --library                             o --added-before
+          o --print                               o --added-in-last
+          o -f                                    o --album
+          o PHOTOS_LIBRARY                        o --burst
+    * osxphotos-exiftool command line             o --cloudasset
+      option                                      o --db
+          o --album-keyword                       o --deleted
+          o --append                              o --deleted-only
+          o --db                                  o --description
+          o --db-config                           o --duplicate
+          o --description-template                o --edited
+          o --dry-run                             o --emacs
+          o --exiftool-merge-keywords             o --exif
+          o --exiftool-merge-persons              o --external-edit
+          o --exiftool-option                     o --favorite
+          o --exiftool-path                       o --folder
+          o --exportdb                            o --from-date
+          o --ignore-date-modified                o --from-time
+          o --keyword-template                    o --has-comment
+          o --library                             o --has-likes
+          o --load-config                         o --has-raw
+          o --person-keyword                      o --hdr
+          o --replace-keywords                    o --hidden
+          o --report                              o --ignore-case
+          o --save-config                         o --in-album
+          o --theme                               o --incloud
+          o --timestamp                           o --is-reference
+          o --verbose                             o --keyword
+          o -V                                    o --label
+          o EXPORT_DIRECTORY                      o --library
+    * osxphotos-export command line               o --live
+      option                                      o --location
+          o --add-exported-to-album               o --max-size
+          o --add-missing-to-album                o --min-size
+          o --add-skipped-to-album                o --missing
+          o --added-after                         o --name
+          o --added-before                        o --no-comment
+          o --added-in-last                       o --no-description
+          o --album                               o --no-keyword
+          o --album-keyword                       o --no-likes
+          o --alt-copy                            o --no-location
+          o --append                              o --no-place
+          o --burst                               o --no-title
+          o --cleanup                             o --not-burst
+          o --cloudasset                          o --not-cloudasset
+          o --config-only                         o --not-edited
+          o --convert-to-jpeg                     o --not-favorite
+          o --current-name                        o --not-hdr
+          o --db                                  o --not-hidden
+          o --deleted                             o --not-in-album
+          o --deleted-only                        o --not-incloud
+          o --description                         o --not-live
+          o --description-template                o --not-missing
+          o --directory                           o --not-panorama
+          o --download-missing                    o --not-portrait
+          o --dry-run                             o --not-reference
+          o --duplicate                           o --not-saved-to-library
+          o --edited                              o --not-screenshot
+          o --edited-suffix                       o --not-selfie
+          o --exif                                o --not-shared
+          o --exiftool                            o --not-slow-mo
+          o --exiftool-merge-keywords             o --not-syndicated
           o --exiftool-merge-persons              o --not-time-lapse
           o --exiftool-option                     o --only-movies
           o --exiftool-path                       o --only-photos
           o --export-as-hardlink                  o --panorama
           o --export-by-date                      o --person
           o --exportdb                            o --place
           o --external-edit                       o --portrait
           o --favorite                            o --query-eval
           o --favorite-rating                     o --query-function
           o --filename                            o --regex
-          o --finder-tag-keywords                 o --screenshot
-          o --finder-tag-template                 o --selected
-          o --folder                              o --selfie
-          o --force-update                        o --shared
-          o --from-date                           o --slow-mo
-          o --from-time                           o --time-lapse
-          o --has-comment                         o --title
-          o --has-likes                           o --to-date
-          o --has-raw                             o --to-time
-          o --hdr                                 o --uti
-          o --hidden                              o --uuid
-          o --ignore-case                         o --uuid-from-file
-          o --ignore-date-modified                o --year
-          o --ignore-signature                    o -i
-          o --in-album                      * osxphotos-run command line option
-          o --incloud                             o --help
-          o --is-reference                        o -h
-          o --jpeg-ext                            o ARGS
-          o --jpeg-quality                        o PYTHON_FILE
-          o --keep                          * osxphotos-show command line
-          o --keyword                         option
-          o --keyword-template                    o --db
-          o --label                               o --library
-          o --library                             o UUID_OR_NAME
-          o --limit                         * osxphotos-snap command line
-          o --live                            option
-          o --load-config                         o --db
-          o --location                            o --library
-          o --max-size                      * osxphotos-sync command line
-          o --min-size                        option
-          o --missing                             o --added-after
-          o --name                                o --added-before
-          o --no-comment                          o --added-in-last
-          o --no-description                      o --album
-          o --no-keyword                          o --append
-          o --no-likes                            o --burst
-          o --no-location                         o --cloudasset
-          o --no-place                            o --db
-          o --no-progress                         o --description
-          o --no-title                            o --dry-run
-          o --not-burst                           o --duplicate
-          o --not-cloudasset                      o --edited
-          o --not-edited                          o --exif
-          o --not-favorite                        o --export
-          o --not-hdr                             o --external-edit
-          o --not-hidden                          o --favorite
-          o --not-in-album                        o --folder
-          o --not-incloud                         o --from-date
-          o --not-live                            o --from-time
-          o --not-missing                         o --has-comment
-          o --not-panorama                        o --has-likes
-          o --not-portrait                        o --has-raw
-          o --not-reference                       o --hdr
-          o --not-screenshot                      o --hidden
-          o --not-selfie                          o --ignore-case
-          o --not-shared                          o --import
-          o --not-slow-mo                         o --in-album
+          o --finder-tag-keywords                 o --saved-to-library
+          o --finder-tag-template                 o --screenshot
+          o --folder                              o --selected
+          o --force-update                        o --selfie
+          o --from-date                           o --shared
+          o --from-time                           o --slow-mo
+          o --has-comment                         o --syndicated
+          o --has-likes                           o --time-lapse
+          o --has-raw                             o --title
+          o --hdr                                 o --to-date
+          o --hidden                              o --to-time
+          o --ignore-case                         o --uti
+          o --ignore-date-modified                o --uuid
+          o --ignore-signature                    o --uuid-from-file
+          o --in-album                            o --year
+          o --incloud                             o -i
+          o --is-reference                  * osxphotos-run command line option
+          o --jpeg-ext                            o --help
+          o --jpeg-quality                        o -h
+          o --keep                                o ARGS
+          o --keyword                             o PYTHON_FILE
+          o --keyword-template              * osxphotos-show command line
+          o --label                           option
+          o --library                             o --db
+          o --limit                               o --library
+          o --live                                o UUID_OR_NAME
+          o --load-config                   * osxphotos-snap command line
+          o --location                        option
+          o --max-size                            o --db
+          o --min-size                            o --library
+          o --missing                       * osxphotos-sync command line
+          o --name                            option
+          o --no-comment                          o --added-after
+          o --no-description                      o --added-before
+          o --no-keyword                          o --added-in-last
+          o --no-likes                            o --album
+          o --no-location                         o --append
+          o --no-place                            o --burst
+          o --no-progress                         o --cloudasset
+          o --no-title                            o --db
+          o --not-burst                           o --description
+          o --not-cloudasset                      o --dry-run
+          o --not-edited                          o --duplicate
+          o --not-favorite                        o --edited
+          o --not-hdr                             o --exif
+          o --not-hidden                          o --export
+          o --not-in-album                        o --external-edit
+          o --not-incloud                         o --favorite
+          o --not-live                            o --folder
+          o --not-missing                         o --from-date
+          o --not-panorama                        o --from-time
+          o --not-portrait                        o --has-comment
+          o --not-reference                       o --has-likes
+          o --not-saved-to-library                o --has-raw
+          o --not-screenshot                      o --hdr
+          o --not-selfie                          o --hidden
+          o --not-shared                          o --ignore-case
+          o --not-slow-mo                         o --import
+          o --not-syndicated                      o --in-album
           o --not-time-lapse                      o --incloud
           o --only-movies                         o --is-reference
           o --only-new                            o --keyword
           o --only-photos                         o --label
           o --original-suffix                     o --library
           o --overwrite                           o --live
           o --panorama                            o --location
@@ -1533,129 +1567,133 @@
           o --query-function                      o --no-title
           o --ramdb                               o --not-burst
           o --regex                               o --not-cloudasset
           o --replace-keywords                    o --not-edited
           o --report                              o --not-favorite
           o --retry                               o --not-hdr
           o --save-config                         o --not-hidden
-          o --screenshot                          o --not-in-album
-          o --selected                            o --not-incloud
-          o --selfie                              o --not-live
-          o --shared                              o --not-missing
-          o --sidecar                             o --not-panorama
-          o --sidecar-drop-ext                    o --not-portrait
-          o --skip-bursts                         o --not-reference
+          o --saved-to-library                    o --not-in-album
+          o --screenshot                          o --not-incloud
+          o --selected                            o --not-live
+          o --selfie                              o --not-missing
+          o --shared                              o --not-panorama
+          o --sidecar                             o --not-portrait
+          o --sidecar-drop-ext                    o --not-reference
+          o --skip-bursts                         o --not-saved-to-library
           o --skip-edited                         o --not-screenshot
           o --skip-live                           o --not-selfie
           o --skip-original-if-edited             o --not-slow-mo
-          o --skip-raw                            o --not-time-lapse
-          o --skip-uuid                           o --only-movies
-          o --skip-uuid-from-file                 o --only-photos
-          o --slow-mo                             o --panorama
-          o --strip                               o --person
+          o --skip-raw                            o --not-syndicated
+          o --skip-uuid                           o --not-time-lapse
+          o --skip-uuid-from-file                 o --only-movies
+          o --slow-mo                             o --only-photos
+          o --strip                               o --panorama
+          o --syndicated                          o --person
           o --theme                               o --place
           o --time-lapse                          o --portrait
           o --timestamp                           o --query-eval
           o --title                               o --query-function
           o --tmpdir                              o --regex
           o --to-date                             o --report
-          o --to-time                             o --screenshot
-          o --touch-file                          o --selected
-          o --update                              o --selfie
-          o --update-errors                       o --set
-          o --use-photokit                        o --slow-mo
-          o --use-photos-export                   o --theme
-          o --uti                                 o --time-lapse
-          o --uuid                                o --timestamp
-          o --uuid-from-file                      o --title
-          o --verbose                             o --to-date
-          o --xattr-template                      o --to-time
-          o --year                                o --unmatched
-          o -i                                    o --uti
-          o -V                                    o --uuid
-          o DEST                                  o --uuid-from-file
-          o PHOTOS_LIBRARY                        o --verbose
-    * osxphotos-exportdb command line             o --year
-      option                                      o -A
-          o --append                              o -e
-          o --check-signatures                    o -i, [1]
-          o --delete-file                         o -m
-          o --delete-uuid                         o -R
-          o --dry-run                             o -s
-          o --errors                              o -U
-          o --export-dir                          o -V
-          o --info                          * osxphotos-theme command line
-          o --last-errors                     option
-          o --last-run                            o --clone
-          o --migrate                             o --config
-          o --migrate-photos-library              o --default
-          o --report                              o --delete
-          o --save-config                         o --edit
-          o --sql                                 o --list
-          o --theme                               o --preview
-          o --timestamp                     * osxphotos-timewarp command line
-          o --touch-file                      option
-          o --update-signatures                   o --add-to-album
-          o --uuid-files                          o --compare-exif
-          o --uuid-info                           o --date
-          o --vacuum                              o --date-added
-          o --verbose                             o --date-added-from-photo
-          o --version                             o --date-delta
-          o -V                                    o --exiftool-path
-          o EXPORT_DATABASE                       o --force
-    * osxphotos-help command line                 o --function
-      option                                      o --inspect
-          o SUBTOPIC                              o --library
-          o TOPIC                                 o --match-time
-    * osxphotos-import command line               o --parse-date
-      option                                      o --plain
-          o --album                               o --pull-exif
-          o --append                              o --push-exif
-          o --check-templates                     o --theme
-          o --clear-location                      o --time
-          o --clear-metadata                      o --time-delta
-          o --description                         o --timestamp, [1]
-          o --dup-check                           o --timezone
-          o --exiftool                            o --use-file-time
-          o --exiftool-path                       o --verbose
-          o --glob                                o -a
-          o --keyword                             o -c
-          o --location                            o -d
-          o --merge-keywords                      o -D
-          o --no-progress                         o -e
-          o --parse-date                          o -F
-          o --post-function                       o -f
-          o --relative-to                         o -i
-          o --report                              o -L
-          o --resume                              o -M
-          o --split-folder                        o -m
-          o --theme                               o -p
-          o --timestamp                           o -P
-          o --title                               o -t
-          o --verbose                             o -T
-          o --walk                                o -V
-          o -a                                    o -z
-          o -C                              * osxphotos-tutorial command line
-          o -d                                option
-          o -D                                    o WIDTH
-          o -e                              * osxphotos-uninstall command line
-          o -f                                option
-          o -g                                    o --yes
-          o -k                                    o -y
-          o -l                                    o PACKAGES
-          o -L                              * osxphotos-uuid command line
-          o -m                                option
-          o -P                                    o --filename
-          o -p                                    o -f
-          o -r                              * osxphotos-version command line
-          o -R                                option
-          o -t                                    o --run
-          o -V                              * overwrite_
-          o -w                                (osxphotos.ExportOptions
-          o FILES                             attribute)
+          o --to-time                             o --saved-to-library
+          o --touch-file                          o --screenshot
+          o --update                              o --selected
+          o --update-errors                       o --selfie
+          o --use-photokit                        o --set
+          o --use-photos-export                   o --slow-mo
+          o --uti                                 o --syndicated
+          o --uuid                                o --theme
+          o --uuid-from-file                      o --time-lapse
+          o --verbose                             o --timestamp
+          o --xattr-template                      o --title
+          o --year                                o --to-date
+          o -i                                    o --to-time
+          o -V                                    o --unmatched
+          o DEST                                  o --uti
+          o PHOTOS_LIBRARY                        o --uuid
+    * osxphotos-exportdb command line             o --uuid-from-file
+      option                                      o --verbose
+          o --append                              o --year
+          o --check-signatures                    o -A
+          o --delete-file                         o -e
+          o --delete-uuid                         o -i, [1]
+          o --dry-run                             o -m
+          o --errors                              o -R
+          o --export-dir                          o -s
+          o --info                                o -U
+          o --last-errors                         o -V
+          o --last-run                      * osxphotos-theme command line
+          o --migrate                         option
+          o --migrate-photos-library              o --clone
+          o --report                              o --config
+          o --save-config                         o --default
+          o --sql                                 o --delete
+          o --theme                               o --edit
+          o --timestamp                           o --list
+          o --touch-file                          o --preview
+          o --update-signatures             * osxphotos-timewarp command line
+          o --uuid-files                      option
+          o --uuid-info                           o --add-to-album
+          o --vacuum                              o --compare-exif
+          o --verbose                             o --date
+          o --version                             o --date-added
+          o -V                                    o --date-added-from-photo
+          o EXPORT_DATABASE                       o --date-delta
+    * osxphotos-help command line                 o --exiftool-path
+      option                                      o --force
+          o SUBTOPIC                              o --function
+          o TOPIC                                 o --inspect
+    * osxphotos-import command line               o --library
+      option                                      o --match-time
+          o --album                               o --parse-date
+          o --append                              o --plain
+          o --check-templates                     o --pull-exif
+          o --clear-location                      o --push-exif
+          o --clear-metadata                      o --theme
+          o --description                         o --time
+          o --dup-check                           o --time-delta
+          o --exiftool                            o --timestamp, [1]
+          o --exiftool-path                       o --timezone
+          o --glob                                o --use-file-time
+          o --keyword                             o --verbose
+          o --location                            o -a
+          o --merge-keywords                      o -c
+          o --no-progress                         o -d
+          o --parse-date                          o -D
+          o --post-function                       o -e
+          o --relative-to                         o -F
+          o --report                              o -f
+          o --resume                              o -i
+          o --split-folder                        o -L
+          o --theme                               o -M
+          o --timestamp                           o -m
+          o --title                               o -p
+          o --verbose                             o -P
+          o --walk                                o -t
+          o -a                                    o -T
+          o -C                                    o -V
+          o -d                                    o -z
+          o -D                              * osxphotos-tutorial command line
+          o -e                                option
+          o -f                                    o WIDTH
+          o -g                              * osxphotos-uninstall command line
+          o -k                                option
+          o -l                                    o --yes
+          o -L                                    o -y
+          o -m                                    o PACKAGES
+          o -P                              * osxphotos-uuid command line
+          o -p                                option
+          o -r                                    o --filename
+          o -R                                    o -f
+          o -t                              * osxphotos-version command line
+          o -V                                option
+          o -w                                    o --run
+          o FILES                           * overwrite_
+                                              (osxphotos.ExportOptions
+                                              attribute)
                                             * owner_(osxphotos.PhotoInfo
                                               property)
 
 ***** P *****
     * PACKAGES
           o osxphotos-install_command       * photos_by_uuid()_
             line_option                       (osxphotos.PhotosDB_method)
@@ -1734,46 +1772,50 @@
       class_method)                           attribute)
     * render()_(osxphotos.PhotoTemplate     * rmdir()_(osxphotos.FileUtilNoOp
       method)                                 class_method)
                                             * run_commands()_
                                               (osxphotos.ExifTool_method)
 
 ***** S *****
-    * score_(osxphotos.PhotoInfo            * sidecar_(osxphotos.ExportOptions
-      property)                               attribute)
-    * ScoreInfo_(class_in_osxphotos)        * sidecar_drop_ext_
-    * screenshot_(osxphotos.PhotoInfo         (osxphotos.ExportOptions
-      property)                               attribute)
-          o (osxphotos.QueryOptions         * slow_mo_(osxphotos.PhotoInfo
-            attribute)                        property)
-    * search_info_(osxphotos.PhotoInfo            o (osxphotos.QueryOptions
+    * saved_to_library_                     * sidecar_(osxphotos.ExportOptions
+      (osxphotos.PhotoInfo_property)          attribute)
+          o (osxphotos.QueryOptions         * sidecar_drop_ext_
+            attribute)                        (osxphotos.ExportOptions
+    * score_(osxphotos.PhotoInfo              attribute)
+      property)                             * slow_mo_(osxphotos.PhotoInfo
+    * ScoreInfo_(class_in_osxphotos)          property)
+    * screenshot_(osxphotos.PhotoInfo             o (osxphotos.QueryOptions
       property)                                     attribute)
-    * search_info_normalized_               * sort_order_(osxphotos.AlbumInfo
+          o (osxphotos.QueryOptions         * sort_order_(osxphotos.AlbumInfo
+            attribute)                        property)
+    * search_info_(osxphotos.PhotoInfo            o (osxphotos.PersonInfo
+      property)                                     property)
+    * search_info_normalized_               * source_(osxphotos.SearchInfo
       (osxphotos.PhotoInfo_property)          property)
-    * SearchInfo_(class_in_osxphotos)             o (osxphotos.PersonInfo
-    * season_(osxphotos.SearchInfo                  property)
-      property)                             * source_(osxphotos.SearchInfo
-    * selected_(osxphotos.QueryOptions        property)
-      attribute)                            * start_date_(osxphotos.MomentInfo
-    * selfie_(osxphotos.PhotoInfo             property)
+    * SearchInfo_(class_in_osxphotos)       * start_date_(osxphotos.MomentInfo
+    * season_(osxphotos.SearchInfo            property)
       property)                             * state_(osxphotos.SearchInfo
+    * selected_(osxphotos.QueryOptions        property)
+      attribute)                            * state_abbreviation_
+    * selfie_(osxphotos.PhotoInfo             (osxphotos.SearchInfo_property)
+      property)                             * streets_(osxphotos.SearchInfo
           o (osxphotos.QueryOptions           property)
-            attribute)                      * state_abbreviation_
-    * set_config()_(osxphotos.ExportDB        (osxphotos.SearchInfo_property)
-      method)                               * streets_(osxphotos.SearchInfo
+            attribute)                      * strip_(osxphotos.ExportOptions
+    * set_config()_(osxphotos.ExportDB        attribute)
+      method)                               * subfolders_(osxphotos.FolderInfo
     * set_debug()_(in_module_osxphotos)       property)
-    * set_export_results()_                 * strip_(osxphotos.ExportOptions
-      (osxphotos.ExportDB_method)             attribute)
-    * set_photoinfo_for_uuid()_             * subfolders_(osxphotos.FolderInfo
+    * set_export_results()_                 * subtitle_(osxphotos.MomentInfo
       (osxphotos.ExportDB_method)             property)
-    * setvalue()_(osxphotos.ExifTool        * subtitle_(osxphotos.MomentInfo
-      method)                                 property)
-    * shared_(osxphotos.PhotoInfo           * SUBTOPIC
-      property)                                   o osxphotos-help_command_line
-          o (osxphotos.QueryOptions                 option
+    * set_photoinfo_for_uuid()_             * SUBTOPIC
+      (osxphotos.ExportDB_method)                 o osxphotos-help_command_line
+    * setvalue()_(osxphotos.ExifTool                option
+      method)                               * syndicated_(osxphotos.PhotoInfo
+    * shared_(osxphotos.PhotoInfo             property)
+      property)                                   o (osxphotos.QueryOptions
+          o (osxphotos.QueryOptions                 attribute)
             attribute)
 
 ***** T *****
     * tables()_(osxphotos.PhotoInfo
       method)
     * text_found_(osxphotos.SearchInfo
       property)
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.2 documentation</title>
+        <title>osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -513,21 +513,23 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.person_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.person_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.persons"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.persons</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.place"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.place</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.portrait"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.portrait</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.project_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.project_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.raw_original"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.raw_original</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.render_template"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.render_template()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.saved_to_library"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.saved_to_library</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.score"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.score</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.screenshot"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.screenshot</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.search_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.search_info_normalized"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info_normalized</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.selfie"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.selfie</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.shared"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.slow_mo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.slow_mo</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.syndicated"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.syndicated</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.tables"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tables()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.time_lapse"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.time_lapse</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.title"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.title</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.tzoffset"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tzoffset</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti_edited"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_edited</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti_original"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_original</span></code></a></li>
@@ -673,14 +675,18 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.slow_mo"><code class="docutils literal notranslate"><span class="pre">QueryOptions.slow_mo</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.time_lapse"><code class="docutils literal notranslate"><span class="pre">QueryOptions.time_lapse</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.title"><code class="docutils literal notranslate"><span class="pre">QueryOptions.title</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.to_date"><code class="docutils literal notranslate"><span class="pre">QueryOptions.to_date</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.uti"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uti</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.uuid"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uuid</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.year"><code class="docutils literal notranslate"><span class="pre">QueryOptions.year</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.syndicated</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.not_syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_syndicated</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.saved_to_library</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.not_saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_saved_to_library</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ScoreInfo"><code class="docutils literal notranslate"><span class="pre">ScoreInfo</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ScoreInfo.asdict"><code class="docutils literal notranslate"><span class="pre">ScoreInfo.asdict()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.SearchInfo"><code class="docutils literal notranslate"><span class="pre">SearchInfo</span></code></a><ul>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -317,21 +317,23 @@
                 # PhotoInfo.person_info
                 # PhotoInfo.persons
                 # PhotoInfo.place
                 # PhotoInfo.portrait
                 # PhotoInfo.project_info
                 # PhotoInfo.raw_original
                 # PhotoInfo.render_template()
+                # PhotoInfo.saved_to_library
                 # PhotoInfo.score
                 # PhotoInfo.screenshot
                 # PhotoInfo.search_info
                 # PhotoInfo.search_info_normalized
                 # PhotoInfo.selfie
                 # PhotoInfo.shared
                 # PhotoInfo.slow_mo
+                # PhotoInfo.syndicated
                 # PhotoInfo.tables()
                 # PhotoInfo.time_lapse
                 # PhotoInfo.title
                 # PhotoInfo.tzoffset
                 # PhotoInfo.uti
                 # PhotoInfo.uti_edited
                 # PhotoInfo.uti_original
@@ -469,14 +471,18 @@
                 # QueryOptions.slow_mo
                 # QueryOptions.time_lapse
                 # QueryOptions.title
                 # QueryOptions.to_date
                 # QueryOptions.uti
                 # QueryOptions.uuid
                 # QueryOptions.year
+                # QueryOptions.syndicated
+                # QueryOptions.not_syndicated
+                # QueryOptions.saved_to_library
+                # QueryOptions.not_saved_to_library
           o ScoreInfo
                 # ScoreInfo.asdict()
           o SearchInfo
                 # SearchInfo.activities
                 # SearchInfo.all
                 # SearchInfo.asdict()
                 # SearchInfo.bodies_of_water
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -212,21 +212,23 @@
 osxphotos.PhotoInfo.person_info py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.persons py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.place py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.portrait py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.project_info py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.raw_original py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.render_template py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.saved_to_library py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.score py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.screenshot py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.search_info py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.search_info_normalized py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.selfie py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.shared py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.slow_mo py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.syndicated py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.tables py:method 1 reference.html#$ -
 osxphotos.PhotoInfo.time_lapse py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.title py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.tzoffset py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti_edited py:property 1 reference.html#$ -
 osxphotos.PhotoInfo.uti_original py:property 1 reference.html#$ -
@@ -341,31 +343,35 @@
 osxphotos.QueryOptions.not_in_album py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_incloud py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_live py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_missing py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_panorama py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_portrait py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_reference py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_saved_to_library py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_screenshot py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_selfie py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_shared py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_slow_mo py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_syndicated py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.not_time_lapse py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.panorama py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.person py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.photos py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.place py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.portrait py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.query_eval py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.regex py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.saved_to_library py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.screenshot py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.selected py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.selfie py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.shared py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.slow_mo py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.syndicated py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.time_lapse py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.title py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.to_date py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.uti py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.uuid py:attribute 1 reference.html#$ -
 osxphotos.QueryOptions.year py:attribute 1 reference.html#$ -
 osxphotos.ScoreInfo py:class 1 reference.html#$ -
@@ -477,33 +483,37 @@
 osxphotos-add-locations.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-in-album -
 osxphotos-add-locations.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-incloud -
 osxphotos-add-locations.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-live -
 osxphotos-add-locations.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-missing -
 osxphotos-add-locations.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-panorama -
 osxphotos-add-locations.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-portrait -
 osxphotos-add-locations.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-reference -
+osxphotos-add-locations.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-saved-to-library -
 osxphotos-add-locations.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-screenshot -
 osxphotos-add-locations.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-selfie -
 osxphotos-add-locations.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-shared -
 osxphotos-add-locations.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-slow-mo -
+osxphotos-add-locations.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-syndicated -
 osxphotos-add-locations.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-time-lapse -
 osxphotos-add-locations.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-only-movies -
 osxphotos-add-locations.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-only-photos -
 osxphotos-add-locations.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-panorama -
 osxphotos-add-locations.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-person -
 osxphotos-add-locations.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-place -
 osxphotos-add-locations.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-portrait -
 osxphotos-add-locations.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-query-eval -
 osxphotos-add-locations.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-query-function -
 osxphotos-add-locations.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-regex -
+osxphotos-add-locations.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-saved-to-library -
 osxphotos-add-locations.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-screenshot -
 osxphotos-add-locations.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-selected -
 osxphotos-add-locations.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-selfie -
 osxphotos-add-locations.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-shared -
 osxphotos-add-locations.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-slow-mo -
+osxphotos-add-locations.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-syndicated -
 osxphotos-add-locations.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-theme -
 osxphotos-add-locations.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-time-lapse -
 osxphotos-add-locations.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-timestamp -
 osxphotos-add-locations.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-title -
 osxphotos-add-locations.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-to-date -
 osxphotos-add-locations.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-to-time -
 osxphotos-add-locations.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uti -
@@ -664,18 +674,20 @@
 osxphotos-export.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-in-album -
 osxphotos-export.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-incloud -
 osxphotos-export.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-live -
 osxphotos-export.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-missing -
 osxphotos-export.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-panorama -
 osxphotos-export.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-portrait -
 osxphotos-export.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-reference -
+osxphotos-export.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-saved-to-library -
 osxphotos-export.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-screenshot -
 osxphotos-export.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-selfie -
 osxphotos-export.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-shared -
 osxphotos-export.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-slow-mo -
+osxphotos-export.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-syndicated -
 osxphotos-export.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-time-lapse -
 osxphotos-export.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-movies -
 osxphotos-export.--only-new std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-new -
 osxphotos-export.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-photos -
 osxphotos-export.--original-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-original-suffix -
 osxphotos-export.--overwrite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-overwrite -
 osxphotos-export.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-export-panorama -
@@ -693,14 +705,15 @@
 osxphotos-export.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-export-query-function -
 osxphotos-export.--ramdb std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ramdb -
 osxphotos-export.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-export-regex -
 osxphotos-export.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-replace-keywords -
 osxphotos-export.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-export-report -
 osxphotos-export.--retry std:cmdoption 1 cli.html#cmdoption-osxphotos-export-retry -
 osxphotos-export.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-export-save-config -
+osxphotos-export.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-saved-to-library -
 osxphotos-export.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-screenshot -
 osxphotos-export.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selected -
 osxphotos-export.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selfie -
 osxphotos-export.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-shared -
 osxphotos-export.--sidecar std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar -
 osxphotos-export.--sidecar-drop-ext std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar-drop-ext -
 osxphotos-export.--skip-bursts std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-bursts -
@@ -708,14 +721,15 @@
 osxphotos-export.--skip-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-live -
 osxphotos-export.--skip-original-if-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-original-if-edited -
 osxphotos-export.--skip-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-raw -
 osxphotos-export.--skip-uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid -
 osxphotos-export.--skip-uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid-from-file -
 osxphotos-export.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-export-slow-mo -
 osxphotos-export.--strip std:cmdoption 1 cli.html#cmdoption-osxphotos-export-strip -
+osxphotos-export.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-export-syndicated -
 osxphotos-export.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-export-theme -
 osxphotos-export.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-export-time-lapse -
 osxphotos-export.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-export-timestamp -
 osxphotos-export.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-export-title -
 osxphotos-export.--tmpdir std:cmdoption 1 cli.html#cmdoption-osxphotos-export-tmpdir -
 osxphotos-export.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-to-date -
 osxphotos-export.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-export-to-time -
@@ -899,35 +913,39 @@
 osxphotos-query.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-in-album -
 osxphotos-query.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-incloud -
 osxphotos-query.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-live -
 osxphotos-query.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-missing -
 osxphotos-query.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-panorama -
 osxphotos-query.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-portrait -
 osxphotos-query.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-reference -
+osxphotos-query.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-saved-to-library -
 osxphotos-query.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-screenshot -
 osxphotos-query.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-selfie -
 osxphotos-query.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-shared -
 osxphotos-query.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-slow-mo -
+osxphotos-query.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-syndicated -
 osxphotos-query.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-time-lapse -
 osxphotos-query.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-query-only-movies -
 osxphotos-query.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-query-only-photos -
 osxphotos-query.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-query-panorama -
 osxphotos-query.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-query-person -
 osxphotos-query.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-query-place -
 osxphotos-query.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-query-portrait -
 osxphotos-query.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-query-print -
 osxphotos-query.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-query-query-eval -
 osxphotos-query.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-query-query-function -
 osxphotos-query.--quiet std:cmdoption 1 cli.html#cmdoption-osxphotos-query-quiet -
 osxphotos-query.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-query-regex -
+osxphotos-query.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-saved-to-library -
 osxphotos-query.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-query-screenshot -
 osxphotos-query.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-query-selected -
 osxphotos-query.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-query-selfie -
 osxphotos-query.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-query-shared -
 osxphotos-query.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-query-slow-mo -
+osxphotos-query.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-query-syndicated -
 osxphotos-query.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-query-time-lapse -
 osxphotos-query.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-query-title -
 osxphotos-query.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-query-to-date -
 osxphotos-query.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-query-to-time -
 osxphotos-query.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uti -
 osxphotos-query.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uuid -
 osxphotos-query.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uuid-from-file -
@@ -988,33 +1006,37 @@
 osxphotos-repl.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-in-album -
 osxphotos-repl.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-incloud -
 osxphotos-repl.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-live -
 osxphotos-repl.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-missing -
 osxphotos-repl.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-panorama -
 osxphotos-repl.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-portrait -
 osxphotos-repl.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-reference -
+osxphotos-repl.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-saved-to-library -
 osxphotos-repl.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-screenshot -
 osxphotos-repl.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-selfie -
 osxphotos-repl.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-shared -
 osxphotos-repl.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-slow-mo -
+osxphotos-repl.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-syndicated -
 osxphotos-repl.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-time-lapse -
 osxphotos-repl.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-only-movies -
 osxphotos-repl.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-only-photos -
 osxphotos-repl.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-panorama -
 osxphotos-repl.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-person -
 osxphotos-repl.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-place -
 osxphotos-repl.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-portrait -
 osxphotos-repl.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-query-eval -
 osxphotos-repl.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-query-function -
 osxphotos-repl.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-regex -
+osxphotos-repl.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-saved-to-library -
 osxphotos-repl.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-screenshot -
 osxphotos-repl.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-selected -
 osxphotos-repl.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-selfie -
 osxphotos-repl.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-shared -
 osxphotos-repl.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-slow-mo -
+osxphotos-repl.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-syndicated -
 osxphotos-repl.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-time-lapse -
 osxphotos-repl.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-title -
 osxphotos-repl.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-to-date -
 osxphotos-repl.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-to-time -
 osxphotos-repl.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uti -
 osxphotos-repl.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uuid -
 osxphotos-repl.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uuid-from-file -
@@ -1084,33 +1106,37 @@
 osxphotos-sync.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-in-album -
 osxphotos-sync.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-incloud -
 osxphotos-sync.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-live -
 osxphotos-sync.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-missing -
 osxphotos-sync.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-panorama -
 osxphotos-sync.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-portrait -
 osxphotos-sync.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-reference -
+osxphotos-sync.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-saved-to-library -
 osxphotos-sync.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-screenshot -
 osxphotos-sync.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-selfie -
 osxphotos-sync.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-slow-mo -
+osxphotos-sync.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-syndicated -
 osxphotos-sync.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-time-lapse -
 osxphotos-sync.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-only-movies -
 osxphotos-sync.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-only-photos -
 osxphotos-sync.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-panorama -
 osxphotos-sync.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-person -
 osxphotos-sync.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-place -
 osxphotos-sync.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-portrait -
 osxphotos-sync.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-query-eval -
 osxphotos-sync.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-query-function -
 osxphotos-sync.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-regex -
 osxphotos-sync.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-R -
+osxphotos-sync.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-saved-to-library -
 osxphotos-sync.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-screenshot -
 osxphotos-sync.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-selected -
 osxphotos-sync.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-selfie -
 osxphotos-sync.--set std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-s -
 osxphotos-sync.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-slow-mo -
+osxphotos-sync.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-syndicated -
 osxphotos-sync.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-theme -
 osxphotos-sync.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-time-lapse -
 osxphotos-sync.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-timestamp -
 osxphotos-sync.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-title -
 osxphotos-sync.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-to-date -
 osxphotos-sync.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-to-time -
 osxphotos-sync.--unmatched std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-U -
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.2 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.2 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.2 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.3 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.2 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1942,15 +1942,15 @@
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.path">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">path</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.path" title="Permalink to this definition">#</a></dt>
 <dd><p>absolute path on disk of the original picture</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.path_derivatives">
-<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">path_derivatives</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.path_derivatives" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">path_derivatives</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">list</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#osxphotos.PhotoInfo.path_derivatives" title="Permalink to this definition">#</a></dt>
 <dd><p>Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.path_edited">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">path_edited</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.path_edited" title="Permalink to this definition">#</a></dt>
 <dd><p>absolute path on disk of the edited picture</p>
@@ -2031,14 +2031,23 @@
 <dt class="field-odd">Return type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>([rendered_strings], [unmatched])</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PhotoInfo.saved_to_library">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">saved_to_library</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PhotoInfo.saved_to_library" title="Permalink to this definition">#</a></dt>
+<dd><p>Return True if syndicated photo has been saved to library;
+returns False if photo is not syndicated or has not been saved to the library.
+Returns None if not Photos 8+.
+Syndicated photos are photos that appear in “Shared with you” album; Photos 8+ only.</p>
+</dd></dl>
+
+<dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.score">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">score</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.score" title="Permalink to this definition">#</a></dt>
 <dd><p>Computed score information for a photo</p>
 <dl class="field-list simple">
 <dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>ScoreInfo instance</p>
 </dd>
@@ -2080,14 +2089,22 @@
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.slow_mo">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">slow_mo</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.slow_mo" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a slow motion video, otherwise False</p>
 </dd></dl>
 
+<dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PhotoInfo.syndicated">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">syndicated</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#osxphotos.PhotoInfo.syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>Return true if photo was shared via syndication (e.g. via Messages, etc.);
+these are photos that appear in “Shared with you” album.
+Photos 8+ only; returns None if not Photos 8+.</p>
+</dd></dl>
+
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.tables">
 <span class="sig-name descname"><span class="pre">tables</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">PhotoTables</span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.tables"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.tables" title="Permalink to this definition">#</a></dt>
 <dd><p>Return PhotoTables object to provide access database tables associated with this photo (Photos 5+)</p>
 </dd></dl>
 
 <dl class="py property">
@@ -2625,15 +2642,15 @@
 or empty list if album is not in any folders</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.QueryOptions">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">QueryOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">added_after</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_before</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_in_last</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst_photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">duplicate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">external_edit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">function</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">callable</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_case</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">max_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">min_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_bursts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">movies</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">person</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">query_eval</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">regex</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selected</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uti</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/queryoptions.html#QueryOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.QueryOptions" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">QueryOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">added_after</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_before</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_in_last</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst_photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">duplicate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">external_edit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">function</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">callable</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_case</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">max_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">min_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_bursts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">movies</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">person</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">query_eval</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">regex</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selected</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uti</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">syndicated</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_syndicated</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">saved_to_library</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_saved_to_library</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/queryoptions.html#QueryOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.QueryOptions" title="Permalink to this definition">#</a></dt>
 <dd><p>QueryOptions class for PhotosDB.query</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="osxphotos.QueryOptions.added_after">
 <span class="sig-name descname"><span class="pre">added_after</span></span><a class="headerlink" href="#osxphotos.QueryOptions.added_after" title="Permalink to this definition">#</a></dt>
 <dd><p>search for photos added after a given date</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type<span class="colon">:</span></dt>
@@ -3507,14 +3524,58 @@
 <dl class="field-list simple">
 <dt class="field-odd">Type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Optional[Iterable[int]]</p>
 </dd>
 </dl>
 </dd></dl>
 
+<dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.QueryOptions.syndicated">
+<span class="sig-name descname"><span class="pre">syndicated</span></span><a class="headerlink" href="#osxphotos.QueryOptions.syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>search for photos that have been shared via syndication (“Shared with You” album via Messages, etc.)</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Optional[bool]</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.QueryOptions.not_syndicated">
+<span class="sig-name descname"><span class="pre">not_syndicated</span></span><a class="headerlink" href="#osxphotos.QueryOptions.not_syndicated" title="Permalink to this definition">#</a></dt>
+<dd><p>search for photos that have not been shared via syndication (“Shared with You” album via Messages, etc.)</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Optional[bool]</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.QueryOptions.saved_to_library">
+<span class="sig-name descname"><span class="pre">saved_to_library</span></span><a class="headerlink" href="#osxphotos.QueryOptions.saved_to_library" title="Permalink to this definition">#</a></dt>
+<dd><p>search for syndicated photos that have been saved to the Photos library</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Optional[bool]</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.QueryOptions.not_saved_to_library">
+<span class="sig-name descname"><span class="pre">not_saved_to_library</span></span><a class="headerlink" href="#osxphotos.QueryOptions.not_saved_to_library" title="Permalink to this definition">#</a></dt>
+<dd><p>search for syndicated photos that have not been saved to the Photos library</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Optional[bool]</p>
+</dd>
+</dl>
+</dd></dl>
+
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ScoreInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ScoreInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">overall</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">curation</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">promotion</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">highlight_visibility</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">behavioral</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">failure</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">harmonious_color</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">immersiveness</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">interaction</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">interesting_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">intrusive_object_presence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">lively_color</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">low_light</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">noise</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_camera_tilt</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_composition</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_lighting</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_pattern</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_perspective</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_post_processing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_reflection</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_symmetry</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sharply_focused_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tastefully_blurred</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">well_chosen_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">well_framed_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">well_timed_shot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/scoreinfo.html#ScoreInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ScoreInfo" title="Permalink to this definition">#</a></dt>
 <dd><p>Computed photo score info associated with a photo from the Photos library</p>
 <dl class="py method">
@@ -3969,21 +4030,23 @@
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.person_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.person_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.persons"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.persons</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.place"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.place</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.portrait"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.portrait</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.project_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.project_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.raw_original"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.raw_original</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.render_template"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.render_template()</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PhotoInfo.saved_to_library"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.saved_to_library</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.score"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.score</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.screenshot"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.screenshot</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.search_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.search_info_normalized"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info_normalized</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.selfie"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.selfie</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.shared"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.slow_mo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.slow_mo</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PhotoInfo.syndicated"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.syndicated</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.tables"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tables()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.time_lapse"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.time_lapse</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.title"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.title</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.tzoffset"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tzoffset</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti_edited"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_edited</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti_original"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti_original</span></code></a></li>
@@ -4129,14 +4192,18 @@
 <li><a class="reference internal" href="#osxphotos.QueryOptions.slow_mo"><code class="docutils literal notranslate"><span class="pre">QueryOptions.slow_mo</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.time_lapse"><code class="docutils literal notranslate"><span class="pre">QueryOptions.time_lapse</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.title"><code class="docutils literal notranslate"><span class="pre">QueryOptions.title</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.to_date"><code class="docutils literal notranslate"><span class="pre">QueryOptions.to_date</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.uti"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uti</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.uuid"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uuid</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.year"><code class="docutils literal notranslate"><span class="pre">QueryOptions.year</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.QueryOptions.syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.syndicated</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.QueryOptions.not_syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_syndicated</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.QueryOptions.saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.saved_to_library</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.QueryOptions.not_saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_saved_to_library</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.ScoreInfo"><code class="docutils literal notranslate"><span class="pre">ScoreInfo</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.ScoreInfo.asdict"><code class="docutils literal notranslate"><span class="pre">ScoreInfo.asdict()</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.SearchInfo"><code class="docutils literal notranslate"><span class="pre">SearchInfo</span></code></a><ul>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -928,15 +928,15 @@
         propertyowner#
             Return name of photo owner for shared photos (Photos 5+ only), or
             None if not shared
         propertypanorama#
             Returns True if photo is a panorama, otherwise False
         propertypath#
             absolute path on disk of the original picture
-        propertypath_derivatives#
+        propertypath_derivatives: list[str]#
             Return any derivative (preview) images associated with the photo as
             a list of paths, sorted by file size (largest first)
         propertypath_edited#
             absolute path on disk of the edited picture
         propertypath_edited_live_photo#
             return path to edited version of live photo movie
         propertypath_live_photo#
@@ -967,14 +967,19 @@
                         render
                       * options â a RenderOptions instance
               Returns:
                   tuple of list of rendered strings and list of unmatched
                   template values
               Return type:
                   ([rendered_strings], [unmatched])
+        propertysaved_to_library: bool | None#
+            Return True if syndicated photo has been saved to library; returns
+            False if photo is not syndicated or has not been saved to the
+            library. Returns None if not Photos 8+. Syndicated photos are
+            photos that appear in âShared with youâ album; Photos 8+ only.
         propertyscore#
             Computed score information for a photo
               Returns:
                   ScoreInfo instance
         propertyscreenshot#
             Returns True if photo is an HDR photo, otherwise False
         propertysearch_info#
@@ -987,14 +992,18 @@
             Returns True if photo is a selfie (front facing camera), otherwise
             False
         propertyshared#
             returns True if photos is in a shared iCloud album otherwise false
             Only valid on Photos 5; returns None on older versions
         propertyslow_mo#
             Returns True if photo is a slow motion video, otherwise False
+        propertysyndicated: bool | None#
+            Return true if photo was shared via syndication (e.g. via Messages,
+            etc.); these are photos that appear in âShared with youâ album.
+            Photos 8+ only; returns None if not Photos 8+.
         tables() &#x2192; PhotoTables[source]#
             Return PhotoTables object to provide access database tables
             associated with this photo (Photos 5+)
         propertytime_lapse#
             Returns True if photo is a time lapse video, otherwise False
         propertytitle#
             name / title of picture
@@ -1293,15 +1302,17 @@
   portrait: Optional[bool] = None, query_eval: Optional[Iterable[str]] = None,
   regex: Optional[Iterable[Tuple[str, str]]] = None, screenshot: Optional[bool]
   = None, selected: Optional[bool] = None, selfie: Optional[bool] = None,
   shared: Optional[bool] = None, slow_mo: Optional[bool] = None, time_lapse:
   Optional[bool] = None, title: Optional[Iterable[str]] = None, to_date:
   Optional[datetime] = None, to_time: Optional[time] = None, uti: Optional
   [Iterable[str]] = None, uuid: Optional[Iterable[str]] = None, year: Optional
-  [Iterable[int]] = None)[source]#
+  [Iterable[int]] = None, syndicated: Optional[bool] = None, not_syndicated:
+  Optional[bool] = None, saved_to_library: Optional[bool] = None,
+  not_saved_to_library: Optional[bool] = None)[source]#
       QueryOptions class for PhotosDB.query
         added_after#
             search for photos added after a given date
               Type:
                   Optional[datetime.datetime]
         added_before#
             search for photos added before a given date
@@ -1617,14 +1628,34 @@
             list of uuids to search for
               Type:
                   Optional[Iterable[str]]
         year#
             search for photos taken in a given year
               Type:
                   Optional[Iterable[int]]
+        syndicated#
+            search for photos that have been shared via syndication (âShared
+            with Youâ album via Messages, etc.)
+              Type:
+                  Optional[bool]
+        not_syndicated#
+            search for photos that have not been shared via syndication
+            (âShared with Youâ album via Messages, etc.)
+              Type:
+                  Optional[bool]
+        saved_to_library#
+            search for syndicated photos that have been saved to the Photos
+            library
+              Type:
+                  Optional[bool]
+        not_saved_to_library#
+            search for syndicated photos that have not been saved to the Photos
+            library
+              Type:
+                  Optional[bool]
   classosxphotos.ScoreInfo(overall: float, curation: float, promotion: float,
   highlight_visibility: float, behavioral: float, failure: float,
   harmonious_color: float, immersiveness: float, interaction: float,
   interesting_subject: float, intrusive_object_presence: float, lively_color:
   float, low_light: float, noise: float, pleasant_camera_tilt: float,
   pleasant_composition: float, pleasant_lighting: float, pleasant_pattern:
   float, pleasant_perspective: float, pleasant_post_processing: float,
@@ -1907,21 +1938,23 @@
                 # PhotoInfo.person_info
                 # PhotoInfo.persons
                 # PhotoInfo.place
                 # PhotoInfo.portrait
                 # PhotoInfo.project_info
                 # PhotoInfo.raw_original
                 # PhotoInfo.render_template()
+                # PhotoInfo.saved_to_library
                 # PhotoInfo.score
                 # PhotoInfo.screenshot
                 # PhotoInfo.search_info
                 # PhotoInfo.search_info_normalized
                 # PhotoInfo.selfie
                 # PhotoInfo.shared
                 # PhotoInfo.slow_mo
+                # PhotoInfo.syndicated
                 # PhotoInfo.tables()
                 # PhotoInfo.time_lapse
                 # PhotoInfo.title
                 # PhotoInfo.tzoffset
                 # PhotoInfo.uti
                 # PhotoInfo.uti_edited
                 # PhotoInfo.uti_original
@@ -2059,14 +2092,18 @@
                 # QueryOptions.slow_mo
                 # QueryOptions.time_lapse
                 # QueryOptions.title
                 # QueryOptions.to_date
                 # QueryOptions.uti
                 # QueryOptions.uuid
                 # QueryOptions.year
+                # QueryOptions.syndicated
+                # QueryOptions.not_syndicated
+                # QueryOptions.saved_to_library
+                # QueryOptions.not_saved_to_library
           o ScoreInfo
                 # ScoreInfo.asdict()
           o SearchInfo
                 # SearchInfo.activities
                 # SearchInfo.all
                 # SearchInfo.asdict()
                 # SearchInfo.bodies_of_water
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.2 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.3 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -158,15 +158,15 @@
         "other": [0, 4, 5, 6],
         "conjunct": [0, 6],
         "thei": [0, 4, 6],
         "overrid": [0, 5],
         "correspond": 0,
         "config_fil": 0,
         "written": [0, 4, 5, 6],
-        "save": [0, 1],
+        "save": [0, 1, 4],
         "toml": [0, 6],
         "exiftool_path": [0, 4],
         "look": [0, 2, 4, 6],
         "flag": [0, 4],
         "pass": [0, 3, 4, 5, 6],
         "m": [0, 4, 5],
         "ignor": [0, 4, 6],
@@ -2248,15 +2248,19 @@
         "cd": 5,
         "da": 5,
         "59": [],
         "indent": 4,
         "shallow": 4,
         "shutil": 4,
         "photot": 4,
-        "60": 5
+        "60": 5,
+        "syndic": [0, 1, 4],
+        "saved_to_librari": [1, 4],
+        "not_synd": [1, 4],
+        "not_saved_to_librari": [1, 4]
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -2507,21 +2511,23 @@
             [4, 3, 1, "", "person_info"],
             [4, 3, 1, "", "persons"],
             [4, 3, 1, "", "place"],
             [4, 3, 1, "", "portrait"],
             [4, 3, 1, "", "project_info"],
             [4, 3, 1, "", "raw_original"],
             [4, 2, 1, "", "render_template"],
+            [4, 3, 1, "", "saved_to_library"],
             [4, 3, 1, "", "score"],
             [4, 3, 1, "", "screenshot"],
             [4, 3, 1, "", "search_info"],
             [4, 3, 1, "", "search_info_normalized"],
             [4, 3, 1, "", "selfie"],
             [4, 3, 1, "", "shared"],
             [4, 3, 1, "", "slow_mo"],
+            [4, 3, 1, "", "syndicated"],
             [4, 2, 1, "", "tables"],
             [4, 3, 1, "", "time_lapse"],
             [4, 3, 1, "", "title"],
             [4, 3, 1, "", "tzoffset"],
             [4, 3, 1, "", "uti"],
             [4, 3, 1, "", "uti_edited"],
             [4, 3, 1, "", "uti_original"],
@@ -2637,31 +2643,35 @@
             [4, 4, 1, "", "not_in_album"],
             [4, 4, 1, "", "not_incloud"],
             [4, 4, 1, "", "not_live"],
             [4, 4, 1, "", "not_missing"],
             [4, 4, 1, "", "not_panorama"],
             [4, 4, 1, "", "not_portrait"],
             [4, 4, 1, "", "not_reference"],
+            [4, 4, 1, "", "not_saved_to_library"],
             [4, 4, 1, "", "not_screenshot"],
             [4, 4, 1, "", "not_selfie"],
             [4, 4, 1, "", "not_shared"],
             [4, 4, 1, "", "not_slow_mo"],
+            [4, 4, 1, "", "not_syndicated"],
             [4, 4, 1, "", "not_time_lapse"],
             [4, 4, 1, "", "panorama"],
             [4, 4, 1, "", "person"],
             [4, 4, 1, "", "photos"],
             [4, 4, 1, "", "place"],
             [4, 4, 1, "", "portrait"],
             [4, 4, 1, "", "query_eval"],
             [4, 4, 1, "", "regex"],
+            [4, 4, 1, "", "saved_to_library"],
             [4, 4, 1, "", "screenshot"],
             [4, 4, 1, "", "selected"],
             [4, 4, 1, "", "selfie"],
             [4, 4, 1, "", "shared"],
             [4, 4, 1, "", "slow_mo"],
+            [4, 4, 1, "", "syndicated"],
             [4, 4, 1, "", "time_lapse"],
             [4, 4, 1, "", "title"],
             [4, 4, 1, "", "to_date"],
             [4, 4, 1, "", "uti"],
             [4, 4, 1, "", "uuid"],
             [4, 4, 1, "", "year"]
         ],
@@ -2744,33 +2754,37 @@
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-in-album", "--not-in-album"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-incloud", "--not-incloud"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-live", "--not-live"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-missing", "--not-missing"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-reference", "--not-reference"],
+            [0, 6, 1, "cmdoption-osxphotos-add-locations-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-shared", "--not-shared"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-slow-mo", "--not-slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-add-locations-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-person", "--person"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-place", "--place"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-portrait", "--portrait"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-query-eval", "--query-eval"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-regex", "--regex"],
+            [0, 6, 1, "cmdoption-osxphotos-add-locations-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-shared", "--shared"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-slow-mo", "--slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-add-locations-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-theme", "--theme"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-timestamp", "--timestamp"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-to-time", "--to-time"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-uti", "--uti"],
@@ -2943,18 +2957,20 @@
             [0, 6, 1, "cmdoption-osxphotos-export-not-in-album", "--not-in-album"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-incloud", "--not-incloud"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-live", "--not-live"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-missing", "--not-missing"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-reference", "--not-reference"],
+            [0, 6, 1, "cmdoption-osxphotos-export-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-shared", "--not-shared"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-slow-mo", "--not-slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-export-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-export-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-export-only-new", "--only-new"],
             [0, 6, 1, "cmdoption-osxphotos-export-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-export-original-suffix", "--original-suffix"],
             [0, 6, 1, "cmdoption-osxphotos-export-overwrite", "--overwrite"],
             [0, 6, 1, "cmdoption-osxphotos-export-panorama", "--panorama"],
@@ -2972,14 +2988,15 @@
             [0, 6, 1, "cmdoption-osxphotos-export-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-export-ramdb", "--ramdb"],
             [0, 6, 1, "cmdoption-osxphotos-export-regex", "--regex"],
             [0, 6, 1, "cmdoption-osxphotos-export-replace-keywords", "--replace-keywords"],
             [0, 6, 1, "cmdoption-osxphotos-export-report", "--report"],
             [0, 6, 1, "cmdoption-osxphotos-export-retry", "--retry"],
             [0, 6, 1, "cmdoption-osxphotos-export-save-config", "--save-config"],
+            [0, 6, 1, "cmdoption-osxphotos-export-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-export-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-export-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-export-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-export-shared", "--shared"],
             [0, 6, 1, "cmdoption-osxphotos-export-sidecar", "--sidecar"],
             [0, 6, 1, "cmdoption-osxphotos-export-sidecar-drop-ext", "--sidecar-drop-ext"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-bursts", "--skip-bursts"],
@@ -2987,14 +3004,15 @@
             [0, 6, 1, "cmdoption-osxphotos-export-skip-live", "--skip-live"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-original-if-edited", "--skip-original-if-edited"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-raw", "--skip-raw"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-uuid", "--skip-uuid"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-uuid-from-file", "--skip-uuid-from-file"],
             [0, 6, 1, "cmdoption-osxphotos-export-slow-mo", "--slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-export-strip", "--strip"],
+            [0, 6, 1, "cmdoption-osxphotos-export-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-export-theme", "--theme"],
             [0, 6, 1, "cmdoption-osxphotos-export-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-export-timestamp", "--timestamp"],
             [0, 6, 1, "cmdoption-osxphotos-export-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-export-tmpdir", "--tmpdir"],
             [0, 6, 1, "cmdoption-osxphotos-export-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-export-to-time", "--to-time"],
@@ -3204,35 +3222,39 @@
             [0, 6, 1, "cmdoption-osxphotos-query-not-in-album", "--not-in-album"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-incloud", "--not-incloud"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-live", "--not-live"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-missing", "--not-missing"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-reference", "--not-reference"],
+            [0, 6, 1, "cmdoption-osxphotos-query-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-shared", "--not-shared"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-slow-mo", "--not-slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-query-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-query-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-query-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-query-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-query-person", "--person"],
             [0, 6, 1, "cmdoption-osxphotos-query-place", "--place"],
             [0, 6, 1, "cmdoption-osxphotos-query-portrait", "--portrait"],
             [0, 6, 1, "cmdoption-osxphotos-query-print", "--print"],
             [0, 6, 1, "cmdoption-osxphotos-query-query-eval", "--query-eval"],
             [0, 6, 1, "cmdoption-osxphotos-query-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-query-quiet", "--quiet"],
             [0, 6, 1, "cmdoption-osxphotos-query-regex", "--regex"],
+            [0, 6, 1, "cmdoption-osxphotos-query-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-query-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-query-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-query-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-query-shared", "--shared"],
             [0, 6, 1, "cmdoption-osxphotos-query-slow-mo", "--slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-query-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-query-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-query-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-query-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-query-to-time", "--to-time"],
             [0, 6, 1, "cmdoption-osxphotos-query-uti", "--uti"],
             [0, 6, 1, "cmdoption-osxphotos-query-uuid", "--uuid"],
             [0, 6, 1, "cmdoption-osxphotos-query-uuid-from-file", "--uuid-from-file"],
@@ -3295,33 +3317,37 @@
             [0, 6, 1, "cmdoption-osxphotos-repl-not-in-album", "--not-in-album"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-incloud", "--not-incloud"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-live", "--not-live"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-missing", "--not-missing"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-reference", "--not-reference"],
+            [0, 6, 1, "cmdoption-osxphotos-repl-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-shared", "--not-shared"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-slow-mo", "--not-slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-repl-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-repl-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-repl-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-repl-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-repl-person", "--person"],
             [0, 6, 1, "cmdoption-osxphotos-repl-place", "--place"],
             [0, 6, 1, "cmdoption-osxphotos-repl-portrait", "--portrait"],
             [0, 6, 1, "cmdoption-osxphotos-repl-query-eval", "--query-eval"],
             [0, 6, 1, "cmdoption-osxphotos-repl-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-repl-regex", "--regex"],
+            [0, 6, 1, "cmdoption-osxphotos-repl-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-repl-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-repl-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-repl-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-repl-shared", "--shared"],
             [0, 6, 1, "cmdoption-osxphotos-repl-slow-mo", "--slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-repl-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-repl-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-repl-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-repl-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-repl-to-time", "--to-time"],
             [0, 6, 1, "cmdoption-osxphotos-repl-uti", "--uti"],
             [0, 6, 1, "cmdoption-osxphotos-repl-uuid", "--uuid"],
             [0, 6, 1, "cmdoption-osxphotos-repl-uuid-from-file", "--uuid-from-file"],
@@ -3399,33 +3425,37 @@
             [0, 6, 1, "cmdoption-osxphotos-sync-not-in-album", "--not-in-album"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-incloud", "--not-incloud"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-live", "--not-live"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-missing", "--not-missing"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-reference", "--not-reference"],
+            [0, 6, 1, "cmdoption-osxphotos-sync-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-slow-mo", "--not-slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-sync-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-sync-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-sync-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-sync-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-sync-person", "--person"],
             [0, 6, 1, "cmdoption-osxphotos-sync-place", "--place"],
             [0, 6, 1, "cmdoption-osxphotos-sync-portrait", "--portrait"],
             [0, 6, 1, "cmdoption-osxphotos-sync-query-eval", "--query-eval"],
             [0, 6, 1, "cmdoption-osxphotos-sync-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-sync-regex", "--regex"],
             [0, 6, 1, "cmdoption-osxphotos-sync-R", "--report"],
+            [0, 6, 1, "cmdoption-osxphotos-sync-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-sync-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-sync-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-sync-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-sync-s", "--set"],
             [0, 6, 1, "cmdoption-osxphotos-sync-slow-mo", "--slow-mo"],
+            [0, 6, 1, "cmdoption-osxphotos-sync-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-sync-theme", "--theme"],
             [0, 6, 1, "cmdoption-osxphotos-sync-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-sync-timestamp", "--timestamp"],
             [0, 6, 1, "cmdoption-osxphotos-sync-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-sync-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-sync-to-time", "--to-time"],
             [0, 6, 1, "cmdoption-osxphotos-sync-U", "--unmatched"],
@@ -4778,14 +4808,21 @@
         "--not-reference": [
             [0, "cmdoption-osxphotos-add-locations-not-reference"],
             [0, "cmdoption-osxphotos-export-not-reference"],
             [0, "cmdoption-osxphotos-query-not-reference"],
             [0, "cmdoption-osxphotos-repl-not-reference"],
             [0, "cmdoption-osxphotos-sync-not-reference"]
         ],
+        "--not-saved-to-library": [
+            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-not-saved-to-library"]
+        ],
         "--not-screenshot": [
             [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
             [0, "cmdoption-osxphotos-export-not-screenshot"],
             [0, "cmdoption-osxphotos-query-not-screenshot"],
             [0, "cmdoption-osxphotos-repl-not-screenshot"],
             [0, "cmdoption-osxphotos-sync-not-screenshot"]
         ],
@@ -4805,14 +4842,21 @@
         "--not-slow-mo": [
             [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
             [0, "cmdoption-osxphotos-export-not-slow-mo"],
             [0, "cmdoption-osxphotos-query-not-slow-mo"],
             [0, "cmdoption-osxphotos-repl-not-slow-mo"],
             [0, "cmdoption-osxphotos-sync-not-slow-mo"]
         ],
+        "--not-syndicated": [
+            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
+            [0, "cmdoption-osxphotos-export-not-syndicated"],
+            [0, "cmdoption-osxphotos-query-not-syndicated"],
+            [0, "cmdoption-osxphotos-repl-not-syndicated"],
+            [0, "cmdoption-osxphotos-sync-not-syndicated"]
+        ],
         "--not-time-lapse": [
             [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
             [0, "cmdoption-osxphotos-export-not-time-lapse"],
             [0, "cmdoption-osxphotos-query-not-time-lapse"],
             [0, "cmdoption-osxphotos-repl-not-time-lapse"],
             [0, "cmdoption-osxphotos-sync-not-time-lapse"]
         ],
@@ -4961,14 +5005,21 @@
             [0, "cmdoption-osxphotos-version-run"]
         ],
         "--save-config": [
             [0, "cmdoption-osxphotos-exiftool-save-config"],
             [0, "cmdoption-osxphotos-export-save-config"],
             [0, "cmdoption-osxphotos-exportdb-save-config"]
         ],
+        "--saved-to-library": [
+            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-saved-to-library"]
+        ],
         "--screenshot": [
             [0, "cmdoption-osxphotos-add-locations-screenshot"],
             [0, "cmdoption-osxphotos-export-screenshot"],
             [0, "cmdoption-osxphotos-query-screenshot"],
             [0, "cmdoption-osxphotos-repl-screenshot"],
             [0, "cmdoption-osxphotos-sync-screenshot"]
         ],
@@ -5037,14 +5088,21 @@
         ],
         "--strip": [
             [0, "cmdoption-osxphotos-export-strip"]
         ],
         "--style": [
             [0, "cmdoption-osxphotos-diff-s"]
         ],
+        "--syndicated": [
+            [0, "cmdoption-osxphotos-add-locations-syndicated"],
+            [0, "cmdoption-osxphotos-export-syndicated"],
+            [0, "cmdoption-osxphotos-query-syndicated"],
+            [0, "cmdoption-osxphotos-repl-syndicated"],
+            [0, "cmdoption-osxphotos-sync-syndicated"]
+        ],
         "--template": [
             [0, "cmdoption-osxphotos-inspect-T"]
         ],
         "--theme": [
             [0, "cmdoption-osxphotos-add-locations-theme"],
             [0, "cmdoption-osxphotos-batch-edit-theme"],
             [0, "cmdoption-osxphotos-exiftool-theme"],
@@ -5418,33 +5476,37 @@
             [0, "cmdoption-osxphotos-add-locations-not-in-album"],
             [0, "cmdoption-osxphotos-add-locations-not-incloud"],
             [0, "cmdoption-osxphotos-add-locations-not-live"],
             [0, "cmdoption-osxphotos-add-locations-not-missing"],
             [0, "cmdoption-osxphotos-add-locations-not-panorama"],
             [0, "cmdoption-osxphotos-add-locations-not-portrait"],
             [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
             [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
             [0, "cmdoption-osxphotos-add-locations-not-selfie"],
             [0, "cmdoption-osxphotos-add-locations-not-shared"],
             [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
             [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
             [0, "cmdoption-osxphotos-add-locations-only-movies"],
             [0, "cmdoption-osxphotos-add-locations-only-photos"],
             [0, "cmdoption-osxphotos-add-locations-panorama"],
             [0, "cmdoption-osxphotos-add-locations-person"],
             [0, "cmdoption-osxphotos-add-locations-place"],
             [0, "cmdoption-osxphotos-add-locations-portrait"],
             [0, "cmdoption-osxphotos-add-locations-query-eval"],
             [0, "cmdoption-osxphotos-add-locations-query-function"],
             [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
             [0, "cmdoption-osxphotos-add-locations-screenshot"],
             [0, "cmdoption-osxphotos-add-locations-selected"],
             [0, "cmdoption-osxphotos-add-locations-selfie"],
             [0, "cmdoption-osxphotos-add-locations-shared"],
             [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-syndicated"],
             [0, "cmdoption-osxphotos-add-locations-theme"],
             [0, "cmdoption-osxphotos-add-locations-time-lapse"],
             [0, "cmdoption-osxphotos-add-locations-timestamp"],
             [0, "cmdoption-osxphotos-add-locations-title"],
             [0, "cmdoption-osxphotos-add-locations-to-date"],
             [0, "cmdoption-osxphotos-add-locations-to-time"],
             [0, "cmdoption-osxphotos-add-locations-uti"],
@@ -5604,18 +5666,20 @@
             [0, "cmdoption-osxphotos-export-not-in-album"],
             [0, "cmdoption-osxphotos-export-not-incloud"],
             [0, "cmdoption-osxphotos-export-not-live"],
             [0, "cmdoption-osxphotos-export-not-missing"],
             [0, "cmdoption-osxphotos-export-not-panorama"],
             [0, "cmdoption-osxphotos-export-not-portrait"],
             [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
             [0, "cmdoption-osxphotos-export-not-screenshot"],
             [0, "cmdoption-osxphotos-export-not-selfie"],
             [0, "cmdoption-osxphotos-export-not-shared"],
             [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-syndicated"],
             [0, "cmdoption-osxphotos-export-not-time-lapse"],
             [0, "cmdoption-osxphotos-export-only-movies"],
             [0, "cmdoption-osxphotos-export-only-new"],
             [0, "cmdoption-osxphotos-export-only-photos"],
             [0, "cmdoption-osxphotos-export-original-suffix"],
             [0, "cmdoption-osxphotos-export-overwrite"],
             [0, "cmdoption-osxphotos-export-panorama"],
@@ -5633,14 +5697,15 @@
             [0, "cmdoption-osxphotos-export-query-function"],
             [0, "cmdoption-osxphotos-export-ramdb"],
             [0, "cmdoption-osxphotos-export-regex"],
             [0, "cmdoption-osxphotos-export-replace-keywords"],
             [0, "cmdoption-osxphotos-export-report"],
             [0, "cmdoption-osxphotos-export-retry"],
             [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-export-saved-to-library"],
             [0, "cmdoption-osxphotos-export-screenshot"],
             [0, "cmdoption-osxphotos-export-selected"],
             [0, "cmdoption-osxphotos-export-selfie"],
             [0, "cmdoption-osxphotos-export-shared"],
             [0, "cmdoption-osxphotos-export-sidecar"],
             [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
             [0, "cmdoption-osxphotos-export-skip-bursts"],
@@ -5648,14 +5713,15 @@
             [0, "cmdoption-osxphotos-export-skip-live"],
             [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
             [0, "cmdoption-osxphotos-export-skip-raw"],
             [0, "cmdoption-osxphotos-export-skip-uuid"],
             [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
             [0, "cmdoption-osxphotos-export-slow-mo"],
             [0, "cmdoption-osxphotos-export-strip"],
+            [0, "cmdoption-osxphotos-export-syndicated"],
             [0, "cmdoption-osxphotos-export-theme"],
             [0, "cmdoption-osxphotos-export-time-lapse"],
             [0, "cmdoption-osxphotos-export-timestamp"],
             [0, "cmdoption-osxphotos-export-title"],
             [0, "cmdoption-osxphotos-export-tmpdir"],
             [0, "cmdoption-osxphotos-export-to-date"],
             [0, "cmdoption-osxphotos-export-to-time"],
@@ -5830,35 +5896,39 @@
             [0, "cmdoption-osxphotos-query-not-in-album"],
             [0, "cmdoption-osxphotos-query-not-incloud"],
             [0, "cmdoption-osxphotos-query-not-live"],
             [0, "cmdoption-osxphotos-query-not-missing"],
             [0, "cmdoption-osxphotos-query-not-panorama"],
             [0, "cmdoption-osxphotos-query-not-portrait"],
             [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
             [0, "cmdoption-osxphotos-query-not-screenshot"],
             [0, "cmdoption-osxphotos-query-not-selfie"],
             [0, "cmdoption-osxphotos-query-not-shared"],
             [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-syndicated"],
             [0, "cmdoption-osxphotos-query-not-time-lapse"],
             [0, "cmdoption-osxphotos-query-only-movies"],
             [0, "cmdoption-osxphotos-query-only-photos"],
             [0, "cmdoption-osxphotos-query-panorama"],
             [0, "cmdoption-osxphotos-query-person"],
             [0, "cmdoption-osxphotos-query-place"],
             [0, "cmdoption-osxphotos-query-portrait"],
             [0, "cmdoption-osxphotos-query-print"],
             [0, "cmdoption-osxphotos-query-query-eval"],
             [0, "cmdoption-osxphotos-query-query-function"],
             [0, "cmdoption-osxphotos-query-quiet"],
             [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-query-saved-to-library"],
             [0, "cmdoption-osxphotos-query-screenshot"],
             [0, "cmdoption-osxphotos-query-selected"],
             [0, "cmdoption-osxphotos-query-selfie"],
             [0, "cmdoption-osxphotos-query-shared"],
             [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-query-syndicated"],
             [0, "cmdoption-osxphotos-query-time-lapse"],
             [0, "cmdoption-osxphotos-query-title"],
             [0, "cmdoption-osxphotos-query-to-date"],
             [0, "cmdoption-osxphotos-query-to-time"],
             [0, "cmdoption-osxphotos-query-uti"],
             [0, "cmdoption-osxphotos-query-uuid"],
             [0, "cmdoption-osxphotos-query-uuid-from-file"],
@@ -5917,33 +5987,37 @@
             [0, "cmdoption-osxphotos-repl-not-in-album"],
             [0, "cmdoption-osxphotos-repl-not-incloud"],
             [0, "cmdoption-osxphotos-repl-not-live"],
             [0, "cmdoption-osxphotos-repl-not-missing"],
             [0, "cmdoption-osxphotos-repl-not-panorama"],
             [0, "cmdoption-osxphotos-repl-not-portrait"],
             [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
             [0, "cmdoption-osxphotos-repl-not-screenshot"],
             [0, "cmdoption-osxphotos-repl-not-selfie"],
             [0, "cmdoption-osxphotos-repl-not-shared"],
             [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-syndicated"],
             [0, "cmdoption-osxphotos-repl-not-time-lapse"],
             [0, "cmdoption-osxphotos-repl-only-movies"],
             [0, "cmdoption-osxphotos-repl-only-photos"],
             [0, "cmdoption-osxphotos-repl-panorama"],
             [0, "cmdoption-osxphotos-repl-person"],
             [0, "cmdoption-osxphotos-repl-place"],
             [0, "cmdoption-osxphotos-repl-portrait"],
             [0, "cmdoption-osxphotos-repl-query-eval"],
             [0, "cmdoption-osxphotos-repl-query-function"],
             [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-repl-saved-to-library"],
             [0, "cmdoption-osxphotos-repl-screenshot"],
             [0, "cmdoption-osxphotos-repl-selected"],
             [0, "cmdoption-osxphotos-repl-selfie"],
             [0, "cmdoption-osxphotos-repl-shared"],
             [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-syndicated"],
             [0, "cmdoption-osxphotos-repl-time-lapse"],
             [0, "cmdoption-osxphotos-repl-title"],
             [0, "cmdoption-osxphotos-repl-to-date"],
             [0, "cmdoption-osxphotos-repl-to-time"],
             [0, "cmdoption-osxphotos-repl-uti"],
             [0, "cmdoption-osxphotos-repl-uuid"],
             [0, "cmdoption-osxphotos-repl-uuid-from-file"],
@@ -6019,32 +6093,36 @@
             [0, "cmdoption-osxphotos-sync-not-in-album"],
             [0, "cmdoption-osxphotos-sync-not-incloud"],
             [0, "cmdoption-osxphotos-sync-not-live"],
             [0, "cmdoption-osxphotos-sync-not-missing"],
             [0, "cmdoption-osxphotos-sync-not-panorama"],
             [0, "cmdoption-osxphotos-sync-not-portrait"],
             [0, "cmdoption-osxphotos-sync-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-saved-to-library"],
             [0, "cmdoption-osxphotos-sync-not-screenshot"],
             [0, "cmdoption-osxphotos-sync-not-selfie"],
             [0, "cmdoption-osxphotos-sync-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-syndicated"],
             [0, "cmdoption-osxphotos-sync-not-time-lapse"],
             [0, "cmdoption-osxphotos-sync-only-movies"],
             [0, "cmdoption-osxphotos-sync-only-photos"],
             [0, "cmdoption-osxphotos-sync-panorama"],
             [0, "cmdoption-osxphotos-sync-person"],
             [0, "cmdoption-osxphotos-sync-place"],
             [0, "cmdoption-osxphotos-sync-portrait"],
             [0, "cmdoption-osxphotos-sync-query-eval"],
             [0, "cmdoption-osxphotos-sync-query-function"],
             [0, "cmdoption-osxphotos-sync-regex"],
             [0, "cmdoption-osxphotos-sync-s"],
+            [0, "cmdoption-osxphotos-sync-saved-to-library"],
             [0, "cmdoption-osxphotos-sync-screenshot"],
             [0, "cmdoption-osxphotos-sync-selected"],
             [0, "cmdoption-osxphotos-sync-selfie"],
             [0, "cmdoption-osxphotos-sync-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-syndicated"],
             [0, "cmdoption-osxphotos-sync-theme"],
             [0, "cmdoption-osxphotos-sync-time-lapse"],
             [0, "cmdoption-osxphotos-sync-timestamp"],
             [0, "cmdoption-osxphotos-sync-title"],
             [0, "cmdoption-osxphotos-sync-to-date"],
             [0, "cmdoption-osxphotos-sync-to-time"],
             [0, "cmdoption-osxphotos-sync-uti"],
@@ -6873,26 +6951,32 @@
         ],
         "not_portrait (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_portrait"]
         ],
         "not_reference (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_reference"]
         ],
+        "not_saved_to_library (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_saved_to_library"]
+        ],
         "not_screenshot (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_screenshot"]
         ],
         "not_selfie (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_selfie"]
         ],
         "not_shared (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_shared"]
         ],
         "not_slow_mo (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_slow_mo"]
         ],
+        "not_syndicated (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_syndicated"]
+        ],
         "not_time_lapse (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_time_lapse"]
         ],
         "orientation (osxphotos.photoinfo property)": [
             [4, "osxphotos.PhotoInfo.orientation"]
         ],
         "original_filename (osxphotos.photoinfo property)": [
@@ -7068,14 +7152,20 @@
         ],
         "rmdir() (osxphotos.fileutilnoop class method)": [
             [4, "osxphotos.FileUtilNoOp.rmdir"]
         ],
         "run_commands() (osxphotos.exiftool method)": [
             [4, "osxphotos.ExifTool.run_commands"]
         ],
+        "saved_to_library (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.saved_to_library"]
+        ],
+        "saved_to_library (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.saved_to_library"]
+        ],
         "score (osxphotos.photoinfo property)": [
             [4, "osxphotos.PhotoInfo.score"]
         ],
         "screenshot (osxphotos.photoinfo property)": [
             [4, "osxphotos.PhotoInfo.screenshot"]
         ],
         "screenshot (osxphotos.queryoptions attribute)": [
@@ -7158,14 +7248,20 @@
         ],
         "subfolders (osxphotos.folderinfo property)": [
             [4, "osxphotos.FolderInfo.subfolders"]
         ],
         "subtitle (osxphotos.momentinfo property)": [
             [4, "osxphotos.MomentInfo.subtitle"]
         ],
+        "syndicated (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.syndicated"]
+        ],
+        "syndicated (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.syndicated"]
+        ],
         "tables() (osxphotos.photoinfo method)": [
             [4, "osxphotos.PhotoInfo.tables"]
         ],
         "text_found (osxphotos.searchinfo property)": [
             [4, "osxphotos.SearchInfo.text_found"]
         ],
         "time_lapse (osxphotos.photoinfo property)": [
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.2 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.2’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.3’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.2â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.3â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.2 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.2/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.3/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/exifinfo.py` & `osxphotos-0.60.3/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/exiftool.py` & `osxphotos-0.60.3/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.3/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/export_db.py` & `osxphotos-0.60.3/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/export_db_utils.py` & `osxphotos-0.60.3/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/fileutil.py` & `osxphotos-0.60.3/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.3/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/imageconverter.py` & `osxphotos-0.60.3/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/momentinfo.py` & `osxphotos-0.60.3/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/path_utils.py` & `osxphotos-0.60.3/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/personinfo.py` & `osxphotos-0.60.3/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photodates.py` & `osxphotos-0.60.3/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photoexporter.py` & `osxphotos-0.60.3/osxphotos/photoexporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photoinfo.py` & `osxphotos-0.60.3/osxphotos/photoinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,19 @@
 from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate, RenderOptions
 from .placeinfo import PlaceInfo4, PlaceInfo5
 from .query_builder import get_query
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
 from .uti import get_preferred_uti_extension, get_uti_for_extension
-from .utils import _get_resource_loc, assert_macos, is_macos, hexdigest, list_directory
+from .utils import _get_resource_loc, assert_macos, hexdigest, is_macos, list_directory
 
 if is_macos:
     from osxmetadata import OSXMetaData
+
     from .text_detection import detect_text
 
 __all__ = ["PhotoInfo", "PhotoInfoNone", "frozen_photoinfo_factory"]
 
 logger = logging.getLogger("osxphotos")
 
 
@@ -130,16 +131,15 @@
         # Photos <= 4 provides no way to get date of adjustment and will update
         # lastmodifieddate anytime photo database record is updated (e.g. adding tags)
         # only report lastmodified date for Photos <=4 if photo is edited;
         # even in this case, the date could be incorrect
         if not self.hasadjustments and self._db._db_version <= _PHOTOS_4_VERSION:
             return None
 
-        imagedate = self._info["lastmodifieddate"]
-        if imagedate:
+        if imagedate := self._info["lastmodifieddate"]:
             seconds = self._info["imageTimeZoneOffsetSeconds"] or 0
             delta = timedelta(seconds=seconds)
             tz = timezone(delta)
             return imagedate.astimezone(tz=tz)
         else:
             return None
 
@@ -168,14 +168,17 @@
             self._path = photopath
             return photopath
 
     def _path_5(self):
         """Returns candidate path for original photo on Photos >= version 5"""
         if self._info["shared"]:
             return self._path_5_shared()
+        if self.syndicated and not self.saved_to_library:
+            # path for "shared with you" syndicated photos that have not yet been saved to the library
+            return self._path_syndication()
         return (
             os.path.join(self._info["directory"], self._info["filename"])
             if self._info["directory"].startswith("/")
             else os.path.join(
                 self._db._masters_path,
                 self._info["directory"],
                 self._info["filename"],
@@ -207,14 +210,29 @@
         return os.path.join(
             self._db._library_path,
             shared_path,
             self._info["directory"],
             filename,
         )
 
+    def _path_syndication(self):
+        """Return path for syndicated photo on Photos >= version 8"""
+        # Photos 8+ stores syndicated photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID.ext
+        # where X is first digit of UUID
+        syndication_path = "scopes/syndication/originals"
+        uuid_dir = self.uuid[0]
+        path = os.path.join(
+            self._db._library_path,
+            syndication_path,
+            uuid_dir,
+            self.filename,
+        )
+        return path if os.path.isfile(path) else None
+
     def _path_4(self):
         """Returns candidate path for original photo on Photos <= version 4"""
         if self._info["has_raw"]:
             # return the path to JPEG even if RAW is original
             vol = (
                 self._db._dbvolumes[self._info["raw_pair_info"]["volumeId"]]
                 if self._info["raw_pair_info"]["volumeId"] is not None
@@ -877,14 +895,18 @@
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
             if self.shared:
                 return self._path_live_photo_shared_5()
+            if self.syndicated and not self.saved_to_library:
+                # syndicated ("Shared with you") photos not yet saved to library
+                return self._path_live_syndicated()
+
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
             photopath = str(photopath)
             if not os.path.isfile(photopath):
                 # In testing, I've seen occasional missing movie for live photo
                 # these appear to be valid -- e.g. video component not yet downloaded from iCloud
                 # TODO: should this be a warning or debug?
@@ -934,42 +956,70 @@
                     # or could do the actual check with "isfile"
                     # TODO: should this be a warning or debug?
                     photopath = None
         else:
             photopath = None
         return photopath
 
+    def _path_live_syndicated(self):
+        """Return path for live syndicated photo on Photos >= version 8"""
+        # Photos 8+ stores live syndicated photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/syndication/originals/X/UUID_3.mov
+        # where X is first digit of UUID
+        syndication_path = "scopes/syndication/originals"
+        uuid_dir = self.uuid[0]
+        filename = f"{pathlib.Path(self.filename).stem}_3.mov"
+        live_photo = os.path.join(
+            self._db._library_path,
+            syndication_path,
+            uuid_dir,
+            filename,
+        )
+        return live_photo if os.path.isfile(live_photo) else None
+
     @cached_property
-    def path_derivatives(self):
+    def path_derivatives(self) -> list[str]:
         """Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
             return self._path_derivatives_5_shared()
 
         directory = self._uuid[0]  # first char of uuid
-        derivative_path = (
-            pathlib.Path(self._db._library_path) / f"resources/derivatives/{directory}"
-        )
+        if self.syndicated and not self.saved_to_library:
+            # syndicated ("Shared with you") photos not yet saved to library
+            derivative_path = "scopes/syndication/resources/derivatives"
+            thumb_path = (
+                f"{derivative_path}/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
+            )
+        else:
+            derivative_path = f"resources/derivatives/{directory}"
+            thumb_path = (
+                f"resources/derivatives/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
+            )
+
+        derivative_path = pathlib.Path(self._db._library_path).joinpath(derivative_path)
+        thumb_path = pathlib.Path(self._db._library_path).joinpath(thumb_path)
+
+        # find all files that start with uuid in derivative path
         files = list(derivative_path.glob(f"{self.uuid}*.*"))
 
         # previews may be missing from derivatives path
         # there are what appear to be low res thumbnails in the "masters" subfolder
-        thumb_path = (
-            pathlib.Path(self._db._library_path)
-            / f"resources/derivatives/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
-        )
         if thumb_path.exists():
             files.append(thumb_path)
 
+        # sort by file size, largest first
         files = sorted(files, reverse=True, key=lambda f: f.stat().st_size)
+
         # return list of filename but skip .THM files (these are actually low-res thumbnails in JPEG format but with .THM extension)
         derivatives = [str(filename) for filename in files if filename.suffix != ".THM"]
         if self.isphoto and len(derivatives) > 1 and derivatives[0].endswith(".mov"):
+            # ensure .mov is first in list as poster image could be larger than the movie preview
             derivatives[1], derivatives[0] = derivatives[0], derivatives[1]
 
         return derivatives
 
     def _path_derivatives_4(self):
         """Return paths to all derivative (preview) files for Photos <= 4"""
         modelid = self._info["modelID"]
@@ -1280,14 +1330,46 @@
         # memoize SearchInfo object
         try:
             return self._search_info_normalized
         except AttributeError:
             self._search_info_normalized = SearchInfo(self, normalized=True)
             return self._search_info_normalized
 
+    @cached_property
+    def syndicated(self) -> bool | None:
+        """Return true if photo was shared via syndication (e.g. via Messages, etc.);
+        these are photos that appear in "Shared with you" album.
+        Photos 8+ only; returns None if not Photos 8+.
+        """
+        if self._db.photos_version < 8:
+            return None
+
+        try:
+            return (
+                self._db._db_syndication_uuid[self.uuid]["syndication_identifier"]
+                is not None
+            )
+        except KeyError:
+            return False
+
+    @cached_property
+    def saved_to_library(self) -> bool | None:
+        """Return True if syndicated photo has been saved to library;
+        returns False if photo is not syndicated or has not been saved to the library.
+        Returns None if not Photos 8+.
+        Syndicated photos are photos that appear in "Shared with you" album; Photos 8+ only.
+        """
+        if self._db.photos_version < 8:
+            return None
+
+        try:
+            return self._db._db_syndication_uuid[self.uuid]["syndication_history"] != 0
+        except KeyError:
+            return False
+
     @property
     def labels(self):
         """returns list of labels applied to photo by Photos image categorization
         only valid on Photos 5, on older libraries returns empty list
         """
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return []
```

### Comparing `osxphotos-0.60.2/osxphotos/photokit.py` & `osxphotos-0.60.3/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photosalbum.py` & `osxphotos-0.60.3/osxphotos/photosalbum.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,21 @@
 
     def add_list(self, photo_list: List[PhotoInfo]):
         photos = []
         for p in photo_list:
             try:
                 photos.append(photoscript.Photo(p.uuid))
             except Exception as e:
+                print(f"Error creating Photo object for photo {self._format_uuid(p.uuid)}: {e}")
                 self.verbose(
                     f"Error creating Photo object for photo {self._format_uuid(p.uuid)}: {e}"
                 )
+        print(f"photos: {photos}")
         for photolist in chunked(photos, 10):
+            print(f"photolist: {photolist}")
             self.album.add(photolist)
         photo_len = len(photo_list)
         self.verbose(
             f"Added {self._format_num(photo_len)} {pluralize(photo_len, 'photo', 'photos')} to album {self._format_album(self.name)}"
         )
 
     def photos(self):
```

### Comparing `osxphotos-0.60.2/osxphotos/photoscript_utils.py` & `osxphotos-0.60.3/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     ref: https://github.com/dogsheep/photos-to-sqlite/issues/16
 """
 
 import logging
 import pathlib
 import uuid as uuidlib
 from functools import lru_cache
-from pprint import pformat
 
 from .._constants import _PHOTOS_4_VERSION, search_category_factory
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
 from ..utils import normalize_unicode
 
 """
     This module should be imported in the class defintion of PhotosDB in photosdb.py
@@ -150,48 +149,48 @@
     conn.close()
 
 
 @property
 def labels(self):
     """return list of all search info labels found in the library"""
     if self._db_version <= _PHOTOS_4_VERSION:
-        logging.warning(f"SearchInfo not implemented for this library version")
+        logging.warning("SearchInfo not implemented for this library version")
         return []
 
     return list(self._db_searchinfo_labels.keys())
 
 
 @property
 def labels_normalized(self):
     """return list of all normalized search info labels found in the library"""
     if self._db_version <= _PHOTOS_4_VERSION:
-        logging.warning(f"SearchInfo not implemented for this library version")
+        logging.warning("SearchInfo not implemented for this library version")
         return []
 
     return list(self._db_searchinfo_labels_normalized.keys())
 
 
 @property
 def labels_as_dict(self):
     """return labels as dict of label: count in reverse sorted order (descending)"""
     if self._db_version <= _PHOTOS_4_VERSION:
-        logging.warning(f"SearchInfo not implemented for this library version")
-        return dict()
+        logging.warning("SearchInfo not implemented for this library version")
+        return {}
 
     labels = {k: len(v) for k, v in self._db_searchinfo_labels.items()}
     labels = dict(sorted(labels.items(), key=lambda kv: kv[1], reverse=True))
     return labels
 
 
 @property
 def labels_normalized_as_dict(self):
     """return normalized labels as dict of label: count in reverse sorted order (descending)"""
     if self._db_version <= _PHOTOS_4_VERSION:
-        logging.warning(f"SearchInfo not implemented for this library version")
-        return dict()
+        logging.warning("SearchInfo not implemented for this library version")
+        return {}
     labels = {k: len(v) for k, v in self._db_searchinfo_labels_normalized.items()}
     labels = dict(sorted(labels.items(), key=lambda kv: kv[1], reverse=True))
     return labels
 
 
 # The following method is not imported into PhotosDB
```

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.3/osxphotos/photosdb/photosdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     from ._photosdb_process_searchinfo import (
         _process_searchinfo,
         labels,
         labels_as_dict,
         labels_normalized,
         labels_normalized_as_dict,
     )
+    from ._photosdb_process_syndicationinfo import _process_syndicationinfo
 
     def __init__(
         self,
         dbfile=None,
         verbose=None,
         exiftool=None,
         rich=None,
@@ -286,14 +287,18 @@
         # Dict to hold information on moments (Photos 5+)
         # key is Z_PK of ZMOMENT table and values are the moment info
         self._db_moment_pk = {}
 
         # Dict to hold data on imports for Photos <= 4
         self._db_import_group = {}
 
+        # Dict to hold syndication info for Photos >= 8
+        # key is UUID and value is dict of syndication info
+        self._db_syndication_uuid = {}
+
         logger.debug(f"dbfile = {dbfile}")
 
         if dbfile is None:
             dbfile = get_last_library_path()
             if dbfile is None:
                 # get_last_library_path must have failed to find library
                 raise FileNotFoundError("Could not get path to photo library database")
@@ -2513,14 +2518,18 @@
         verbose("Processing comments and likes for shared photos.")
         self._process_comments()
 
         # process moments
         verbose("Processing moments.")
         self._process_moments()
 
+        if self.photos_version >= 8:
+            verbose("Processing syndication info.")
+            self._process_syndicationinfo()
+
         verbose("Done processing details from Photos library.")
 
     def _process_moments(self):
         """Process data from ZMOMENT table"""
         # _db_moment_pk is dict in form {pk: {moment info}} by ZMOMENT.Z_PK
 
         if self._db_version <= _PHOTOS_4_VERSION:
@@ -3512,14 +3521,24 @@
             photos = [p for p in photos if p.date_added and p.date_added < added_before]
 
         if options.added_in_last:
             added_after = datetime.now() - options.added_in_last
             added_after = datetime_naive_to_local(added_after)
             photos = [p for p in photos if p.date_added and p.date_added > added_after]
 
+        if options.syndicated:
+            photos = [p for p in photos if p.syndicated]
+        elif options.not_syndicated:
+            photos = [p for p in photos if not p.syndicated]
+
+        if options.saved_to_library:
+            photos = [p for p in photos if p.syndicated and p.saved_to_library]
+        elif options.not_saved_to_library:
+            photos = [p for p in photos if p.syndicated and not p.saved_to_library]
+
         if options.function:
             for function in options.function:
                 photos = function[0](photos)
 
         # burst should be checked last, ref #640
         if options.burst_photos:
             # add the burst_photos to the export set
```

### Comparing `osxphotos-0.60.2/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.3/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/phototables.py` & `osxphotos-0.60.3/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.3/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/phototemplate.md` & `osxphotos-0.60.3/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/phototemplate.py` & `osxphotos-0.60.3/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/phototemplate.tx` & `osxphotos-0.60.3/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/phototz.py` & `osxphotos-0.60.3/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/placeinfo.py` & `osxphotos-0.60.3/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/pyrepl.py` & `osxphotos-0.60.3/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.3/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/query_builder.py` & `osxphotos-0.60.3/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/queryoptions.py` & `osxphotos-0.60.3/osxphotos/queryoptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,18 @@
         slow_mo: search for slow-mo photos
         time_lapse: search for time-lapse photos
         title: list of titles to search for
         to_date: search for photos taken on or before this date
         uti: list of UTIs to search for
         uuid: list of uuids to search for
         year: search for photos taken in a given year
+        syndicated: search for photos that have been shared via syndication ("Shared with You" album via Messages, etc.)
+        not_syndicated: search for photos that have not been shared via syndication ("Shared with You" album via Messages, etc.)
+        saved_to_library: search for syndicated photos that have been saved to the Photos library
+        not_saved_to_library: search for syndicated photos that have not been saved to the Photos library
     """
 
     added_after: Optional[datetime.datetime] = None
     added_before: Optional[datetime.datetime] = None
     added_in_last: Optional[datetime.timedelta] = None
     album: Optional[Iterable[str]] = None
     burst_photos: Optional[bool] = None
@@ -188,14 +192,18 @@
     time_lapse: Optional[bool] = None
     title: Optional[Iterable[str]] = None
     to_date: Optional[datetime.datetime] = None
     to_time: Optional[datetime.time] = None
     uti: Optional[Iterable[str]] = None
     uuid: Optional[Iterable[str]] = None
     year: Optional[Iterable[int]] = None
+    syndicated: Optional[bool] = None
+    not_syndicated: Optional[bool] = None
+    saved_to_library: Optional[bool] = None
+    not_saved_to_library: Optional[bool] = None
 
     def asdict(self):
         return asdict(self)
 
 
 def query_options_from_kwargs(**kwargs) -> QueryOptions:
     """Validate query options and create a QueryOptions instance.
@@ -257,14 +265,16 @@
         ("selfie", "not_selfie"),
         ("shared", "not_shared"),
         ("slow_mo", "not_slow_mo"),
         ("time_lapse", "not_time_lapse"),
         ("deleted", "not_deleted"),
         ("deleted", "deleted_only"),
         ("deleted_only", "not_deleted"),
+        ("syndicated", "not_syndicated"),
+        ("saved_to_library", "not_saved_to_library"),
     ]
     # TODO: add option to validate requiring at least one query arg
     for arg, not_arg in exclusive:
         if kwargs.get(arg) and kwargs.get(not_arg):
             arg = arg.replace("_", "-")
             not_arg = not_arg.replace("_", "-")
             raise IncompatibleQueryOptions(
```

### Comparing `osxphotos-0.60.2/osxphotos/scoreinfo.py` & `osxphotos-0.60.3/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/searchinfo.py` & `osxphotos-0.60.3/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/sqlgrep.py` & `osxphotos-0.60.3/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/sqlite_utils.py` & `osxphotos-0.60.3/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.3/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/template_counter.py` & `osxphotos-0.60.3/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.3/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.3/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/text_detection.py` & `osxphotos-0.60.3/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/timeutils.py` & `osxphotos-0.60.3/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/timezones.py` & `osxphotos-0.60.3/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/tutorial.md` & `osxphotos-0.60.3/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/uti.py` & `osxphotos-0.60.3/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos/utils.py` & `osxphotos-0.60.3/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.3/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.2
+Version: 0.60.3
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.2/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.3/osxphotos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 osxphotos/docs/docs.zip
 osxphotos/photosdb/__init__.py
 osxphotos/photosdb/_photosdb_process_comments.py
 osxphotos/photosdb/_photosdb_process_exif.py
 osxphotos/photosdb/_photosdb_process_faceinfo.py
 osxphotos/photosdb/_photosdb_process_scoreinfo.py
 osxphotos/photosdb/_photosdb_process_searchinfo.py
+osxphotos/photosdb/_photosdb_process_syndicationinfo.py
 osxphotos/photosdb/photosdb.py
 osxphotos/photosdb/photosdb_utils.py
 osxphotos/queries/README.md
 osxphotos/queries/cloud_album_owner.sql.mako
 osxphotos/queries/shared_owner.sql.mako
 osxphotos/queries/title.sql.mako
 osxphotos/templates/DESCRIPTION.txt
```

### Comparing `osxphotos-0.60.2/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.3/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/setup.py` & `osxphotos-0.60.3/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_10_12_6.py` & `osxphotos-0.60.3/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.3/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.3/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.3/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.3/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli.py` & `osxphotos-0.60.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_add_locations.py` & `osxphotos-0.60.3/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_add_to_album.py` & `osxphotos-0.60.3/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_all_commands.py` & `osxphotos-0.60.3/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_batch_edit.py` & `osxphotos-0.60.3/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_dump.py` & `osxphotos-0.60.3/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_exiftool.py` & `osxphotos-0.60.3/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_export_cloud.py` & `osxphotos-0.60.3/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_export_projects.py` & `osxphotos-0.60.3/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_exportdb.py` & `osxphotos-0.60.3/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_import.py` & `osxphotos-0.60.3/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_orphans.py` & `osxphotos-0.60.3/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_param_types.py` & `osxphotos-0.60.3/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_sync.py` & `osxphotos-0.60.3/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_timewarp.py` & `osxphotos-0.60.3/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_utils.py` & `osxphotos-0.60.3/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cli_verbose.py` & `osxphotos-0.60.3/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.3/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_comments.py` & `osxphotos-0.60.3/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_concurrent_export.py` & `osxphotos-0.60.3/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_configoptions.py` & `osxphotos-0.60.3/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_datetime_formatter.py` & `osxphotos-0.60.3/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_datetime_utils.py` & `osxphotos-0.60.3/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_debug.py` & `osxphotos-0.60.3/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_empty_library_4_0.py` & `osxphotos-0.60.3/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_exif_info.py` & `osxphotos-0.60.3/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_exiftool.py` & `osxphotos-0.60.3/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_exiftool_caching.py` & `osxphotos-0.60.3/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.3/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.3/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.3/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_export_db.py` & `osxphotos-0.60.3/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.3/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_exportresults.py` & `osxphotos-0.60.3/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_faceinfo.py` & `osxphotos-0.60.3/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_fileutil.py` & `osxphotos-0.60.3/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_highsierra.py` & `osxphotos-0.60.3/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_image_converter.py` & `osxphotos-0.60.3/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.3/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.3/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.3/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.3/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.3/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.3/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.3/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.3/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_movies_4_0.py` & `osxphotos-0.60.3/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_movies_5_0.py` & `osxphotos-0.60.3/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_path_utils.py` & `osxphotos-0.60.3/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_personinfo.py` & `osxphotos-0.60.3/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_photokit.py` & `osxphotos-0.60.3/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_photosdb_utils.py` & `osxphotos-0.60.3/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_placeinfo.py` & `osxphotos-0.60.3/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.3/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.3/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_projects_catalina.py` & `osxphotos-0.60.3/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_projects_sierra.py` & `osxphotos-0.60.3/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_score_info.py` & `osxphotos-0.60.3/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.3/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.3/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.3/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.3/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.3/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_sidecar_xmp.py` & `osxphotos-0.60.3/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.3/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.3/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.3/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.3/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_sqlitekvstore.py` & `osxphotos-0.60.3/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_template.py` & `osxphotos-0.60.3/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_template_counter.py` & `osxphotos-0.60.3/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_template_today.py` & `osxphotos-0.60.3/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_uti.py` & `osxphotos-0.60.3/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_utils.py` & `osxphotos-0.60.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.3/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.2/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.3/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

