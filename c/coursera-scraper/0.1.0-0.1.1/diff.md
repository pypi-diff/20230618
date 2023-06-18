# Comparing `tmp/coursera-scraper-0.1.0.tar.gz` & `tmp/coursera-scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coursera-scraper-0.1.0.tar", last modified: Sun Jun 18 11:32:18 2023, max compression
+gzip compressed data, was "coursera-scraper-0.1.1.tar", last modified: Sun Jun 18 11:53:25 2023, max compression
```

## Comparing `coursera-scraper-0.1.0.tar` & `coursera-scraper-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:32:18.871772 coursera-scraper-0.1.0/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     2047 2023-06-18 11:32:18.871052 coursera-scraper-0.1.0/PKG-INFO
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:32:18.866804 coursera-scraper-0.1.0/coursera_scraper.egg-info/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     2047 2023-06-18 11:32:18.000000 coursera-scraper-0.1.0/coursera_scraper.egg-info/PKG-INFO
--rw-r--r--   0 talhapersonal   (503) staff       (20)      261 2023-06-18 11:32:18.000000 coursera-scraper-0.1.0/coursera_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)        1 2023-06-18 11:32:18.000000 coursera-scraper-0.1.0/coursera_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)       34 2023-06-18 11:32:18.000000 coursera-scraper-0.1.0/coursera_scraper.egg-info/requires.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)        8 2023-06-18 11:32:18.000000 coursera-scraper-0.1.0/coursera_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:32:18.869456 coursera-scraper-0.1.0/scraper/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     1121 2023-06-18 09:49:40.000000 coursera-scraper-0.1.0/scraper/constants.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)      739 2023-06-18 11:07:00.000000 coursera-scraper-0.1.0/scraper/main.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)     4770 2023-06-18 10:19:49.000000 coursera-scraper-0.1.0/scraper/utils.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)       38 2023-06-18 11:32:18.872084 coursera-scraper-0.1.0/setup.cfg
--rw-r--r--   0 talhapersonal   (503) staff       (20)     1016 2023-06-18 11:32:11.000000 coursera-scraper-0.1.0/setup.py
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:53:25.463163 coursera-scraper-0.1.1/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     2152 2023-06-18 11:53:25.462690 coursera-scraper-0.1.1/PKG-INFO
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:53:25.460437 coursera-scraper-0.1.1/coursera_scraper.egg-info/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     2152 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 talhapersonal   (503) staff       (20)      261 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)        1 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)       34 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/requires.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)        8 2023-06-18 11:53:25.000000 coursera-scraper-0.1.1/coursera_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:53:25.461983 coursera-scraper-0.1.1/scraper/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     1121 2023-06-18 09:49:40.000000 coursera-scraper-0.1.1/scraper/constants.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)      715 2023-06-18 11:52:33.000000 coursera-scraper-0.1.1/scraper/main.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     4793 2023-06-18 11:51:22.000000 coursera-scraper-0.1.1/scraper/utils.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)       38 2023-06-18 11:53:25.463327 coursera-scraper-0.1.1/setup.cfg
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     1016 2023-06-18 11:53:06.000000 coursera-scraper-0.1.1/setup.py
```

### Comparing `coursera-scraper-0.1.0/PKG-INFO` & `coursera-scraper-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursera-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
 Home-page: https://github.com/talhakhalidmtk/coursera-scraper
 Author: Talha Khalid
 Author-email: talhakhalidmtk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,20 @@
 
 The scraped data is stored in a dictionary format for each course.
 
 ## Prerequisites
 You can install the required Python packages by running the following command:
 ```bash
 pip install -r requirements.txt
+
+pip install coursera-scraper
+
+from coursera-scraper import scraper
+
+results = scraper(keyword='python')
 ```
 
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `coursera-scraper-0.1.0/coursera_scraper.egg-info/PKG-INFO` & `coursera-scraper-0.1.1/coursera_scraper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursera-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
 Home-page: https://github.com/talhakhalidmtk/coursera-scraper
 Author: Talha Khalid
 Author-email: talhakhalidmtk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,20 @@
 
 The scraped data is stored in a dictionary format for each course.
 
 ## Prerequisites
 You can install the required Python packages by running the following command:
 ```bash
 pip install -r requirements.txt
+
+pip install coursera-scraper
+
+from coursera-scraper import scraper
+
+results = scraper(keyword='python')
 ```
 
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `coursera-scraper-0.1.0/scraper/constants.py` & `coursera-scraper-0.1.1/scraper/constants.py`

 * *Files identical despite different names*

### Comparing `coursera-scraper-0.1.0/scraper/main.py` & `coursera-scraper-0.1.1/scraper/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from utils import go_to_course
 from constants import TIME_TO_WAIT
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from webdriver_manager.chrome import ChromeDriverManager
 
 
-def main(keyword):
+def scraper(keyword):
     options = webdriver.ChromeOptions()
     options.add_argument("--headless")
     driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()), options=options)
 
     url = f'https://www.coursera.org/search?query={keyword}&page=1&index' \
           f'=prod_all_launched_products_term_optimization_skills_test_for_precise_xdp_imprecise_variant'
     driver.get(url)
     driver.implicitly_wait(TIME_TO_WAIT)
-    go_to_course(driver)
-    print("DONE")
-
-
-main(keyword='python')
+    return go_to_course(driver, keyword)
```

### Comparing `coursera-scraper-0.1.0/scraper/utils.py` & `coursera-scraper-0.1.1/scraper/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     x = txt.split('·')
     return {
         'difficulty': x[0].strip(),
         'duration': x[-1].strip(),
     }
 
 
-def go_to_course(driver):
+def go_to_course(driver, keyword):
     data = []
     pages = get_total_pagination_pages(driver)
     print("Total Pages are: " + str(pages))
     for x in range(pages):
         if x + 1 == pages:  # checking if last page is displayed then close program (scraping)
             driver.close()
             break
@@ -100,23 +100,23 @@
             driver.switch_to.window(driver.window_handles[1])
 
             data.append({
                 'title': get_value('text', TITLE_XPATH, driver),
                 'institute': get_value('text', COURSE_CARD_XPATH
                                        + '[' + str(y + 1) + ']' + COURSE_CARD_LINK_XPATH + INSTITUTE_XPATH, driver),
                 'rating': get_value('text', RATING_XPATH, driver).replace("\nstars", ""),
-                'recentViews': get_value('text', RECENT_VIEWS_XPATH, driver),
-                'studentsEnrolled': get_students_and_time([STUDENTS_ENROLLED_XPATH1, STUDENTS_ENROLLED_XPATH2], driver),
-                'timeReq': get_students_and_time([TIME_REQ_XPATH1, TIME_REQ_XPATH2], driver),
+                'recent_views': get_value('text', RECENT_VIEWS_XPATH, driver),
+                'students_enrolled': get_students_and_time([STUDENTS_ENROLLED_XPATH1, STUDENTS_ENROLLED_XPATH2], driver),
+                'time_req': get_students_and_time([TIME_REQ_XPATH1, TIME_REQ_XPATH2], driver),
                 'skills': get_value('list', SKILL_XPATH, driver),
                 'learner': get_value('text', LEARNERS_XPATH, driver),
                 'difficulty': details_from_card['difficulty'],
                 'duration': details_from_card['duration'],
                 'subCourse': get_value('text', SUBCOURSE_XPATH, driver),
             })
             print(str(y) + ": " + str(data[-1]))
 
-            pd.DataFrame(data=data).to_csv('coursera.csv')
+            pd.DataFrame(data=data).to_csv(f'coursera {keyword}.csv')
 
             driver.close()
             driver.switch_to.window(driver.window_handles[0])
     return data
```

### Comparing `coursera-scraper-0.1.0/setup.py` & `coursera-scraper-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("scraper/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="coursera-scraper",
-    version="0.1.0",
+    version="0.1.1",
     author="Talha Khalid",
     author_email="talhakhalidmtk@gmail.com",
     description="This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/talhakhalidmtk/coursera-scraper",
     packages=["scraper"],
```

