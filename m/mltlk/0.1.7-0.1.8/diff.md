# Comparing `tmp/mltlk-0.1.7.tar.gz` & `tmp/mltlk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.7.tar", last modified: Tue May 30 13:26:47 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.8.tar", last modified: Wed May 31 08:20:11 2023, max compression
```

## Comparing `mltlk-0.1.7.tar` & `mltlk-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.289176 mltlk-0.1.7/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.7/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.7/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:26:47.288370 mltlk-0.1.7/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.7/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.7/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.7/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.7/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    33375 2023-05-30 13:24:23.000000 mltlk-0.1.7/Wikipedia_exploration.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.7/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.264558 mltlk-0.1.7/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.7/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.7/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.7/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.278140 mltlk-0.1.7/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 13:22:24.000000 mltlk-0.1.7/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     8047 2023-05-30 13:23:32.000000 mltlk-0.1.7/mltlk/exploration_textdata.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.7/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.7/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.7/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.7/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.285427 mltlk-0.1.7/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:26:46.000000 mltlk-0.1.7/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 13:26:47.000000 mltlk-0.1.7/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 13:26:46.000000 mltlk-0.1.7/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 13:26:47.000000 mltlk-0.1.7/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 13:26:47.000000 mltlk-0.1.7/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 13:26:47.289479 mltlk-0.1.7/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-30 13:22:32.000000 mltlk-0.1.7/setup.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.286887 mltlk-0.1.7/stopwords/
--rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.7/stopwords/custom.csv
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-31 08:20:11.543416 mltlk-0.1.8/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.8/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.8/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-31 08:20:11.542472 mltlk-0.1.8/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.8/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    55130 2023-05-31 08:17:59.000000 mltlk-0.1.8/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    43723 2023-05-31 08:17:38.000000 mltlk-0.1.8/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.8/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    33375 2023-05-30 13:24:23.000000 mltlk-0.1.8/Wikipedia_exploration.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.8/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-31 08:20:11.494137 mltlk-0.1.8/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.8/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.8/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.8/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-31 08:20:11.529924 mltlk-0.1.8/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)      144 2023-05-31 06:32:50.000000 mltlk-0.1.8/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2483 2023-05-31 08:16:28.000000 mltlk-0.1.8/mltlk/exploration_tabdata.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     8047 2023-05-30 13:23:32.000000 mltlk-0.1.8/mltlk/exploration_textdata.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32391 2023-05-31 06:43:35.000000 mltlk-0.1.8/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.8/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.8/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.8/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-31 08:20:11.539046 mltlk-0.1.8/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-31 08:20:10.000000 mltlk-0.1.8/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      499 2023-05-31 08:20:11.000000 mltlk-0.1.8/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-31 08:20:10.000000 mltlk-0.1.8/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-31 08:20:11.000000 mltlk-0.1.8/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-31 08:20:11.000000 mltlk-0.1.8/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-31 08:20:11.543683 mltlk-0.1.8/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-31 06:33:12.000000 mltlk-0.1.8/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-31 08:20:11.540419 mltlk-0.1.8/stopwords/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.8/stopwords/custom.csv
```

### Comparing `mltlk-0.1.7/LICENSE` & `mltlk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/Spiral.ipynb` & `mltlk-0.1.8/Wikipedia_exploration.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9639120370370371%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.7\\n']}}}, 2: {'source': {insert: [(1, 'Load data, "*

 * *            "clean text and use bag-of-words + TF-IDF preprocessing.')], delete: [1]}}, 3: "*

 * *            "{'outputs': {0: {'text': ['\\x1b[1m\\x1b[33mInfo: \\x1b[0mClean texts keeping letters "*

 * *            "and digits\\n', '\\x1b[1m\\x1b[33mInfo: \\x1b[0mLoad 180 stopwords from "*

 * *            "\\x1b[36menglish, stopwords/custom.csv\\x1b[0m\\n', '\\x1b[1m\\x1b[33mInfo: "*

 * *            "\\x1b[0mUsed bag-of-words  […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.4\n"
+                        "0.1.7\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -29,114 +29,110 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## Load data\n",
-                "Load data, encode labels and scale inputs using standard scaler."
+                "Load data, clean text and use bag-of-words + TF-IDF preprocessing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mScaled input data using standard scaler\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m3\u001b[0m categories\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mLoad 180 stopwords from \u001b[36menglish, stopwords/custom.csv\u001b[0m\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mUsed bag-of-words with stopwords removed and TF-IDF\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
-                "session = load_data(\"data/spiral.csv\", conf={\"preprocess\": \"scale\"})"
+                "session = load_data(\"data/wikipedia_300.csv.gz\", conf={\n",
+                "    \"preprocess\": \"bag-of-words\",\n",
+                "    \"TF-IDF\": True,\n",
+                "    \"stopwords\": [\"english\", \"stopwords/custom.csv\"],\n",
+                "    \"clean_text\": \"letters digits\",\n",
+                "})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Show data stats"
+                "## Build corpus\n",
+                "Build a corpus from the dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>%</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>\u03a3%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>33.3%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>33.3%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>1</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>33.3%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>66.7%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>33.3%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>100.0%</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Examples:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>300</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Features:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>2</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#666;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>Categories:</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'>3</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:green;row-toggle-background:0;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
+                            "<table><tr><td style='text-align:left;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:black;row-toggle-background:0;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;' colspan=2>Corpus summary</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Total documents:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>300</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Total words:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>656748</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Unique words:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>53151</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Categories:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Average words/doc:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>3247.71</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Max words/doc:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>15287</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Min words/doc:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>80</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Stdev words/doc:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>2670.54</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
                 }
             ],
             "source": [
-                "data_stats(session)"
+                "corpus = build_corpus(session)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Evaluate model using cross-validation"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "#### Neural network"
+                "## Top words\n",
+                "Show top words in the dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m7.12\u001b[0m sec\n",
-                        "\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.36%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.33%</td></tr></table>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>2</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>99.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;1</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>1.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>1</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>97.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;1</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>2.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>2</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>1.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>1</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>1</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>96.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>3.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>3</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>1.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>1</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Word</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Count</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Appears for<br>categories</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Top 2 categories</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>game</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>6282</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Games <font color='#9d93fb'>(6124)</font>, Programming <font color='#9d93fb'>(158)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>1</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>4977</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Games <font color='#9d93fb'>(4863)</font>, Programming <font color='#9d93fb'>(114)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>software</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>3394</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming <font color='#9d93fb'>(2612)</font>, Games <font color='#9d93fb'>(782)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>3</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>video</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>3162</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Games <font color='#9d93fb'>(3082)</font>, Programming <font color='#9d93fb'>(80)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>4</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>system</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>3118</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming <font color='#9d93fb'>(1767)</font>, Games <font color='#9d93fb'>(1351)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>5</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>computer</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>2780</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Programming <font color='#9d93fb'>(1485)</font>, Games <font color='#9d93fb'>(1295)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>6</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>design</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2349</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming <font color='#9d93fb'>(1181)</font>, Games <font color='#9d93fb'>(1168)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>7</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>also</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>2342</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Games <font color='#9d93fb'>(1390)</font>, Programming <font color='#9d93fb'>(952)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>8</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>systems</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2312</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Programming <font color='#9d93fb'>(1556)</font>, Games <font color='#9d93fb'>(756)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>9</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>used</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>2269</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>2 (100.0%)</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games <font color='#9d93fb'>(1154)</font>, Programming <font color='#9d93fb'>(1115)</font></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -146,64 +142,61 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "evaluate_model(MLPClassifier(max_iter=2000, random_state=42), session, reload=False, conf={\n",
-                "    \"mode\": \"CV-10\",\n",
-                "    \"categories\": True,\n",
-                "    \"seed\": 42,\n",
-                "})"
+                "top_words(corpus, n=10, sidx=0)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Random Forest"
+                "## Overlapping words\n",
+                "Check overlapping words between all categories."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.21\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.76%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.67%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap<br><font style='font-weight: normal'>(Jaccard Similarity)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>24.31%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>2</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>99.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>1.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>1</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>98.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>2.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>2</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>1</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>96.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;2</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>4.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>4</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap<br><font style='font-weight: normal'>(Overlap Coefficient)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>43.36%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -213,61 +206,52 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "evaluate_model(RandomForestClassifier(random_state=42), session, reload=False, conf={\n",
-                "    \"mode\": \"CV-10\",\n",
-                "    \"categories\": True,\n",
-                "    \"seed\": 42,\n",
-                "})"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Build final model and predict example\n",
-                "Build final model using all data and predict an unknown example."
+                "overlap_all_categories(corpus)\n",
+                "overlap_all_categories(corpus, similarity=\"oc\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.12\u001b[0m sec\n"
+                        "\n"
                     ]
-                }
-            ],
-            "source": [
-                "build_model(RandomForestClassifier(), session)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {},
-            "outputs": [
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Unique words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No documents</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;filter:brightness(100%);font:Verdana 12px;'>Total words:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;filter:brightness(100%);font:Verdana 12px;'>53151</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Overlap:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>12923</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Overlap (Jaccard Similarity):</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>24.31%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Overlap (Overlap Coefficient):</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>43.36%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32m1\u001b[0m\n"
+                        "\n"
                     ]
                 }
             ],
             "source": [
-                "predict([-0.3, 0.3], session)"
+                "overlap(corpus, \"Games\", \"Programming\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `mltlk-0.1.7/Weather.ipynb` & `mltlk-0.1.8/Weather.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9818310657596372%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.8\\n']}}}, 7: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m2.67\\x1b[0m sec\\n')], delete: [0]}}}}, 9: {'outputs': {0: {'text': "*

 * *            "['\\x1b[1m\\x1b[33mInfo: \\x1b[0mBuilding final model on all data took "*

 * *            "\\x1b[34m0.28\\x1b[0m sec\\n']}}}, insert: [(11, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('metadata', OrderedDict()), ('s […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.4\n"
+                        "0.1.8\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -96,15 +96,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.10\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m2.67\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>64.29%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>63.24%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>62.86%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>64.29%</td></tr></table>"
@@ -182,15 +182,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.12\u001b[0m sec\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.28\u001b[0m sec\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(RandomForestClassifier(), session)"
             ]
         },
@@ -208,14 +208,57 @@
                 }
             ],
             "source": [
                 "predict([\"sunny\",\"mild\",\"normal\",False], session)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Plot data"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Feature<br><font style='font-weight: normal'>(nominal)</font></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Values (occurences)</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>outlook</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>sunny <font color='#7566f9'>(5)</font>, overcast <font color='#7566f9'>(4)</font>, rainy <font color='#7566f9'>(5)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>temperature</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>hot <font color='#7566f9'>(4)</font>, mild <font color='#7566f9'>(6)</font>, cool <font color='#7566f9'>(4)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>humidity</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>high <font color='#7566f9'>(7)</font>, normal <font color='#7566f9'>(7)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>windy</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>False <font color='#7566f9'>(8)</font>, True <font color='#7566f9'>(6)</font></td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "plot_data(session)"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
```

### Comparing `mltlk-0.1.7/Wikipedia.ipynb` & `mltlk-0.1.8/Wikipedia.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/Wikipedia_word2vec.ipynb` & `mltlk-0.1.8/Wikipedia_word2vec.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/data/spiral.csv` & `mltlk-0.1.8/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/data/wikipedia_300.csv.gz` & `mltlk-0.1.8/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/mltlk/exploration_textdata.py` & `mltlk-0.1.8/mltlk/exploration_textdata.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/mltlk/ml.py` & `mltlk-0.1.8/mltlk/ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,24 +44,32 @@
         conf["preprocess"] = ""
     conf["preprocess"] = conf["preprocess"].lower()
     
     # Load data
     if not exists(file):
         error("data file " + colored(file, "cyan") + " not found")
         return None
-    data = pd.read_csv(file).values
+    data = pd.read_csv(file)
+    cols = list(data.columns)
+    data = data.values
+    
     session["file"] = file
     
     # Set X features to be all but last column
     if Xcols is None:
         Xcols = range(0,len(data[0]) - 1)
     # Set y to be last column
     if ycol is None:
         ycol = len(data[0]) - 1
     
+    # Update columns
+    session["columns"] = []
+    for idx in Xcols:
+        session["columns"].append(cols[idx])
+    
     # Convert to X and y
     X = []
     y = []
     for r in data:
         row = []
         for c,val in enumerate(r):
             if c in Xcols:
```

### Comparing `mltlk-0.1.7/mltlk/resampling.py` & `mltlk-0.1.8/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/mltlk/utils.py` & `mltlk-0.1.8/mltlk/utils.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.7/mltlk/word2vec.py` & `mltlk-0.1.8/mltlk/word2vec.py`

 * *Files identical despite different names*

