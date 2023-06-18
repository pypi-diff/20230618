# Comparing `tmp/coursera-scraper-0.1.2.tar.gz` & `tmp/coursera-scraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coursera-scraper-0.1.2.tar", last modified: Sun Jun 18 11:59:04 2023, max compression
+gzip compressed data, was "coursera-scraper-0.1.3.tar", last modified: Sun Jun 18 15:21:20 2023, max compression
```

## Comparing `coursera-scraper-0.1.2.tar` & `coursera-scraper-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:59:04.878028 coursera-scraper-0.1.2/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     2115 2023-06-18 11:59:04.877685 coursera-scraper-0.1.2/PKG-INFO
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:59:04.875872 coursera-scraper-0.1.2/coursera_scraper.egg-info/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     2115 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/PKG-INFO
--rw-r--r--   0 talhapersonal   (503) staff       (20)      261 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)        1 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)       34 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/requires.txt
--rw-r--r--   0 talhapersonal   (503) staff       (20)        8 2023-06-18 11:59:04.000000 coursera-scraper-0.1.2/coursera_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 11:59:04.877151 coursera-scraper-0.1.2/scraper/
--rw-r--r--   0 talhapersonal   (503) staff       (20)     1121 2023-06-18 09:49:40.000000 coursera-scraper-0.1.2/scraper/constants.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)      717 2023-06-18 11:56:48.000000 coursera-scraper-0.1.2/scraper/main.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)     4794 2023-06-18 11:57:09.000000 coursera-scraper-0.1.2/scraper/utils.py
--rw-r--r--   0 talhapersonal   (503) staff       (20)       38 2023-06-18 11:59:04.878172 coursera-scraper-0.1.2/setup.cfg
--rw-r--r--   0 talhapersonal   (503) staff       (20)     1016 2023-06-18 11:58:37.000000 coursera-scraper-0.1.2/setup.py
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 15:21:20.960705 coursera-scraper-0.1.3/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     2107 2023-06-18 15:21:20.960305 coursera-scraper-0.1.3/PKG-INFO
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 15:21:20.958239 coursera-scraper-0.1.3/coursera_scraper.egg-info/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     2107 2023-06-18 15:21:20.000000 coursera-scraper-0.1.3/coursera_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 talhapersonal   (503) staff       (20)      261 2023-06-18 15:21:20.000000 coursera-scraper-0.1.3/coursera_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)        1 2023-06-18 15:21:20.000000 coursera-scraper-0.1.3/coursera_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)       34 2023-06-18 15:21:20.000000 coursera-scraper-0.1.3/coursera_scraper.egg-info/requires.txt
+-rw-r--r--   0 talhapersonal   (503) staff       (20)        8 2023-06-18 15:21:20.000000 coursera-scraper-0.1.3/coursera_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 talhapersonal   (503) staff       (20)        0 2023-06-18 15:21:20.959537 coursera-scraper-0.1.3/scraper/
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     1121 2023-06-18 09:49:40.000000 coursera-scraper-0.1.3/scraper/constants.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)      761 2023-06-18 15:20:20.000000 coursera-scraper-0.1.3/scraper/main.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     4879 2023-06-18 15:20:29.000000 coursera-scraper-0.1.3/scraper/utils.py
+-rw-r--r--   0 talhapersonal   (503) staff       (20)       38 2023-06-18 15:21:20.960852 coursera-scraper-0.1.3/setup.cfg
+-rw-r--r--   0 talhapersonal   (503) staff       (20)     1022 2023-06-18 15:20:51.000000 coursera-scraper-0.1.3/setup.py
```

### Comparing `coursera-scraper-0.1.2/PKG-INFO` & `coursera-scraper-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: coursera-scraper
-Version: 0.1.2
-Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
+Version: 0.1.3
+Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as link, title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
 Home-page: https://github.com/talhakhalidmtk/coursera-scraper
 Author: Talha Khalid
 Author-email: talhakhalidmtk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Coursera Scraper
 
-This repository contains a Python script that utilizes Selenium to scrape data from Coursera. The script collects information about various courses and their details from Coursera's website.
+This repository contains a Python script that utilizes Selenium to scrape data from Coursera. 
 
 ## Scraped Fields
 
 The script scrapes the following fields for each course:
-1. Title: The title of the course.
+1. Link: Link of the course
+2. Title: The title of the course.
 2. Institute: The institution offering the course (if available).
 3. Rating: The course rating.
 4. Recent Views: The number of recent views for the course.
 5. Students Enrolled: The number of students enrolled in the course.
 6. Time Requirement: The approximate time required to complete the course.
 7. Skills: A list of skills covered in the course.
 8. Learner Count: The total number of learners who have taken the course.
@@ -35,15 +36,16 @@
 ## Prerequisites
 You can install the required Python packages by running the following command:
 ```bash
 pip install coursera-scraper
 
 from scraper.main import scraper
 
-results = scraper(keyword='python')
+for course_detail in scraper(keyword='python'):
+    # do some processing on course detail
 ```
 
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `coursera-scraper-0.1.2/coursera_scraper.egg-info/PKG-INFO` & `coursera-scraper-0.1.3/coursera_scraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: coursera-scraper
-Version: 0.1.2
-Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
+Version: 0.1.3
+Summary: This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as link, title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.
 Home-page: https://github.com/talhakhalidmtk/coursera-scraper
 Author: Talha Khalid
 Author-email: talhakhalidmtk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Coursera Scraper
 
-This repository contains a Python script that utilizes Selenium to scrape data from Coursera. The script collects information about various courses and their details from Coursera's website.
+This repository contains a Python script that utilizes Selenium to scrape data from Coursera. 
 
 ## Scraped Fields
 
 The script scrapes the following fields for each course:
-1. Title: The title of the course.
+1. Link: Link of the course
+2. Title: The title of the course.
 2. Institute: The institution offering the course (if available).
 3. Rating: The course rating.
 4. Recent Views: The number of recent views for the course.
 5. Students Enrolled: The number of students enrolled in the course.
 6. Time Requirement: The approximate time required to complete the course.
 7. Skills: A list of skills covered in the course.
 8. Learner Count: The total number of learners who have taken the course.
@@ -35,15 +36,16 @@
 ## Prerequisites
 You can install the required Python packages by running the following command:
 ```bash
 pip install coursera-scraper
 
 from scraper.main import scraper
 
-results = scraper(keyword='python')
+for course_detail in scraper(keyword='python'):
+    # do some processing on course detail
 ```
 
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `coursera-scraper-0.1.2/scraper/constants.py` & `coursera-scraper-0.1.3/scraper/constants.py`

 * *Files identical despite different names*

### Comparing `coursera-scraper-0.1.2/scraper/main.py` & `coursera-scraper-0.1.3/scraper/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .utils import go_to_course
 from .constants import TIME_TO_WAIT
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from webdriver_manager.chrome import ChromeDriverManager
 
 
-def scraper(keyword):
+def scraper(keyword, csv=True):
     options = webdriver.ChromeOptions()
     options.add_argument("--headless")
     driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()), options=options)
 
     url = f'https://www.coursera.org/search?query={keyword}&page=1&index' \
           f'=prod_all_launched_products_term_optimization_skills_test_for_precise_xdp_imprecise_variant'
     driver.get(url)
     driver.implicitly_wait(TIME_TO_WAIT)
-    return go_to_course(driver, keyword)
+    for course in go_to_course(driver, keyword, csv):
+        yield course
```

### Comparing `coursera-scraper-0.1.2/scraper/utils.py` & `coursera-scraper-0.1.3/scraper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     x = txt.split('·')
     return {
         'difficulty': x[0].strip(),
         'duration': x[-1].strip(),
     }
 
 
-def go_to_course(driver, keyword):
+def go_to_course(driver, keyword, csv):
     data = []
     pages = get_total_pagination_pages(driver)
     print("Total Pages are: " + str(pages))
     for x in range(pages):
         if x + 1 == pages:  # checking if last page is displayed then close program (scraping)
             driver.close()
             break
@@ -84,26 +84,27 @@
         elif x != 0:
             # going to next page in pagination
             driver.find_element('xpath',
                                 PAGINATION_CONTAINER + '//button[@data-e2e="pagination-controls-next"]').click()
             driver.implicitly_wait(TIME_TO_NEXT_PAGE)  # waiting for next page to load
 
         links = get_total_courses_in_page(driver)
-        print('total links in page no.' + str(x + 1) + ' is : ' + str(len(links)))
+        print('Total links in page # ' + str(x + 1) + ' are : ' + str(len(links)))
 
         for y in range(len(links)):
             details_from_card = get_details_from_card(get_value('text', COURSE_CARD_XPATH + '[' + str(
                 y + 1) + ']' + COURSE_CARD_LINK_XPATH + DIFFICULTY_XPATH, driver))
 
             driver.find_element('xpath', COURSE_CARD_XPATH + '[' + str(
                 y + 1) + ']' + COURSE_CARD_LINK_XPATH).click()  # going to course detail
             driver.implicitly_wait(5)
             driver.switch_to.window(driver.window_handles[1])
 
             data.append({
+                'link': driver.current_url,
                 'title': get_value('text', TITLE_XPATH, driver),
                 'institute': get_value('text', COURSE_CARD_XPATH
                                        + '[' + str(y + 1) + ']' + COURSE_CARD_LINK_XPATH + INSTITUTE_XPATH, driver),
                 'rating': get_value('text', RATING_XPATH, driver).replace("\nstars", ""),
                 'recent_views': get_value('text', RECENT_VIEWS_XPATH, driver),
                 'students_enrolled': get_students_and_time([STUDENTS_ENROLLED_XPATH1, STUDENTS_ENROLLED_XPATH2], driver),
                 'time_req': get_students_and_time([TIME_REQ_XPATH1, TIME_REQ_XPATH2], driver),
@@ -111,12 +112,14 @@
                 'learner': get_value('text', LEARNERS_XPATH, driver),
                 'difficulty': details_from_card['difficulty'],
                 'duration': details_from_card['duration'],
                 'subCourse': get_value('text', SUBCOURSE_XPATH, driver),
             })
             print(str(y) + ": " + str(data[-1]))
 
-            pd.DataFrame(data=data).to_csv(f'coursera {keyword}.csv')
+            if csv:
+                pd.DataFrame(data=data).to_csv(f'coursera {keyword}.csv')
+
+            yield data[-1]
 
             driver.close()
             driver.switch_to.window(driver.window_handles[0])
-    return data
```

### Comparing `coursera-scraper-0.1.2/setup.py` & `coursera-scraper-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("scraper/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="coursera-scraper",
-    version="0.1.2",
+    version="0.1.3",
     author="Talha Khalid",
     author_email="talhakhalidmtk@gmail.com",
-    description="This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.",
+    description="This Python script utilizes Selenium to scrape data from Coursera, providing detailed information about various courses such as link, title, rating, recent views, students enrolled, time requirement, skills, learner count, difficulty level, duration, and sub-course details.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/talhakhalidmtk/coursera-scraper",
     packages=["scraper"],
     install_requires=[
         "pandas",
         "selenium",
```

