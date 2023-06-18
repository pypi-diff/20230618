# Comparing `tmp/okntool-4.1.0.tar.gz` & `tmp/okntool-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okntool-4.1.0.tar", last modified: Mon Jun  5 00:48:40 2023, max compression
+gzip compressed data, was "okntool-5.1.0.tar", last modified: Sun Jun 18 11:51:42 2023, max compression
```

## Comparing `okntool-4.1.0.tar` & `okntool-5.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 00:48:40.316515 okntool-4.1.0/
--rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.1.0/LICENSE
--rw-rw-rw-   0        0        0      555 2023-06-05 00:48:40.315518 okntool-4.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4138 2023-06-01 23:23:02.000000 okntool-4.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 00:48:40.307560 okntool-4.1.0/okntool/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.1.0/okntool/__init__.py
--rw-rw-rw-   0        0        0     1257 2023-06-02 03:16:07.000000 okntool-4.1.0/okntool/indi_va_table_template.html
--rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.1.0/okntool/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0   108619 2023-06-05 00:42:34.000000 okntool-4.1.0/okntool/okntool.py
--rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.1.0/okntool/simpler_plot_config.json
--rw-rw-rw-   0        0        0     1889 2023-06-04 23:07:46.000000 okntool-4.1.0/okntool/sum_va_table_template.html
-drwxrwxrwx   0        0        0        0 2023-06-05 00:48:40.315518 okntool-4.1.0/okntool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 00:48:22.000000 okntool-4.1.0/okntool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 00:48:40.000000 okntool-4.1.0/okntool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 00:48:40.316515 okntool-4.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1239 2023-06-05 00:00:56.000000 okntool-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:51:42.789047 okntool-5.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-5.1.0/LICENSE
+-rw-rw-rw-   0        0        0      555 2023-06-18 11:51:42.789047 okntool-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4138 2023-06-01 23:23:02.000000 okntool-5.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 11:51:42.780492 okntool-5.1.0/okntool/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-5.1.0/okntool/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-06-07 23:25:14.000000 okntool-5.1.0/okntool/indi_va_table_template.html
+-rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-5.1.0/okntool/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0   129036 2023-06-18 11:51:27.000000 okntool-5.1.0/okntool/okntool.py
+-rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-5.1.0/okntool/simpler_plot_config.json
+-rw-rw-rw-   0        0        0     2379 2023-06-18 11:04:19.000000 okntool-5.1.0/okntool/sum_va_table_template.html
+drwxrwxrwx   0        0        0        0 2023-06-18 11:51:42.787474 okntool-5.1.0/okntool.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-06-18 11:51:42.000000 okntool-5.1.0/okntool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-18 11:51:42.000000 okntool-5.1.0/okntool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:51:42.000000 okntool-5.1.0/okntool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-18 11:51:42.000000 okntool-5.1.0/okntool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 11:51:31.000000 okntool-5.1.0/okntool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-06-18 11:51:42.000000 okntool-5.1.0/okntool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 11:51:42.000000 okntool-5.1.0/okntool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:51:42.789047 okntool-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-06-18 11:51:27.000000 okntool-5.1.0/setup.py
```

### Comparing `okntool-4.1.0/LICENSE` & `okntool-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okntool-4.1.0/PKG-INFO` & `okntool-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.1.0
+Version: 5.1.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.1.0/README.md` & `okntool-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `okntool-4.1.0/okntool/oknserver_graph_plot_config.json` & `okntool-5.1.0/okntool/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.1.0/okntool/okntool.py` & `okntool-5.1.0/okntool/okntool.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import sys
 import argparse
 import json
 import csv
 import numpy as np
 import matplotlib.pyplot as plt
 import os
-import importlib.resources as config_resources
+import importlib.resources as okntool_resources
 from matplotlib.lines import Line2D
+import chevron
 
 logmar_level_array = [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0, -0.1, -0.2,
                       "no logMAR", "right_down", "right_up", "left_down", "left_up"]
 
 
 # This function is to get header position from the given array
 def get_index(search_input, array_in):
@@ -1451,22 +1452,22 @@
                 # event_marker_time_f = float(event_marker_sts - start_marker)
                 # print(event_marker_time_f - event_marker_time_i)
                 event_marker_array.append(float(event_marker_sts - start_marker))
 
     return event_marker_array
 
 
-def get_config_location(config_name_input):
-    config_exist = config_resources.is_resource("okntool", config_name_input)
-    if config_exist:
-        with config_resources.path("okntool", config_name_input) as p:
-            config_location = p
+def get_resource_file_location(file_name_input):
+    resource_file_exist = okntool_resources.is_resource("okntool", file_name_input)
+    if resource_file_exist:
+        with okntool_resources.path("okntool", file_name_input) as p:
+            resource_file_location = p
     else:
-        config_location = None
-    return config_location
+        resource_file_location = None
+    return resource_file_location
 
 
 def draw_simpler_graph(folder_dir_input, config_input, referenced_csv_to_be_used, output_file_dir_input=None):
     graph_line_color = config_input["graph_line_color"]
     graph_line_thickness = config_input["graph_line_thickness"]
     x_label = config_input["x_label"]
     x_label_x_position = config_input["x_label_x_position"]
@@ -1796,44 +1797,408 @@
         folder_name = raw_file_name[raw_file_name.find("./") + 2:raw_file_name.find(".mp4")]
         trial_id = folder_name[folder_name.find("trial-"):folder_name.find("-disks")]
         output_array.append([trial_id, logmar_level, folder_name])
 
     return output_array
 
 
-def check_image_file_name(file_name_input, ending_array_input):
+def check_file_name(file_name_input, ending_array_input):
     return True if any([end in file_name_input for end in ending_array_input]) else False
 
 
+def create_indi_va_table_html(dir_input, referenced_csv, template_input,
+                              decider_name_input, output_file_dir_input=None):
+    if output_file_dir_input:
+        csv_dir = os.path.join(output_file_dir_input, "indi_va_table.csv")
+        html_dir = os.path.join(output_file_dir_input, "indi_va_table.html")
+    else:
+        csv_dir = os.path.join(dir_input, "indi_va_table.csv")
+        html_dir = os.path.join(dir_input, "indi_va_table.html")
+    read_folder_and_create_indi_csv_data(dir_input, referenced_csv, csv_dir, decider_name_input)
+    read_csv_data_and_create_indi_va_table_html(csv_dir, template_input, html_dir)
+
+
+def read_folder_and_create_indi_csv_data(dir_input, referenced_csv, csv_dir, decider_name_input):
+    info_array = get_info_array_for_ind_va_table(dir_input, referenced_csv, "logMAR", "filename", decider_name_input)
+    logmar_level = None
+    index = 1
+    okn_index_array = []
+    temp_dict = {}
+    total_count = 0
+
+    for info_index, info in enumerate(info_array):
+        if logmar_level != info["logmar_level"]:
+            logmar_level = info["logmar_level"]
+            if index == 1:
+                trial_string = f"trial_{index}"
+                temp_dict["logMAR"] = logmar_level
+                okn_result = info["okn"]
+                if okn_result == 1:
+                    total_count += 1
+                temp_dict[trial_string] = okn_result
+            else:
+                temp_dict["total"] = total_count
+                okn_index_array.append(temp_dict)
+                temp_dict = {}
+                index = 1
+                total_count = 0
+                trial_string = f"trial_{index}"
+                temp_dict["logMAR"] = logmar_level
+                okn_result = info["okn"]
+                if okn_result == 1:
+                    total_count += 1
+                temp_dict[trial_string] = okn_result
+        else:
+            index += 1
+            trial_string = f"trial_{index}"
+            okn_result = info["okn"]
+            if okn_result == 1:
+                total_count += 1
+            temp_dict[trial_string] = okn_result
+            if info_index == len(info_array) - 1:
+                temp_dict["total"] = total_count
+                okn_index_array.append(temp_dict)
+
+    header_array = ["logMAR", "trial_1", "trial_2", "trial_3", "trial_4", "trial_5", "total"]
+    with open(csv_dir, mode='w', newline="") as destination_file:
+        csv_writer = csv.DictWriter(destination_file, fieldnames=header_array)
+        csv_writer.writeheader()
+
+        for d in okn_index_array:
+            csv_writer.writerow(d)
+        print(f"Individual va table csv is successfully created in {csv_dir}")
+        destination_file.close()
+
+
+def read_csv_data_and_create_indi_va_table_html(csv_dir_input, template_html_input, output_file_dir_input):
+    if os.path.isfile(csv_dir_input):
+        file_to_open = open(csv_dir_input)
+        csv_reader = csv.reader(file_to_open)
+        header_array = []
+        rows = []
+        count_one = 0
+
+        for row in csv_reader:
+            if count_one <= 0:
+                header_array = row
+                count_one += 1
+            else:
+                rows.append(row)
+
+        logmar_position = get_index("logMAR", header_array)
+        trial_one_position = get_index("trial_1", header_array)
+        trial_two_position = get_index("trial_2", header_array)
+        trial_three_position = get_index("trial_3", header_array)
+        trial_four_position = get_index("trial_4", header_array)
+        trial_five_position = get_index("trial_5", header_array)
+        total_position = get_index("total", header_array)
+
+        total_okn = 0
+        data_array = []
+        for row in rows:
+            temp_dict = {}
+            logmar_level = row[logmar_position]
+            temp_dict["logMAR"] = logmar_level
+            trial_one = row[trial_one_position]
+            if trial_one == 1:
+                total_okn += 1
+                temp_dict["trial_1_unicode"] = "&#x2713;"
+            else:
+                temp_dict["trial_1_unicode"] = "&#x0058;"
+            trial_two = int(row[trial_two_position])
+            if trial_two == 1:
+                total_okn += 1
+                temp_dict["trial_2_unicode"] = "&#x2713;"
+            else:
+                temp_dict["trial_2_unicode"] = "&#x0058;"
+            trial_three = int(row[trial_three_position])
+            if trial_three == 1:
+                total_okn += 1
+                temp_dict["trial_3_unicode"] = "&#x2713;"
+            else:
+                temp_dict["trial_3_unicode"] = "&#x0058;"
+            trial_four = int(row[trial_four_position])
+            if trial_four == 1:
+                total_okn += 1
+                temp_dict["trial_4_unicode"] = "&#x2713;"
+            else:
+                temp_dict["trial_4_unicode"] = "&#x0058;"
+            trial_five = int(row[trial_five_position])
+            if trial_five == 1:
+                total_okn += 1
+                temp_dict["trial_5_unicode"] = "&#x2713;"
+            else:
+                temp_dict["trial_5_unicode"] = "&#x0058;"
+            total = row[total_position]
+            temp_dict["Total"] = total
+            data_array.append(temp_dict)
+
+        final_va = round(1.1 - (total_okn * 0.02), 2)
+        okn_index_data = {"data": data_array, "letter_score": total_okn, "va": {"VA": final_va, "bestline_VA": None}}
+
+        with open(template_html_input, 'r') as template:
+            html_data = chevron.render(template, okn_index_data)
+
+        with open(output_file_dir_input, 'w') as output_html_file:
+            output_html_file.write(html_data)
+            print(f"Individual va table html is successfully created in {output_file_dir_input}")
+
+        template.close()
+        output_html_file.close()
+    else:
+        print(f"Individual va table csv could not be found in {csv_dir_input}.")
+
+
+def get_info_array_for_ind_va_table(dir_input, referenced_csv_dir, logmar_header_input,
+                                    file_name_header_input, decider_name_input):
+    file_to_open = open(referenced_csv_dir)
+    csv_reader = csv.reader(file_to_open)
+    header_array = []
+    rows = []
+    count_one = 0
+    output_array = []
+
+    for row in csv_reader:
+        if count_one <= 0:
+            header_array = row
+            count_one += 1
+        else:
+            rows.append(row)
+
+    file_name_header_position = get_index(file_name_header_input, header_array)
+    logmar_header_position = get_index(logmar_header_input, header_array)
+
+    for row in rows:
+        raw_file_name = str(row[file_name_header_position])
+        logmar_level = float(row[logmar_header_position])
+        folder_name = raw_file_name[raw_file_name.find("./") + 2:raw_file_name.find(".mp4")]
+        trial_id = folder_name[folder_name.find("trial-"):folder_name.find("-disks")]
+        is_there_okn = get_okn_result_from_signal_file(dir_input, folder_name, decider_name_input)
+        if is_there_okn is not None:
+            temp_dict = {"trial_id": trial_id, "logmar_level": logmar_level, "folder_name": folder_name,
+                         "okn": is_there_okn}
+            output_array.append(temp_dict)
+
+    return output_array
+
+
+def get_okn_result_from_signal_file(dir_input, folder_name_input, decider_file_name_input):
+    decider_file_dir = os.path.join(dir_input, folder_name_input, decider_file_name_input)
+    try:
+        # Opening oknserver graph plot config
+        with open(decider_file_dir) as f:
+            info = json.load(f)
+    except FileNotFoundError:
+        print(f"There is no {decider_file_name_input} in {decider_file_dir}")
+        info = None
+
+    if info:
+        is_there_okn = info["okn_present"]
+        if is_there_okn is True:
+            return 1
+        else:
+            return 0
+    else:
+        return None
+
+
+def create_sum_va_table_html(dir_input, template_input, output_file_dir_input=None):
+    if output_file_dir_input:
+        csv_dir = os.path.join(output_file_dir_input, "sum_va_table.csv")
+        html_dir = os.path.join(output_file_dir_input, "sum_va_table.html")
+    else:
+        csv_dir = os.path.join(dir_input, "sum_va_table.csv")
+        html_dir = os.path.join(dir_input, "sum_va_table.html")
+    read_folder_and_create_sum_csv_data(dir_input, csv_dir)
+    read_csv_data_and_create_sum_va_table_html(csv_dir, template_input, html_dir)
+
+
+def read_folder_and_create_sum_csv_data(dir_input, output_dir):
+    folder_array = [name for name in os.listdir(dir_input) if os.path.isdir(os.path.join(dir_input, name))]
+    info_array = []
+    for name in folder_array:
+        indi_csv_dir = os.path.join(dir_input, name, "indi_va_table.csv")
+        file_to_open = open(indi_csv_dir)
+        csv_reader = csv.reader(file_to_open)
+        header_array = []
+        rows = []
+        count_one = 0
+        total = 0
+        temp_dict = {}
+        temp_dict["folder"] = name
+
+        for row in csv_reader:
+            if count_one <= 0:
+                header_array = row
+                count_one += 1
+            else:
+                rows.append(row)
+
+        logmar_position = get_index("logMAR", header_array)
+        total_position = get_index("total", header_array)
+
+        for row in rows:
+            logmar_level = row[logmar_position]
+            if float(logmar_level) == 1.0:
+                logmar_level = 1
+            elif float(logmar_level) == 0.0:
+                logmar_level = 0
+            else:
+                logmar_level = str(logmar_level).replace(".", "_")
+            logmar_string = f"log_{logmar_level}"
+            logmar_total = int(row[total_position])
+            total += logmar_total
+            temp_dict[logmar_string] = logmar_total
+        temp_dict["Total"] = total
+        info_array.append(temp_dict)
+
+    csv_header_array = ["folder", "log_1", "log_0_9", "log_0_8", "log_0_7", "log_0_6",
+                        "log_0_5", "log_0_4", "log_0_3", "log_0_2", "log_0_1", "log_0", "Total"]
+    with open(output_dir, mode='w', newline="") as destination_file:
+        csv_writer = csv.DictWriter(destination_file, fieldnames=csv_header_array)
+        csv_writer.writeheader()
+
+        for info in info_array:
+            csv_writer.writerow(info)
+        print(f"Summary va table csv is successfully created in {output_dir}")
+        destination_file.close()
+
+
+def read_csv_data_and_create_sum_va_table_html(csv_dir_input, template_html_input, output_dir):
+    if os.path.isfile(csv_dir_input):
+        file_to_open = open(csv_dir_input)
+        csv_reader = csv.reader(file_to_open)
+        header_array = []
+        rows = []
+        count_one = 0
+
+        for row in csv_reader:
+            if count_one <= 0:
+                header_array = row
+                count_one += 1
+            else:
+                rows.append(row)
+
+        folder_name_position = get_index("folder", header_array)
+        log_1_position = get_index("log_1", header_array)
+        log_0_9_position = get_index("log_0_9", header_array)
+        log_0_8_position = get_index("log_0_8", header_array)
+        log_0_7_position = get_index("log_0_7", header_array)
+        log_0_6_position = get_index("log_0_6", header_array)
+        log_0_5_position = get_index("log_0_5", header_array)
+        log_0_4_position = get_index("log_0_4", header_array)
+        log_0_3_position = get_index("log_0_3", header_array)
+        log_0_2_position = get_index("log_0_2", header_array)
+        log_0_1_position = get_index("log_0_1", header_array)
+        log_0_position = get_index("log_0", header_array)
+        total_position = get_index("Total", header_array)
+
+        log_1_okn = 0
+        log_0_9_okn = 0
+        log_0_8_okn = 0
+        log_0_7_okn = 0
+        log_0_6_okn = 0
+        log_0_5_okn = 0
+        log_0_4_okn = 0
+        log_0_3_okn = 0
+        log_0_2_okn = 0
+        log_0_1_okn = 0
+        log_0_okn = 0
+
+        data_array = []
+        for row in rows:
+            temp_dict = {}
+            temp_dict["folder"] = row[folder_name_position]
+            temp_dict["log_1"] = row[log_1_position]
+            temp_dict["log_0_9"] = row[log_0_9_position]
+            temp_dict["log_0_8"] = row[log_0_8_position]
+            temp_dict["log_0_7"] = row[log_0_7_position]
+            temp_dict["log_0_6"] = row[log_0_6_position]
+            temp_dict["log_0_5"] = row[log_0_5_position]
+            temp_dict["log_0_4"] = row[log_0_4_position]
+            temp_dict["log_0_3"] = row[log_0_3_position]
+            temp_dict["log_0_2"] = row[log_0_2_position]
+            temp_dict["log_0_1"] = row[log_0_1_position]
+            temp_dict["log_0"] = row[log_0_position]
+            temp_dict["Total"] = row[total_position]
+            data_array.append(temp_dict)
+            log_1_okn += int(row[log_1_position])
+            log_0_9_okn += int(row[log_0_9_position])
+            log_0_8_okn += int(row[log_0_8_position])
+            log_0_7_okn += int(row[log_0_7_position])
+            log_0_6_okn += int(row[log_0_6_position])
+            log_0_5_okn += int(row[log_0_5_position])
+            log_0_4_okn += int(row[log_0_4_position])
+            log_0_3_okn += int(row[log_0_3_position])
+            log_0_2_okn += int(row[log_0_2_position])
+            log_0_1_okn += int(row[log_0_1_position])
+            log_0_okn += int(row[log_0_position])
+
+        total_dict = {
+            "total_1": log_1_okn,
+            "total_0_9": log_0_9_okn,
+            "total_0_8": log_0_8_okn,
+            "total_0_7": log_0_7_okn,
+            "total_0_6": log_0_6_okn,
+            "total_0_5": log_0_5_okn,
+            "total_0_4": log_0_4_okn,
+            "total_0_3": log_0_3_okn,
+            "total_0_2": log_0_2_okn,
+            "total_0_1": log_0_1_okn,
+            "total_0": log_0_okn,
+        }
+        okn_index_data = {"data": data_array, "total": total_dict}
+
+        with open(template_html_input, 'r') as template:
+            html_data = chevron.render(template, okn_index_data)
+
+        with open(output_dir, 'w') as output_html_file:
+            output_html_file.write(html_data)
+            print(f"Individual va table html is successfully created in {output_dir}")
+
+        template.close()
+        output_html_file.close()
+    else:
+        print(f"Summary va table csv could not be found in {csv_dir_input}.")
+
+
 def main():
     parser = argparse.ArgumentParser(prog='okntool',
                                      description='okn related graphs plotting program.')
-    parser.add_argument('--version', action='version', version='4.1.0'),
+    parser.add_argument('--version', action='version', version='5.1.0'),
     parser.add_argument("-t", dest="plot_type", required=True, default=sys.stdin,
                         help="trial, summary, (staircase or progress), tidy or simpler", metavar="plot type")
     parser.add_argument("-d", dest="directory_input", required=True, default=sys.stdin,
                         help="directory folder to be processed", metavar="directory")
     parser.add_argument("-c", dest="config_dir", required=False, default=sys.stdin,
-                        help="config file to be used", metavar="config location")
+                        help="config or resource file", metavar="config location")
     parser.add_argument("-r", dest="referenced_csv", required=False, default=sys.stdin,
                         help="referenced csv file to be referenced", metavar="referenced csv")
     parser.add_argument("-o", dest="output", required=False, default=sys.stdin,
-                        help="output directory and file name", metavar="output")
+                        help="output folder or file directory", metavar="output")
+    parser.add_argument("-p", dest="template", required=False, default=sys.stdin,
+                        help="template file location or file name", metavar="template")
+    parser.add_argument("-n", dest="decider_name", required=False, default=sys.stdin,
+                        help="decider name for each sub folder", metavar="decider name")
 
     args = parser.parse_args()
     directory_input = str(args.directory_input)
     type_input = str(args.plot_type)
     config_file_location = str(args.config_dir)
     referenced_csv_dir = str(args.referenced_csv)
     output_dir = str(args.output)
-    config_dir_exist = False
+    template_dir = str(args.template)
+    decider_name = str(args.decider_name)
     config_input = False if "_io.TextIOWrapper" in config_file_location else True
     referenced_csv_input = False if "_io.TextIOWrapper" in referenced_csv_dir else True
     output_dir_input = False if "_io.TextIOWrapper" in output_dir else True
+    template_dir_input = False if "_io.TextIOWrapper" in template_dir else True
+    decider_name_input = False if "_io.TextIOWrapper" in decider_name else True
     image_file_ending_array = ['.png', '.jpg', '.jpeg', '.tiff', '.bmp', '.gif']
+    va_table_related_file_ending_array = ['.csv', '.html']
     output_file_name = None
     if output_dir_input:
         output_folder = os.path.join(output_dir, os.pardir)
         output_folder_exist = os.path.isdir(output_folder)
         if output_folder_exist:
             output_file_name = os.path.basename(output_dir)
     else:
@@ -1843,145 +2208,156 @@
     # config_name_dict["summary"] = "oknserver_graph_plot_config.json"
     # config_name_dict["staircase"] = "oknserver_graph_plot_config.json"
     # config_name_dict["progress"] = "oknserver_graph_plot_config.json"
     # config_name_dict["tidy"] = "oknserver_graph_plot_config.json"
     # config_name_dict["simpler"] = "simpler_plot_config.json"
 
     # Dictionary to retrieve the name of config file according the type
-    config_name_dict = {"trial": "oknserver_graph_plot_config.json", "summary": "oknserver_graph_plot_config.json",
-                        "staircase": "oknserver_graph_plot_config.json", "progress": "oknserver_graph_plot_config.json",
-                        "tidy": "oknserver_graph_plot_config.json", "simpler": "simpler_plot_config.json"}
+    resource_name_dict = {"trial": "oknserver_graph_plot_config.json",
+                          "summary": "oknserver_graph_plot_config.json",
+                          "staircase": "oknserver_graph_plot_config.json",
+                          "progress": "oknserver_graph_plot_config.json",
+                          "tidy": "oknserver_graph_plot_config.json",
+                          "simpler": "simpler_plot_config.json",
+                          "indi_va_table": "indi_va_table_template.html",
+                          "sum_va_table": "sum_va_table_template.html"}
 
-    config_name = config_name_dict[type_input]
+    resource_name = resource_name_dict[type_input]
 
     # print(config_file_location)
-    if not config_input:
-        print("There is no config input.")
-        config_location = get_config_location(config_name)
-        if config_location:
-            print(f"Therefore, okntool is using built-in config: {config_location}.")
-            config_dir_exist = True
+    if config_input:
+        resource_dir_exist = os.path.isfile(config_file_location)
+        if resource_dir_exist:
+            resource_location = config_file_location
+            print(f"Config/resource location input:{resource_location} is valid.")
         else:
-            print(f"Error in retrieving config:{config_location}.")
+            resource_location = None
+            print(f"Config/resource location input:{config_file_location} does not exist.")
             return
     else:
-        config_dir_exist = os.path.isfile(config_file_location)
-        if not config_dir_exist:
-            print(f"Config location input:{config_file_location} does not exist.")
-            return
+        print("There is no config input.")
+        resource_location = get_resource_file_location(resource_name)
+        if resource_location:
+            print(f"Therefore, okntool is using built-in config: {resource_location}.")
+            resource_dir_exist = True
         else:
-            config_location = config_file_location
-            print(f"Config location input:{directory_input} is valid.")
+            print(f"Error in retrieving config:{resource_location}.")
+            return
 
     print("------------------")
     print(f"OKN TOOL PLOT INFO")
     print(f"Input directory:{directory_input}")
     print(f"Plot type:{type_input}")
-    print(f"Config: {config_location}")
+    print(f"Config/resource: {resource_location}")
 
     # check whether input directory exists or not
     dir_exist = os.path.isdir(directory_input)
     if not dir_exist:
         print(f"Directory input:{directory_input} does not exist.")
         print(f"Therefore, okntool could not process {type_input}")
         return
     else:
         print(f"Directory input:{directory_input} is valid.")
 
-    if config_dir_exist and dir_exist:
-        try:
-            # Opening oknserver graph plot config
-            with open(config_location) as f:
-                plot_config_info = json.load(f)
-        except FileNotFoundError:
-            plot_config_info = None
-        if plot_config_info is not None:
-            print(f"{config_name} is found.")
-        else:
-            print(f"Essential config file:{config_name} is missing.")
+    type_does_not_need_config = ["indi_va_table", "sum_va_table"]
+
+    if type_input in type_does_not_need_config:
+        plot_config_info = {"config_need": False}
     else:
-        plot_config_info = None
+        if resource_dir_exist and dir_exist:
+            try:
+                # Opening oknserver graph plot config
+                with open(resource_location) as f:
+                    plot_config_info = json.load(f)
+            except FileNotFoundError:
+                plot_config_info = None
+            if plot_config_info is not None:
+                print(f"{resource_name} is found.")
+            else:
+                print(f"Essential config file:{resource_name} is missing.")
+        else:
+            plot_config_info = None
 
     if output_dir_input:
         if output_folder_exist:
             print("Output file location input is found and output folder exists.")
         else:
             print("Output file location input is found but output folder does not exist.")
             print("Therefore, default output location will be used.")
     else:
         print("There is no output file location input.")
         print("Therefore, default output location will be used.")
 
-    if config_dir_exist and dir_exist and plot_config_info is not None:
+    if resource_dir_exist and dir_exist and plot_config_info is not None:
         if type_input == "trial":
             # Retrieve trial plot info from config
             trial_plot_info = plot_config_info["trial_plot"]
 
             csv_name = f"updated_{os.path.basename(directory_input)}.csv"
             print(f"csv name {csv_name}")
             updated_csv_dir = os.path.join(directory_input, csv_name)
             print(f"update csv dir {updated_csv_dir}")
             signal_csv_folder_name = trial_plot_info["signal_csv_folder_name"]
             signal_csv_name = trial_plot_info["signal_csv_name"]
             signal_csv_dir = os.path.join(directory_input, signal_csv_folder_name, signal_csv_name)
             print(f"signal csv dir {signal_csv_dir}")
             if output_folder_exist:
-                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                file_name_valid = check_file_name(output_file_name, image_file_ending_array)
                 if file_name_valid:
                     draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir, output_dir)
                 else:
                     print("Invalid image file name")
                     return
             else:
                 draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir)
         elif type_input == "summary":
             # Retrieve summary plot info from config
             summary_plot_info = plot_config_info["summary_plot"]
 
             if output_folder_exist:
-                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                file_name_valid = check_file_name(output_file_name, image_file_ending_array)
                 if file_name_valid:
                     plot_combined_graph(directory_input, summary_plot_info, output_dir)
                 else:
                     print("Invalid image file name")
                     return
             else:
                 plot_combined_graph(directory_input, summary_plot_info)
         elif type_input == "staircase" or type_input == "progress":
             # Retrieve progress plot info from config
             progress_plot_info = plot_config_info["progress_plot"]
 
             if output_folder_exist:
-                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                file_name_valid = check_file_name(output_file_name, image_file_ending_array)
                 if file_name_valid:
                     draw_progress_graph(directory_input, progress_plot_info, output_dir)
                 else:
                     print("Invalid image file name")
                     return
             else:
                 draw_progress_graph(directory_input, progress_plot_info)
         elif type_input == "tidy":
             # Retrieve progress plot info from config
             tidy_plot_info = plot_config_info["tidy_plot"]
 
             if output_folder_exist:
-                file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                file_name_valid = check_file_name(output_file_name, image_file_ending_array)
                 if file_name_valid:
                     draw_tidy_graph(directory_input, tidy_plot_info, output_dir)
                 else:
                     print("Invalid image file name")
                     return
             else:
                 draw_tidy_graph(directory_input, tidy_plot_info)
         elif type_input == "simpler":
             # Retrieve simpler plot info from config
             simpler_plot_info = plot_config_info["simpler_plot"]
             if referenced_csv_input:
                 if output_folder_exist:
-                    file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                    file_name_valid = check_file_name(output_file_name, image_file_ending_array)
                     if file_name_valid:
                         draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir, output_dir)
                     else:
                         print("Invalid image file name")
                         return
                 else:
                     draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
@@ -1998,21 +2374,100 @@
                 two_folder_back_dir = os.path.abspath(os.path.join(one_folder_back_dir, os.pardir))
                 referenced_csv_dir = os.path.join(two_folder_back_dir, referenced_csv_name)
                 referenced_csv_dir_exist = os.path.isfile(referenced_csv_dir)
                 if referenced_csv_dir_exist:
                     print(f"Default referenced csv location:{referenced_csv_dir} is found.")
                     print("Start plotting simpler plot...")
                     if output_folder_exist:
-                        file_name_valid = check_image_file_name(output_file_name, image_file_ending_array)
+                        file_name_valid = check_file_name(output_file_name, image_file_ending_array)
                         if file_name_valid:
                             draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir, output_dir)
                         else:
                             print("Invalid image file name")
                             return
                     else:
                         draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
                 else:
                     print(f"Default referenced csv location:{referenced_csv_dir} cannot be found.")
+        elif type_input == "indi_va_table":
+            if template_dir_input:
+                if os.path.isfile(template_dir):
+                    print(f"Template file:{template_dir} is found.")
+                else:
+                    print(f"Template file:{template_dir} could not be found.")
+            else:
+                print("There is no template file input.")
+                print("Therefore, retrieving default template file.")
+                template_dir = get_resource_file_location("indi_va_table_template.html")
+                if template_dir:
+                    print("Retrieving template file is successful.")
+                else:
+                    print("Error in retrieving template file.")
+                    return
+            if decider_name_input:
+                print(f"Decider file name input:{decider_name} is found.")
+            else:
+                decider_name = "decider.json"
+                print("There is no decide file name input.")
+                print(f"Therefore, using default decide file name:{decider_name}")
+            if referenced_csv_input:
+                if output_dir_input:
+                    if os.path.isdir(output_dir):
+                        create_indi_va_table_html(directory_input, referenced_csv_dir,
+                                                  template_dir, decider_name, output_dir)
+                    else:
+                        print("Output location input must be directory for \"va_table\" type.")
+                        print("Not file directory")
+                        return
+                else:
+                    create_indi_va_table_html(directory_input, referenced_csv_dir, template_dir, decider_name)
+            else:
+                print("There is no referenced csv input in the commandline.")
+                referenced_csv_name = "protocol.simpler.csv"
+                print(f"Therefore using default name => {referenced_csv_name} as default referenced csv")
+                # os.path.abspath(os.path.join(directory_input, os.pardir)) == retrieve the parent path
+                one_folder_back_dir = os.path.abspath(os.path.join(directory_input, os.pardir))
+                two_folder_back_dir = os.path.abspath(os.path.join(one_folder_back_dir, os.pardir))
+                referenced_csv_dir = os.path.join(two_folder_back_dir, referenced_csv_name)
+                referenced_csv_dir_exist = os.path.isfile(referenced_csv_dir)
+                if referenced_csv_dir_exist:
+                    print(f"Default referenced csv location:{referenced_csv_dir} is found.")
+                    if output_dir_input:
+                        if os.path.isdir(output_dir):
+                            create_indi_va_table_html(directory_input, referenced_csv_dir,
+                                                      template_dir, decider_name, output_dir)
+                        else:
+                            print("Output location input must be directory for \"va_table\" type.")
+                            print("Not file directory")
+                            return
+                    else:
+                        create_indi_va_table_html(directory_input, referenced_csv_dir, template_dir, decider_name)
+                else:
+                    print(f"Default referenced csv location:{referenced_csv_dir} cannot be found.")
+        elif type_input == "sum_va_table":
+            if template_dir_input:
+                if os.path.isfile(template_dir):
+                    print(f"Template file:{template_dir} is found.")
+                else:
+                    print(f"Template file:{template_dir} could not be found.")
+            else:
+                print("There is no template file input.")
+                print("Therefore, retrieving default template file.")
+                template_dir = get_resource_file_location("sum_va_table_template.html")
+                if template_dir:
+                    print("Retrieving template file is successful.")
+                else:
+                    print("Error in retrieving template file.")
+                    return
+            if output_dir_input:
+                if os.path.isdir(output_dir):
+                    create_sum_va_table_html(directory_input, template_dir, output_dir)
+                else:
+                    print("Output location input must be directory for \"va_table\" type.")
+                    print("Not file directory")
+                    return
+            else:
+                create_sum_va_table_html(directory_input, template_dir)
         else:
             print("wrong plot type or invalid plot type.")
     else:
         return
```

### Comparing `okntool-4.1.0/okntool/simpler_plot_config.json` & `okntool-5.1.0/okntool/simpler_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.1.0/okntool.egg-info/PKG-INFO` & `okntool-5.1.0/okntool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.1.0
+Version: 5.1.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.1.0/setup.py` & `okntool-5.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw okn related graphs.'
 
 setup(
     name='okntool',
-    version='4.1.0',
+    version='5.1.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/okntool',
     description='OKN related graphs drawing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

