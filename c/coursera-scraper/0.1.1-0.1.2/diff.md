# Comparing `tmp/coursera-scraper-0.1.1.tar.gz` & `tmp/coursera-scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coursera-scraper-0.1.1.tar", last modified: Sun Jun 18 11:53:25 2023, max compression
+gzip compressed data, was "coursera-scraper-0.1.2.tar", last modified: Sun Jun 18 11:59:04 2023, max compression
```

## Comparing `coursera-scraper-0.1.1.tar` & `coursera-scraper-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:53:25.463163 coursera-scraper-0.1.1/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     2152 2023-06-18 11:53:25.462690 coursera-scraper-0.1.1/PKG-INFO
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:53:25.460437 coursera-scraper-0.1.1/coursera_scraper.egg-info/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     2152 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/PKG-INFO
--rw-r--r--   0 talhapersonal   (503) staff       (20)      261 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)        1 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)       34 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/requires.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)        8 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:53:25.461983 coursera-scraper-0.1.1/scraper/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     1121 2023-06-18 09:49:40.000000 coursera-scraper-0.1.1/scraper/constants.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)      715 2023-06-18 11:52:33.000000 coursera-scraper-0.1.1/scraper/main.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)     4793 2023-06-18 11:51:22.000000 coursera-scraper-0.1.1/scraper/utils.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)       38 2023-06-18 11:53:25.463327 coursera-scraper-0.1.1/setup.cfg
--rw-r--r--   0 talhapersonal   (503) staff       (20)     1016 2023-06-18 11:53:06.000000 coursera-scraper-0.1.1/setup.py
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:59:04.878028 coursera-scraper-0.1.2/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     2115 2023-06-18 11:59:04.877685 coursera-scraper-0.1.2/PKG-INFO
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:59:04.875872 coursera-scraper-0.1.2/coursera_scraper.egg-info/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     2115 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 talhapersonal   (503) staff       (20)      261 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)        1 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)       34 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/requires.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)        8 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:59:04.877151 coursera-scraper-0.1.2/scraper/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     1121 2023-06-18 09:49:40.000000 coursera-scraper-0.1.2/scraper/constants.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)      717 2023-06-18 11:56:48.000000 coursera-scraper-0.1.2/scraper/main.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     4794 2023-06-18 11:57:09.000000 coursera-scraper-0.1.2/scraper/utils.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)       38 2023-06-18 11:59:04.878172 coursera-scraper-0.1.2/setup.cfg
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     1016 2023-06-18 11:58:37.000000 coursera-scraper-0.1.2/setup.py
```

### Comparing `coursera-scraper-0.1.1/PKG-INFO` & `coursera-scraper-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursera-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
 Home-page: https://github.com/talhakhalidmtk/coursera-scraper
 Author: Talha Khalid
 Author-email: talhakhalidmtk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,19 +31,17 @@
 11. Sub-course: Additional information about the course or its sub-courses.
 
 The scraped data is stored in a dictionary format for each course.
 
 ## Prerequisites
 You can install the required Python packages by running the following command:
 ```bash
-pip install -r requirements.txt
-
 pip install coursera-scraper
 
-from coursera-scraper import scraper
+from scraper.main import scraper
 
 results = scraper(keyword='python')
 ```
 
 
 ## Contributing
```

### Comparing `coursera-scraper-0.1.1/coursera_scraper.egg-info/PKG-INFO` & `coursera-scraper-0.1.2/coursera_scraper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursera-scraper
-Version: 0.1.1
+Version: 0.1.2
 Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
 Home-page: https://github.com/talhakhalidmtk/coursera-scraper
 Author: Talha Khalid
 Author-email: talhakhalidmtk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,19 +31,17 @@
 11. Sub-course: Additional information about the course or its sub-courses.
 
 The scraped data is stored in a dictionary format for each course.
 
 ## Prerequisites
 You can install the required Python packages by running the following command:
 ```bash
-pip install -r requirements.txt
-
 pip install coursera-scraper
 
-from coursera-scraper import scraper
+from scraper.main import scraper
 
 results = scraper(keyword='python')
 ```
 
 
 ## Contributing
```

### Comparing `coursera-scraper-0.1.1/scraper/constants.py` & `coursera-scraper-0.1.2/scraper/constants.py`

 * *Files identical despite different names*

### Comparing `coursera-scraper-0.1.1/scraper/main.py` & `coursera-scraper-0.1.2/scraper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from utils import go_to_course
-from constants import TIME_TO_WAIT
+from .utils import go_to_course
+from .constants import TIME_TO_WAIT
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from webdriver_manager.chrome import ChromeDriverManager
 
 
 def scraper(keyword):
     options = webdriver.ChromeOptions()
```

### Comparing `coursera-scraper-0.1.1/scraper/utils.py` & `coursera-scraper-0.1.2/scraper/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from constants import STUDENTS_ENROLLED_XPATH1, STUDENTS_ENROLLED_XPATH2, TIME_REQ_XPATH1, TIME_REQ_XPATH2, \
+from .constants import STUDENTS_ENROLLED_XPATH1, STUDENTS_ENROLLED_XPATH2, TIME_REQ_XPATH1, TIME_REQ_XPATH2, \
     PAGINATION_BUTTON_XPATH, TIME_TO_WAIT, COURSE_CARD_XPATH, PAGINATION_CONTAINER, TIME_TO_NEXT_PAGE, DIFFICULTY_XPATH, \
     COURSE_CARD_LINK_XPATH, INSTITUTE_XPATH, RATING_XPATH, RECENT_VIEWS_XPATH, TITLE_XPATH, SKILL_XPATH, \
     SUBCOURSE_XPATH, LEARNERS_XPATH
 import pandas as pd
 
 
 def get_students_and_time(path_list, driver):
```

### Comparing `coursera-scraper-0.1.1/setup.py` & `coursera-scraper-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("scraper/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="coursera-scraper",
-    version="0.1.1",
+    version="0.1.2",
     author="Talha Khalid",
     author_email="talhakhalidmtk@gmail.com",
     description="This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/talhakhalidmtk/coursera-scraper",
     packages=["scraper"],
```

