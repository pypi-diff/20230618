# Comparing `tmp/disaster_id_scan-0.2.0.tar.gz` & `tmp/disaster_id_scan-0.3.0.tar.gz`

## Comparing `disaster_id_scan-0.2.0.tar` & `disaster_id_scan-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/__main__.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/id_scanner.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/mrz.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/store.py
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/ui.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/src/disaster_id_scan/cli/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/.gitignore
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/README.md
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 disaster_id_scan-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/__init__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/__main__.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/id_scanner.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/mrz.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/store.py
+-rw-r--r--   0        0        0    16795 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/ui.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/src/disaster_id_scan/cli/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/.gitignore
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/README.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 disaster_id_scan-0.3.0/PKG-INFO
```

### Comparing `disaster_id_scan-0.2.0/.github/workflows/pypi-publish.yml` & `disaster_id_scan-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.2.0/src/disaster_id_scan/id_scanner.py` & `disaster_id_scan-0.3.0/src/disaster_id_scan/id_scanner.py`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.2.0/src/disaster_id_scan/store.py` & `disaster_id_scan-0.3.0/src/disaster_id_scan/store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: 2023-present anjomro <py@anjomro.de>
 #
 # SPDX-License-Identifier: EUPL-1.2
+from csv import DictWriter
 from datetime import date, datetime
 from pathlib import Path
 
 import jsonpickle
 
 
 class Person:
@@ -37,39 +38,90 @@
 
     def __str__(self):
         return f"""-- Person --
 Name: {self.last_name}
 First Name: {self.first_name}
 Date of Birth: {self.date_of_birth}"""
 
+
 class Registrants:
     '''
     Class to hold a list of registrants.
     '''
     registrants: list[Person]
 
     save_path: Path
-    json_filename: str = "data_savepoint.json"
+    json_filename: str = "disaster-id-scan_autosave.json"
+
+    export_filename: str = "disaster-id-scan_export.csv"
 
     def __init__(self):
         self.registrants = []
 
-    def add(self, person: Person):
+    def add(self, person: Person) -> int:
+        '''
+        Add a person to the list of registrants, return the id of the person.
+        '''
         self.registrants.append(person)
+        return len(self.registrants) - 1
 
     def get_savepoint_path(self) -> Path:
         return self.save_path.joinpath(Registrants.json_filename)
 
+    def get_export_path(self) -> Path:
+        return self.save_path.joinpath(Registrants.export_filename)
+
     def get_name_list(self) -> list[str]:
         return [f"{person.last_name}, {person.first_name} #{id}" for id, person in enumerate(self.registrants)]
 
-    def get_person_by_list_entry(self, list_entry: str) -> Person:
-        id = int(list_entry.split("#")[1])
-        return self.registrants[id]
+    def get_person_by_list_entry(self, list_entry: str) -> (int, Person):
+        person_id = int(list_entry.split("#")[1])
+        return person_id, self.registrants[person_id]
+
+    def get_person_by_id(self, person_id: int) -> Person:
+        return self.registrants[person_id]
+
+    def update(self, person_id: int, person: Person):
+        self.registrants[person_id] = person
+        self.save()
+
+    def delete(self, person_id: int):
+        self.registrants.pop(person_id)
+        self.save()
 
     def set_path(self, path: Path):
         self.save_path = path
-        # TODO: Check if json file exists, if so load it
+        # Check if json file exists, if so load it
+        if self.get_savepoint_path().exists():
+            with open(self.get_savepoint_path(), "r") as f:
+                self.registrants = jsonpickle.decode(f.read())
+        # Save immediately, to keep export file up to date
+        self.save()
 
     def save(self):
         with open(self.get_savepoint_path(), "w") as f:
-            f.write(jsonpickle.encode(self))
+            f.write(jsonpickle.encode(self.registrants))
+        # Export to csv (Xenios-Format? Whatever...)
+        # Name, Vorname, geb, Alter(ca.), Nationalitaet, Staat, Unterkunft,
+
+        with open(self.get_export_path(), "w") as f:
+            writer = DictWriter(f, fieldnames=["Name", "Vorname", "geb", "Alter(ca.)", "Nationalitaet", "Staat",
+                                               "Unterkunft", "Katastrophenort", "Katastrophentag", "Registrierungszeit"])
+            writer.writeheader()
+            for person in self.registrants:
+                # Calculate approximate age
+                if person.date_of_birth is not None:
+                    age = datetime.now().year - person.date_of_birth.year
+                else:
+                    age = None
+                writer.writerow({
+                    "Name": person.last_name,
+                    "Vorname": person.first_name,
+                    "geb": person.date_of_birth.strftime("%d.%m.%Y") if person.date_of_birth is not None else None,
+                    "Alter(ca.)": age,
+                    "Nationalitaet": person.nationality,
+                    "Staat": person.residence,
+                    "Unterkunft": person.place_of_shelter,
+                    "Katastrophenort": person.place_of_catastrophe,
+                    "Katastrophentag": person.date_of_catastrope.strftime("%d.%m.%Y") if person.date_of_catastrope is not None else None,
+                    "Registrierungszeit": person.time_of_registration.strftime("%d.%m.%Y %H:%M:%S") if person.time_of_registration is not None else None
+                })
```

### Comparing `disaster_id_scan-0.2.0/src/disaster_id_scan/ui.py` & `disaster_id_scan-0.3.0/src/disaster_id_scan/ui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+# SPDX-FileCopyrightText: 2023-present anjomro <py@anjomro.de>
+#
+# SPDX-License-Identifier: EUPL-1.2
 import tkinter as tk
 from pathlib import Path
 from tkinter import ttk
 import sv_ttk
 from tkinter import filedialog
 import cv2
 from PIL import ImageTk, Image
 import threading
 import easyocr
 from tkcalendar import DateEntry
 
 from disaster_id_scan.mrz import parse_mrz
 from disaster_id_scan.store import Person, Registrants
 
-store = Registrants()
-
 
 def get_available_cameras():
     camera_indexes = []
     for i in range(10):
         cap = cv2.VideoCapture(i)
         if cap.read()[0]:
             camera_indexes.append(i)
@@ -113,17 +114,19 @@
         self.image_label.imgtk = imgtk
         self.image_label.configure(image=imgtk, width=imgtk.width(), height=imgtk.height())
         self.image_label.after(10, self.show_frame)  # Update the frame every 10 milliseconds
 
 
 class GUI:
     def __init__(self):
+        self.loaded_person_id: int = None
         self.window = tk.Tk()
         self.window.title("Disaster ID Scan")
         # self.style = ttk.Style("cosmo")
+        self.store = Registrants()
 
         self.frame = tk.LabelFrame(self.window, text="Camera")
         self.frame.grid(row=0, column=0, rowspan=4, padx=10, pady=20)
         # Create black placeholder 640x480 as list
         # placeholder_array = [[0 for _ in range(640)] for _ in range(480)]
         # imgtk = ImageTk.PhotoImage(image=Image.fromarray(placeholder_array))
         self.image_label = tk.Label(self.frame)
@@ -131,39 +134,36 @@
         self.image_label.grid(row=0, column=0, columnspan=2, padx=10, pady=10)
 
         self.buttons_frame = tk.LabelFrame(self.frame, text="Actions")
         self.buttons_frame.grid(row=1, column=0, columnspan=2, padx=10, pady=10, ipady=5, ipadx=5)
 
         self.camera_indexes = get_available_cameras()
 
-
         self.camera_label = ttk.Label(self.buttons_frame, text="Camera:")
         self.camera_label.grid(row=0, column=1, padx=5, sticky="e")
         self.camera_combobox = ttk.Combobox(self.buttons_frame, values=[str(idx) for idx in self.camera_indexes],
                                             state="readonly")
-        self.camera_combobox.current(0)
         if self.camera_indexes:
             self.camera_combobox.current(self.camera_indexes[0])
         self.camera_combobox.grid(row=0, column=2, pady=5)
 
-
         self.start_stop_video = ttk.Button(self.buttons_frame, text="Start video", command=self.start_or_stop_video)
         self.capture_text = ttk.Button(self.buttons_frame, text="Recognize Text", command=self.capture_frame_text)
         self.select_data_folder = ttk.Button(self.buttons_frame, text="Select Data Folder",
                                              command=self.open_data_folder_selector)
         self.start_stop_video.grid(row=1, column=0, padx=5)
         self.capture_text.grid(row=1, column=1, padx=5)
         self.select_data_folder.grid(row=1, column=2, padx=5)
 
         # LabelFrame to Load existing person / data
         self.load_frame = ttk.LabelFrame(self.window, text="Load Person")
         self.load_frame.grid(row=1, column=3, columnspan=2, pady=10, padx=10, ipadx=5, ipady=5, sticky="nsew")
         # Create Combobox to select existing person
         self.load_frame.columnconfigure(0, weight=1)
-        self.person_combobox = ttk.Combobox(self.load_frame, values=store.get_name_list(), state="readonly")
+        self.person_combobox = ttk.Combobox(self.load_frame, values=self.store.get_name_list(), state="readonly")
         self.person_combobox.grid(row=0, column=0, columnspan=2, padx=5, pady=5, sticky="ew")
         self.load_person_button = ttk.Button(self.load_frame, text="Load Person", command=self.load_person_from_list)
         self.load_person_button.grid(row=0, column=2, padx=5, pady=5, sticky="e")
 
         self.data_frame = ttk.LabelFrame(self.window, text="Data")
         self.data_frame.grid(row=0, column=3, columnspan=2, pady=10, padx=10, sticky="nsew")
         # self.data_frame.pack(pady=10)
@@ -210,18 +210,27 @@
 
         self.error_label = tk.Label(self.window, text="", fg="red")
         # self.error_label.pack()
 
         self.video_streamer = None
         self.data_folder_selected = False
 
-        self.submit_button = ttk.Button(self.data_frame, text="Submit", command=self.submit_click)
-        self.reset_button = ttk.Button(self.data_frame, text="Reset", command=self.clear_form)
-        self.submit_button.grid(row=4, column=1, pady=20)
-        self.reset_button.grid(row=4, column=2)
+        self.create_button = ttk.Button(self.data_frame, text="Create", command=self.create_person)
+        self.save_changes_button = ttk.Button(self.data_frame, text="Save Changes", command=self.save_changes)
+        self.clear_button = ttk.Button(self.data_frame, text="Reset", command=self.clear_form)
+        self.delete_button = ttk.Button(self.data_frame, text="Delete", command=self.delete_person)
+
+        self.create_button.grid(row=4, column=0, pady=20)
+        self.save_changes_button.grid(row=4, column=1, pady=20)
+        self.clear_button.grid(row=4, column=2)
+        self.delete_button.grid(row=4, column=3)
+
+        # Save changes and delete buttons are disabled until a person is loaded
+        self.save_changes_button.config(state="disabled")
+        self.delete_button.config(state="disabled")
 
     def start_or_stop_video(self):
         if not self.data_folder_selected:
             self.display_error("Please select a data folder.")
             return
 
         if self.video_streamer and self.video_streamer.is_running:
@@ -243,70 +252,94 @@
     def capture_frame_text(self):
         if not self.video_streamer or not self.video_streamer.is_running:
             self.display_error("Please start the video before recognizing text.")
             return
 
         frame = self.video_streamer.cap.read()[1]
         reader = easyocr.Reader(['de'])
-        text = reader.readtext(frame, paragraph=True)
+        text = reader.readtext(frame, paragraph=True, allowlist='ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789<')
         print(text)
         for element in text:
             if "<" in element[1]:
                 # Assume that it could be the MRZ, try to parse it
                 possible_mrz = element[1]
                 possible_mrz = possible_mrz.upper()
                 parsed = parse_mrz(possible_mrz)
                 if parsed is not None:
                     # Set the values in the form
                     self.set_person(parsed)
-
+                    self.set_buttons_enabled(False)
     def open_data_folder_selector(self):
         folder_selected = filedialog.askdirectory()
         if folder_selected:
             self.data_folder_selected = True
             self.display_error("")
             print("Selected data folder:", folder_selected)
-            store.set_path(Path(folder_selected))
+            self.store.set_path(Path(folder_selected))
+            self.update_person_combobox()
         else:
             self.data_folder_selected = False
             self.display_error("Please select a data folder.")
 
     def update_person_combobox(self):
-        self.person_combobox['values'] = store.get_name_list()
+        self.person_combobox['values'] = self.store.get_name_list()
 
     def get_person_from_form(self) -> Person:
-
         human = Person()
         human.first_name = self.first_name_entry.get()
         human.last_name = self.last_name_entry.get()
         human.date_of_birth = self.date_of_birth_entry.get_date()
         human.nationality = self.nationality_entry.get()
         human.residence = self.residence_entry.get()
         human.place_of_catastrophe = self.place_of_catastrophe_entry.get()
         human.place_of_shelter = self.place_of_shelter_entry.get()
         human.date_of_catastrophe = self.date_of_catastrophe_entry.get_date()
         return human
 
-    def submit_click(self):
+    def create_person(self):
         human = self.get_person_from_form()
-        store.add(human)
-        store.save()
+        self.store.add(human)
+        self.store.save()
         self.clear_form()
         self.update_person_combobox()
 
+    def save_changes(self):
+        human = self.get_person_from_form()
+        # Get the ID of the person that is currently loaded
+        person_id, _ = self.store.get_person_by_list_entry(self.person_combobox.get())
+        self.store.update(self.loaded_person_id, human)
+        self.update_person_combobox()
+        # Set the combobox to the person that was just edited
+        self.person_combobox.current(person_id)
+
+
+    def delete_person(self):
+        selected_id, _ = self.store.get_person_by_list_entry(self.person_combobox.get())
+        self.store.delete(self.loaded_person_id)
+        self.clear_form()
+        self.update_person_combobox()
+        if self.loaded_person_id == selected_id:
+            self.person_combobox.current(0)
+        elif self.loaded_person_id > selected_id:
+            self.person_combobox.current(self.loaded_person_id - 1)
+        else:
+            self.person_combobox.current(self.loaded_person_id)
+        self.set_buttons_enabled(False)
+
     def clear_form(self):
         self.first_name_entry.delete(0, tk.END)
         self.last_name_entry.delete(0, tk.END)
         self.date_of_birth_entry.set_date(None)
         self.nationality_entry.delete(0, tk.END)
         self.residence_entry.delete(0, tk.END)
         # Don't clear the place of catastrophe and shelter, because they are often the same
         # self.place_of_catastrophe_entry.delete(0, tk.END)
         # self.place_of_shelter_entry.delete(0, tk.END)
         # self.date_of_catastrophe_entry.set_date(None)
+        self.set_buttons_enabled(False)
 
     def set_text(self, entry: tk.Entry, text: str):
         # Sets the text of an entry, removes old text
         entry.delete(0, tk.END)
         entry.insert(0, text)
 
     def set_text_if_not_none(self, entry: tk.Entry, text: str):
@@ -325,18 +358,29 @@
         self.set_text_if_not_none(self.place_of_shelter_entry, person.place_of_shelter)
         if person.date_of_catastrope is not None:
             self.date_of_catastrophe_entry.set_date(person.date_of_catastrope)
 
     def load_person_from_list(self):
         # Get the choosen list entry from combobox
         selected_person = self.person_combobox.get()
-        # Get the person object from the store
-        person = store.get_person_by_list_entry(selected_person)
+        # Get the person object from the self.store
+        person_id, person = self.store.get_person_by_list_entry(selected_person)
         # Set the values in the form
         self.set_person(person)
+        # Set the loaded person id
+        self.loaded_person_id = person_id
+        # Enable the save and delete button
+        self.set_buttons_enabled(True)
+
+    def set_buttons_enabled(self, enabled: bool):
+        '''
+        Enables or disables the save and delete button. They should only be enabled if a person is loaded.
+        '''
+        self.save_changes_button.config(state=tk.NORMAL if enabled else tk.DISABLED)
+        self.delete_button.config(state=tk.NORMAL if enabled else tk.DISABLED)
 
     def display_error(self, message):
         self.error_label.config(text=message)
 
     def start_gui(self):
         sv_ttk.use_light_theme()
         self.window.mainloop()
```

### Comparing `disaster_id_scan-0.2.0/src/disaster_id_scan/cli/__init__.py` & `disaster_id_scan-0.3.0/src/disaster_id_scan/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.2.0/LICENSE.txt` & `disaster_id_scan-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.2.0/README.md` & `disaster_id_scan-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.2.0/pyproject.toml` & `disaster_id_scan-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,14 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "click",
   "easyocr",
   "opencv-python",
-  "mrz",
-  "tk",
   "tkcalendar",
   "jsonpickle",
   "sv-ttk",
 ]
 
 [project.urls]
 Documentation = "https://github.com/anjomro/disaster-id-scan#readme"
@@ -163,7 +161,12 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.hatch.build.targets.app]
+scripts = ["disaster-id-scan"]
+python_version = "3.10"
+pyapp-version = "0.8.0"
```

### Comparing `disaster_id_scan-0.2.0/PKG-INFO` & `disaster_id_scan-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disaster-id-scan
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/anjomro/disaster-id-scan#readme
 Project-URL: Issues, https://github.com/anjomro/disaster-id-scan/issues
 Project-URL: Source, https://github.com/anjomro/disaster-id-scan
 Author-email: anjomro <py@anjomro.de>
 License-Expression: EUPL-1.2
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -16,18 +16,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: click
 Requires-Dist: easyocr
 Requires-Dist: jsonpickle
-Requires-Dist: mrz
 Requires-Dist: opencv-python
 Requires-Dist: sv-ttk
-Requires-Dist: tk
 Requires-Dist: tkcalendar
 Description-Content-Type: text/markdown
 
 # Disaster ID Scan
 
 [![PyPI - Version](https://img.shields.io/pypi/v/disaster-id-scan.svg)](https://pypi.org/project/disaster-id-scan)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/disaster-id-scan.svg)](https://pypi.org/project/disaster-id-scan)
```

