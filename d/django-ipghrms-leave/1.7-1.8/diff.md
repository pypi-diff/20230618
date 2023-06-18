# Comparing `tmp/django-ipghrms-leave-1.7.tar.gz` & `tmp/django-ipghrms-leave-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-leave-1.7.tar", last modified: Sat Jun  3 14:24:45 2023, max compression
+gzip compressed data, was "django-ipghrms-leave-1.8.tar", last modified: Mon Jun  5 04:30:03 2023, max compression
```

## Comparing `django-ipghrms-leave-1.7.tar` & `django-ipghrms-leave-1.8.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:45.056480 django-ipghrms-leave-1.7/
--rw-rw-rw-   0        0        0     1065 2023-03-27 14:45:38.000000 django-ipghrms-leave-1.7/LICENSE
--rw-rw-rw-   0        0        0      214 2023-03-27 14:21:05.000000 django-ipghrms-leave-1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      945 2023-06-03 14:24:45.056480 django-ipghrms-leave-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-03-27 14:21:43.000000 django-ipghrms-leave-1.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.527927 django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-03 14:24:44.000000 django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18263 2023-06-03 14:24:44.000000 django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 14:24:44.000000 django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 14:24:44.000000 django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.607691 django-ipghrms-leave-1.7/leave/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/__init__.py
--rw-rw-rw-   0        0        0     2212 2023-06-02 21:00:06.000000 django-ipghrms-leave-1.7/leave/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.610704 django-ipghrms-leave-1.7/leave/api/
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.616657 django-ipghrms-leave-1.7/leave/api/__pycache__/
--rw-rw-rw-   0        0        0     1223 2023-02-05 08:06:39.000000 django-ipghrms-leave-1.7/leave/api/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0     9993 2023-02-05 08:09:34.000000 django-ipghrms-leave-1.7/leave/api/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     1189 2023-02-05 08:06:35.000000 django-ipghrms-leave-1.7/leave/api/urls.py
--rw-rw-rw-   0        0        0    13296 2023-02-05 08:09:31.000000 django-ipghrms-leave-1.7/leave/api/views.py
--rw-rw-rw-   0        0        0      178 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/apps.py
--rw-rw-rw-   0        0        0    11646 2023-05-30 04:20:36.000000 django-ipghrms-leave-1.7/leave/forms.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.722374 django-ipghrms-leave-1.7/leave/migrations/
--rw-rw-rw-   0        0        0     4776 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      317 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0002_remove_taskdelegate_date.py
--rw-rw-rw-   0        0        0      450 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0003_rename_taskdelegate_leavedelegate.py
--rw-rw-rw-   0        0        0      619 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0004_alter_leavedelegate_employee.py
--rw-rw-rw-   0        0        0      384 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0005_rename_is_approve_leavedelegate_is_confirm.py
--rw-rw-rw-   0        0        0      430 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0006_leavedelegate_is_confirm2.py
--rw-rw-rw-   0        0        0      400 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0007_leavetype_total.py
--rw-rw-rw-   0        0        0      649 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py
--rw-rw-rw-   0        0        0      705 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py
--rw-rw-rw-   0        0        0      980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py
--rw-rw-rw-   0        0        0     1507 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py
--rw-rw-rw-   0        0        0      766 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py
--rw-rw-rw-   0        0        0      425 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0013_leave_is_finish.py
--rw-rw-rw-   0        0        0     2028 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0014_leavehr_leavede.py
--rw-rw-rw-   0        0        0     1198 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py
--rw-rw-rw-   0        0        0      427 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0016_leave_is_print.py
--rw-rw-rw-   0        0        0      750 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py
--rw-rw-rw-   0        0        0      464 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0018_alter_leavecount_balance.py
--rw-rw-rw-   0        0        0      406 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0019_leave_s_is_delegate.py
--rw-rw-rw-   0        0        0      331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0020_remove_leave_s_is_delegate.py
--rw-rw-rw-   0        0        0      572 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0021_leave_is_approve_leave_is_reject.py
--rw-rw-rw-   0        0        0      664 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py
--rw-rw-rw-   0        0        0      359 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0023_remove_leavedelegate_is_send.py
--rw-rw-rw-   0        0        0      407 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/0024_alter_leave_is_active.py
--rw-rw-rw-   0        0        0      795 2022-12-10 14:29:58.000000 django-ipghrms-leave-1.7/leave/migrations/0025_auto_20221210_2329.py
--rw-rw-rw-   0        0        0      590 2022-12-10 14:56:41.000000 django-ipghrms-leave-1.7/leave/migrations/0026_auto_20221210_2356.py
--rw-rw-rw-   0        0        0      460 2022-12-10 15:22:16.000000 django-ipghrms-leave-1.7/leave/migrations/0027_auto_20221211_0022.py
--rw-rw-rw-   0        0        0      590 2022-12-10 17:02:09.000000 django-ipghrms-leave-1.7/leave/migrations/0028_auto_20221211_0202.py
--rw-rw-rw-   0        0        0     1255 2022-12-11 02:51:24.000000 django-ipghrms-leave-1.7/leave/migrations/0029_leavedep.py
--rw-rw-rw-   0        0        0      577 2022-12-11 03:06:33.000000 django-ipghrms-leave-1.7/leave/migrations/0030_auto_20221211_1206.py
--rw-rw-rw-   0        0        0      414 2022-12-11 04:16:56.000000 django-ipghrms-leave-1.7/leave/migrations/0031_leave_is_update.py
--rw-rw-rw-   0        0        0      413 2022-12-17 06:24:38.000000 django-ipghrms-leave-1.7/leave/migrations/0032_leave_dep_send_pr.py
--rw-rw-rw-   0        0        0      414 2022-12-17 06:40:11.000000 django-ipghrms-leave-1.7/leave/migrations/0033_leave_pr_confirm.py
--rw-rw-rw-   0        0        0      382 2022-12-17 06:43:34.000000 django-ipghrms-leave-1.7/leave/migrations/0034_rename_pr_confirm_leave_pr_approve.py
--rw-rw-rw-   0        0        0      652 2022-12-17 07:14:52.000000 django-ipghrms-leave-1.7/leave/migrations/0035_leave_file.py
--rw-rw-rw-   0        0        0      409 2022-12-17 08:47:37.000000 django-ipghrms-leave-1.7/leave/migrations/0036_leave_unit_send_pr.py
--rw-rw-rw-   0        0        0      445 2022-12-20 07:39:43.000000 django-ipghrms-leave-1.7/leave/migrations/0037_alter_leavetype_total.py
--rw-rw-rw-   0        0        0      416 2022-12-20 07:43:17.000000 django-ipghrms-leave-1.7/leave/migrations/0038_alter_leavetype_total.py
--rw-rw-rw-   0        0        0      448 2022-12-20 07:50:53.000000 django-ipghrms-leave-1.7/leave/migrations/0039_alter_leavetype_total.py
--rw-rw-rw-   0        0        0      475 2022-12-20 07:55:29.000000 django-ipghrms-leave-1.7/leave/migrations/0040_alter_leavecount_balance.py
--rw-rw-rw-   0        0        0      474 2022-12-20 07:55:59.000000 django-ipghrms-leave-1.7/leave/migrations/0041_alter_leavecount_total.py
--rw-rw-rw-   0        0        0      466 2022-12-20 07:56:29.000000 django-ipghrms-leave-1.7/leave/migrations/0042_alter_leave_days.py
--rw-rw-rw-   0        0        0      488 2022-12-20 07:58:42.000000 django-ipghrms-leave-1.7/leave/migrations/0043_leavecount_balance_carry.py
--rw-rw-rw-   0        0        0      472 2022-12-20 08:17:40.000000 django-ipghrms-leave-1.7/leave/migrations/0044_leavecount_taken.py
--rw-rw-rw-   0        0        0      740 2022-12-20 08:22:31.000000 django-ipghrms-leave-1.7/leave/migrations/0045_auto_20221220_1722.py
--rw-rw-rw-   0        0        0     1060 2022-12-20 08:25:13.000000 django-ipghrms-leave-1.7/leave/migrations/0046_month_year.py
--rw-rw-rw-   0        0        0     1850 2022-12-20 08:29:51.000000 django-ipghrms-leave-1.7/leave/migrations/0047_auto_20221220_1729.py
--rw-rw-rw-   0        0        0     1638 2022-12-21 01:08:08.000000 django-ipghrms-leave-1.7/leave/migrations/0048_auto_20221221_1008.py
--rw-rw-rw-   0        0        0      843 2022-12-21 01:09:38.000000 django-ipghrms-leave-1.7/leave/migrations/0049_auto_20221221_1009.py
--rw-rw-rw-   0        0        0      494 2022-12-21 02:48:00.000000 django-ipghrms-leave-1.7/leave/migrations/0050_leavecount_total_balance_leave.py
--rw-rw-rw-   0        0        0      493 2022-12-21 02:56:16.000000 django-ipghrms-leave-1.7/leave/migrations/0051_alter_leavecount_taken.py
--rw-rw-rw-   0        0        0      495 2022-12-25 12:08:36.000000 django-ipghrms-leave-1.7/leave/migrations/0052_leavecount_prov_total_earn.py
--rw-rw-rw-   0        0        0      499 2022-12-25 12:23:35.000000 django-ipghrms-leave-1.7/leave/migrations/0053_leavecount_total_taken.py
--rw-rw-rw-   0        0        0      777 2022-12-25 13:32:11.000000 django-ipghrms-leave-1.7/leave/migrations/0054_auto_20221225_2232.py
--rw-rw-rw-   0        0        0      461 2022-12-26 14:37:12.000000 django-ipghrms-leave-1.7/leave/migrations/0055_leave_description.py
--rw-rw-rw-   0        0        0      638 2022-12-29 17:21:13.000000 django-ipghrms-leave-1.7/leave/migrations/0056_auto_20221230_0221.py
--rw-rw-rw-   0        0        0      342 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.7/leave/migrations/0057_alter_leavecount_options.py
--rw-rw-rw-   0        0        0      583 2023-01-10 05:27:23.000000 django-ipghrms-leave-1.7/leave/migrations/0058_leaveperiod_employee.py
--rw-rw-rw-   0        0        0      642 2023-01-10 06:35:47.000000 django-ipghrms-leave-1.7/leave/migrations/0059_auto_20230110_1535.py
--rw-rw-rw-   0        0        0      415 2023-01-13 15:24:54.000000 django-ipghrms-leave-1.7/leave/migrations/0060_leavecount_update_date.py
--rw-rw-rw-   0        0        0      486 2023-01-14 03:47:27.000000 django-ipghrms-leave-1.7/leave/migrations/0061_leavecount_balance_month.py
--rw-rw-rw-   0        0        0      441 2023-01-18 02:16:22.000000 django-ipghrms-leave-1.7/leave/migrations/0062_leavehr_comment.py
--rw-rw-rw-   0        0        0      409 2023-01-19 02:02:15.000000 django-ipghrms-leave-1.7/leave/migrations/0063_leave_is_done.py
--rw-rw-rw-   0        0        0      407 2023-01-22 06:45:20.000000 django-ipghrms-leave-1.7/leave/migrations/0064_leave_pr_send.py
--rw-rw-rw-   0        0        0      412 2023-01-22 08:06:42.000000 django-ipghrms-leave-1.7/leave/migrations/0065_leave_vice_send_pr.py
--rw-rw-rw-   0        0        0      414 2023-01-22 08:31:12.000000 django-ipghrms-leave-1.7/leave/migrations/0066_leave_pr_notify.py
--rw-rw-rw-   0        0        0      416 2023-01-29 06:59:00.000000 django-ipghrms-leave-1.7/leave/migrations/0067_leave_is_send_to_div.py
--rw-rw-rw-   0        0        0      858 2023-02-02 00:25:33.000000 django-ipghrms-leave-1.7/leave/migrations/0068_auto_20230202_0925.py
--rw-rw-rw-   0        0        0      427 2023-02-02 05:46:44.000000 django-ipghrms-leave-1.7/leave/migrations/0069_leave_is_special.py
--rw-rw-rw-   0        0        0      430 2023-02-02 05:47:51.000000 django-ipghrms-leave-1.7/leave/migrations/0070_leave_is_create_by_hr.py
--rw-rw-rw-   0        0        0      793 2023-03-13 10:08:08.000000 django-ipghrms-leave-1.7/leave/migrations/0071_auto_20230313_1908.py
--rw-rw-rw-   0        0        0      770 2023-03-13 14:31:35.000000 django-ipghrms-leave-1.7/leave/migrations/0072_auto_20230313_2331.py
--rw-rw-rw-   0        0        0      818 2023-03-13 14:38:15.000000 django-ipghrms-leave-1.7/leave/migrations/0073_auto_20230313_2338.py
--rw-rw-rw-   0        0        0      794 2023-03-13 14:41:54.000000 django-ipghrms-leave-1.7/leave/migrations/0074_auto_20230313_2341.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.912872 django-ipghrms-leave-1.7/leave/migrations/__pycache__/
--rw-rw-rw-   0        0        0     2438 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     2406 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-rw-rw-   0        0        0     2442 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-rw-   0        0        0      513 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      499 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-37.pyc
--rw-rw-rw-   0        0        0      517 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc
--rw-rw-rw-   0        0        0      633 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc
--rw-rw-rw-   0        0        0      625 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc
--rw-rw-rw-   0        0        0      637 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc
--rw-rw-rw-   0        0        0      813 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc
--rw-rw-rw-   0        0        0      799 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc
--rw-rw-rw-   0        0        0      817 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc
--rw-rw-rw-   0        0        0      589 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc
--rw-rw-rw-   0        0        0      575 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc
--rw-rw-rw-   0        0        0      593 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc
--rw-rw-rw-   0        0        0      630 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc
--rw-rw-rw-   0        0        0      616 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc
--rw-rw-rw-   0        0        0      634 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc
--rw-rw-rw-   0        0        0      590 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      576 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc
--rw-rw-rw-   0        0        0      594 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc
--rw-rw-rw-   0        0        0      659 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      641 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      663 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      765 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      747 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      769 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc
--rw-rw-rw-   0        0        0      798 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc
--rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc
--rw-rw-rw-   0        0        0     1365 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     1343 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0     1369 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc
--rw-rw-rw-   0        0        0      800 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc
--rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc
--rw-rw-rw-   0        0        0      613 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc
--rw-rw-rw-   0        0        0      599 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc
--rw-rw-rw-   0        0        0      617 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc
--rw-rw-rw-   0        0        0     1398 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc
--rw-rw-rw-   0        0        0     1378 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc
--rw-rw-rw-   0        0        0     1402 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc
--rw-rw-rw-   0        0        0      887 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      867 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      891 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      614 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc
--rw-rw-rw-   0        0        0      600 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc
--rw-rw-rw-   0        0        0      618 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      759 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      783 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      664 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc
--rw-rw-rw-   0        0        0      650 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc
--rw-rw-rw-   0        0        0      668 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc
--rw-rw-rw-   0        0        0      598 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc
--rw-rw-rw-   0        0        0      584 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc
--rw-rw-rw-   0        0        0      602 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc
--rw-rw-rw-   0        0        0      527 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc
--rw-rw-rw-   0        0        0      513 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc
--rw-rw-rw-   0        0        0      531 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc
--rw-rw-rw-   0        0        0      655 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc
--rw-rw-rw-   0        0        0      639 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc
--rw-rw-rw-   0        0        0      659 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc
--rw-rw-rw-   0        0        0      676 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      658 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      680 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      559 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc
--rw-rw-rw-   0        0        0      545 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc
--rw-rw-rw-   0        0        0      563 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc
--rw-rw-rw-   0        0        0      601 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc
--rw-rw-rw-   0        0        0      587 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc
--rw-rw-rw-   0        0        0      605 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc
--rw-rw-rw-   0        0        0      767 2022-12-10 14:30:02.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc
--rw-rw-rw-   0        0        0      636 2022-12-10 14:56:45.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc
--rw-rw-rw-   0        0        0      551 2022-12-10 15:22:20.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc
--rw-rw-rw-   0        0        0      636 2022-12-10 17:02:14.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc
--rw-rw-rw-   0        0        0     1231 2022-12-11 02:51:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc
--rw-rw-rw-   0        0        0      621 2022-12-11 03:06:37.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc
--rw-rw-rw-   0        0        0      582 2022-12-11 04:17:00.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc
--rw-rw-rw-   0        0        0      583 2022-12-17 06:24:49.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc
--rw-rw-rw-   0        0        0      583 2022-12-17 06:40:16.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc
--rw-rw-rw-   0        0        0      557 2022-12-17 06:43:37.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc
--rw-rw-rw-   0        0        0      853 2022-12-17 07:14:57.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc
--rw-rw-rw-   0        0        0      580 2022-12-17 08:47:40.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc
--rw-rw-rw-   0        0        0      631 2022-12-20 07:39:49.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      592 2022-12-20 07:43:20.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      634 2022-12-20 07:50:58.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      665 2022-12-20 07:55:32.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc
--rw-rw-rw-   0        0        0      662 2022-12-20 07:56:02.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      646 2022-12-20 07:56:33.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc
--rw-rw-rw-   0        0        0      678 2022-12-20 07:58:45.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc
--rw-rw-rw-   0        0        0      654 2022-12-20 08:17:44.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc
--rw-rw-rw-   0        0        0      810 2022-12-20 08:22:35.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc
--rw-rw-rw-   0        0        0      871 2022-12-20 08:25:17.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc
--rw-rw-rw-   0        0        0     1293 2022-12-20 08:29:55.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc
--rw-rw-rw-   0        0        0      978 2022-12-21 01:08:12.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc
--rw-rw-rw-   0        0        0      843 2022-12-21 01:09:42.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc
--rw-rw-rw-   0        0        0      690 2022-12-21 02:48:03.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc
--rw-rw-rw-   0        0        0      688 2022-12-21 02:56:19.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc
--rw-rw-rw-   0        0        0      687 2022-12-25 12:08:43.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc
--rw-rw-rw-   0        0        0      694 2022-12-25 12:23:40.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc
--rw-rw-rw-   0        0        0      885 2022-12-25 13:32:16.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc
--rw-rw-rw-   0        0        0      635 2022-12-26 14:37:20.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc
--rw-rw-rw-   0        0        0      776 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc
--rw-rw-rw-   0        0        0      517 2022-12-29 17:21:36.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc
--rw-rw-rw-   0        0        0      751 2023-01-10 05:27:31.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc
--rw-rw-rw-   0        0        0      676 2023-01-10 06:35:52.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc
--rw-rw-rw-   0        0        0      592 2023-01-13 15:25:02.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      676 2023-01-14 03:47:32.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc
--rw-rw-rw-   0        0        0      612 2023-01-18 02:16:27.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc
--rw-rw-rw-   0        0        0      575 2023-01-19 02:02:21.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc
--rw-rw-rw-   0        0        0      573 2023-01-22 06:45:26.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc
--rw-rw-rw-   0        0        0      583 2023-01-22 08:06:46.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc
--rw-rw-rw-   0        0        0      582 2023-01-22 08:31:16.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc
--rw-rw-rw-   0        0        0      589 2023-01-29 06:59:04.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc
--rw-rw-rw-   0        0        0      765 2023-02-02 00:25:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc
--rw-rw-rw-   0        0        0      593 2023-02-02 05:46:50.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc
--rw-rw-rw-   0        0        0      601 2023-02-02 05:47:54.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc
--rw-rw-rw-   0        0        0      799 2023-03-13 10:08:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc
--rw-rw-rw-   0        0        0      786 2023-03-13 14:31:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc
--rw-rw-rw-   0        0        0      810 2023-03-13 14:38:19.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc
--rw-rw-rw-   0        0        0      798 2023-03-13 14:41:58.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc
--rw-rw-rw-   0        0        0      145 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      143 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      151 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11410 2023-05-30 19:39:55.000000 django-ipghrms-leave-1.7/leave/models.py
--rw-rw-rw-   0        0        0      727 2022-12-11 02:52:39.000000 django-ipghrms-leave-1.7/leave/signals.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.451101 django-ipghrms-leave-1.7/leave/templates/
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.950763 django-ipghrms-leave-1.7/leave/templates/leave/
--rw-rw-rw-   0        0        0     3156 2023-03-14 11:55:22.000000 django-ipghrms-leave-1.7/leave/templates/leave/bal_s_list.html
--rw-rw-rw-   0        0        0     8894 2023-03-15 07:00:38.000000 django-ipghrms-leave-1.7/leave/templates/leave/c_apply_detail.html
--rw-rw-rw-   0        0        0     2029 2023-03-14 11:58:26.000000 django-ipghrms-leave-1.7/leave/templates/leave/c_apply_list.html
--rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.7/leave/templates/leave/c_deleg_detail.html
--rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.7/leave/templates/leave/c_deleg_list.html
--rw-rw-rw-   0        0        0    11028 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.7/leave/templates/leave/c_ver_detail.html
--rw-rw-rw-   0        0        0     1630 2023-03-14 11:57:58.000000 django-ipghrms-leave-1.7/leave/templates/leave/c_ver_list.html
--rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.7/leave/templates/leave/dash.html
--rw-rw-rw-   0        0        0     8646 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.7/leave/templates/leave/de_appr_detail.html
--rw-rw-rw-   0        0        0     1629 2023-02-21 06:30:12.000000 django-ipghrms-leave-1.7/leave/templates/leave/de_appr_list.html
--rw-rw-rw-   0        0        0     3714 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.7/leave/templates/leave/de_detail.html
--rw-rw-rw-   0        0        0     1993 2023-03-14 11:41:50.000000 django-ipghrms-leave-1.7/leave/templates/leave/de_list.html
--rw-rw-rw-   0        0        0     5899 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.7/leave/templates/leave/deleg_detail.html
--rw-rw-rw-   0        0        0     1715 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.7/leave/templates/leave/deleg_list.html
--rw-rw-rw-   0        0        0    15438 2023-03-14 11:47:10.000000 django-ipghrms-leave-1.7/leave/templates/leave/dep_detail.html
--rw-rw-rw-   0        0        0     1979 2023-03-14 11:56:58.000000 django-ipghrms-leave-1.7/leave/templates/leave/dep_list.html
--rw-rw-rw-   0        0        0     2096 2023-03-14 11:56:34.000000 django-ipghrms-leave-1.7/leave/templates/leave/dep_req_list.html
--rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.7/leave/templates/leave/detail.html
--rw-rw-rw-   0        0        0      233 2023-01-20 19:07:34.000000 django-ipghrms-leave-1.7/leave/templates/leave/error.html
--rw-rw-rw-   0        0        0        0 2023-03-14 10:03:00.000000 django-ipghrms-leave-1.7/leave/templates/leave/error2.html
--rw-rw-rw-   0        0        0     2388 2023-02-13 20:54:48.000000 django-ipghrms-leave-1.7/leave/templates/leave/form.html
--rw-rw-rw-   0        0        0     2616 2023-05-30 19:16:08.000000 django-ipghrms-leave-1.7/leave/templates/leave/form2.html
--rw-rw-rw-   0        0        0    12233 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_app_detail.html
--rw-rw-rw-   0        0        0     2791 2023-02-08 23:36:22.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_app_list.html
--rw-rw-rw-   0        0        0     9600 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_cert_detail.html
--rw-rw-rw-   0        0        0     2395 2023-02-08 23:45:10.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_cert_list.html
--rw-rw-rw-   0        0        0    13993 2023-05-30 07:43:02.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_leave_record.html
--rw-rw-rw-   0        0        0     2481 2023-04-10 17:37:56.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_period_list.html
--rw-rw-rw-   0        0        0     8049 2023-04-10 17:41:00.000000 django-ipghrms-leave-1.7/leave/templates/leave/hr_raw_list.html
--rw-rw-rw-   0        0        0     2160 2023-02-08 23:42:58.000000 django-ipghrms-leave-1.7/leave/templates/leave/list.html
--rw-rw-rw-   0        0        0    11403 2023-03-15 07:01:00.000000 django-ipghrms-leave-1.7/leave/templates/leave/s_apply_detail.html
--rw-rw-rw-   0        0        0     2355 2023-02-07 16:15:16.000000 django-ipghrms-leave-1.7/leave/templates/leave/s_apply_list.html
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.968716 django-ipghrms-leave-1.7/leave/templates/leave_chart/
--rw-rw-rw-   0        0        0     3992 2023-01-29 14:41:00.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/chart_leave.html
--rw-rw-rw-   0        0        0     1146 2023-01-23 16:35:15.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/emp.js
--rw-rw-rw-   0        0        0     1334 2023-01-23 16:35:32.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type.js
--rw-rw-rw-   0        0        0     2207 2023-02-05 07:02:46.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type2.js
--rw-rw-rw-   0        0        0     2240 2023-01-30 01:41:48.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type3.js
--rw-rw-rw-   0        0        0     2219 2023-02-05 07:27:37.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_month.js
--rw-rw-rw-   0        0        0     2257 2023-02-05 07:35:06.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_month_unit.js
--rw-rw-rw-   0        0        0     2211 2023-02-05 07:55:31.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_tri.js
--rw-rw-rw-   0        0        0     2215 2023-02-05 07:17:54.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_unit.js
--rw-rw-rw-   0        0        0     2211 2023-02-05 07:01:28.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year.js
--rw-rw-rw-   0        0        0     2257 2023-02-05 07:28:20.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_month.js
--rw-rw-rw-   0        0        0     2294 2023-02-05 07:57:33.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_month_unit.js
--rw-rw-rw-   0        0        0     2249 2023-02-05 07:44:38.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_tri.js
--rw-rw-rw-   0        0        0     2287 2023-02-05 08:07:00.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_tri_unit.js
--rw-rw-rw-   0        0        0     2253 2023-02-05 07:21:46.000000 django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_unit.js
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.970710 django-ipghrms-leave-1.7/leave/templates/leave_print/
--rw-rw-rw-   0        0        0     1869 2022-11-30 07:59:44.000000 django-ipghrms-leave-1.7/leave/templates/leave_print/layout.html
--rw-rw-rw-   0        0        0     5245 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.7/leave/templates/leave_print/leave_print.html
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.973702 django-ipghrms-leave-1.7/leave/templates/leave_report/
--rw-rw-rw-   0        0        0    18125 2023-02-05 10:10:59.000000 django-ipghrms-leave-1.7/leave/templates/leave_report/dash.html
--rw-rw-rw-   0        0        0     1956 2023-02-05 08:54:19.000000 django-ipghrms-leave-1.7/leave/templates/leave_report/list.html
--rw-rw-rw-   0        0        0     1917 2023-01-30 07:04:02.000000 django-ipghrms-leave-1.7/leave/templates/leave_report/list_day.html
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.976694 django-ipghrms-leave-1.7/leave/templates/pdf/
--rw-rw-rw-   0        0        0      128 2023-02-24 10:02:16.000000 django-ipghrms-leave-1.7/leave/templates/pdf/cop.html
--rw-rw-rw-   0        0        0      610 2023-02-02 15:25:15.000000 django-ipghrms-leave-1.7/leave/templates/pdf/layout.html
--rw-rw-rw-   0        0        0     7845 2023-03-15 14:31:17.000000 django-ipghrms-leave-1.7/leave/templates/pdf/leave.html
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.978688 django-ipghrms-leave-1.7/leave/templatetags/
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:44.979685 django-ipghrms-leave-1.7/leave/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      483 2023-01-14 07:10:52.000000 django-ipghrms-leave-1.7/leave/templatetags/__pycache__/orderby.cpython-310.pyc
--rw-rw-rw-   0        0        0      215 2023-01-14 07:10:49.000000 django-ipghrms-leave-1.7/leave/templatetags/orderby.py
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/tests.py
--rw-rw-rw-   0        0        0     5470 2023-05-30 07:29:56.000000 django-ipghrms-leave-1.7/leave/urls.py
--rw-rw-rw-   0        0        0     2788 2023-02-05 10:03:59.000000 django-ipghrms-leave-1.7/leave/urls_report.py
--rw-rw-rw-   0        0        0    15575 2023-05-30 07:51:10.000000 django-ipghrms-leave-1.7/leave/utils.py
--rw-rw-rw-   0        0        0     2737 2023-03-13 18:08:06.000000 django-ipghrms-leave-1.7/leave/utils_2.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:45.000630 django-ipghrms-leave-1.7/leave/views/
--rw-rw-rw-   0        0        0      325 2023-01-29 14:29:10.000000 django-ipghrms-leave-1.7/leave/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:24:45.055483 django-ipghrms-leave-1.7/leave/views/__pycache__/
--rw-rw-rw-   0        0        0      417 2023-01-29 14:29:14.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      370 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      378 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3566 2023-03-15 10:05:12.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     2343 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     2331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     2601 2023-01-29 07:19:53.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     2460 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     2469 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_v.cpython-39.pyc
--rw-rw-rw-   0        0        0      737 2023-01-23 14:19:18.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_chart.cpython-310.pyc
--rw-rw-rw-   0        0        0     2506 2023-03-15 10:08:49.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     1993 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     1980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     2279 2023-02-20 14:30:35.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     1550 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     1574 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_v.cpython-39.pyc
--rw-rw-rw-   0        0        0    25037 2023-03-13 19:37:38.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     1813 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     1814 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_m.cpython-39.pyc
--rw-rw-rw-   0        0        0    10718 2023-03-13 18:47:18.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     2398 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     2192 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_v.cpython-39.pyc
--rw-rw-rw-   0        0        0    11609 2023-03-13 18:27:21.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     6368 2022-11-07 06:40:44.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     6062 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_m.cpython-39.pyc
--rw-rw-rw-   0        0        0    17186 2023-02-15 01:07:16.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_report.cpython-310.pyc
--rw-rw-rw-   0        0        0     2026 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s.cpython-39.pyc
--rw-rw-rw-   0        0        0      821 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_m.cpython-310.pyc
--rw-rw-rw-   0        0        0      819 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_m.cpython-37.pyc
--rw-rw-rw-   0        0        0      827 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     4849 2023-03-15 14:22:55.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     2143 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     2161 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     1279 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_staff.cpython-39.pyc
--rw-rw-rw-   0        0        0     3232 2023-03-13 18:30:54.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     1961 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     1926 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/leave_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     1565 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/print.cpython-310.pyc
--rw-rw-rw-   0        0        0     1555 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/print.cpython-37.pyc
--rw-rw-rw-   0        0        0     1571 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/__pycache__/print.cpython-39.pyc
--rw-rw-rw-   0        0        0     4191 2023-03-15 10:04:22.000000 django-ipghrms-leave-1.7/leave/views/leave_c_m.py
--rw-rw-rw-   0        0        0     2732 2023-01-29 07:19:51.000000 django-ipghrms-leave-1.7/leave/views/leave_c_v.py
--rw-rw-rw-   0        0        0      527 2023-01-23 14:19:06.000000 django-ipghrms-leave-1.7/leave/views/leave_chart.py
--rw-rw-rw-   0        0        0     2610 2023-03-15 10:08:46.000000 django-ipghrms-leave-1.7/leave/views/leave_de_m.py
--rw-rw-rw-   0        0        0     2853 2023-02-20 14:30:30.000000 django-ipghrms-leave-1.7/leave/views/leave_de_v.py
--rw-rw-rw-   0        0        0    73902 2023-05-30 19:13:30.000000 django-ipghrms-leave-1.7/leave/views/leave_hr_m.py
--rw-rw-rw-   0        0        0    44603 2023-02-09 05:04:14.000000 django-ipghrms-leave-1.7/leave/views/leave_hr_m_back.py
--rw-rw-rw-   0        0        0    16680 2023-03-13 18:47:16.000000 django-ipghrms-leave-1.7/leave/views/leave_hr_v.py
--rw-rw-rw-   0        0        0    20569 2023-03-13 18:27:19.000000 django-ipghrms-leave-1.7/leave/views/leave_m.py
--rw-rw-rw-   0        0        0    31199 2023-02-15 01:07:13.000000 django-ipghrms-leave-1.7/leave/views/leave_report.py
--rw-rw-rw-   0        0        0      514 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/leave_s_m.py
--rw-rw-rw-   0        0        0     5451 2023-03-15 14:22:52.000000 django-ipghrms-leave-1.7/leave/views/leave_s_v.py
--rw-rw-rw-   0        0        0     3684 2023-03-13 18:30:52.000000 django-ipghrms-leave-1.7/leave/views/leave_v.py
--rw-rw-rw-   0        0        0     1674 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views/print.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.7/leave/views.py
--rw-rw-rw-   0        0        0      505 2023-06-03 14:24:45.058475 django-ipghrms-leave-1.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-leave-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:03.565170 django-ipghrms-leave-1.8/
+-rw-rw-rw-   0        0        0     1065 2023-03-27 14:45:38.000000 django-ipghrms-leave-1.8/LICENSE
+-rw-rw-rw-   0        0        0      214 2023-03-27 14:21:05.000000 django-ipghrms-leave-1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      924 2023-06-05 04:30:03.565170 django-ipghrms-leave-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-03-27 14:21:43.000000 django-ipghrms-leave-1.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 04:29:58.266331 django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/
+-rw-rw-rw-   0        0        0      924 2023-06-05 04:29:57.000000 django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18263 2023-06-05 04:29:58.000000 django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 04:29:57.000000 django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 04:29:57.000000 django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 04:29:58.368514 django-ipghrms-leave-1.8/leave/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/__init__.py
+-rw-rw-rw-   0        0        0     2212 2023-06-05 04:20:59.000000 django-ipghrms-leave-1.8/leave/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:29:58.388505 django-ipghrms-leave-1.8/leave/api/
+drwxrwxrwx   0        0        0        0 2023-06-05 04:29:58.414608 django-ipghrms-leave-1.8/leave/api/__pycache__/
+-rw-rw-rw-   0        0        0     1223 2023-02-05 08:06:39.000000 django-ipghrms-leave-1.8/leave/api/__pycache__/urls.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9993 2023-02-05 08:09:34.000000 django-ipghrms-leave-1.8/leave/api/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1189 2023-02-05 08:06:35.000000 django-ipghrms-leave-1.8/leave/api/urls.py
+-rw-rw-rw-   0        0        0    13296 2023-02-05 08:09:31.000000 django-ipghrms-leave-1.8/leave/api/views.py
+-rw-rw-rw-   0        0        0      178 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/apps.py
+-rw-rw-rw-   0        0        0    11646 2023-05-30 04:25:13.000000 django-ipghrms-leave-1.8/leave/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:29:58.970038 django-ipghrms-leave-1.8/leave/migrations/
+-rw-rw-rw-   0        0        0     4776 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      317 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0002_remove_taskdelegate_date.py
+-rw-rw-rw-   0        0        0      450 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0003_rename_taskdelegate_leavedelegate.py
+-rw-rw-rw-   0        0        0      619 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0004_alter_leavedelegate_employee.py
+-rw-rw-rw-   0        0        0      384 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0005_rename_is_approve_leavedelegate_is_confirm.py
+-rw-rw-rw-   0        0        0      430 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0006_leavedelegate_is_confirm2.py
+-rw-rw-rw-   0        0        0      400 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0007_leavetype_total.py
+-rw-rw-rw-   0        0        0      649 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py
+-rw-rw-rw-   0        0        0      705 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py
+-rw-rw-rw-   0        0        0      980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py
+-rw-rw-rw-   0        0        0     1507 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py
+-rw-rw-rw-   0        0        0      766 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py
+-rw-rw-rw-   0        0        0      425 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0013_leave_is_finish.py
+-rw-rw-rw-   0        0        0     2028 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0014_leavehr_leavede.py
+-rw-rw-rw-   0        0        0     1198 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py
+-rw-rw-rw-   0        0        0      427 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0016_leave_is_print.py
+-rw-rw-rw-   0        0        0      750 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py
+-rw-rw-rw-   0        0        0      464 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0018_alter_leavecount_balance.py
+-rw-rw-rw-   0        0        0      406 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0019_leave_s_is_delegate.py
+-rw-rw-rw-   0        0        0      331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0020_remove_leave_s_is_delegate.py
+-rw-rw-rw-   0        0        0      572 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0021_leave_is_approve_leave_is_reject.py
+-rw-rw-rw-   0        0        0      664 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py
+-rw-rw-rw-   0        0        0      359 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0023_remove_leavedelegate_is_send.py
+-rw-rw-rw-   0        0        0      407 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/0024_alter_leave_is_active.py
+-rw-rw-rw-   0        0        0      795 2022-12-10 14:29:58.000000 django-ipghrms-leave-1.8/leave/migrations/0025_auto_20221210_2329.py
+-rw-rw-rw-   0        0        0      590 2022-12-10 14:56:41.000000 django-ipghrms-leave-1.8/leave/migrations/0026_auto_20221210_2356.py
+-rw-rw-rw-   0        0        0      460 2022-12-10 15:22:16.000000 django-ipghrms-leave-1.8/leave/migrations/0027_auto_20221211_0022.py
+-rw-rw-rw-   0        0        0      590 2022-12-10 17:02:09.000000 django-ipghrms-leave-1.8/leave/migrations/0028_auto_20221211_0202.py
+-rw-rw-rw-   0        0        0     1255 2022-12-11 02:51:24.000000 django-ipghrms-leave-1.8/leave/migrations/0029_leavedep.py
+-rw-rw-rw-   0        0        0      577 2022-12-11 03:06:33.000000 django-ipghrms-leave-1.8/leave/migrations/0030_auto_20221211_1206.py
+-rw-rw-rw-   0        0        0      414 2022-12-11 04:16:56.000000 django-ipghrms-leave-1.8/leave/migrations/0031_leave_is_update.py
+-rw-rw-rw-   0        0        0      413 2022-12-17 06:24:38.000000 django-ipghrms-leave-1.8/leave/migrations/0032_leave_dep_send_pr.py
+-rw-rw-rw-   0        0        0      414 2022-12-17 06:40:11.000000 django-ipghrms-leave-1.8/leave/migrations/0033_leave_pr_confirm.py
+-rw-rw-rw-   0        0        0      382 2022-12-17 06:43:34.000000 django-ipghrms-leave-1.8/leave/migrations/0034_rename_pr_confirm_leave_pr_approve.py
+-rw-rw-rw-   0        0        0      652 2022-12-17 07:14:52.000000 django-ipghrms-leave-1.8/leave/migrations/0035_leave_file.py
+-rw-rw-rw-   0        0        0      409 2022-12-17 08:47:37.000000 django-ipghrms-leave-1.8/leave/migrations/0036_leave_unit_send_pr.py
+-rw-rw-rw-   0        0        0      445 2022-12-20 07:39:43.000000 django-ipghrms-leave-1.8/leave/migrations/0037_alter_leavetype_total.py
+-rw-rw-rw-   0        0        0      416 2022-12-20 07:43:17.000000 django-ipghrms-leave-1.8/leave/migrations/0038_alter_leavetype_total.py
+-rw-rw-rw-   0        0        0      448 2022-12-20 07:50:53.000000 django-ipghrms-leave-1.8/leave/migrations/0039_alter_leavetype_total.py
+-rw-rw-rw-   0        0        0      475 2022-12-20 07:55:29.000000 django-ipghrms-leave-1.8/leave/migrations/0040_alter_leavecount_balance.py
+-rw-rw-rw-   0        0        0      474 2022-12-20 07:55:59.000000 django-ipghrms-leave-1.8/leave/migrations/0041_alter_leavecount_total.py
+-rw-rw-rw-   0        0        0      466 2022-12-20 07:56:29.000000 django-ipghrms-leave-1.8/leave/migrations/0042_alter_leave_days.py
+-rw-rw-rw-   0        0        0      488 2022-12-20 07:58:42.000000 django-ipghrms-leave-1.8/leave/migrations/0043_leavecount_balance_carry.py
+-rw-rw-rw-   0        0        0      472 2022-12-20 08:17:40.000000 django-ipghrms-leave-1.8/leave/migrations/0044_leavecount_taken.py
+-rw-rw-rw-   0        0        0      740 2022-12-20 08:22:31.000000 django-ipghrms-leave-1.8/leave/migrations/0045_auto_20221220_1722.py
+-rw-rw-rw-   0        0        0     1060 2022-12-20 08:25:13.000000 django-ipghrms-leave-1.8/leave/migrations/0046_month_year.py
+-rw-rw-rw-   0        0        0     1850 2022-12-20 08:29:51.000000 django-ipghrms-leave-1.8/leave/migrations/0047_auto_20221220_1729.py
+-rw-rw-rw-   0        0        0     1638 2022-12-21 01:08:08.000000 django-ipghrms-leave-1.8/leave/migrations/0048_auto_20221221_1008.py
+-rw-rw-rw-   0        0        0      843 2022-12-21 01:09:38.000000 django-ipghrms-leave-1.8/leave/migrations/0049_auto_20221221_1009.py
+-rw-rw-rw-   0        0        0      494 2022-12-21 02:48:00.000000 django-ipghrms-leave-1.8/leave/migrations/0050_leavecount_total_balance_leave.py
+-rw-rw-rw-   0        0        0      493 2022-12-21 02:56:16.000000 django-ipghrms-leave-1.8/leave/migrations/0051_alter_leavecount_taken.py
+-rw-rw-rw-   0        0        0      495 2022-12-25 12:08:36.000000 django-ipghrms-leave-1.8/leave/migrations/0052_leavecount_prov_total_earn.py
+-rw-rw-rw-   0        0        0      499 2022-12-25 12:23:35.000000 django-ipghrms-leave-1.8/leave/migrations/0053_leavecount_total_taken.py
+-rw-rw-rw-   0        0        0      777 2022-12-25 13:32:11.000000 django-ipghrms-leave-1.8/leave/migrations/0054_auto_20221225_2232.py
+-rw-rw-rw-   0        0        0      461 2022-12-26 14:37:12.000000 django-ipghrms-leave-1.8/leave/migrations/0055_leave_description.py
+-rw-rw-rw-   0        0        0      638 2022-12-29 17:21:13.000000 django-ipghrms-leave-1.8/leave/migrations/0056_auto_20221230_0221.py
+-rw-rw-rw-   0        0        0      342 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.8/leave/migrations/0057_alter_leavecount_options.py
+-rw-rw-rw-   0        0        0      583 2023-01-10 05:27:23.000000 django-ipghrms-leave-1.8/leave/migrations/0058_leaveperiod_employee.py
+-rw-rw-rw-   0        0        0      642 2023-01-10 06:35:47.000000 django-ipghrms-leave-1.8/leave/migrations/0059_auto_20230110_1535.py
+-rw-rw-rw-   0        0        0      415 2023-01-13 15:24:54.000000 django-ipghrms-leave-1.8/leave/migrations/0060_leavecount_update_date.py
+-rw-rw-rw-   0        0        0      486 2023-01-14 03:47:27.000000 django-ipghrms-leave-1.8/leave/migrations/0061_leavecount_balance_month.py
+-rw-rw-rw-   0        0        0      441 2023-01-18 02:16:22.000000 django-ipghrms-leave-1.8/leave/migrations/0062_leavehr_comment.py
+-rw-rw-rw-   0        0        0      409 2023-01-19 02:02:15.000000 django-ipghrms-leave-1.8/leave/migrations/0063_leave_is_done.py
+-rw-rw-rw-   0        0        0      407 2023-01-22 06:45:20.000000 django-ipghrms-leave-1.8/leave/migrations/0064_leave_pr_send.py
+-rw-rw-rw-   0        0        0      412 2023-01-22 08:06:42.000000 django-ipghrms-leave-1.8/leave/migrations/0065_leave_vice_send_pr.py
+-rw-rw-rw-   0        0        0      414 2023-01-22 08:31:12.000000 django-ipghrms-leave-1.8/leave/migrations/0066_leave_pr_notify.py
+-rw-rw-rw-   0        0        0      416 2023-01-29 06:59:00.000000 django-ipghrms-leave-1.8/leave/migrations/0067_leave_is_send_to_div.py
+-rw-rw-rw-   0        0        0      858 2023-02-02 00:25:33.000000 django-ipghrms-leave-1.8/leave/migrations/0068_auto_20230202_0925.py
+-rw-rw-rw-   0        0        0      427 2023-02-02 05:46:44.000000 django-ipghrms-leave-1.8/leave/migrations/0069_leave_is_special.py
+-rw-rw-rw-   0        0        0      430 2023-02-02 05:47:51.000000 django-ipghrms-leave-1.8/leave/migrations/0070_leave_is_create_by_hr.py
+-rw-rw-rw-   0        0        0      793 2023-03-13 10:08:08.000000 django-ipghrms-leave-1.8/leave/migrations/0071_auto_20230313_1908.py
+-rw-rw-rw-   0        0        0      770 2023-03-13 14:31:35.000000 django-ipghrms-leave-1.8/leave/migrations/0072_auto_20230313_2331.py
+-rw-rw-rw-   0        0        0      818 2023-03-13 14:38:15.000000 django-ipghrms-leave-1.8/leave/migrations/0073_auto_20230313_2338.py
+-rw-rw-rw-   0        0        0      794 2023-03-13 14:41:54.000000 django-ipghrms-leave-1.8/leave/migrations/0074_auto_20230313_2341.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:01.046903 django-ipghrms-leave-1.8/leave/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     2438 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2406 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0001_initial.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2442 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-rw-   0        0        0      513 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      499 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-37.pyc
+-rw-rw-rw-   0        0        0      517 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc
+-rw-rw-rw-   0        0        0      633 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      625 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc
+-rw-rw-rw-   0        0        0      637 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      813 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc
+-rw-rw-rw-   0        0        0      799 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc
+-rw-rw-rw-   0        0        0      817 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc
+-rw-rw-rw-   0        0        0      589 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc
+-rw-rw-rw-   0        0        0      575 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc
+-rw-rw-rw-   0        0        0      593 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      630 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc
+-rw-rw-rw-   0        0        0      616 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc
+-rw-rw-rw-   0        0        0      634 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc
+-rw-rw-rw-   0        0        0      590 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      576 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc
+-rw-rw-rw-   0        0        0      594 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc
+-rw-rw-rw-   0        0        0      659 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      641 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      663 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      765 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      747 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      769 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc
+-rw-rw-rw-   0        0        0      798 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc
+-rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1365 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1343 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1369 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc
+-rw-rw-rw-   0        0        0      800 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc
+-rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc
+-rw-rw-rw-   0        0        0      613 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc
+-rw-rw-rw-   0        0        0      599 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc
+-rw-rw-rw-   0        0        0      617 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1398 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1378 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1402 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc
+-rw-rw-rw-   0        0        0      887 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      867 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      891 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      614 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc
+-rw-rw-rw-   0        0        0      600 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc
+-rw-rw-rw-   0        0        0      618 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      759 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      783 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      664 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc
+-rw-rw-rw-   0        0        0      650 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc
+-rw-rw-rw-   0        0        0      668 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      598 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      584 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc
+-rw-rw-rw-   0        0        0      602 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      527 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      513 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc
+-rw-rw-rw-   0        0        0      531 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      655 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc
+-rw-rw-rw-   0        0        0      639 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc
+-rw-rw-rw-   0        0        0      659 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc
+-rw-rw-rw-   0        0        0      676 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      658 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      680 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      559 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc
+-rw-rw-rw-   0        0        0      545 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc
+-rw-rw-rw-   0        0        0      563 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc
+-rw-rw-rw-   0        0        0      601 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc
+-rw-rw-rw-   0        0        0      587 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc
+-rw-rw-rw-   0        0        0      605 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc
+-rw-rw-rw-   0        0        0      767 2022-12-10 14:30:02.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc
+-rw-rw-rw-   0        0        0      636 2022-12-10 14:56:45.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc
+-rw-rw-rw-   0        0        0      551 2022-12-10 15:22:20.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc
+-rw-rw-rw-   0        0        0      636 2022-12-10 17:02:14.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1231 2022-12-11 02:51:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc
+-rw-rw-rw-   0        0        0      621 2022-12-11 03:06:37.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc
+-rw-rw-rw-   0        0        0      582 2022-12-11 04:17:00.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0      583 2022-12-17 06:24:49.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      583 2022-12-17 06:40:16.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc
+-rw-rw-rw-   0        0        0      557 2022-12-17 06:43:37.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc
+-rw-rw-rw-   0        0        0      853 2022-12-17 07:14:57.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc
+-rw-rw-rw-   0        0        0      580 2022-12-17 08:47:40.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      631 2022-12-20 07:39:49.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      592 2022-12-20 07:43:20.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      634 2022-12-20 07:50:58.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      665 2022-12-20 07:55:32.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc
+-rw-rw-rw-   0        0        0      662 2022-12-20 07:56:02.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      646 2022-12-20 07:56:33.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc
+-rw-rw-rw-   0        0        0      678 2022-12-20 07:58:45.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc
+-rw-rw-rw-   0        0        0      654 2022-12-20 08:17:44.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc
+-rw-rw-rw-   0        0        0      810 2022-12-20 08:22:35.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc
+-rw-rw-rw-   0        0        0      871 2022-12-20 08:25:17.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1293 2022-12-20 08:29:55.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc
+-rw-rw-rw-   0        0        0      978 2022-12-21 01:08:12.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc
+-rw-rw-rw-   0        0        0      843 2022-12-21 01:09:42.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc
+-rw-rw-rw-   0        0        0      690 2022-12-21 02:48:03.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc
+-rw-rw-rw-   0        0        0      688 2022-12-21 02:56:19.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc
+-rw-rw-rw-   0        0        0      687 2022-12-25 12:08:43.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc
+-rw-rw-rw-   0        0        0      694 2022-12-25 12:23:40.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc
+-rw-rw-rw-   0        0        0      885 2022-12-25 13:32:16.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc
+-rw-rw-rw-   0        0        0      635 2022-12-26 14:37:20.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc
+-rw-rw-rw-   0        0        0      776 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc
+-rw-rw-rw-   0        0        0      517 2022-12-29 17:21:36.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc
+-rw-rw-rw-   0        0        0      751 2023-01-10 05:27:31.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc
+-rw-rw-rw-   0        0        0      676 2023-01-10 06:35:52.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc
+-rw-rw-rw-   0        0        0      592 2023-01-13 15:25:02.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      676 2023-01-14 03:47:32.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc
+-rw-rw-rw-   0        0        0      612 2023-01-18 02:16:27.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc
+-rw-rw-rw-   0        0        0      575 2023-01-19 02:02:21.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc
+-rw-rw-rw-   0        0        0      573 2023-01-22 06:45:26.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc
+-rw-rw-rw-   0        0        0      583 2023-01-22 08:06:46.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      582 2023-01-22 08:31:16.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc
+-rw-rw-rw-   0        0        0      589 2023-01-29 06:59:04.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc
+-rw-rw-rw-   0        0        0      765 2023-02-02 00:25:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc
+-rw-rw-rw-   0        0        0      593 2023-02-02 05:46:50.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc
+-rw-rw-rw-   0        0        0      601 2023-02-02 05:47:54.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      799 2023-03-13 10:08:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc
+-rw-rw-rw-   0        0        0      786 2023-03-13 14:31:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc
+-rw-rw-rw-   0        0        0      810 2023-03-13 14:38:19.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc
+-rw-rw-rw-   0        0        0      798 2023-03-13 14:41:58.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc
+-rw-rw-rw-   0        0        0      145 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      143 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      151 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11389 2023-05-30 04:25:28.000000 django-ipghrms-leave-1.8/leave/models.py
+-rw-rw-rw-   0        0        0      727 2022-12-11 02:52:39.000000 django-ipghrms-leave-1.8/leave/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:29:58.153235 django-ipghrms-leave-1.8/leave/templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.192041 django-ipghrms-leave-1.8/leave/templates/leave/
+-rw-rw-rw-   0        0        0     3156 2023-03-13 19:55:21.000000 django-ipghrms-leave-1.8/leave/templates/leave/bal_s_list.html
+-rw-rw-rw-   0        0        0     8894 2023-03-14 15:00:37.000000 django-ipghrms-leave-1.8/leave/templates/leave/c_apply_detail.html
+-rw-rw-rw-   0        0        0     2029 2023-03-13 19:58:25.000000 django-ipghrms-leave-1.8/leave/templates/leave/c_apply_list.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/templates/leave/c_deleg_detail.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/templates/leave/c_deleg_list.html
+-rw-rw-rw-   0        0        0    11028 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave/c_ver_detail.html
+-rw-rw-rw-   0        0        0     1630 2023-03-13 19:57:57.000000 django-ipghrms-leave-1.8/leave/templates/leave/c_ver_list.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/templates/leave/dash.html
+-rw-rw-rw-   0        0        0     8646 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave/de_appr_detail.html
+-rw-rw-rw-   0        0        0     1629 2023-02-20 14:30:10.000000 django-ipghrms-leave-1.8/leave/templates/leave/de_appr_list.html
+-rw-rw-rw-   0        0        0     3714 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave/de_detail.html
+-rw-rw-rw-   0        0        0     1993 2023-03-13 19:41:48.000000 django-ipghrms-leave-1.8/leave/templates/leave/de_list.html
+-rw-rw-rw-   0        0        0     5899 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave/deleg_detail.html
+-rw-rw-rw-   0        0        0     1715 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/templates/leave/deleg_list.html
+-rw-rw-rw-   0        0        0    15438 2023-03-13 19:47:09.000000 django-ipghrms-leave-1.8/leave/templates/leave/dep_detail.html
+-rw-rw-rw-   0        0        0     1979 2023-03-13 19:56:56.000000 django-ipghrms-leave-1.8/leave/templates/leave/dep_list.html
+-rw-rw-rw-   0        0        0     2096 2023-03-13 19:56:32.000000 django-ipghrms-leave-1.8/leave/templates/leave/dep_req_list.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/templates/leave/detail.html
+-rw-rw-rw-   0        0        0      233 2023-01-20 03:07:32.000000 django-ipghrms-leave-1.8/leave/templates/leave/error.html
+-rw-rw-rw-   0        0        0        0 2023-03-13 18:02:58.000000 django-ipghrms-leave-1.8/leave/templates/leave/error2.html
+-rw-rw-rw-   0        0        0     2388 2023-02-13 04:54:46.000000 django-ipghrms-leave-1.8/leave/templates/leave/form.html
+-rw-rw-rw-   0        0        0     2616 2023-05-30 04:26:00.000000 django-ipghrms-leave-1.8/leave/templates/leave/form2.html
+-rw-rw-rw-   0        0        0    12233 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_app_detail.html
+-rw-rw-rw-   0        0        0     2791 2023-02-08 07:36:20.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_app_list.html
+-rw-rw-rw-   0        0        0     9600 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_cert_detail.html
+-rw-rw-rw-   0        0        0     2395 2023-02-08 07:45:08.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_cert_list.html
+-rw-rw-rw-   0        0        0    13993 2023-05-30 04:26:45.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_leave_record.html
+-rw-rw-rw-   0        0        0     2481 2023-04-10 02:56:35.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_period_list.html
+-rw-rw-rw-   0        0        0     8049 2023-04-10 02:56:45.000000 django-ipghrms-leave-1.8/leave/templates/leave/hr_raw_list.html
+-rw-rw-rw-   0        0        0     2160 2023-02-08 07:42:56.000000 django-ipghrms-leave-1.8/leave/templates/leave/list.html
+-rw-rw-rw-   0        0        0    11403 2023-03-14 15:00:58.000000 django-ipghrms-leave-1.8/leave/templates/leave/s_apply_detail.html
+-rw-rw-rw-   0        0        0     2355 2023-02-07 00:15:15.000000 django-ipghrms-leave-1.8/leave/templates/leave/s_apply_list.html
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.674177 django-ipghrms-leave-1.8/leave/templates/leave_chart/
+-rw-rw-rw-   0        0        0     3992 2023-01-29 14:41:00.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/chart_leave.html
+-rw-rw-rw-   0        0        0     1146 2023-01-23 16:35:15.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/emp.js
+-rw-rw-rw-   0        0        0     1334 2023-01-23 16:35:32.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type.js
+-rw-rw-rw-   0        0        0     2207 2023-02-05 07:02:46.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type2.js
+-rw-rw-rw-   0        0        0     2240 2023-01-30 01:41:48.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type3.js
+-rw-rw-rw-   0        0        0     2219 2023-02-05 07:27:37.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_month.js
+-rw-rw-rw-   0        0        0     2257 2023-02-05 07:35:06.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_month_unit.js
+-rw-rw-rw-   0        0        0     2211 2023-02-05 07:55:31.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_tri.js
+-rw-rw-rw-   0        0        0     2215 2023-02-05 07:17:54.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_unit.js
+-rw-rw-rw-   0        0        0     2211 2023-02-05 07:01:28.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year.js
+-rw-rw-rw-   0        0        0     2257 2023-02-05 07:28:20.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_month.js
+-rw-rw-rw-   0        0        0     2294 2023-02-05 07:57:33.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_month_unit.js
+-rw-rw-rw-   0        0        0     2249 2023-02-05 07:44:38.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_tri.js
+-rw-rw-rw-   0        0        0     2287 2023-02-05 08:07:00.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_tri_unit.js
+-rw-rw-rw-   0        0        0     2253 2023-02-05 07:21:46.000000 django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_unit.js
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.715600 django-ipghrms-leave-1.8/leave/templates/leave_print/
+-rw-rw-rw-   0        0        0     1869 2022-11-30 07:59:44.000000 django-ipghrms-leave-1.8/leave/templates/leave_print/layout.html
+-rw-rw-rw-   0        0        0     5245 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.8/leave/templates/leave_print/leave_print.html
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.859318 django-ipghrms-leave-1.8/leave/templates/leave_report/
+-rw-rw-rw-   0        0        0    18125 2023-02-05 10:10:59.000000 django-ipghrms-leave-1.8/leave/templates/leave_report/dash.html
+-rw-rw-rw-   0        0        0     1956 2023-02-05 08:54:19.000000 django-ipghrms-leave-1.8/leave/templates/leave_report/list.html
+-rw-rw-rw-   0        0        0     1917 2023-01-30 07:04:02.000000 django-ipghrms-leave-1.8/leave/templates/leave_report/list_day.html
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.934364 django-ipghrms-leave-1.8/leave/templates/pdf/
+-rw-rw-rw-   0        0        0      128 2023-02-24 10:02:16.000000 django-ipghrms-leave-1.8/leave/templates/pdf/cop.html
+-rw-rw-rw-   0        0        0      610 2023-02-02 15:25:15.000000 django-ipghrms-leave-1.8/leave/templates/pdf/layout.html
+-rw-rw-rw-   0        0        0     7845 2023-03-15 14:31:17.000000 django-ipghrms-leave-1.8/leave/templates/pdf/leave.html
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.954425 django-ipghrms-leave-1.8/leave/templatetags/
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:02.960661 django-ipghrms-leave-1.8/leave/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      483 2023-01-14 07:10:52.000000 django-ipghrms-leave-1.8/leave/templatetags/__pycache__/orderby.cpython-310.pyc
+-rw-rw-rw-   0        0        0      215 2023-01-14 07:10:49.000000 django-ipghrms-leave-1.8/leave/templatetags/orderby.py
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/tests.py
+-rw-rw-rw-   0        0        0     5470 2023-05-30 04:25:40.000000 django-ipghrms-leave-1.8/leave/urls.py
+-rw-rw-rw-   0        0        0     2788 2023-02-05 10:03:59.000000 django-ipghrms-leave-1.8/leave/urls_report.py
+-rw-rw-rw-   0        0        0    15575 2023-05-30 04:25:46.000000 django-ipghrms-leave-1.8/leave/utils.py
+-rw-rw-rw-   0        0        0     2737 2023-03-13 18:08:06.000000 django-ipghrms-leave-1.8/leave/utils_2.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:03.112156 django-ipghrms-leave-1.8/leave/views/
+-rw-rw-rw-   0        0        0      325 2023-01-29 14:29:10.000000 django-ipghrms-leave-1.8/leave/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 04:30:03.556970 django-ipghrms-leave-1.8/leave/views/__pycache__/
+-rw-rw-rw-   0        0        0      417 2023-01-29 14:29:14.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      370 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      378 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3566 2023-03-15 10:05:12.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2343 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2601 2023-01-29 07:19:53.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2460 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2469 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0      737 2023-01-23 14:19:18.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_chart.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2506 2023-03-15 10:08:49.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1993 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2279 2023-02-20 14:30:35.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1550 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1574 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0    25037 2023-03-13 19:37:38.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1813 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1814 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10718 2023-03-13 18:47:18.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2398 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2192 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11609 2023-03-13 18:27:21.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6368 2022-11-07 06:40:44.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6062 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0    17186 2023-02-15 01:07:16.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_report.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2026 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s.cpython-39.pyc
+-rw-rw-rw-   0        0        0      821 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0      819 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0      827 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4849 2023-03-15 14:22:55.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2143 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2161 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1279 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_staff.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3232 2023-03-13 18:30:54.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1961 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1926 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/leave_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1565 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/print.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1555 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/print.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1571 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/__pycache__/print.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4191 2023-03-15 10:04:22.000000 django-ipghrms-leave-1.8/leave/views/leave_c_m.py
+-rw-rw-rw-   0        0        0     2732 2023-01-29 07:19:51.000000 django-ipghrms-leave-1.8/leave/views/leave_c_v.py
+-rw-rw-rw-   0        0        0      527 2023-01-23 14:19:06.000000 django-ipghrms-leave-1.8/leave/views/leave_chart.py
+-rw-rw-rw-   0        0        0     2610 2023-03-15 10:08:46.000000 django-ipghrms-leave-1.8/leave/views/leave_de_m.py
+-rw-rw-rw-   0        0        0     2853 2023-02-20 14:30:30.000000 django-ipghrms-leave-1.8/leave/views/leave_de_v.py
+-rw-rw-rw-   0        0        0    73903 2023-06-05 04:21:56.000000 django-ipghrms-leave-1.8/leave/views/leave_hr_m.py
+-rw-rw-rw-   0        0        0    44603 2023-02-09 05:04:14.000000 django-ipghrms-leave-1.8/leave/views/leave_hr_m_back.py
+-rw-rw-rw-   0        0        0    16680 2023-03-13 18:47:16.000000 django-ipghrms-leave-1.8/leave/views/leave_hr_v.py
+-rw-rw-rw-   0        0        0    20552 2023-06-05 04:22:22.000000 django-ipghrms-leave-1.8/leave/views/leave_m.py
+-rw-rw-rw-   0        0        0    31199 2023-02-15 01:07:13.000000 django-ipghrms-leave-1.8/leave/views/leave_report.py
+-rw-rw-rw-   0        0        0      514 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/leave_s_m.py
+-rw-rw-rw-   0        0        0     5469 2023-06-05 04:22:52.000000 django-ipghrms-leave-1.8/leave/views/leave_s_v.py
+-rw-rw-rw-   0        0        0     3684 2023-03-13 18:30:52.000000 django-ipghrms-leave-1.8/leave/views/leave_v.py
+-rw-rw-rw-   0        0        0     1674 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views/print.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.8/leave/views.py
+-rw-rw-rw-   0        0        0      505 2023-06-05 04:30:03.580822 django-ipghrms-leave-1.8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-leave-1.8/setup.py
```

### Comparing `django-ipghrms-leave-1.7/LICENSE` & `django-ipghrms-leave-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/PKG-INFO` & `django-ipghrms-leave-1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-leave
-Version: 1.7
+Version: 1.8
 Summary: Django IPG HRMS APP LEAVE
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 
 
@@ -37,8 +36,7 @@
 
 3. Run ``python manage.py migrate`` to create leave model
 
 4. Another Apps Need for this Apps::
     4.1. custom::
     4.2. employee::
     4.3. user
-
```

### Comparing `django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/PKG-INFO` & `django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-leave
-Version: 1.7
+Version: 1.8
 Summary: Django IPG HRMS APP LEAVE
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 
 
@@ -37,8 +36,7 @@
 
 3. Run ``python manage.py migrate`` to create leave model
 
 4. Another Apps Need for this Apps::
     4.1. custom::
     4.2. employee::
     4.3. user
-
```

### Comparing `django-ipghrms-leave-1.7/django_ipghrms_leave.egg-info/SOURCES.txt` & `django-ipghrms-leave-1.8/django_ipghrms_leave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/admin.py` & `django-ipghrms-leave-1.8/leave/admin.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/api/__pycache__/urls.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/api/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/api/__pycache__/views.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/api/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/api/urls.py` & `django-ipghrms-leave-1.8/leave/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/api/views.py` & `django-ipghrms-leave-1.8/leave/api/views.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/forms.py` & `django-ipghrms-leave-1.8/leave/forms.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0001_initial.py` & `django-ipghrms-leave-1.8/leave/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0004_alter_leavedelegate_employee.py` & `django-ipghrms-leave-1.8/leave/migrations/0004_alter_leavedelegate_employee.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py` & `django-ipghrms-leave-1.8/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py` & `django-ipghrms-leave-1.8/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py` & `django-ipghrms-leave-1.8/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py` & `django-ipghrms-leave-1.8/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py` & `django-ipghrms-leave-1.8/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0014_leavehr_leavede.py` & `django-ipghrms-leave-1.8/leave/migrations/0014_leavehr_leavede.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py` & `django-ipghrms-leave-1.8/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py` & `django-ipghrms-leave-1.8/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0021_leave_is_approve_leave_is_reject.py` & `django-ipghrms-leave-1.8/leave/migrations/0021_leave_is_approve_leave_is_reject.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py` & `django-ipghrms-leave-1.8/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0025_auto_20221210_2329.py` & `django-ipghrms-leave-1.8/leave/migrations/0025_auto_20221210_2329.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0026_auto_20221210_2356.py` & `django-ipghrms-leave-1.8/leave/migrations/0026_auto_20221210_2356.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0028_auto_20221211_0202.py` & `django-ipghrms-leave-1.8/leave/migrations/0028_auto_20221211_0202.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0029_leavedep.py` & `django-ipghrms-leave-1.8/leave/migrations/0029_leavedep.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0030_auto_20221211_1206.py` & `django-ipghrms-leave-1.8/leave/migrations/0030_auto_20221211_1206.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0035_leave_file.py` & `django-ipghrms-leave-1.8/leave/migrations/0035_leave_file.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0045_auto_20221220_1722.py` & `django-ipghrms-leave-1.8/leave/migrations/0045_auto_20221220_1722.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0046_month_year.py` & `django-ipghrms-leave-1.8/leave/migrations/0046_month_year.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0047_auto_20221220_1729.py` & `django-ipghrms-leave-1.8/leave/migrations/0047_auto_20221220_1729.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0048_auto_20221221_1008.py` & `django-ipghrms-leave-1.8/leave/migrations/0048_auto_20221221_1008.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0049_auto_20221221_1009.py` & `django-ipghrms-leave-1.8/leave/migrations/0049_auto_20221221_1009.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0054_auto_20221225_2232.py` & `django-ipghrms-leave-1.8/leave/migrations/0054_auto_20221225_2232.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0056_auto_20221230_0221.py` & `django-ipghrms-leave-1.8/leave/migrations/0056_auto_20221230_0221.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0058_leaveperiod_employee.py` & `django-ipghrms-leave-1.8/leave/migrations/0058_leaveperiod_employee.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0059_auto_20230110_1535.py` & `django-ipghrms-leave-1.8/leave/migrations/0059_auto_20230110_1535.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0068_auto_20230202_0925.py` & `django-ipghrms-leave-1.8/leave/migrations/0068_auto_20230202_0925.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0071_auto_20230313_1908.py` & `django-ipghrms-leave-1.8/leave/migrations/0071_auto_20230313_1908.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0072_auto_20230313_2331.py` & `django-ipghrms-leave-1.8/leave/migrations/0072_auto_20230313_2331.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0073_auto_20230313_2338.py` & `django-ipghrms-leave-1.8/leave/migrations/0073_auto_20230313_2338.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/0074_auto_20230313_2341.py` & `django-ipghrms-leave-1.8/leave/migrations/0074_auto_20230313_2341.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0001_initial.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0001_initial.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/models.py` & `django-ipghrms-leave-1.8/leave/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 	employee = models.ForeignKey(Employee, on_delete=models.CASCADE, related_name='leaveperiod', null=True)
 	start_month = models.ForeignKey(Month, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Fulan Hahu", related_name="start_month")
 	start_year = models.ForeignKey(Year, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Tinan Hahu", related_name="start_year")
 	start_date = models.DateField(null=True, blank=True, verbose_name="Data Hahu")
 	end_date = models.DateField(null=True, blank=True, verbose_name="Data Remate")
 	end_month = models.ForeignKey(Month, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Fulan Remata", related_name="end_month")
 	end_year = models.ForeignKey(Year, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Tinan Remata", related_name="end_year")
-	balance_carry = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True, default=0.00, verbose_name="Balansu Carry Forward") # Balance Cary Forward
+	balance_carry = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True, default=0.00, verbose_name="Balansu Carry Forward") 
 	is_active = models.BooleanField(default=False)
 
 	def __str__(self):
-		return f'{self.employee} - {self.start_month} - {self.start_year} - {self.end_month} - {self.end_year}'
+		return f' {self.employee} - {self.start_month} - {self.start_year} - {self.end_month} - {self.end_year}'
 	
 
 class LeaveType(models.Model):
 	name = models.CharField(max_length=20, null=True, blank=True, verbose_name="Naran")
 	total = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True)
 	start_total = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True, verbose_name="Balance Start")
 	def __str__(self):
```

### Comparing `django-ipghrms-leave-1.7/leave/signals.py` & `django-ipghrms-leave-1.8/leave/signals.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/bal_s_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/bal_s_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/c_apply_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/c_apply_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/c_apply_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/c_apply_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/c_ver_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/c_ver_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/c_ver_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/c_ver_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/de_appr_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/de_appr_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/de_appr_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/de_appr_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/de_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/de_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/de_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/de_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/deleg_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/deleg_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/deleg_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/deleg_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/dep_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/dep_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/dep_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/dep_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/dep_req_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/dep_req_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/form.html` & `django-ipghrms-leave-1.8/leave/templates/leave/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/form2.html` & `django-ipghrms-leave-1.8/leave/templates/leave/form2.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_app_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_app_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_app_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_app_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_cert_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_cert_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_cert_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_cert_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_leave_record.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_leave_record.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_period_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_period_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/hr_raw_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/hr_raw_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/s_apply_detail.html` & `django-ipghrms-leave-1.8/leave/templates/leave/s_apply_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave/s_apply_list.html` & `django-ipghrms-leave-1.8/leave/templates/leave/s_apply_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/chart_leave.html` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/chart_leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/emp.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/emp.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type2.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type3.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type3.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_month.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_month.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_month_unit.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_month_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_tri.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_tri.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_unit.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_month.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_month.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_month_unit.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_month_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_tri.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_tri.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_tri_unit.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_tri_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_chart/type_year_unit.js` & `django-ipghrms-leave-1.8/leave/templates/leave_chart/type_year_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_print/layout.html` & `django-ipghrms-leave-1.8/leave/templates/leave_print/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_print/leave_print.html` & `django-ipghrms-leave-1.8/leave/templates/leave_print/leave_print.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_report/dash.html` & `django-ipghrms-leave-1.8/leave/templates/leave_report/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_report/list.html` & `django-ipghrms-leave-1.8/leave/templates/leave_report/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/leave_report/list_day.html` & `django-ipghrms-leave-1.8/leave/templates/leave_report/list_day.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/pdf/layout.html` & `django-ipghrms-leave-1.8/leave/templates/pdf/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/templates/pdf/leave.html` & `django-ipghrms-leave-1.8/leave/templates/pdf/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/urls.py` & `django-ipghrms-leave-1.8/leave/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/urls_report.py` & `django-ipghrms-leave-1.8/leave/urls_report.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/utils.py` & `django-ipghrms-leave-1.8/leave/utils.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/utils_2.py` & `django-ipghrms-leave-1.8/leave/utils_2.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_m.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_m.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_m.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_v.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_v.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_c_v.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_c_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_chart.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_chart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_m.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_m.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_m.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_v.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_v.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_de_v.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_de_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_m.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_m.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_m.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_v.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_v.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_hr_v.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_hr_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_m.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_m.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_m.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_report.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_m.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_m.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_m.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_v.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_v.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_s_v.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_s_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_staff.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_staff.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_v.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_v.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/leave_v.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/leave_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/print.cpython-310.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/print.cpython-37.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/print.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/__pycache__/print.cpython-39.pyc` & `django-ipghrms-leave-1.8/leave/views/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_c_m.py` & `django-ipghrms-leave-1.8/leave/views/leave_c_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_c_v.py` & `django-ipghrms-leave-1.8/leave/views/leave_c_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_chart.py` & `django-ipghrms-leave-1.8/leave/views/leave_chart.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_de_m.py` & `django-ipghrms-leave-1.8/leave/views/leave_de_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_de_v.py` & `django-ipghrms-leave-1.8/leave/views/leave_de_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_hr_m.py` & `django-ipghrms-leave-1.8/leave/views/leave_hr_m.py`

 * *Files 0% similar despite different names*

```diff
@@ -885,14 +885,15 @@
 			messages.success(request, f'Manda ona.')
 			return redirect('leave-hr-leave-record', c_emp.hashed)
 		else:
 			messages.error(request, "Funsionario Refere Laiha Chefe Ekipa no Chefe Divizaun, Halo favor kontakto Rekurso Humano")
 			return redirect('leave-hr-leave-record', c_emp.hashed)
 
 
+
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveUpdateRecord(request):
 	employee = Employee.objects.filter(status_id=1)
 	for emp in employee:
 		contract = Contract.objects.filter(employee=emp, is_active=True).exists()
 		if contract:
```

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_hr_m_back.py` & `django-ipghrms-leave-1.8/leave/views/leave_hr_m_back.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_hr_v.py` & `django-ipghrms-leave-1.8/leave/views/leave_hr_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_m.py` & `django-ipghrms-leave-1.8/leave/views/leave_m.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
 def LeaveSend(request, hashid):
 	group = request.user.groups.all()[0].name
 	objects = get_object_or_404(Leave, hashed=hashid)
 	c_emp = c_staff(request.user)
 	empdiv = CurEmpDivision.objects.get(employee=c_emp)
 	if group == "staff" or group == "hr":
 		check_ekipa = EmpPosition.objects.filter(Q(department__isnull=False)&Q(department=empdiv.department), is_active=True, is_manager=True).exists()
-		check_div = EmpPosition.objects.filter(Q(unit__isnull=False)&Q(unit=empdiv.unit), is_active=True, is_manager=True).exists()
+		check_div = EmpPosition.objects.filter(Q(unit__isnull=False)&Q(unit=empdiv.unit), is_active=True).exists()
 		if check_ekipa and check_div or check_ekipa:
 			objects.is_send =  True
 			objects.is_finish =  False
 			objects.save()
 			messages.success(request, f'Manda ona.')
 		elif check_div:
 			objects.is_send_to_div =  True
```

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_report.py` & `django-ipghrms-leave-1.8/leave/views/leave_report.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_s_m.py` & `django-ipghrms-leave-1.8/leave/views/leave_s_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_s_v.py` & `django-ipghrms-leave-1.8/leave/views/leave_s_v.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 	cgroup = leave.user.groups.all()[0].name
 	leavedep = LeaveDep.objects.filter(leave=leave).first()
 	leaveunit = LeaveUnit.objects.filter(leave=leave).first()
 	leavehr = LeaveHR.objects.filter(leave=leave).first()
 	leavede = LeaveDE.objects.filter(leave=leave).first()
 	ipginfo = IPGInfo.objects.filter(is_active=True).last()
 	response = HttpResponse(content_type='application/pdf')
+	signature = None
 	if leavede.user:
 		signature = EmpSignature.objects.filter(employee=leavede.user.employeeuser.employee).last()
 	if leaveunit.user:
 		signature = EmpSignature.objects.filter(employee=leaveunit.user.employeeuser.employee).last()
 
 	response['Content-Disposition'] = f'inline; filename="Leave_ON_{leave.start_date.day}_{leave.start_date.month}_{leave.start_date.year}.pdf"'
 	template = get_template('pdf/leave.html')
```

### Comparing `django-ipghrms-leave-1.7/leave/views/leave_v.py` & `django-ipghrms-leave-1.8/leave/views/leave_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.7/leave/views/print.py` & `django-ipghrms-leave-1.8/leave/views/print.py`

 * *Files identical despite different names*

