# Comparing `tmp/sarcgraph-0.1.1.tar.gz` & `tmp/sarcgraph-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcgraph-0.1.1.tar", last modified: Mon May  1 17:13:39 2023, max compression
+gzip compressed data, was "sarcgraph-0.2.1.tar", last modified: Sun Jun 18 19:34:05 2023, max compression
```

## Comparing `sarcgraph-0.1.1.tar` & `sarcgraph-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:13:39.210000 sarcgraph-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    10473 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9768 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 17:13:39.220000 sarcgraph-0.1.1/sarcgraph/
--rw-rw-rw-   0        0        0        0 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/sarcgraph/__init__.py
--rw-rw-rw-   0        0        0    38694 2023-04-27 23:54:10.000000 sarcgraph-0.1.1/sarcgraph/sg.py
--rw-rw-rw-   0        0        0    60155 2023-04-25 23:24:08.000000 sarcgraph-0.1.1/sarcgraph/sg_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:13:39.230000 sarcgraph-0.1.1/sarcgraph.egg-info/
--rw-rw-rw-   0        0        0    10473 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 17:07:28.000000 sarcgraph-0.1.1/sarcgraph.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      149 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/sarcgraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 17:13:40.000000 sarcgraph-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1265 2023-05-01 17:10:10.000000 sarcgraph-0.1.1/setup.py
+drwxr-xr-x   0 ghost     (1000) ghost     (1000)        0 2023-06-18 19:34:05.122261 sarcgraph-0.2.1/
+-rw-r--r--   0 ghost     (1000) ghost     (1000)     1067 2023-06-18 17:49:00.000000 sarcgraph-0.2.1/LICENSE
+-rw-r--r--   0 ghost     (1000) ghost     (1000)    11216 2023-06-18 19:34:05.122261 sarcgraph-0.2.1/PKG-INFO
+-rw-r--r--   0 ghost     (1000) ghost     (1000)    10547 2023-06-18 17:49:00.000000 sarcgraph-0.2.1/README.md
+drwxr-xr-x   0 ghost     (1000) ghost     (1000)        0 2023-06-18 19:34:05.122261 sarcgraph-0.2.1/sarcgraph/
+-rw-r--r--   0 ghost     (1000) ghost     (1000)       22 2023-06-18 19:26:27.000000 sarcgraph-0.2.1/sarcgraph/__init__.py
+-rw-r--r--   0 ghost     (1000) ghost     (1000)    37712 2023-06-18 19:04:11.000000 sarcgraph-0.2.1/sarcgraph/sg.py
+-rw-r--r--   0 ghost     (1000) ghost     (1000)    60113 2023-06-18 17:49:01.000000 sarcgraph-0.2.1/sarcgraph/sg_tools.py
+drwxr-xr-x   0 ghost     (1000) ghost     (1000)        0 2023-06-18 19:34:05.122261 sarcgraph-0.2.1/sarcgraph.egg-info/
+-rw-r--r--   0 ghost     (1000) ghost     (1000)    11216 2023-06-18 19:34:05.000000 sarcgraph-0.2.1/sarcgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ghost     (1000) ghost     (1000)      282 2023-06-18 19:34:05.000000 sarcgraph-0.2.1/sarcgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ghost     (1000) ghost     (1000)        1 2023-06-18 19:34:05.000000 sarcgraph-0.2.1/sarcgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ghost     (1000) ghost     (1000)        1 2023-06-18 19:34:05.000000 sarcgraph-0.2.1/sarcgraph.egg-info/not-zip-safe
+-rw-r--r--   0 ghost     (1000) ghost     (1000)      149 2023-06-18 19:34:05.000000 sarcgraph-0.2.1/sarcgraph.egg-info/requires.txt
+-rw-r--r--   0 ghost     (1000) ghost     (1000)       10 2023-06-18 19:34:05.000000 sarcgraph-0.2.1/sarcgraph.egg-info/top_level.txt
+-rw-r--r--   0 ghost     (1000) ghost     (1000)       38 2023-06-18 19:34:05.122261 sarcgraph-0.2.1/setup.cfg
+-rw-r--r--   0 ghost     (1000) ghost     (1000)     1223 2023-06-18 19:31:11.000000 sarcgraph-0.2.1/setup.py
```

### Comparing `sarcgraph-0.1.1/LICENSE` & `sarcgraph-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Sarc-Graph
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Sarc-Graph
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sarcgraph-0.1.1/PKG-INFO` & `sarcgraph-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,200 +1,229 @@
-Metadata-Version: 2.1
-Name: sarcgraph
-Version: 0.1.1
-Summary: A software for sarcomere detection and tracking
-Home-page: https://pypi.org/project/sarcgraph/
-Author: Saeed Mohammadzadeh
-Author-email: saeedmhz@bu.edu
-Maintainer: [('Saeed Mohammadzadeh', 'saeedmhz@bu.edu'), ('Emma Lejeune', 'elejeune@bu.edu')]
-License: MIT
-Project-URL: Source, https://github.com/Sarc-Graph/sarcgraph
-Project-URL: Documentation, https://sarc-graph.readthedocs.io/en/latest/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **SarcGraph**
-
-[![python](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/) ![os](https://img.shields.io/badge/os-ubuntu%20|%20macos%20|%20windows-blue.svg) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Sarc-Graph/sarcgraph#license)
-
-[![flake8](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml/badge.svg)](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml) [![codecov](https://codecov.io/gh/Sarc-Graph/sarcgraph/branch/main/graph/badge.svg?token=XNE85EJ4GX)](https://codecov.io/gh/Sarc-Graph/sarcgraph) [![Documentation Status](https://readthedocs.org/projects/sarc-graph/badge/?version=latest)](https://sarc-graph.readthedocs.io/en/latest/?badge=latest)
-
-## **Table of Contents**
-* [Project Summary](#summary)
-* [Installation Instructions](#install)
-* [Contents](#contents)
-* [Tutorial](#tutorial) - [Notebooks](https://github.com/Sarc-Graph/sarcgraph/tree/main/tutorials)
-* [Validation](#validation)
-* [References to Related Work](#references)
-* [Contact Information](#contact)
-* [Acknowledgements](#acknowledge)
-
-## **Project Summary** <a name="summary"></a>
-
-**SarcGraph** is a tool for automatic detection, tracking and analysis of
-z-discs and sarcomeres in movies of beating *human induced pluripotent stem
-cell-derived cardiomyocytes (hiPSC-CMs)*.
-
-<br />
-<center><img src="figures/intro.png" width=30%></center>
-<br />
-
-SarcGraph was initially introduced in [Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443).
-This package is created to make SarcGraph more accessible to the broader
-research community.
-
-**For more information visit [SarcGraph documentation](https://sarc-graph.readthedocs.io/en/latest/).**
-
-## **Installation Instructions** <a name="install"></a>
-
-### **Get a copy of the [SarcGraph repository](https://github.com/Sarc-Graph/sarcgraph) on your local machine**
-
-You can do this by clicking the green ``<> code`` button and selecting ``Download Zip`` or by running the following command in terminal:
-
-```bash
-git clone https://github.com/Sarc-Graph/sarcgraph.git
-```
-
-### **Create and activate a conda virtual environment**
-
-1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
-
-2. Open a terminal and move to the directory of the ``sarcgraph`` repository. Then, type the following command in terminal to create a virtual envirnoment and install the required packages:
-
-```bash
-cd sarcgraph
-conda env create --file=environment.yml
-```
-
-3. Activate your virtual environment.
-
-```bash
-conda activate sarcgraph
-```
-
-### **Install SarcGraph**
-
-SarcGraph can be installed using ``pip``:
-
-```bash
-pip install sarcgraph
-```
-
-## **Contents** <a name="contents"></a>
-
-```bash
-|___ sarcgraph
-|        |___ docs/
-|        |___ figures/
-|                |___ *.png
-|        |___ samples/
-|        |___ sarcgraph/
-|                |___ __init__.py
-|                |___ sg.py
-|                |___ sg_tools.py
-|        |___ tests/
-|        |___ tutorials/
-|                |___ *.ipynb
-```
-
-## **Tutorial** <a name="tutorial"></a>
-
-This GitHub repository contains a folder called ``tutorials`` that contains demos to extensively show how this package can be used to analyze videos or images of hiPSC-CMs.
-
-### **Package Contents** <a name="whats-in-package"></a>
-
-The package contains two seperate modules: `sg` for sarcomere detection and tracking and `sg_tools` for running further analysis and visualizations.
-
-#### **sarcgraph.sg** <a name="sarcgraph.py"></a>
-`sarcgraph.sg` module takes a video/image file as input (more details in tutorials). This module then processes the input file to detect and track z-discs and sarcomeres through running 3 tasks:
-
- - Z-disc Segmentation,
- - Z-disc Tracking,
- - Sarcomere Detection.
-
-Here is a list of functions developed for each task:
-
-- `zdisc_segmentation`: Detect z-discs in each frame of the input video/image and saves the following information into a pandas `DataFrame`:
-
-> - `frame`: (frame number) 
-> - `x` and `y`: (X and Y position of the center of a z-disc)
-> - `p1_x`, `p1_y` and `p2_x`, `p2_y`: (X and Y position of both ends of a z-disc)
-
-- `zdisc_tracking`: Tracks detected z-discs in the input video over all frames and adds the following information to the pandas `DataFrame`:
-
-> - `particle`: (z-disc id)
-> - `freq`: (number of frames in which a z-discs is tracked)
-frame,sarc_id,x,y,length,width,angle,z-discs
-
-- `sarcomere_detection`: Detects sarcomeres in the input video/image using tracked z-discs `DataFrame` and saves the following information into a new pandas `DataFrame`:
-
-> - `frame`: (frame number)
-> - `sarc_id`: (sarcomere id)
-> - `x` and `y`: (X and Y position of the center of a sarcomere)
-> - `length`: (sarcomere length)
-> - `width`: (sarcomere width)
-> - `angle`: (sarcomere angle)
-> - `zdiscs`: (ids of the two z-discs forming a sarcomere)
-
-
-#### **sarcgraph.sg_tools** <a name="sarcgraph_tools.py"></a>
-
-`sarcgraph.sg_tools` module consists of 3 subclasses:
-
-- `TimeSeries`: Process timeseries of detected and tracked sarcomeres
-
-> - `sarcomeres_gpr()`: Applies Gaussian Process Regression (GPR) on each recovered timeseries characteristic of all detected sarcomeres to reduce the noise and fill in the missing data
-
-- `Analysis`: Extract more information from detected sarcomeres characteristics timeseries
-
-> - `compute_F_J`: Computes the average deformation gradient (F) and its jacobian (J)
-> - `compute_OOP`: Computes the Orientation Order Parameter (OOP)
-> - `compute_metrics`: Computes {OOP, C_iso, C_OOP, s_til, s_avg} as defined in the [SarcGraph paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443)
-> - `compute_ts_params`: Computes timeseries constants (contraction time, relaxation time, flat time, period, offset)
-> - `create_spatial_graph`: Generates a spatial graph of tracked z-discs where edges indicate sarcomeres and edge weights indicate the ratio of the frames in which each sarcomere is detected
-
-- `Visualization`: Visualize detected sarcomeres information
-
-> - `zdiscs_and_sarcs`: Visualizes detected z-discs and sarcomeres in the chosen frame
-> - `contraction`:Visualizes detected sarcomeres in every frame as a gif file
-> - `normalized_sarcs_length`: Plots normalized length of all detected sarcomeres vs frame number
-> - `OOP`: Plots recovered Orientational Order Parameter
-> - `F`: Plots recovered deformation gradient
-> - `J`: Plots recovered deformation jacobian
-> - `F_eigenval_animation`: Visualizes the eigenvalues of F vs frame number
-> - `timeseries_params`: Visualizes time series parameters
-> - `dendrogram`: Clusters timeseries and plots as a dendrogram of the clusters
-> - `spatial_graph`: Visualizes the spatial graph
-> - `tracked_vs_untracked`: Visualizes metrics that compare the effect of tracking sarcomeres in a video vs only detecting sarcomeres in each frame without tracking
-
-To use this module an object of the class `SarcGraphTools` should be created by setting the `input_dir` to the folder that contains the output saved from running full sarcomere detection and timeseries processing on the input data.
-
-## Validation <a name="validation"></a>
-
-To validate our methods and ensure correct implementation, we generated challenging synthetic videos with characteristics similar to beating hiPSC-CMs. We used these videos to evaluate the sarcomere detection algorithm by comparing recovered metrics to their known ground truth. The figure shows this process for one of many tested validation examples.
-
-<br />
-<center><img src="figures/validation.png" width=75%></center>
-<br />
-
-## References to Related Work <a name="references"></a>
-
-* Zhao, B., Zhang, K., Chen, C. S., & Lejeune, E. (2021). Sarc-graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Computational Biology, 17(10), e1009443.
-
-* Allan, D. B., Caswell, T., Keim, N. C., Wel, C. M. van der, & Verweij, R. W. (2023). Soft-matter/trackpy: v0.6.1 (Version v0.6.1). Zenodo. https://doi.org/10.5281/zenodo.7670439
-
-* Toepfer, C. N., Sharma, A., Cicconet, M., Garfinkel, A. C., MÃ¼cke, M., Neyazi, M., Willcox, J. A., Agarwal, R., Schmid, M., Rao, J., & others. (2019). SarcTrack: An adaptable software tool for efficient large-scale analysis of sarcomere function in hiPSC-cardiomyocytes. Circulation Research, 124(8), 1172â€“1183.
-
-* Morris, T. A., Naik, 94 J., Fibben, K. S., Kong, X., Kiyono, T., Yokomori, K., & Grosberg, A. (2020). Striated myocyte structural integrity: Automated analysis of sarcomeric z-discs. PLoS Computational Biology, 16(3), e1007676.
-
-* Pasqualin, C., Gannier, F., Yu, A., MalÃ©cot, C. O., Bredeloux, P., & Maupoil, V. (2016). SarcOptiM for ImageJ: High-frequency online sarcomere length computing on stimulated cardiomyocytes. American Journal of Physiology-Cell Physiology, 311(2), C277â€“C283.
-
-* Ribeiro, A. J. S., Schwab, O., Mandegar, M. A., Ang, Y.-S., Conklin, B. R., Srivastava, D., & Pruitt, B. L. (2017). Multi-imaging method to assay the contractile mechanical output of micropatterned human iPSC-derived cardiac myocytes. Circulation Research, 120(10), 1572â€“1583. https://doi.org/10.1161/CIRCRESAHA.116.310363
-
-## Contact Information <a name="contact"></a>
-
-For information about this software, please get in touch with [Saeed Mohammadzadeh](mailto:saeedmhz@bu.edu) or [Emma Lejeune](mailto:elejeune@bu.edu).
-
-## Acknowledgements <a name="acknowledge"></a>
+Metadata-Version: 2.1
+Name: sarcgraph
+Version: 0.2.1
+Summary: A software for sarcomere detection and tracking
+Home-page: https://pypi.org/project/sarcgraph/
+Author: Saeed Mohammadzadeh
+Author-email: saeedmhz@bu.edu
+Maintainer: [('Saeed Mohammadzadeh', 'saeedmhz@bu.edu'), ('Emma Lejeune', 'elejeune@bu.edu')]
+License: MIT
+Project-URL: Source, https://github.com/Sarc-Graph/sarcgraph
+Project-URL: Documentation, https://sarc-graph.readthedocs.io/en/latest/
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **SarcGraph**
+
+[![python](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/) ![os](https://img.shields.io/badge/os-ubuntu%20|%20macos%20|%20windows-blue.svg) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Sarc-Graph/sarcgraph#license)
+
+[![flake8](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml/badge.svg)](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml) [![codecov](https://codecov.io/gh/Sarc-Graph/sarcgraph/branch/main/graph/badge.svg?token=XNE85EJ4GX)](https://codecov.io/gh/Sarc-Graph/sarcgraph) [![Documentation Status](https://readthedocs.org/projects/sarc-graph/badge/?version=latest)](https://sarc-graph.readthedocs.io/en/latest/?badge=latest)
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Sarc-Graph/sarcgraph/main)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7963553.svg)](https://doi.org/10.5281/zenodo.7963553)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05322/status.svg)](https://doi.org/10.21105/joss.05322)
+
+## **Table of Contents**
+* [Project Summary](#summary)
+* [Installation Instructions](#install)
+* [Contents](#contents)
+* [Tutorial](#tutorial) - [Notebooks](https://github.com/Sarc-Graph/sarcgraph/tree/main/tutorials)
+* [Validation](#validation)
+* [References to Related Work](#references)
+* [Contact Information](#contact)
+* [Acknowledgements](#acknowledge)
+
+## **Project Summary** <a name="summary"></a>
+
+**SarcGraph** is a tool for automatic detection, tracking and analysis of
+z-discs and sarcomeres in movies of beating *human induced pluripotent stem
+cell-derived cardiomyocytes (hiPSC-CMs)*.
+
+<br />
+<center><img src="figures/intro.png" width=30%></center>
+<br />
+
+SarcGraph was initially introduced in [Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443).
+This package is created to make SarcGraph more accessible to the broader
+research community.
+
+**For more information visit [SarcGraph documentation](https://sarc-graph.readthedocs.io/en/latest/).**
+
+## **Installation Instructions** <a name="install"></a>
+
+### **Stable Version** <a name="install-stable"></a>
+
+#### From Conda
+
+Follow the instructions to install [Anaconda](https://www.anaconda.com/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
+
+Create a new Conda envirnoment and install sarcgraph.
+
+```bash
+conda create --name sarcgraph-env -c conda-forge -c saeedmhz sarcgraph
+```
+
+**Note:** Type ``y`` and press ``Enter`` when prompted.
+
+Activate the environment.
+
+```bash
+conda activate sarcgraph-env
+```
+#### From PyPI
+
+Please check the [Getting Started](https://sarc-graph.readthedocs.io/en/latest/installation.html) section in the documentation.
+
+### **Developer's Version** <a name="install-dev"></a>
+
+#### **Get a copy of the [SarcGraph repository](https://github.com/Sarc-Graph/sarcgraph) on your local machine**
+
+You can do this by clicking the green ``<> code`` button and selecting ``Download Zip`` or by running the following command in terminal and move to the directory of the ``sarcgraph`` repository.:
+
+```bash
+git clone https://github.com/Sarc-Graph/sarcgraph.git
+cd sarcgraph
+```
+
+#### **Create and activate a conda virtual environment**
+
+1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
+
+2. Type the following command in terminal to create a virtual envirnoment and install the required packages:
+
+```bash
+conda env create --file=environment.yml
+```
+
+3. Activate your virtual environment.
+
+```bash
+conda activate sarcgraph
+```
+
+#### **Install SarcGraph**
+
+Install SarcGraph in editable mode:
+
+```bash
+pip install -e .
+```
+
+## **Contents** <a name="contents"></a>
+
+```bash
+|___ sarcgraph
+|        |___ docs/
+|        |___ figures/
+|                |___ *.png
+|        |___ samples/
+|        |___ sarcgraph/
+|                |___ __init__.py
+|                |___ sg.py
+|                |___ sg_tools.py
+|        |___ tests/
+|        |___ tutorials/
+|                |___ *.ipynb
+```
+
+## **Tutorial** <a name="tutorial"></a>
+
+This GitHub repository contains a folder called ``tutorials`` that contains demos to extensively show how this package can be used to analyze videos or images of hiPSC-CMs.
+
+### **Package Contents** <a name="whats-in-package"></a>
+
+The package contains two seperate modules: `sg` for sarcomere detection and tracking and `sg_tools` for running further analysis and visualizations.
+
+#### **sarcgraph.sg** <a name="sarcgraph.py"></a>
+`sarcgraph.sg` module takes a video/image file as input (more details in tutorials). This module then processes the input file to detect and track z-discs and sarcomeres through running 3 tasks:
+
+ - Z-disc Segmentation,
+ - Z-disc Tracking,
+ - Sarcomere Detection.
+
+Here is a list of functions developed for each task:
+
+- `zdisc_segmentation`: Detect z-discs in each frame of the input video/image and saves the following information into a pandas `DataFrame`:
+
+> - `frame`: (frame number) 
+> - `x` and `y`: (X and Y position of the center of a z-disc)
+> - `p1_x`, `p1_y` and `p2_x`, `p2_y`: (X and Y position of both ends of a z-disc)
+
+- `zdisc_tracking`: Tracks detected z-discs in the input video over all frames and adds the following information to the pandas `DataFrame`:
+
+> - `particle`: (z-disc id)
+> - `freq`: (number of frames in which a z-discs is tracked)
+frame,sarc_id,x,y,length,width,angle,z-discs
+
+- `sarcomere_detection`: Detects sarcomeres in the input video/image using tracked z-discs `DataFrame` and saves the following information into a new pandas `DataFrame`:
+
+> - `frame`: (frame number)
+> - `sarc_id`: (sarcomere id)
+> - `x` and `y`: (X and Y position of the center of a sarcomere)
+> - `length`: (sarcomere length)
+> - `width`: (sarcomere width)
+> - `angle`: (sarcomere angle)
+> - `zdiscs`: (ids of the two z-discs forming a sarcomere)
+
+
+#### **sarcgraph.sg_tools** <a name="sarcgraph_tools.py"></a>
+
+`sarcgraph.sg_tools` module consists of 3 subclasses:
+
+- `TimeSeries`: Process timeseries of detected and tracked sarcomeres
+
+> - `sarcomeres_gpr()`: Applies Gaussian Process Regression (GPR) on each recovered timeseries characteristic of all detected sarcomeres to reduce the noise and fill in the missing data
+
+- `Analysis`: Extract more information from detected sarcomeres characteristics timeseries
+
+> - `compute_F_J`: Computes the average deformation gradient (F) and its jacobian (J)
+> - `compute_OOP`: Computes the Orientation Order Parameter (OOP)
+> - `compute_metrics`: Computes {OOP, C_iso, C_OOP, s_til, s_avg} as defined in the [SarcGraph paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443)
+> - `compute_ts_params`: Computes timeseries constants (contraction time, relaxation time, flat time, period, offset)
+> - `create_spatial_graph`: Generates a spatial graph of tracked z-discs where edges indicate sarcomeres and edge weights indicate the ratio of the frames in which each sarcomere is detected
+
+- `Visualization`: Visualize detected sarcomeres information
+
+> - `zdiscs_and_sarcs`: Visualizes detected z-discs and sarcomeres in the chosen frame
+> - `contraction`:Visualizes detected sarcomeres in every frame as a gif file
+> - `normalized_sarcs_length`: Plots normalized length of all detected sarcomeres vs frame number
+> - `OOP`: Plots recovered Orientational Order Parameter
+> - `F`: Plots recovered deformation gradient
+> - `J`: Plots recovered deformation jacobian
+> - `F_eigenval_animation`: Visualizes the eigenvalues of F vs frame number
+> - `timeseries_params`: Visualizes time series parameters
+> - `dendrogram`: Clusters timeseries and plots as a dendrogram of the clusters
+> - `spatial_graph`: Visualizes the spatial graph
+> - `tracked_vs_untracked`: Visualizes metrics that compare the effect of tracking sarcomeres in a video vs only detecting sarcomeres in each frame without tracking
+
+To use this module an object of the class `SarcGraphTools` should be created by setting the `input_dir` to the folder that contains the output saved from running full sarcomere detection and timeseries processing on the input data.
+
+## Validation <a name="validation"></a>
+
+To validate our methods and ensure correct implementation, we generated challenging synthetic videos with characteristics similar to beating hiPSC-CMs. We used these videos to evaluate the sarcomere detection algorithm by comparing recovered metrics to their known ground truth. The figure shows this process for one of many tested validation examples.
+
+<br />
+<center><img src="figures/validation.png" width=75%></center>
+<br />
+
+## References to Related Work <a name="references"></a>
+
+* Zhao, B., Zhang, K., Chen, C. S., & Lejeune, E. (2021). Sarc-graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Computational Biology, 17(10), e1009443.
+
+* Allan, D. B., Caswell, T., Keim, N. C., Wel, C. M. van der, & Verweij, R. W. (2023). Soft-matter/trackpy: v0.6.1 (Version v0.6.1). Zenodo. https://doi.org/10.5281/zenodo.7670439
+
+* Toepfer, C. N., Sharma, A., Cicconet, M., Garfinkel, A. C., Mücke, M., Neyazi, M., Willcox, J. A., Agarwal, R., Schmid, M., Rao, J., & others. (2019). SarcTrack: An adaptable software tool for efficient large-scale analysis of sarcomere function in hiPSC-cardiomyocytes. Circulation Research, 124(8), 1172–1183.
+
+* Morris, T. A., Naik, 94 J., Fibben, K. S., Kong, X., Kiyono, T., Yokomori, K., & Grosberg, A. (2020). Striated myocyte structural integrity: Automated analysis of sarcomeric z-discs. PLoS Computational Biology, 16(3), e1007676.
+
+* Pasqualin, C., Gannier, F., Yu, A., Malécot, C. O., Bredeloux, P., & Maupoil, V. (2016). SarcOptiM for ImageJ: High-frequency online sarcomere length computing on stimulated cardiomyocytes. American Journal of Physiology-Cell Physiology, 311(2), C277–C283.
+
+* Ribeiro, A. J. S., Schwab, O., Mandegar, M. A., Ang, Y.-S., Conklin, B. R., Srivastava, D., & Pruitt, B. L. (2017). Multi-imaging method to assay the contractile mechanical output of micropatterned human iPSC-derived cardiac myocytes. Circulation Research, 120(10), 1572–1583. https://doi.org/10.1161/CIRCRESAHA.116.310363
+
+## Contact Information <a name="contact"></a>
+
+For information about this software, please get in touch with [Saeed Mohammadzadeh](mailto:saeedmhz@bu.edu) or [Emma Lejeune](mailto:elejeune@bu.edu).
+
+## Acknowledgements <a name="acknowledge"></a>
```

### Comparing `sarcgraph-0.1.1/README.md` & `sarcgraph-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,183 +1,212 @@
-# **SarcGraph**
-
-[![python](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/) ![os](https://img.shields.io/badge/os-ubuntu%20|%20macos%20|%20windows-blue.svg) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Sarc-Graph/sarcgraph#license)
-
-[![flake8](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml/badge.svg)](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml) [![codecov](https://codecov.io/gh/Sarc-Graph/sarcgraph/branch/main/graph/badge.svg?token=XNE85EJ4GX)](https://codecov.io/gh/Sarc-Graph/sarcgraph) [![Documentation Status](https://readthedocs.org/projects/sarc-graph/badge/?version=latest)](https://sarc-graph.readthedocs.io/en/latest/?badge=latest)
-
-## **Table of Contents**
-* [Project Summary](#summary)
-* [Installation Instructions](#install)
-* [Contents](#contents)
-* [Tutorial](#tutorial) - [Notebooks](https://github.com/Sarc-Graph/sarcgraph/tree/main/tutorials)
-* [Validation](#validation)
-* [References to Related Work](#references)
-* [Contact Information](#contact)
-* [Acknowledgements](#acknowledge)
-
-## **Project Summary** <a name="summary"></a>
-
-**SarcGraph** is a tool for automatic detection, tracking and analysis of
-z-discs and sarcomeres in movies of beating *human induced pluripotent stem
-cell-derived cardiomyocytes (hiPSC-CMs)*.
-
-<br />
-<center><img src="figures/intro.png" width=30%></center>
-<br />
-
-SarcGraph was initially introduced in [Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443).
-This package is created to make SarcGraph more accessible to the broader
-research community.
-
-**For more information visit [SarcGraph documentation](https://sarc-graph.readthedocs.io/en/latest/).**
-
-## **Installation Instructions** <a name="install"></a>
-
-### **Get a copy of the [SarcGraph repository](https://github.com/Sarc-Graph/sarcgraph) on your local machine**
-
-You can do this by clicking the green ``<> code`` button and selecting ``Download Zip`` or by running the following command in terminal:
-
-```bash
-git clone https://github.com/Sarc-Graph/sarcgraph.git
-```
-
-### **Create and activate a conda virtual environment**
-
-1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
-
-2. Open a terminal and move to the directory of the ``sarcgraph`` repository. Then, type the following command in terminal to create a virtual envirnoment and install the required packages:
-
-```bash
-cd sarcgraph
-conda env create --file=environment.yml
-```
-
-3. Activate your virtual environment.
-
-```bash
-conda activate sarcgraph
-```
-
-### **Install SarcGraph**
-
-SarcGraph can be installed using ``pip``:
-
-```bash
-pip install sarcgraph
-```
-
-## **Contents** <a name="contents"></a>
-
-```bash
-|___ sarcgraph
-|        |___ docs/
-|        |___ figures/
-|                |___ *.png
-|        |___ samples/
-|        |___ sarcgraph/
-|                |___ __init__.py
-|                |___ sg.py
-|                |___ sg_tools.py
-|        |___ tests/
-|        |___ tutorials/
-|                |___ *.ipynb
-```
-
-## **Tutorial** <a name="tutorial"></a>
-
-This GitHub repository contains a folder called ``tutorials`` that contains demos to extensively show how this package can be used to analyze videos or images of hiPSC-CMs.
-
-### **Package Contents** <a name="whats-in-package"></a>
-
-The package contains two seperate modules: `sg` for sarcomere detection and tracking and `sg_tools` for running further analysis and visualizations.
-
-#### **sarcgraph.sg** <a name="sarcgraph.py"></a>
-`sarcgraph.sg` module takes a video/image file as input (more details in tutorials). This module then processes the input file to detect and track z-discs and sarcomeres through running 3 tasks:
-
- - Z-disc Segmentation,
- - Z-disc Tracking,
- - Sarcomere Detection.
-
-Here is a list of functions developed for each task:
-
-- `zdisc_segmentation`: Detect z-discs in each frame of the input video/image and saves the following information into a pandas `DataFrame`:
-
-> - `frame`: (frame number) 
-> - `x` and `y`: (X and Y position of the center of a z-disc)
-> - `p1_x`, `p1_y` and `p2_x`, `p2_y`: (X and Y position of both ends of a z-disc)
-
-- `zdisc_tracking`: Tracks detected z-discs in the input video over all frames and adds the following information to the pandas `DataFrame`:
-
-> - `particle`: (z-disc id)
-> - `freq`: (number of frames in which a z-discs is tracked)
-frame,sarc_id,x,y,length,width,angle,z-discs
-
-- `sarcomere_detection`: Detects sarcomeres in the input video/image using tracked z-discs `DataFrame` and saves the following information into a new pandas `DataFrame`:
-
-> - `frame`: (frame number)
-> - `sarc_id`: (sarcomere id)
-> - `x` and `y`: (X and Y position of the center of a sarcomere)
-> - `length`: (sarcomere length)
-> - `width`: (sarcomere width)
-> - `angle`: (sarcomere angle)
-> - `zdiscs`: (ids of the two z-discs forming a sarcomere)
-
-
-#### **sarcgraph.sg_tools** <a name="sarcgraph_tools.py"></a>
-
-`sarcgraph.sg_tools` module consists of 3 subclasses:
-
-- `TimeSeries`: Process timeseries of detected and tracked sarcomeres
-
-> - `sarcomeres_gpr()`: Applies Gaussian Process Regression (GPR) on each recovered timeseries characteristic of all detected sarcomeres to reduce the noise and fill in the missing data
-
-- `Analysis`: Extract more information from detected sarcomeres characteristics timeseries
-
-> - `compute_F_J`: Computes the average deformation gradient (F) and its jacobian (J)
-> - `compute_OOP`: Computes the Orientation Order Parameter (OOP)
-> - `compute_metrics`: Computes {OOP, C_iso, C_OOP, s_til, s_avg} as defined in the [SarcGraph paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443)
-> - `compute_ts_params`: Computes timeseries constants (contraction time, relaxation time, flat time, period, offset)
-> - `create_spatial_graph`: Generates a spatial graph of tracked z-discs where edges indicate sarcomeres and edge weights indicate the ratio of the frames in which each sarcomere is detected
-
-- `Visualization`: Visualize detected sarcomeres information
-
-> - `zdiscs_and_sarcs`: Visualizes detected z-discs and sarcomeres in the chosen frame
-> - `contraction`:Visualizes detected sarcomeres in every frame as a gif file
-> - `normalized_sarcs_length`: Plots normalized length of all detected sarcomeres vs frame number
-> - `OOP`: Plots recovered Orientational Order Parameter
-> - `F`: Plots recovered deformation gradient
-> - `J`: Plots recovered deformation jacobian
-> - `F_eigenval_animation`: Visualizes the eigenvalues of F vs frame number
-> - `timeseries_params`: Visualizes time series parameters
-> - `dendrogram`: Clusters timeseries and plots as a dendrogram of the clusters
-> - `spatial_graph`: Visualizes the spatial graph
-> - `tracked_vs_untracked`: Visualizes metrics that compare the effect of tracking sarcomeres in a video vs only detecting sarcomeres in each frame without tracking
-
-To use this module an object of the class `SarcGraphTools` should be created by setting the `input_dir` to the folder that contains the output saved from running full sarcomere detection and timeseries processing on the input data.
-
-## Validation <a name="validation"></a>
-
-To validate our methods and ensure correct implementation, we generated challenging synthetic videos with characteristics similar to beating hiPSC-CMs. We used these videos to evaluate the sarcomere detection algorithm by comparing recovered metrics to their known ground truth. The figure shows this process for one of many tested validation examples.
-
-<br />
-<center><img src="figures/validation.png" width=75%></center>
-<br />
-
-## References to Related Work <a name="references"></a>
-
-* Zhao, B., Zhang, K., Chen, C. S., & Lejeune, E. (2021). Sarc-graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Computational Biology, 17(10), e1009443.
-
-* Allan, D. B., Caswell, T., Keim, N. C., Wel, C. M. van der, & Verweij, R. W. (2023). Soft-matter/trackpy: v0.6.1 (Version v0.6.1). Zenodo. https://doi.org/10.5281/zenodo.7670439
-
-* Toepfer, C. N., Sharma, A., Cicconet, M., Garfinkel, A. C., Mücke, M., Neyazi, M., Willcox, J. A., Agarwal, R., Schmid, M., Rao, J., & others. (2019). SarcTrack: An adaptable software tool for efficient large-scale analysis of sarcomere function in hiPSC-cardiomyocytes. Circulation Research, 124(8), 1172–1183.
-
-* Morris, T. A., Naik, 94 J., Fibben, K. S., Kong, X., Kiyono, T., Yokomori, K., & Grosberg, A. (2020). Striated myocyte structural integrity: Automated analysis of sarcomeric z-discs. PLoS Computational Biology, 16(3), e1007676.
-
-* Pasqualin, C., Gannier, F., Yu, A., Malécot, C. O., Bredeloux, P., & Maupoil, V. (2016). SarcOptiM for ImageJ: High-frequency online sarcomere length computing on stimulated cardiomyocytes. American Journal of Physiology-Cell Physiology, 311(2), C277–C283.
-
-* Ribeiro, A. J. S., Schwab, O., Mandegar, M. A., Ang, Y.-S., Conklin, B. R., Srivastava, D., & Pruitt, B. L. (2017). Multi-imaging method to assay the contractile mechanical output of micropatterned human iPSC-derived cardiac myocytes. Circulation Research, 120(10), 1572–1583. https://doi.org/10.1161/CIRCRESAHA.116.310363
-
-## Contact Information <a name="contact"></a>
-
-For information about this software, please get in touch with [Saeed Mohammadzadeh](mailto:saeedmhz@bu.edu) or [Emma Lejeune](mailto:elejeune@bu.edu).
-
-## Acknowledgements <a name="acknowledge"></a>
+# **SarcGraph**
+
+[![python](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/) ![os](https://img.shields.io/badge/os-ubuntu%20|%20macos%20|%20windows-blue.svg) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Sarc-Graph/sarcgraph#license)
+
+[![flake8](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml/badge.svg)](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml) [![codecov](https://codecov.io/gh/Sarc-Graph/sarcgraph/branch/main/graph/badge.svg?token=XNE85EJ4GX)](https://codecov.io/gh/Sarc-Graph/sarcgraph) [![Documentation Status](https://readthedocs.org/projects/sarc-graph/badge/?version=latest)](https://sarc-graph.readthedocs.io/en/latest/?badge=latest)
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Sarc-Graph/sarcgraph/main)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7963553.svg)](https://doi.org/10.5281/zenodo.7963553)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05322/status.svg)](https://doi.org/10.21105/joss.05322)
+
+## **Table of Contents**
+* [Project Summary](#summary)
+* [Installation Instructions](#install)
+* [Contents](#contents)
+* [Tutorial](#tutorial) - [Notebooks](https://github.com/Sarc-Graph/sarcgraph/tree/main/tutorials)
+* [Validation](#validation)
+* [References to Related Work](#references)
+* [Contact Information](#contact)
+* [Acknowledgements](#acknowledge)
+
+## **Project Summary** <a name="summary"></a>
+
+**SarcGraph** is a tool for automatic detection, tracking and analysis of
+z-discs and sarcomeres in movies of beating *human induced pluripotent stem
+cell-derived cardiomyocytes (hiPSC-CMs)*.
+
+<br />
+<center><img src="figures/intro.png" width=30%></center>
+<br />
+
+SarcGraph was initially introduced in [Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443).
+This package is created to make SarcGraph more accessible to the broader
+research community.
+
+**For more information visit [SarcGraph documentation](https://sarc-graph.readthedocs.io/en/latest/).**
+
+## **Installation Instructions** <a name="install"></a>
+
+### **Stable Version** <a name="install-stable"></a>
+
+#### From Conda
+
+Follow the instructions to install [Anaconda](https://www.anaconda.com/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
+
+Create a new Conda envirnoment and install sarcgraph.
+
+```bash
+conda create --name sarcgraph-env -c conda-forge -c saeedmhz sarcgraph
+```
+
+**Note:** Type ``y`` and press ``Enter`` when prompted.
+
+Activate the environment.
+
+```bash
+conda activate sarcgraph-env
+```
+#### From PyPI
+
+Please check the [Getting Started](https://sarc-graph.readthedocs.io/en/latest/installation.html) section in the documentation.
+
+### **Developer's Version** <a name="install-dev"></a>
+
+#### **Get a copy of the [SarcGraph repository](https://github.com/Sarc-Graph/sarcgraph) on your local machine**
+
+You can do this by clicking the green ``<> code`` button and selecting ``Download Zip`` or by running the following command in terminal and move to the directory of the ``sarcgraph`` repository.:
+
+```bash
+git clone https://github.com/Sarc-Graph/sarcgraph.git
+cd sarcgraph
+```
+
+#### **Create and activate a conda virtual environment**
+
+1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
+
+2. Type the following command in terminal to create a virtual envirnoment and install the required packages:
+
+```bash
+conda env create --file=environment.yml
+```
+
+3. Activate your virtual environment.
+
+```bash
+conda activate sarcgraph
+```
+
+#### **Install SarcGraph**
+
+Install SarcGraph in editable mode:
+
+```bash
+pip install -e .
+```
+
+## **Contents** <a name="contents"></a>
+
+```bash
+|___ sarcgraph
+|        |___ docs/
+|        |___ figures/
+|                |___ *.png
+|        |___ samples/
+|        |___ sarcgraph/
+|                |___ __init__.py
+|                |___ sg.py
+|                |___ sg_tools.py
+|        |___ tests/
+|        |___ tutorials/
+|                |___ *.ipynb
+```
+
+## **Tutorial** <a name="tutorial"></a>
+
+This GitHub repository contains a folder called ``tutorials`` that contains demos to extensively show how this package can be used to analyze videos or images of hiPSC-CMs.
+
+### **Package Contents** <a name="whats-in-package"></a>
+
+The package contains two seperate modules: `sg` for sarcomere detection and tracking and `sg_tools` for running further analysis and visualizations.
+
+#### **sarcgraph.sg** <a name="sarcgraph.py"></a>
+`sarcgraph.sg` module takes a video/image file as input (more details in tutorials). This module then processes the input file to detect and track z-discs and sarcomeres through running 3 tasks:
+
+ - Z-disc Segmentation,
+ - Z-disc Tracking,
+ - Sarcomere Detection.
+
+Here is a list of functions developed for each task:
+
+- `zdisc_segmentation`: Detect z-discs in each frame of the input video/image and saves the following information into a pandas `DataFrame`:
+
+> - `frame`: (frame number) 
+> - `x` and `y`: (X and Y position of the center of a z-disc)
+> - `p1_x`, `p1_y` and `p2_x`, `p2_y`: (X and Y position of both ends of a z-disc)
+
+- `zdisc_tracking`: Tracks detected z-discs in the input video over all frames and adds the following information to the pandas `DataFrame`:
+
+> - `particle`: (z-disc id)
+> - `freq`: (number of frames in which a z-discs is tracked)
+frame,sarc_id,x,y,length,width,angle,z-discs
+
+- `sarcomere_detection`: Detects sarcomeres in the input video/image using tracked z-discs `DataFrame` and saves the following information into a new pandas `DataFrame`:
+
+> - `frame`: (frame number)
+> - `sarc_id`: (sarcomere id)
+> - `x` and `y`: (X and Y position of the center of a sarcomere)
+> - `length`: (sarcomere length)
+> - `width`: (sarcomere width)
+> - `angle`: (sarcomere angle)
+> - `zdiscs`: (ids of the two z-discs forming a sarcomere)
+
+
+#### **sarcgraph.sg_tools** <a name="sarcgraph_tools.py"></a>
+
+`sarcgraph.sg_tools` module consists of 3 subclasses:
+
+- `TimeSeries`: Process timeseries of detected and tracked sarcomeres
+
+> - `sarcomeres_gpr()`: Applies Gaussian Process Regression (GPR) on each recovered timeseries characteristic of all detected sarcomeres to reduce the noise and fill in the missing data
+
+- `Analysis`: Extract more information from detected sarcomeres characteristics timeseries
+
+> - `compute_F_J`: Computes the average deformation gradient (F) and its jacobian (J)
+> - `compute_OOP`: Computes the Orientation Order Parameter (OOP)
+> - `compute_metrics`: Computes {OOP, C_iso, C_OOP, s_til, s_avg} as defined in the [SarcGraph paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443)
+> - `compute_ts_params`: Computes timeseries constants (contraction time, relaxation time, flat time, period, offset)
+> - `create_spatial_graph`: Generates a spatial graph of tracked z-discs where edges indicate sarcomeres and edge weights indicate the ratio of the frames in which each sarcomere is detected
+
+- `Visualization`: Visualize detected sarcomeres information
+
+> - `zdiscs_and_sarcs`: Visualizes detected z-discs and sarcomeres in the chosen frame
+> - `contraction`:Visualizes detected sarcomeres in every frame as a gif file
+> - `normalized_sarcs_length`: Plots normalized length of all detected sarcomeres vs frame number
+> - `OOP`: Plots recovered Orientational Order Parameter
+> - `F`: Plots recovered deformation gradient
+> - `J`: Plots recovered deformation jacobian
+> - `F_eigenval_animation`: Visualizes the eigenvalues of F vs frame number
+> - `timeseries_params`: Visualizes time series parameters
+> - `dendrogram`: Clusters timeseries and plots as a dendrogram of the clusters
+> - `spatial_graph`: Visualizes the spatial graph
+> - `tracked_vs_untracked`: Visualizes metrics that compare the effect of tracking sarcomeres in a video vs only detecting sarcomeres in each frame without tracking
+
+To use this module an object of the class `SarcGraphTools` should be created by setting the `input_dir` to the folder that contains the output saved from running full sarcomere detection and timeseries processing on the input data.
+
+## Validation <a name="validation"></a>
+
+To validate our methods and ensure correct implementation, we generated challenging synthetic videos with characteristics similar to beating hiPSC-CMs. We used these videos to evaluate the sarcomere detection algorithm by comparing recovered metrics to their known ground truth. The figure shows this process for one of many tested validation examples.
+
+<br />
+<center><img src="figures/validation.png" width=75%></center>
+<br />
+
+## References to Related Work <a name="references"></a>
+
+* Zhao, B., Zhang, K., Chen, C. S., & Lejeune, E. (2021). Sarc-graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Computational Biology, 17(10), e1009443.
+
+* Allan, D. B., Caswell, T., Keim, N. C., Wel, C. M. van der, & Verweij, R. W. (2023). Soft-matter/trackpy: v0.6.1 (Version v0.6.1). Zenodo. https://doi.org/10.5281/zenodo.7670439
+
+* Toepfer, C. N., Sharma, A., Cicconet, M., Garfinkel, A. C., Mücke, M., Neyazi, M., Willcox, J. A., Agarwal, R., Schmid, M., Rao, J., & others. (2019). SarcTrack: An adaptable software tool for efficient large-scale analysis of sarcomere function in hiPSC-cardiomyocytes. Circulation Research, 124(8), 1172–1183.
+
+* Morris, T. A., Naik, 94 J., Fibben, K. S., Kong, X., Kiyono, T., Yokomori, K., & Grosberg, A. (2020). Striated myocyte structural integrity: Automated analysis of sarcomeric z-discs. PLoS Computational Biology, 16(3), e1007676.
+
+* Pasqualin, C., Gannier, F., Yu, A., Malécot, C. O., Bredeloux, P., & Maupoil, V. (2016). SarcOptiM for ImageJ: High-frequency online sarcomere length computing on stimulated cardiomyocytes. American Journal of Physiology-Cell Physiology, 311(2), C277–C283.
+
+* Ribeiro, A. J. S., Schwab, O., Mandegar, M. A., Ang, Y.-S., Conklin, B. R., Srivastava, D., & Pruitt, B. L. (2017). Multi-imaging method to assay the contractile mechanical output of micropatterned human iPSC-derived cardiac myocytes. Circulation Research, 120(10), 1572–1583. https://doi.org/10.1161/CIRCRESAHA.116.310363
+
+## Contact Information <a name="contact"></a>
+
+For information about this software, please get in touch with [Saeed Mohammadzadeh](mailto:saeedmhz@bu.edu) or [Emma Lejeune](mailto:elejeune@bu.edu).
+
+## Acknowledgements <a name="acknowledge"></a>
```

### Comparing `sarcgraph-0.1.1/sarcgraph/sg.py` & `sarcgraph-0.2.1/sarcgraph/sg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,982 +1,982 @@
-import numpy as np
-import pandas as pd
-import trackpy as tp
-import networkx as nx
-
-import skvideo.io
-import skimage.io
-import skvideo.utils
-
-from skimage.filters import laplace, gaussian, threshold_otsu
-from skimage import measure
-from sklearn.cluster import OPTICS
-from sklearn.neighbors import NearestNeighbors
-from scipy.spatial import distance_matrix
-from pathlib import Path
-from typing import List, Union, Tuple
-
-
-class SarcGraph:
-    def __init__(self, output_dir: str = "test-run", file_type: str = "video"):
-        """Zdiscs and sarcomeres segmentation and tracking.
-
-        Attributes
-        ----------
-        output_dir : str, optional
-            location to save processed information, by default ``'test-run'``
-        file_type : str, optional
-            use ``'image'`` for single-frame samples and ``'video'`` for
-            multi-frame samples, by default ``'video'``
-        """
-        if file_type not in ["video", "image"]:
-            raise ValueError(
-                f"{file_type} is not recognized as a valid file_type. Choose "
-                "from ['video', 'image']."
-            )
-        if not isinstance(output_dir, str):
-            raise TypeError("output_dir must be a string.")
-        Path(f"{output_dir}").mkdir(parents=True, exist_ok=True)
-        self.output_dir = output_dir
-        self.file_type = file_type
-
-    ###########################################################
-    #                    Utility Functions                    #
-    ###########################################################
-    def _data_loader(self, file_path: str) -> np.ndarray:
-        """Loads a video/image file.
-
-        Parameters
-        ----------
-        file_path : str
-            A video/image file address
-
-        Returns
-        -------
-        numpy.ndarray
-            All frames in the raw format
-        """
-        if self.file_type == "video":
-            data = skvideo.io.vread(file_path)
-            if data.shape[0] > 1:
-                return data
-        return skimage.io.imread(file_path)
-
-    def _to_gray(self, frames: np.ndarray) -> np.ndarray:
-        """Convert RGB frames to grayscale.
-
-        Parameters
-        ----------
-        frames : np.ndarray
-            RGB frames
-
-        Returns
-        -------
-        numpy.ndarray
-            All frames in gray scale
-        """
-        frames_gray = skvideo.utils.rgb2gray(frames)
-        if self.file_type == "video" and frames_gray.shape[0] < 2:
-            raise ValueError(
-                "Failed to load video correctly! Manually load the video into "
-                "a numpy array and input to the function as raw_frames."
-            )
-        if self.file_type == "image" and frames_gray.shape[0] > 1:
-            raise ValueError(
-                "Trying to load a video while file_type='image'. Load the "
-                "image manually or change the file_type to 'video."
-            )
-
-        return frames_gray
-
-    def _save_numpy(
-        self, data: Union[List, np.ndarray], file_name: str
-    ) -> None:
-        """Saves a numpy array.
-
-        Parameters
-        ----------
-        data : np.ndarray
-        file_name: str
-        """
-        if not isinstance(file_name, str):
-            raise TypeError("file_name must be a string.")
-        if isinstance(data, np.ndarray) or isinstance(data, List):
-            np.save(
-                f"./{self.output_dir}/{file_name}.npy", data, allow_pickle=True
-            )
-            return
-
-        raise TypeError("data must be a numpy.ndarray or a List.")
-
-    def _save_dataframe(self, data: pd.DataFrame, file_name: str) -> None:
-        """Saves a pandas dataframe.
-
-        Parameters
-        ----------
-        data : pd.DataFrame
-        file_name: str
-        """
-        if not isinstance(file_name, str):
-            raise TypeError("file_name must be a string.")
-        if isinstance(data, pd.DataFrame):
-            data.to_csv(f"./{self.output_dir}/{file_name}.csv")
-            return
-        raise TypeError(
-            f"'data' type is {type(data)}. 'data' must be a pandas DataFrame."
-        )
-
-    def _filter_frames(
-        self, frames: np.ndarray, sigma: float = 1.0
-    ) -> np.ndarray:
-        """Convolves all frames with laplacian and gaussian filters.
-
-        Parameters
-        ----------
-        frames : np.ndarray
-        sigma : float
-            Standard deviation for Gaussian kernel
-
-        Returns
-        -------
-        np.ndarray, shape=(frames, dim_1, dim_2)
-        """
-        if frames.ndim > 4 or frames.ndim < 3:
-            raise ValueError(
-                "Input array must have the shape (frames, dim_1, dim_2, "
-                "channels=1 (optional))"
-            )
-        if frames.ndim == 4:
-            if frames.shape[3] != 1:
-                raise ValueError(
-                    "Number of channels in the input array must be 1. Input "
-                    "shape: (frames, dim_1, dim_2, channels=1 (optional))"
-                )
-            frames = frames[:, :, :, 0]
-        filtered_frames = np.zeros(frames.shape)
-        for i, frame in enumerate(frames):
-            laplacian = laplace(frame)
-            filtered_frames[i] = gaussian(laplacian, sigma=sigma)
-        return filtered_frames
-
-    #############################################################
-    #                    Z-Disc Segmentation                    #
-    #############################################################
-    def _process_input(
-        self,
-        file_path: Union[str, None] = None,
-        raw_frames: Union[np.ndarray, None] = None,
-        sigma: float = 1.0,
-        save_output: bool = True,
-    ) -> np.ndarray:
-        """Loads a video/image and filter all frames.
-
-        Parameters
-        ----------
-        file_path : str
-            The address of an image or a video file to be loaded
-        raw_frames  : np.ndarray, shape=(frames, dim_1, dim_2, channels)
-            Raw input image or video given as a 4 dimensional array
-        sigma : float
-            Standard deviation for Gaussian kernel
-        save_output : bool
-            by default True
-
-        Returns
-        -------
-        np.ndarray, shape=(frames, dim_1, dim_2)
-        """
-        if raw_frames is None:
-            if file_path is None:
-                raise ValueError(
-                    "Either file_path or raw_frames should be given as"
-                    " input."
-                )
-            else:
-                try:
-                    raw_frames = self._data_loader(file_path)
-                except Exception:
-                    raise ValueError(
-                        f"Not able to load a file from {file_path}."
-                    )
-
-        if not isinstance(raw_frames, np.ndarray):
-            raise TypeError("raw_frames must be a numpy array.")
-        raw_frames_gray = self._to_gray(raw_frames)
-        raw_frames_filtered = self._filter_frames(raw_frames_gray, sigma)
-        if save_output:
-            self._save_numpy(raw_frames_gray, file_name="raw-frames")
-            self._save_numpy(raw_frames_filtered, file_name="filtered-frames")
-        return raw_frames_filtered
-
-    def _detect_contours(
-        self,
-        filtered_frames: np.ndarray,
-        min_length: int = 8,
-        save_output: bool = True,
-    ) -> List[np.ndarray]:
-        """Returns contours of detected zdiscs in each frame.
-
-        Parameters
-        ----------
-        filtered_frames : np.ndarray, shape=(frames, dim_1, dim_2)
-        min_length : int
-            Zdisc contours shorter than ``min_length`` pixels will be ignored.
-        save_output : bool
-            by default True
-
-        Notes
-        -----
-        .. warning::
-            Here we use the ``skimage.measure.find_contours`` function to find
-            contours. This function returns contours with coordinates in
-            ``(row, column)`` order, which corresponds to ``(y, x)`` in
-            Cartesian coordinates. Therefore, in the rest of the code, we use
-            ``y`` for the first dimension and ``x`` for the second dimension.
-            For example, for plotting we use ``plt.plot(y, x)``.
-
-        Returns
-        -------
-        List[np.ndarray]
-        """
-        if filtered_frames.ndim != 3:
-            raise ValueError(
-                "The input must be a 3d numpy array: (frames, " "dim 1, dim 2)"
-            )
-        if not isinstance(min_length, int):
-            try:
-                min_length = int(min_length)
-            except ValueError:
-                raise ValueError("min_length must be an integer.") from None
-        length_checker = np.vectorize(len)
-        valid_contours = []
-        for frame in filtered_frames:
-            contour_thresh = threshold_otsu(frame)
-            contours = np.array(
-                measure.find_contours(frame, contour_thresh), dtype="object"
-            )
-            contours_size = list(length_checker(contours))
-            valid_contours.append(
-                contours[np.greater_equal(contours_size, min_length)]
-            )
-        valid_contours = np.array(valid_contours, dtype="object")
-        if save_output:
-            self._save_numpy(valid_contours, file_name="contours")
-        return valid_contours
-
-    def _process_contour(self, contour: Union[List, np.ndarray]) -> np.ndarray:
-        """Computes the center location of a zdisc as well as its two end
-        points given its 2d contour.
-
-        Parameters
-        ----------
-        contour : np.ndarray, shape=(contour_length, 2)
-
-        Returns
-        -------
-        np.ndarray, shape=(6,)
-            zdisc center, end point 1, end point 2
-        """
-        if len(contour) < 3:
-            raise ValueError("A contour must have at least 3 coordinates.")
-        # center of a contour
-        center_coords = np.mean(contour, axis=0)
-        # coordinates of the two points on the contour with maximum distance
-        dist_mat = distance_matrix(contour, contour)
-        indices = np.unravel_index(dist_mat.argmax(), dist_mat.shape)
-        p1, p2 = contour[indices[0]], contour[indices[1]]
-        return np.hstack((center_coords, p1, p2))
-
-    def _zdiscs_to_pandas(self, zdiscs_all: List[np.ndarray]) -> pd.DataFrame:
-        """Creates a pandas dataframe from the information of detected zdiscs
-        in all frames.
-
-        Parameters
-        ----------
-        zdiscs_all : List[np.ndarray]
-            A list of numpy arrays each containing information of detected
-            zdiscs in a frame, (zdisc center, end point 1, end point 2)
-
-        Returns
-        -------
-        pd.DataFrame
-            Columns are ``frame`` (frame number), ``x`` and ``y`` (zdiscs
-            center position), ``p1_x``, ``p1_y``, ``p2_x``, ``p2_y`` (zdiscs
-            end points positions).
-        """
-        if self.file_type == "video" and len(zdiscs_all) < 2:
-            raise ValueError(
-                "Only one frame detected. Video is not loaded correctly."
-            )
-        if self.file_type == "image" and len(zdiscs_all) > 1:
-            raise ValueError(
-                "More than one frame detected. The image is not loaded "
-                "correctly."
-            )
-        data_frame = []
-        for i, zdiscs_frame in enumerate(zdiscs_all):
-            if type(zdiscs_frame) != np.ndarray:
-                raise TypeError("Input should be a list of numpy arrays.")
-            if zdiscs_frame.ndim != 2 or zdiscs_frame.shape[1] != 6:
-                raise ValueError(
-                    "Each numpy array must have the shape: (number of zdiscs, "
-                    "6)"
-                )
-            frame_id = i * np.ones((len(zdiscs_frame), 1), dtype=int)
-            zdiscs_frame_extended = np.hstack((frame_id, zdiscs_frame))
-            data_frame.append(
-                pd.DataFrame(
-                    zdiscs_frame_extended,
-                    columns=[
-                        "frame",
-                        "x",
-                        "y",
-                        "p1_x",
-                        "p1_y",
-                        "p2_x",
-                        "p2_y",
-                    ],
-                )
-            )
-        return pd.concat(data_frame)
-
-    def zdisc_segmentation(
-        self,
-        file_path: Union[str, None] = None,
-        raw_frames: Union[np.ndarray, None] = None,
-        sigma: float = 1.0,
-        min_length: int = 8,
-        save_output: bool = True,
-    ) -> pd.DataFrame:
-        """Finds Z-Discs in a video/image and extracts related information,
-        (frame number, center position, end points).
-
-        Parameters
-        ----------
-        file_path : str
-            address of the input video/image file
-        raw_frames  : np.ndarray, shape=(frames, dim_1, dim_2, channels)
-            Raw input image or video given as a 4 dimensional array
-        sigma : float
-            Standard deviation for Gaussian kernel
-        min_length : int
-            Minimum length for zdisc contours measured in pixels
-        save_output : bool
-            by default True
-
-        Returns
-        -------
-        pd.DataFrame
-            Information of all detected zdiscs in every frame. Columns are
-            ``'frame'`` (frame number), ``'x'`` and ``'y'`` (zdiscs center
-            position), ``'p1_x'``, ``'p1_y'``, ``'p2_x'``, ``'p2_y'`` (zdiscs
-            end points positions).
-        """
-        filtered_frames = self._process_input(
-            file_path, raw_frames, sigma, save_output
-        )
-        contours_all = self._detect_contours(
-            filtered_frames, min_length, save_output
-        )
-        zdiscs_all = []
-        for contours_frame in contours_all:
-            zdiscs_frame = np.zeros((len(contours_frame), 6))
-            for i, contour in enumerate(contours_frame):
-                zdiscs_frame[i] = self._process_contour(contour)
-            zdiscs_all.append(zdiscs_frame)
-        zdiscs_all_dataframe = self._zdiscs_to_pandas(zdiscs_all)
-        if save_output:
-            self._save_dataframe(
-                zdiscs_all_dataframe, file_name="segmented-zdiscs"
-            )
-        return zdiscs_all_dataframe
-
-    #########################################################
-    #                    Z-disc Tracking                    #
-    #########################################################
-    def _merge_tracked_zdiscs(
-        self,
-        tracked_zdiscs: pd.DataFrame,
-        full_track_ratio: float = 0.75,
-    ) -> pd.DataFrame:
-        """A post processing step to group related partially tracked zdiscs
-        using the OPTICS algorithm. Increases the robustness of zdisc tracking
-        as well as the number of fully tracked zdiscs.
-
-        Parameters
-        ----------
-        tracked_zdiscs : pd.DataFrame
-            tracked zdiscs information for all frames
-        full_track_ratio : float, optional
-            If a tracked zdisc appears in enough number of frames defined by
-            this ratio, it is considered a fully tracked zdisc. The default
-            value 0.75 means if a zdisc is tracked in more than 75 percent of
-            all frames it is fully tracked.
-
-        Returns
-        -------
-        pd.DataFrame
-
-        Notes
-        -----
-        For a detailed description of the OPTICS algorithm check:
-        https://scikit-learn.org/stable/modules/generated/sklearn.cluster.OPTICS.html
-        """
-        num_frames = tracked_zdiscs.frame.max() + 1
-        tracked_zdiscs_grouped = tracked_zdiscs.groupby("particle")["particle"]
-        tracked_zdiscs["freq"] = tracked_zdiscs_grouped.transform("count")
-        fully_tracked_zdiscs = tracked_zdiscs.loc[
-            tracked_zdiscs.freq == num_frames
-        ]
-        partially_tracked_zdiscs = tracked_zdiscs.loc[
-            tracked_zdiscs.freq < num_frames
-        ]
-
-        if partially_tracked_zdiscs.empty:
-            return fully_tracked_zdiscs
-
-        partially_tracked_clusters = (
-            partially_tracked_zdiscs[["x", "y", "particle"]]
-            .groupby(by=["particle"])
-            .mean()
-        )
-
-        # merge related clusters (neighbors)
-        all_clusters_xy = (
-            tracked_zdiscs.groupby("particle").mean()[["x", "y"]].to_numpy()
-        )
-        clusters_min_dist = np.min(
-            distance_matrix(all_clusters_xy, all_clusters_xy)
-            + 1e6 * np.eye(len(all_clusters_xy)),
-            axis=1,
-        )
-        optics_max_eps = np.mean(clusters_min_dist)
-        data = np.array(partially_tracked_clusters)
-        optics_model = OPTICS(max_eps=optics_max_eps, min_samples=2)
-        optics_result = optics_model.fit_predict(data)
-        optics_clusters = np.unique(optics_result)
-
-        all_merged_zdiscs = []
-        for i, optics_cluster in enumerate(optics_clusters):
-            index = np.where(optics_result == optics_cluster)[0]
-            particles_in_cluster = partially_tracked_clusters.iloc[
-                index
-            ].index.to_numpy()
-            if optics_cluster >= 0:
-                merged_zdiscs = (
-                    partially_tracked_zdiscs.loc[
-                        partially_tracked_zdiscs["particle"].isin(
-                            particles_in_cluster
-                        )
-                    ]
-                    .groupby("frame")
-                    .mean()
-                )
-                if len(merged_zdiscs) > num_frames * full_track_ratio:
-                    merged_zdiscs.particle = -(i + 1)
-                    merged_zdiscs.freq = len(merged_zdiscs)
-                    all_merged_zdiscs.append(merged_zdiscs.reset_index())
-            else:
-                for p in particles_in_cluster:
-                    no_merge_zdiscs = partially_tracked_zdiscs.loc[
-                        partially_tracked_zdiscs["particle"] == p
-                    ]
-                    if len(no_merge_zdiscs) > num_frames * full_track_ratio:
-                        all_merged_zdiscs.append(no_merge_zdiscs)
-        if all_merged_zdiscs:
-            all_merged_zdiscs = pd.concat(all_merged_zdiscs)
-            return pd.concat((fully_tracked_zdiscs, all_merged_zdiscs))
-        else:
-            return fully_tracked_zdiscs
-
-    def zdisc_tracking(
-        self,
-        file_path: str = None,
-        raw_frames: np.array = None,
-        segmented_zdiscs: pd.DataFrame = None,
-        sigma: float = 1.0,
-        min_length: int = 8,
-        tp_depth: float = 4.0,
-        full_track_ratio: float = 0.75,
-        skip_merging: bool = False,
-        save_output: bool = True,
-    ) -> pd.DataFrame:
-        """Track detected Z-Discs in a video. The input could be the address to
-        a video/image sample (``file_path``), raw frames as a numpy array
-        (``raw_frames``), or segmented zdiscs information in a pandas datafram
-        (``segmented_zdiscs``)e. If the function is run with no inputs, it will
-        search for 'raw-frames.npy', or 'segmented-zdiscs.csv' in the
-        specified output directory ``SarcGraph().output_dir``.
-
-        Parameters
-        ----------
-        file_path : str
-            The address of an image or a video file to be loaded
-        raw_frames : np.ndarray, shape=(frames, dim_1, dim_2, channels)
-            Raw input image or video given as a 4 dimensional array
-        segmented_zdiscs : pd.DataFrame
-            Information of all detected zdiscs in every frame.
-        sigma : float
-            Standard deviation for Gaussian kernel, by default ``1.0``
-        min_length : int
-            Minimum length for zdisc contours measured in pixels, by default
-            ``8``
-        tp_depth : float, optional
-            the maximum distance features can move between frames, by default
-            ``4.0``
-        full_track_ratio : float, optional
-            by default ``0.75``
-        skip_merging : bool, optional
-            skipping the merging step will result in fewer fully tracked
-            zdiscs, by default ``False``
-        save_output : bool
-            by default ``True``
-
-        Returns
-        -------
-        pd.DataFrame
-            tracked zdiscs information. Columns are ``'frame'`` (frame number),
-            ``'x'`` and ``'y'`` (zdiscs center position), ``'p1_x'``,
-            ``'p1_y'``, ``'p2_x'``, ``'p2_y'`` (zdiscs end points positions),
-            and ``'particle'`` (id of each tracked zdisc).
-
-        Notes
-        -----
-        - If ``SarcGraph().file_type='image'``, tracking will be skipped.
-
-        - For a detailed description of the Trackpy package check:
-            http://soft-matter.github.io/trackpy/v0.5.0/tutorial.html
-
-        - For a detailed description of the OPTICS algorithm check:
-            https://scikit-learn.org/stable/modules/generated/sklearn.cluster.OPTICS.html
-
-        See Also
-        --------
-        :func:`sarcgraph.sg.SarcGraph.zdisc_segmentation`
-
-        :func:`sarcgraph.sg.SarcGraph._merge_tracked_zdiscs`
-
-        """
-        if segmented_zdiscs is None:
-            segmented_zdiscs = self.zdisc_segmentation(
-                file_path, raw_frames, sigma, min_length, save_output
-            )
-
-        if type(segmented_zdiscs) != pd.DataFrame:
-            raise TypeError("segmented_zdiscs shoulb be a dataframe.")
-
-        correct_columns = set(("frame", "x", "y")).issubset(
-            set(segmented_zdiscs.columns)
-        )
-
-        if not correct_columns:
-            raise ValueError(
-                "segmented_zdiscs must contain at least three columns: 'x', "
-                "'y', 'frame'."
-            )
-
-        # skip tracking if the sample is an image
-        if self.file_type == "image":
-            segmented_zdiscs["particle"] = np.arange(len(segmented_zdiscs))
-            tracked_zdiscs = segmented_zdiscs
-        else:
-            # run tracking with the trackpy package:
-            num_frames = len(segmented_zdiscs.frame.unique())
-            t = tp.link_df(
-                segmented_zdiscs, search_range=tp_depth, memory=num_frames
-            )
-            tracked_zdiscs = tp.filter_stubs(t, 2).reset_index(drop=True)
-            if skip_merging is False:
-                tracked_zdiscs = self._merge_tracked_zdiscs(
-                    tracked_zdiscs,
-                    full_track_ratio,
-                )
-
-        if save_output:
-            self._save_dataframe(tracked_zdiscs, "tracked-zdiscs")
-
-        return tracked_zdiscs
-
-    #############################################################
-    #                    Sarcomere Detection                    #
-    #############################################################
-    def _zdisc_to_graph(self, zdiscs: np.array, K: int = 3) -> nx.Graph:
-        """Creates a graph with zdiscs as nodes. Each zdisc is connected to its
-        ``K`` nearest neighbors.
-
-        Parameters
-        ----------
-        zdiscs : np.array, shape=(N, 3)
-            zdiscs information as an array. The first two columns are the x and
-            y location of zdisc centers and the last is the particle id.
-        K : int, optional
-            number of nearest neighbors for each zdisc, by default 3
-
-        Returns
-        -------
-        nx.Graph
-        """
-        num_nodes = len(zdiscs)
-        G = nx.Graph()
-        G.add_nodes_from(range(num_nodes))
-
-        # add the position of each zdisc as a node attribute to the graph
-        nodes_pos_dict = {i: pos for i, pos in enumerate(zdiscs[:, 0:2])}
-        nodes_particle_dict = {j: id for j, id in enumerate(zdiscs[:, -1])}
-
-        nx.set_node_attributes(G, values=nodes_pos_dict, name="pos")
-        nx.set_node_attributes(
-            G, values=nodes_particle_dict, name="particle_id"
-        )
-
-        # find K nearest zdisc to each zdisc
-        neigh = NearestNeighbors(n_neighbors=2)
-        neigh.fit(zdiscs[:, 0:2])
-        nearestNeighbors = neigh.kneighbors(
-            zdiscs[:, 0:2], K + 1, return_distance=False
-        )
-
-        # connect each zdisc to K nearest neighbors
-        edges = []
-        for node, neighbors in enumerate(nearestNeighbors[:, 1:]):
-            for neighbor in neighbors:
-                edges.append((node, neighbor))
-        G.add_edges_from(edges)
-
-        return G
-
-    def _score_graph(
-        self,
-        G: nx.Graph,
-        c_avg_length: float = 1.0,
-        c_angle: float = 1.0,
-        c_length_diff: float = 1.0,
-        l_avg: float = 15.0,
-        l_max: float = 30.0,
-    ) -> nx.Graph:
-        """Assigns a score to each connection of the input graph. Higher score
-        indicates the two corresponding zdiscs are likely to be two ends of a
-        sarcomere.
-
-        Parameters
-        ----------
-        G : nx.Graph
-        c_avg_length : float, optional
-            comparison of the length of a connection with ``l_avg`` affects the
-            connection score, ``c_avg_length`` sets the relative effect of this
-            score metric compared to the other two, by default 1.0
-        c_angle : float, optional
-            the angle between a connection and its neighboring connections
-            affects the connection score, ``c_angle`` sets the relative effect
-            of this score metric compared to the other two, by default 1.0
-        c_length_diff : float, optional
-            comparison of the length of a connection with the length of all
-            neighboring connections affects the score, ``c_length_diff`` sets
-            the relative effect of this score metric compared to the other two,
-            by default 1.0
-        l_avg : float, optional
-            an initial guess for the average length of sarcomeres in pixels, by
-            default 15.0
-        l_max : float, optional
-            Max allowable length for the length of sarcomeres in pixels, by
-            default 30.0
-
-        Returns
-        -------
-        nx.Graph
-            a graph of zdiscs with all connections scored
-        """
-        edges_attr_dict = {}
-        for node in range(G.number_of_nodes()):
-            for neighbor in G.neighbors(node):
-                score = 0
-                v1 = G.nodes[neighbor]["pos"] - G.nodes[node]["pos"]
-                l1 = np.linalg.norm(v1)
-                if l1 <= l_max:
-                    avg_length_score = np.exp(-np.pi * (1 - l1 / l_avg) ** 2)
-                    for far_neighbor in G.neighbors(neighbor):
-                        if far_neighbor in [node, neighbor]:
-                            pass
-                        else:
-                            v2 = (
-                                G.nodes[neighbor]["pos"]
-                                - G.nodes[far_neighbor]["pos"]
-                            )  # vector connecting neighbor to far_neighbor
-                            l2 = np.linalg.norm(v2)
-
-                            d_theta = np.arccos(np.dot(v1, v2) / (l1 * l2)) / (
-                                np.pi / 2
-                            )
-                            d_l = np.abs(l2 - l1) / l1
-
-                            angle_score = (
-                                np.power(1 - d_theta, 2) if d_theta >= 1 else 0
-                            )
-                            diff_length_score = 1 / (1 + d_l)
-
-                            score = np.max(
-                                (
-                                    score,
-                                    c_length_diff * diff_length_score
-                                    + c_angle * angle_score,
-                                )
-                            )
-                    score += c_avg_length * avg_length_score
-                edges_attr_dict[(node, neighbor)] = score
-
-        edges_attr_dict_keep_max = {}
-        for key in edges_attr_dict.keys():
-            node_1 = key[0]
-            node_2 = key[1]
-            max_score = max(
-                edges_attr_dict[(node_1, node_2)],
-                edges_attr_dict[(node_2, node_1)],
-            )
-            edges_attr_dict_keep_max[(min(key), max(key))] = max_score
-        nx.set_edge_attributes(
-            G, values=edges_attr_dict_keep_max, name="score"
-        )
-        return G
-
-    def _prune_graph(
-        self,
-        G: nx.Graph,
-        score_threshold: float = 0.1,
-        angle_threshold: float = 1.2,
-    ) -> nx.Graph:
-        """Prunes the input graph to get rid of invalid or less probable
-        connections.
-
-        Parameters
-        ----------
-        G : nx.Graph
-            A scored graph of zdiscs clusters
-        score_threshold : float
-            any connection with a score less than the threshold will be
-            removed, by default 0.1
-        angle_threshold : float
-            if a zdisc has two valid connection the angle between must be
-            higher than the theshold, otherwise the connection with a lower
-            score will be removed, by default 1.2 (in radians)
-
-        Returns
-        -------
-        nx.Graph
-        """
-        nx.set_edge_attributes(G, values=0, name="validity")
-        for node in range(G.number_of_nodes()):
-            vectors = []
-            scores = []
-            neighbors = list(G.neighbors(node))
-            for neighbor in neighbors:
-                vectors.append(G.nodes[neighbor]["pos"] - G.nodes[node]["pos"])
-                scores.append(G[node][neighbor]["score"])
-
-            # sort by scores
-            if np.max(scores) > score_threshold:
-                sort_indices = np.argsort(scores)[::-1]
-                best_vector = vectors[sort_indices[0]]
-                G[node][neighbors[sort_indices[0]]]["validity"] += 1
-                for idx in sort_indices[1:]:
-                    s = scores[idx]
-                    n = neighbors[idx]
-                    v = vectors[idx]
-
-                    l1 = np.linalg.norm(best_vector)
-                    l2 = np.linalg.norm(v)
-                    theta = np.arccos(np.dot(v, best_vector) / (l1 * l2)) / (
-                        np.pi / 2
-                    )
-
-                    if theta > angle_threshold and s > score_threshold:
-                        G[node][n]["validity"] += 1
-                        break
-
-        edges2remove = []
-        for edge in G.edges():
-            if G.edges[edge]["validity"] < 2:
-                edges2remove.append(edge)
-        G.remove_edges_from(edges2remove)
-
-        return G
-
-    def sarcomere_detection(
-        self,
-        file_path: str = None,
-        raw_frames: np.array = None,
-        segmented_zdiscs: pd.DataFrame = None,
-        tracked_zdiscs: pd.DataFrame = None,
-        sigma: float = 1.0,
-        min_length: int = 8,
-        tp_depth: float = 4.0,
-        full_track_ratio: float = 0.75,
-        skip_merging: bool = False,
-        c_avg_length: float = 1,
-        c_angle: float = 1,
-        c_diff_length: float = 1,
-        l_avg: float = 12.0,
-        score_threshold: float = 0.01,
-        angle_threshold: float = 1.2,
-        save_output: bool = True,
-    ) -> Tuple[pd.DataFrame, List[nx.Graph]]:
-        """Detect sarcomeres in a video/image. The input could be the address
-        to the video/image sample (``file_path``), raw frames as a numpy array
-        (``raw_frames``), segmented zdiscs information in a pandas dataframe
-        (``segmented_zdiscs``), or a dataframe of tracked zdiscs
-        (``tracked_zdiscs``).
-
-        Parameters
-        ----------
-        file_path : str
-            The address of an image or a video file to be loaded
-        raw_frames  : np.ndarray, shape=(frames, dim_1, dim_2, channels)
-            Raw input image or video given as a 4 dimensional array
-        segmented_zdiscs : pd.DataFrame
-            Information of all detected zdiscs in every frame.
-        tracked_zdiscs : pd.DataFrame
-            Information of tracked zdiscs
-        sigma : float
-            Standard deviation for Gaussian kernel, by default ``1.0``
-        min_length : int
-            Minimum length for zdisc contours measured in pixels, by default
-            ``8``
-        tp_depth : float, optional
-            the maximum distance features can move between frames, by default
-            ``4.0``
-        full_track_ratio : float, optional
-            Frame ratio to seperate partially tracked vs fully tracked
-            sarcomeres, by default ``0.75``
-        skip_merging : bool, optional
-            skipping the merging step will result in fewer fully tracked
-            zdiscs, by default ``False``
-        c_avg_length : float, optional
-            comparison of the length of a connection with ``l_avg`` affects the
-            connection score, ``c_avg_length`` sets the relative effect of this
-            score metric compared to the other two, by default ``1.0``
-        c_angle : float, optional
-            the angle between a connection and its neighboring connections
-            affects the connection score, ``c_angle`` sets the relative effect
-            of this score metric compared to the other two, by default ``1.0``
-        c_length_diff : float, optional
-            comparison of the length of a connection with the length of all
-            neighboring connections affects the score, ``c_length_diff`` sets
-            the relative effect of this score metric compared to the other two,
-            by default ``1.0``
-        l_avg : float, optional
-            an initial guess for the average length of sarcomeres in pixels, by
-            default ``15.0``
-        score_threshold : float
-            any connection with a score less than the threshold will be
-            removed, by default ``0.1``
-        angle_threshold : float
-            if a zdisc has two valid connection the angle between must be
-            higher than the theshold, otherwise the connection with a lower
-            score will be removed, by default ``1.2`` (in radians)
-        save_output : bool
-            by default ``True``
-
-        Returns
-        -------
-        pd.DataFrame
-            Detected sarcomeres information. Columns are ``'frame'`` (frame
-            number), ``'sarc_id'`` (sarcomere id), ``'zdiscs'`` (particle id of
-            the two zdiscs forming a sarcomere), ``'x'`` and ``'y'`` (sarcomere
-            center position), ``'length'``, ``'width'``, and ``'angle'``
-            (sarcomere length, width, and angle).
-        List[nx.Graph]:
-            A list of graphs each indicating connected sarcomeres (myofibrils)
-
-        Notes
-        -----
-        - For a detailed description of the Trackpy package check:
-          http://soft-matter.github.io/trackpy/v0.5.0/tutorial.html
-
-        - For a detailed description of the OPTICS algorithm check:
-          https://scikit-learn.org/stable/modules/generated/sklearn.cluster.OPTICS.html
-
-        See Also
-        --------
-        :func:`sarcgraph.sg.SarcGraph.zdisc_segmentation`
-
-        :func:`sarcgraph.sg.SarcGraph.zdisc_tracking`
-        """
-        if tracked_zdiscs is None:
-            tracked_zdiscs = self.zdisc_tracking(
-                file_path,
-                raw_frames,
-                segmented_zdiscs,
-                sigma,
-                min_length,
-                tp_depth,
-                full_track_ratio,
-                skip_merging,
-                save_output,
-            )
-
-        zdiscs_clusters = (
-            tracked_zdiscs.groupby("particle")
-            .mean()
-            .reset_index()[["x", "y", "particle"]]
-            .to_numpy()
-        )
-        G = self._zdisc_to_graph(zdiscs_clusters)
-        G = self._score_graph(G, c_avg_length, c_angle, c_diff_length, l_avg)
-        G = self._prune_graph(G, score_threshold, angle_threshold)
-
-        myofibrils = [G.subgraph(c).copy() for c in nx.connected_components(G)]
-
-        sarcs = []
-        num_frames = tracked_zdiscs.frame.max() + 1
-        z0 = pd.DataFrame(np.arange(0, num_frames, 1), columns=["frame"])
-        for i, edge in enumerate(G.edges):
-            p1 = int(G.nodes[edge[0]]["particle_id"])
-            p2 = int(G.nodes[edge[1]]["particle_id"])
-            z1 = tracked_zdiscs[tracked_zdiscs.particle == p1]
-            z2 = tracked_zdiscs[tracked_zdiscs.particle == p2]
-            z1.columns = np.insert(z2.columns.values[1:] + "_p1", 0, "frame")
-            z2.columns = np.insert(z2.columns.values[1:] + "_p2", 0, "frame")
-
-            sarc = pd.merge(z0, z1, how="outer", on="frame")
-            sarc = pd.merge(sarc, z2, how="outer", on="frame")
-
-            sarc["sarc_id"] = i
-            sarc["zdiscs"] = ",".join(
-                map(str, sorted((p1, p2)))
-            )  # list(map(float, sarc.zdiscs[0].split(',')))
-            sarc["x"] = (sarc.x_p1 + sarc.x_p2) / 2
-            sarc["y"] = (sarc.y_p1 + sarc.y_p2) / 2
-            length = np.sqrt(
-                (sarc.x_p1 - sarc.x_p2) ** 2 + (sarc.y_p1 - sarc.y_p2) ** 2
-            )
-            sarc["length"] = length
-            width1 = np.sqrt(
-                (sarc.p1_x_p1 - sarc.p2_x_p1) ** 2
-                + (sarc.p1_y_p1 - sarc.p2_y_p1) ** 2
-            )
-            width2 = np.sqrt(
-                (sarc.p1_x_p2 - sarc.p2_x_p2) ** 2
-                + (sarc.p1_y_p2 - sarc.p2_y_p2) ** 2
-            )
-            sarc["width"] = (width1 + width2) / 2
-            angle = np.arctan2(sarc.y_p2 - sarc.y_p1, sarc.x_p2 - sarc.x_p1)
-            angle[angle < 0] += np.pi
-            sarc["angle"] = angle
-            sarcs.append(
-                sarc[
-                    [
-                        "frame",
-                        "sarc_id",
-                        "x",
-                        "y",
-                        "length",
-                        "width",
-                        "angle",
-                        "zdiscs",
-                    ]
-                ]
-            )
-        sarcs = pd.concat(sarcs).reset_index().drop("index", axis=1)
-
-        if save_output:
-            self._save_dataframe(sarcs, "sarcomeres")
-
-        return sarcs, myofibrils
+import numpy as np
+import pandas as pd
+import trackpy as tp
+import networkx as nx
+
+import skvideo.io
+import skimage.io
+import skvideo.utils
+
+from skimage.filters import laplace, gaussian, threshold_otsu
+from skimage import measure
+from sklearn.cluster import OPTICS
+from sklearn.neighbors import NearestNeighbors
+from scipy.spatial import distance_matrix
+from pathlib import Path
+from typing import List, Union, Tuple
+
+
+class SarcGraph:
+    def __init__(self, output_dir: str = "test-run", file_type: str = "video"):
+        """Zdiscs and sarcomeres segmentation and tracking.
+
+        Attributes
+        ----------
+        output_dir : str, optional
+            location to save processed information, by default ``'test-run'``
+        file_type : str, optional
+            use ``'image'`` for single-frame samples and ``'video'`` for
+            multi-frame samples, by default ``'video'``
+        """
+        if file_type not in ["video", "image"]:
+            raise ValueError(
+                f"{file_type} is not recognized as a valid file_type. Choose "
+                "from ['video', 'image']."
+            )
+        if not isinstance(output_dir, str):
+            raise TypeError("output_dir must be a string.")
+        Path(f"{output_dir}").mkdir(parents=True, exist_ok=True)
+        self.output_dir = output_dir
+        self.file_type = file_type
+
+    ###########################################################
+    #                    Utility Functions                    #
+    ###########################################################
+    def _data_loader(self, file_path: str) -> np.ndarray:
+        """Loads a video/image file.
+
+        Parameters
+        ----------
+        file_path : str
+            A video/image file address
+
+        Returns
+        -------
+        numpy.ndarray
+            All frames in the raw format
+        """
+        if self.file_type == "video":
+            data = skvideo.io.vread(file_path)
+            if data.shape[0] > 1:
+                return data
+        return skimage.io.imread(file_path)
+
+    def _to_gray(self, frames: np.ndarray) -> np.ndarray:
+        """Convert RGB frames to grayscale.
+
+        Parameters
+        ----------
+        frames : np.ndarray
+            RGB frames
+
+        Returns
+        -------
+        numpy.ndarray
+            All frames in gray scale
+        """
+        frames_gray = skvideo.utils.rgb2gray(frames)
+        if self.file_type == "video" and frames_gray.shape[0] < 2:
+            raise ValueError(
+                "Failed to load video correctly! Manually load the video into "
+                "a numpy array and input to the function as raw_frames."
+            )
+        if self.file_type == "image" and frames_gray.shape[0] > 1:
+            raise ValueError(
+                "Trying to load a video while file_type='image'. Load the "
+                "image manually or change the file_type to 'video."
+            )
+
+        return frames_gray
+
+    def _save_numpy(
+        self, data: Union[List, np.ndarray], file_name: str
+    ) -> None:
+        """Saves a numpy array.
+
+        Parameters
+        ----------
+        data : np.ndarray
+        file_name: str
+        """
+        if not isinstance(file_name, str):
+            raise TypeError("file_name must be a string.")
+        if isinstance(data, np.ndarray) or isinstance(data, List):
+            np.save(
+                f"./{self.output_dir}/{file_name}.npy", data, allow_pickle=True
+            )
+            return
+
+        raise TypeError("data must be a numpy.ndarray or a List.")
+
+    def _save_dataframe(self, data: pd.DataFrame, file_name: str) -> None:
+        """Saves a pandas dataframe.
+
+        Parameters
+        ----------
+        data : pd.DataFrame
+        file_name: str
+        """
+        if not isinstance(file_name, str):
+            raise TypeError("file_name must be a string.")
+        if isinstance(data, pd.DataFrame):
+            data.to_csv(f"./{self.output_dir}/{file_name}.csv")
+            return
+        raise TypeError(
+            f"'data' type is {type(data)}. 'data' must be a pandas DataFrame."
+        )
+
+    def _filter_frames(
+        self, frames: np.ndarray, sigma: float = 1.0
+    ) -> np.ndarray:
+        """Convolves all frames with laplacian and gaussian filters.
+
+        Parameters
+        ----------
+        frames : np.ndarray
+        sigma : float
+            Standard deviation for Gaussian kernel
+
+        Returns
+        -------
+        np.ndarray, shape=(frames, dim_1, dim_2)
+        """
+        if frames.ndim > 4 or frames.ndim < 3:
+            raise ValueError(
+                "Input array must have the shape (frames, dim_1, dim_2, "
+                "channels=1 (optional))"
+            )
+        if frames.ndim == 4:
+            if frames.shape[3] != 1:
+                raise ValueError(
+                    "Number of channels in the input array must be 1. Input "
+                    "shape: (frames, dim_1, dim_2, channels=1 (optional))"
+                )
+            frames = frames[:, :, :, 0]
+        filtered_frames = np.zeros(frames.shape)
+        for i, frame in enumerate(frames):
+            laplacian = laplace(frame)
+            filtered_frames[i] = gaussian(laplacian, sigma=sigma)
+        return filtered_frames
+
+    #############################################################
+    #                    Z-Disc Segmentation                    #
+    #############################################################
+    def _process_input(
+        self,
+        file_path: Union[str, None] = None,
+        raw_frames: Union[np.ndarray, None] = None,
+        sigma: float = 1.0,
+        save_output: bool = True,
+    ) -> np.ndarray:
+        """Loads a video/image and filter all frames.
+
+        Parameters
+        ----------
+        file_path : str
+            The address of an image or a video file to be loaded
+        raw_frames  : np.ndarray, shape=(frames, dim_1, dim_2, channels)
+            Raw input image or video given as a 4 dimensional array
+        sigma : float
+            Standard deviation for Gaussian kernel
+        save_output : bool
+            by default True
+
+        Returns
+        -------
+        np.ndarray, shape=(frames, dim_1, dim_2)
+        """
+        if raw_frames is None:
+            if file_path is None:
+                raise ValueError(
+                    "Either file_path or raw_frames should be given as"
+                    " input."
+                )
+            else:
+                try:
+                    raw_frames = self._data_loader(file_path)
+                except Exception:
+                    raise ValueError(
+                        f"Not able to load a file from {file_path}."
+                    )
+
+        if not isinstance(raw_frames, np.ndarray):
+            raise TypeError("raw_frames must be a numpy array.")
+        raw_frames_gray = self._to_gray(raw_frames)
+        raw_frames_filtered = self._filter_frames(raw_frames_gray, sigma)
+        if save_output:
+            self._save_numpy(raw_frames_gray, file_name="raw-frames")
+            self._save_numpy(raw_frames_filtered, file_name="filtered-frames")
+        return raw_frames_filtered
+
+    def _detect_contours(
+        self,
+        filtered_frames: np.ndarray,
+        min_length: int = 8,
+        save_output: bool = True,
+    ) -> List[np.ndarray]:
+        """Returns contours of detected zdiscs in each frame.
+
+        Parameters
+        ----------
+        filtered_frames : np.ndarray, shape=(frames, dim_1, dim_2)
+        min_length : int
+            Zdisc contours shorter than ``min_length`` pixels will be ignored.
+        save_output : bool
+            by default True
+
+        Returns
+        -------
+        List[np.ndarray]
+
+        Notes
+        -----
+        .. warning::
+            Here we use the ``skimage.measure.find_contours`` function to find
+            contours. This function returns contours with coordinates in
+            ``(row, column)`` order, which corresponds to ``(y, x)`` in
+            Cartesian coordinates. Therefore, in the rest of the code, we use
+            ``y`` for the first dimension and ``x`` for the second dimension.
+            For example, for plotting we use ``plt.plot(y, x)``.
+        """
+        if filtered_frames.ndim != 3:
+            raise ValueError(
+                "The input must be a 3d numpy array: (frames, " "dim 1, dim 2)"
+            )
+        if not isinstance(min_length, int):
+            try:
+                min_length = int(min_length)
+            except ValueError:
+                raise ValueError("min_length must be an integer.") from None
+        length_checker = np.vectorize(len)
+        valid_contours = []
+        for frame in filtered_frames:
+            contour_thresh = threshold_otsu(frame)
+            contours = np.array(
+                measure.find_contours(frame, contour_thresh), dtype="object"
+            )
+            contours_size = list(length_checker(contours))
+            valid_contours.append(
+                contours[np.greater_equal(contours_size, min_length)]
+            )
+        valid_contours = np.array(valid_contours, dtype="object")
+        if save_output:
+            self._save_numpy(valid_contours, file_name="contours")
+        return valid_contours
+
+    def _process_contour(self, contour: Union[List, np.ndarray]) -> np.ndarray:
+        """Computes the center location of a zdisc as well as its two end
+        points given its 2d contour.
+
+        Parameters
+        ----------
+        contour : np.ndarray, shape=(contour_length, 2)
+
+        Returns
+        -------
+        np.ndarray, shape=(6,)
+            zdisc center, end point 1, end point 2
+        """
+        if len(contour) < 3:
+            raise ValueError("A contour must have at least 3 coordinates.")
+        # center of a contour
+        center_coords = np.mean(contour, axis=0)
+        # coordinates of the two points on the contour with maximum distance
+        dist_mat = distance_matrix(contour, contour)
+        indices = np.unravel_index(dist_mat.argmax(), dist_mat.shape)
+        p1, p2 = contour[indices[0]], contour[indices[1]]
+        return np.hstack((center_coords, p1, p2))
+
+    def _zdiscs_to_pandas(self, zdiscs_all: List[np.ndarray]) -> pd.DataFrame:
+        """Creates a pandas dataframe from the information of detected zdiscs
+        in all frames.
+
+        Parameters
+        ----------
+        zdiscs_all : List[np.ndarray]
+            A list of numpy arrays each containing information of detected
+            zdiscs in a frame, (zdisc center, end point 1, end point 2)
+
+        Returns
+        -------
+        pd.DataFrame
+            Columns are ``frame`` (frame number), ``x`` and ``y`` (zdiscs
+            center position), ``p1_x``, ``p1_y``, ``p2_x``, ``p2_y`` (zdiscs
+            end points positions).
+        """
+        if self.file_type == "video" and len(zdiscs_all) < 2:
+            raise ValueError(
+                "Only one frame detected. Video is not loaded correctly."
+            )
+        if self.file_type == "image" and len(zdiscs_all) > 1:
+            raise ValueError(
+                "More than one frame detected. The image is not loaded "
+                "correctly."
+            )
+        data_frame = []
+        for i, zdiscs_frame in enumerate(zdiscs_all):
+            if type(zdiscs_frame) != np.ndarray:
+                raise TypeError("Input should be a list of numpy arrays.")
+            if zdiscs_frame.ndim != 2 or zdiscs_frame.shape[1] != 6:
+                raise ValueError(
+                    "Each numpy array must have the shape: (number of zdiscs, "
+                    "6)"
+                )
+            frame_id = i * np.ones((len(zdiscs_frame), 1), dtype=int)
+            zdiscs_frame_extended = np.hstack((frame_id, zdiscs_frame))
+            data_frame.append(
+                pd.DataFrame(
+                    zdiscs_frame_extended,
+                    columns=[
+                        "frame",
+                        "x",
+                        "y",
+                        "p1_x",
+                        "p1_y",
+                        "p2_x",
+                        "p2_y",
+                    ],
+                )
+            )
+        return pd.concat(data_frame)
+
+    def zdisc_segmentation(
+        self,
+        file_path: Union[str, None] = None,
+        raw_frames: Union[np.ndarray, None] = None,
+        sigma: float = 1.0,
+        min_length: int = 8,
+        save_output: bool = True,
+    ) -> pd.DataFrame:
+        """Finds Z-Discs in a video/image and extracts related information,
+        (frame number, center position, end points).
+
+        Parameters
+        ----------
+        file_path : str
+            address of the input video/image file
+        raw_frames  : np.ndarray, shape=(frames, dim_1, dim_2, channels)
+            Raw input image or video given as a 4 dimensional array
+        sigma : float
+            Standard deviation for Gaussian kernel
+        min_length : int
+            Minimum length for zdisc contours measured in pixels
+        save_output : bool
+            by default True
+
+        Returns
+        -------
+        pd.DataFrame
+            Information of all detected zdiscs in every frame. Columns are
+            ``'frame'`` (frame number), ``'x'`` and ``'y'`` (zdiscs center
+            position), ``'p1_x'``, ``'p1_y'``, ``'p2_x'``, ``'p2_y'`` (zdiscs
+            end points positions).
+        """
+        filtered_frames = self._process_input(
+            file_path, raw_frames, sigma, save_output
+        )
+        contours_all = self._detect_contours(
+            filtered_frames, min_length, save_output
+        )
+        zdiscs_all = []
+        for contours_frame in contours_all:
+            zdiscs_frame = np.zeros((len(contours_frame), 6))
+            for i, contour in enumerate(contours_frame):
+                zdiscs_frame[i] = self._process_contour(contour)
+            zdiscs_all.append(zdiscs_frame)
+        zdiscs_all_dataframe = self._zdiscs_to_pandas(zdiscs_all)
+        if save_output:
+            self._save_dataframe(
+                zdiscs_all_dataframe, file_name="segmented-zdiscs"
+            )
+        return zdiscs_all_dataframe
+
+    #########################################################
+    #                    Z-disc Tracking                    #
+    #########################################################
+    def _merge_tracked_zdiscs(
+        self,
+        tracked_zdiscs: pd.DataFrame,
+        full_track_ratio: float = 0.75,
+    ) -> pd.DataFrame:
+        """A post processing step to group related partially tracked zdiscs
+        using the OPTICS algorithm. Increases the robustness of zdisc tracking
+        as well as the number of fully tracked zdiscs.
+
+        Parameters
+        ----------
+        tracked_zdiscs : pd.DataFrame
+            tracked zdiscs information for all frames
+        full_track_ratio : float, optional
+            If a tracked zdisc appears in enough number of frames defined by
+            this ratio, it is considered a fully tracked zdisc. The default
+            value 0.75 means if a zdisc is tracked in more than 75 percent of
+            all frames it is fully tracked.
+
+        Returns
+        -------
+        pd.DataFrame
+
+        Notes
+        -----
+        For a detailed description of the OPTICS algorithm check:
+        https://scikit-learn.org/stable/modules/generated/sklearn.cluster.OPTICS.html
+        """
+        num_frames = tracked_zdiscs.frame.max() + 1
+        tracked_zdiscs_grouped = tracked_zdiscs.groupby("particle")["particle"]
+        tracked_zdiscs["freq"] = tracked_zdiscs_grouped.transform("count")
+        fully_tracked_zdiscs = tracked_zdiscs.loc[
+            tracked_zdiscs.freq == num_frames
+        ]
+        partially_tracked_zdiscs = tracked_zdiscs.loc[
+            tracked_zdiscs.freq < num_frames
+        ]
+
+        if partially_tracked_zdiscs.empty:
+            return fully_tracked_zdiscs
+
+        partially_tracked_clusters = (
+            partially_tracked_zdiscs[["x", "y", "particle"]]
+            .groupby(by=["particle"])
+            .mean()
+        )
+
+        # merge related clusters (neighbors)
+        all_clusters_xy = (
+            tracked_zdiscs.groupby("particle").mean()[["x", "y"]].to_numpy()
+        )
+        clusters_min_dist = np.min(
+            distance_matrix(all_clusters_xy, all_clusters_xy)
+            + 1e6 * np.eye(len(all_clusters_xy)),
+            axis=1,
+        )
+        optics_max_eps = np.mean(clusters_min_dist)
+        data = np.array(partially_tracked_clusters)
+        optics_model = OPTICS(max_eps=optics_max_eps, min_samples=2)
+        optics_result = optics_model.fit_predict(data)
+        optics_clusters = np.unique(optics_result)
+
+        all_merged_zdiscs = []
+        for i, optics_cluster in enumerate(optics_clusters):
+            index = np.where(optics_result == optics_cluster)[0]
+            particles_in_cluster = partially_tracked_clusters.iloc[
+                index
+            ].index.to_numpy()
+            if optics_cluster >= 0:
+                merged_zdiscs = (
+                    partially_tracked_zdiscs.loc[
+                        partially_tracked_zdiscs["particle"].isin(
+                            particles_in_cluster
+                        )
+                    ]
+                    .groupby("frame")
+                    .mean()
+                )
+                if len(merged_zdiscs) > num_frames * full_track_ratio:
+                    merged_zdiscs.particle = -(i + 1)
+                    merged_zdiscs.freq = len(merged_zdiscs)
+                    all_merged_zdiscs.append(merged_zdiscs.reset_index())
+            else:
+                for p in particles_in_cluster:
+                    no_merge_zdiscs = partially_tracked_zdiscs.loc[
+                        partially_tracked_zdiscs["particle"] == p
+                    ]
+                    if len(no_merge_zdiscs) > num_frames * full_track_ratio:
+                        all_merged_zdiscs.append(no_merge_zdiscs)
+        if all_merged_zdiscs:
+            all_merged_zdiscs = pd.concat(all_merged_zdiscs)
+            return pd.concat((fully_tracked_zdiscs, all_merged_zdiscs))
+        else:
+            return fully_tracked_zdiscs
+
+    def zdisc_tracking(
+        self,
+        file_path: str = None,
+        raw_frames: np.array = None,
+        segmented_zdiscs: pd.DataFrame = None,
+        sigma: float = 1.0,
+        min_length: int = 8,
+        tp_depth: float = 4.0,
+        full_track_ratio: float = 0.75,
+        skip_merging: bool = False,
+        save_output: bool = True,
+    ) -> pd.DataFrame:
+        """Track detected Z-Discs in a video. The input could be the address to
+        a video/image sample (``file_path``), raw frames as a numpy array
+        (``raw_frames``), or segmented zdiscs information in a pandas datafram
+        (``segmented_zdiscs``)e. If the function is run with no inputs, it will
+        search for 'raw-frames.npy', or 'segmented-zdiscs.csv' in the
+        specified output directory ``SarcGraph().output_dir``.
+
+        Parameters
+        ----------
+        file_path : str
+            The address of an image or a video file to be loaded
+        raw_frames : np.ndarray, shape=(frames, dim_1, dim_2, channels)
+            Raw input image or video given as a 4 dimensional array
+        segmented_zdiscs : pd.DataFrame
+            Information of all detected zdiscs in every frame.
+        sigma : float
+            Standard deviation for Gaussian kernel, by default ``1.0``
+        min_length : int
+            Minimum length for zdisc contours measured in pixels, by default
+            ``8``
+        tp_depth : float, optional
+            the maximum distance features can move between frames, by default
+            ``4.0``
+        full_track_ratio : float, optional
+            by default ``0.75``
+        skip_merging : bool, optional
+            skipping the merging step will result in fewer fully tracked
+            zdiscs, by default ``False``
+        save_output : bool
+            by default ``True``
+
+        Returns
+        -------
+        pd.DataFrame
+            tracked zdiscs information. Columns are ``'frame'`` (frame number),
+            ``'x'`` and ``'y'`` (zdiscs center position), ``'p1_x'``,
+            ``'p1_y'``, ``'p2_x'``, ``'p2_y'`` (zdiscs end points positions),
+            and ``'particle'`` (id of each tracked zdisc).
+
+        Notes
+        -----
+        - If ``SarcGraph().file_type='image'``, tracking will be skipped.
+
+        - For a detailed description of the Trackpy package check:
+            http://soft-matter.github.io/trackpy/v0.5.0/tutorial.html
+
+        - For a detailed description of the OPTICS algorithm check:
+            https://scikit-learn.org/stable/modules/generated/sklearn.cluster.OPTICS.html
+
+        See Also
+        --------
+        :func:`sarcgraph.sg.SarcGraph.zdisc_segmentation`
+
+        :func:`sarcgraph.sg.SarcGraph._merge_tracked_zdiscs`
+
+        """
+        if segmented_zdiscs is None:
+            segmented_zdiscs = self.zdisc_segmentation(
+                file_path, raw_frames, sigma, min_length, save_output
+            )
+
+        if type(segmented_zdiscs) != pd.DataFrame:
+            raise TypeError("segmented_zdiscs shoulb be a dataframe.")
+
+        correct_columns = set(("frame", "x", "y")).issubset(
+            set(segmented_zdiscs.columns)
+        )
+
+        if not correct_columns:
+            raise ValueError(
+                "segmented_zdiscs must contain at least three columns: 'x', "
+                "'y', 'frame'."
+            )
+
+        # skip tracking if the sample is an image
+        if self.file_type == "image":
+            segmented_zdiscs["particle"] = np.arange(len(segmented_zdiscs))
+            tracked_zdiscs = segmented_zdiscs
+        else:
+            # run tracking with the trackpy package:
+            num_frames = len(segmented_zdiscs.frame.unique())
+            t = tp.link_df(
+                segmented_zdiscs, search_range=tp_depth, memory=num_frames
+            )
+            tracked_zdiscs = tp.filter_stubs(t, 2).reset_index(drop=True)
+            if skip_merging is False:
+                tracked_zdiscs = self._merge_tracked_zdiscs(
+                    tracked_zdiscs,
+                    full_track_ratio,
+                )
+
+        if save_output:
+            self._save_dataframe(tracked_zdiscs, "tracked-zdiscs")
+
+        return tracked_zdiscs
+
+    #############################################################
+    #                    Sarcomere Detection                    #
+    #############################################################
+    def _zdisc_to_graph(self, zdiscs: np.array, K: int = 3) -> nx.Graph:
+        """Creates a graph with zdiscs as nodes. Each zdisc is connected to its
+        ``K`` nearest neighbors.
+
+        Parameters
+        ----------
+        zdiscs : np.array, shape=(N, 3)
+            zdiscs information as an array. The first two columns are the x and
+            y location of zdisc centers and the last is the particle id.
+        K : int, optional
+            number of nearest neighbors for each zdisc, by default 3
+
+        Returns
+        -------
+        nx.Graph
+        """
+        num_nodes = len(zdiscs)
+        G = nx.Graph()
+        G.add_nodes_from(range(num_nodes))
+
+        # add the position of each zdisc as a node attribute to the graph
+        nodes_pos_dict = {i: pos for i, pos in enumerate(zdiscs[:, 0:2])}
+        nodes_particle_dict = {j: id for j, id in enumerate(zdiscs[:, -1])}
+
+        nx.set_node_attributes(G, values=nodes_pos_dict, name="pos")
+        nx.set_node_attributes(
+            G, values=nodes_particle_dict, name="particle_id"
+        )
+
+        # find K nearest zdisc to each zdisc
+        neigh = NearestNeighbors(n_neighbors=2)
+        neigh.fit(zdiscs[:, 0:2])
+        nearestNeighbors = neigh.kneighbors(
+            zdiscs[:, 0:2], K + 1, return_distance=False
+        )
+
+        # connect each zdisc to K nearest neighbors
+        edges = []
+        for node, neighbors in enumerate(nearestNeighbors[:, 1:]):
+            for neighbor in neighbors:
+                edges.append((node, neighbor))
+        G.add_edges_from(edges)
+
+        return G
+
+    def _score_graph(
+        self,
+        G: nx.Graph,
+        c_avg_length: float = 1.0,
+        c_angle: float = 1.0,
+        c_length_diff: float = 1.0,
+        l_avg: float = 15.0,
+        l_max: float = 30.0,
+    ) -> nx.Graph:
+        """Assigns a score to each connection of the input graph. Higher score
+        indicates the two corresponding zdiscs are likely to be two ends of a
+        sarcomere.
+
+        Parameters
+        ----------
+        G : nx.Graph
+        c_avg_length : float, optional
+            comparison of the length of a connection with ``l_avg`` affects the
+            connection score, ``c_avg_length`` sets the relative effect of this
+            score metric compared to the other two, by default 1.0
+        c_angle : float, optional
+            the angle between a connection and its neighboring connections
+            affects the connection score, ``c_angle`` sets the relative effect
+            of this score metric compared to the other two, by default 1.0
+        c_length_diff : float, optional
+            comparison of the length of a connection with the length of all
+            neighboring connections affects the score, ``c_length_diff`` sets
+            the relative effect of this score metric compared to the other two,
+            by default 1.0
+        l_avg : float, optional
+            an initial guess for the average length of sarcomeres in pixels, by
+            default 15.0
+        l_max : float, optional
+            Max allowable length for the length of sarcomeres in pixels, by
+            default 30.0
+
+        Returns
+        -------
+        nx.Graph
+            a graph of zdiscs with all connections scored
+        """
+        edges_attr_dict = {}
+        for node in range(G.number_of_nodes()):
+            for neighbor in G.neighbors(node):
+                score = 0
+                v1 = G.nodes[neighbor]["pos"] - G.nodes[node]["pos"]
+                l1 = np.linalg.norm(v1)
+                if l1 <= l_max:
+                    avg_length_score = np.exp(-np.pi * (1 - l1 / l_avg) ** 2)
+                    for far_neighbor in G.neighbors(neighbor):
+                        if far_neighbor in [node, neighbor]:
+                            pass
+                        else:
+                            v2 = (
+                                G.nodes[neighbor]["pos"]
+                                - G.nodes[far_neighbor]["pos"]
+                            )  # vector connecting neighbor to far_neighbor
+                            l2 = np.linalg.norm(v2)
+
+                            d_theta = np.arccos(np.dot(v1, v2) / (l1 * l2)) / (
+                                np.pi / 2
+                            )
+                            d_l = np.abs(l2 - l1) / l1
+
+                            angle_score = (
+                                np.power(1 - d_theta, 2) if d_theta >= 1 else 0
+                            )
+                            diff_length_score = 1 / (1 + d_l)
+
+                            score = np.max(
+                                (
+                                    score,
+                                    c_length_diff * diff_length_score
+                                    + c_angle * angle_score,
+                                )
+                            )
+                    score += c_avg_length * avg_length_score
+                edges_attr_dict[(node, neighbor)] = score
+
+        edges_attr_dict_keep_max = {}
+        for key in edges_attr_dict.keys():
+            node_1 = key[0]
+            node_2 = key[1]
+            max_score = max(
+                edges_attr_dict[(node_1, node_2)],
+                edges_attr_dict[(node_2, node_1)],
+            )
+            edges_attr_dict_keep_max[(min(key), max(key))] = max_score
+        nx.set_edge_attributes(
+            G, values=edges_attr_dict_keep_max, name="score"
+        )
+        return G
+
+    def _prune_graph(
+        self,
+        G: nx.Graph,
+        score_threshold: float = 0.1,
+        angle_threshold: float = 1.2,
+    ) -> nx.Graph:
+        """Prunes the input graph to get rid of invalid or less probable
+        connections.
+
+        Parameters
+        ----------
+        G : nx.Graph
+            A scored graph of zdiscs clusters
+        score_threshold : float
+            any connection with a score less than the threshold will be
+            removed, by default 0.1
+        angle_threshold : float
+            if a zdisc has two valid connection the angle between must be
+            higher than the theshold, otherwise the connection with a lower
+            score will be removed, by default 1.2 (in radians)
+
+        Returns
+        -------
+        nx.Graph
+        """
+        nx.set_edge_attributes(G, values=0, name="validity")
+        for node in range(G.number_of_nodes()):
+            vectors = []
+            scores = []
+            neighbors = list(G.neighbors(node))
+            for neighbor in neighbors:
+                vectors.append(G.nodes[neighbor]["pos"] - G.nodes[node]["pos"])
+                scores.append(G[node][neighbor]["score"])
+
+            # sort by scores
+            if np.max(scores) > score_threshold:
+                sort_indices = np.argsort(scores)[::-1]
+                best_vector = vectors[sort_indices[0]]
+                G[node][neighbors[sort_indices[0]]]["validity"] += 1
+                for idx in sort_indices[1:]:
+                    s = scores[idx]
+                    n = neighbors[idx]
+                    v = vectors[idx]
+
+                    l1 = np.linalg.norm(best_vector)
+                    l2 = np.linalg.norm(v)
+                    theta = np.arccos(np.dot(v, best_vector) / (l1 * l2)) / (
+                        np.pi / 2
+                    )
+
+                    if theta > angle_threshold and s > score_threshold:
+                        G[node][n]["validity"] += 1
+                        break
+
+        edges2remove = []
+        for edge in G.edges():
+            if G.edges[edge]["validity"] < 2:
+                edges2remove.append(edge)
+        G.remove_edges_from(edges2remove)
+
+        return G
+
+    def sarcomere_detection(
+        self,
+        file_path: str = None,
+        raw_frames: np.array = None,
+        segmented_zdiscs: pd.DataFrame = None,
+        tracked_zdiscs: pd.DataFrame = None,
+        sigma: float = 1.0,
+        min_length: int = 8,
+        tp_depth: float = 4.0,
+        full_track_ratio: float = 0.75,
+        skip_merging: bool = False,
+        c_avg_length: float = 1,
+        c_angle: float = 1,
+        c_diff_length: float = 1,
+        l_avg: float = 12.0,
+        score_threshold: float = 0.01,
+        angle_threshold: float = 1.2,
+        save_output: bool = True,
+    ) -> Tuple[pd.DataFrame, List[nx.Graph]]:
+        """Detect sarcomeres in a video/image. The input could be the address
+        to the video/image sample (``file_path``), raw frames as a numpy array
+        (``raw_frames``), segmented zdiscs information in a pandas dataframe
+        (``segmented_zdiscs``), or a dataframe of tracked zdiscs
+        (``tracked_zdiscs``).
+
+        Parameters
+        ----------
+        file_path : str
+            The address of an image or a video file to be loaded
+        raw_frames  : np.ndarray, shape=(frames, dim_1, dim_2, channels)
+            Raw input image or video given as a 4 dimensional array
+        segmented_zdiscs : pd.DataFrame
+            Information of all detected zdiscs in every frame.
+        tracked_zdiscs : pd.DataFrame
+            Information of tracked zdiscs
+        sigma : float
+            Standard deviation for Gaussian kernel, by default ``1.0``
+        min_length : int
+            Minimum length for zdisc contours measured in pixels, by default
+            ``8``
+        tp_depth : float, optional
+            the maximum distance features can move between frames, by default
+            ``4.0``
+        full_track_ratio : float, optional
+            Frame ratio to seperate partially tracked vs fully tracked
+            sarcomeres, by default ``0.75``
+        skip_merging : bool, optional
+            skipping the merging step will result in fewer fully tracked
+            zdiscs, by default ``False``
+        c_avg_length : float, optional
+            comparison of the length of a connection with ``l_avg`` affects the
+            connection score, ``c_avg_length`` sets the relative effect of this
+            score metric compared to the other two, by default ``1.0``
+        c_angle : float, optional
+            the angle between a connection and its neighboring connections
+            affects the connection score, ``c_angle`` sets the relative effect
+            of this score metric compared to the other two, by default ``1.0``
+        c_length_diff : float, optional
+            comparison of the length of a connection with the length of all
+            neighboring connections affects the score, ``c_length_diff`` sets
+            the relative effect of this score metric compared to the other two,
+            by default ``1.0``
+        l_avg : float, optional
+            an initial guess for the average length of sarcomeres in pixels, by
+            default ``15.0``
+        score_threshold : float
+            any connection with a score less than the threshold will be
+            removed, by default ``0.1``
+        angle_threshold : float
+            if a zdisc has two valid connection the angle between must be
+            higher than the theshold, otherwise the connection with a lower
+            score will be removed, by default ``1.2`` (in radians)
+        save_output : bool
+            by default ``True``
+
+        Returns
+        -------
+        pd.DataFrame
+            Detected sarcomeres information. Columns are ``'frame'`` (frame
+            number), ``'sarc_id'`` (sarcomere id), ``'zdiscs'`` (particle id of
+            the two zdiscs forming a sarcomere), ``'x'`` and ``'y'`` (sarcomere
+            center position), ``'length'``, ``'width'``, and ``'angle'``
+            (sarcomere length, width, and angle).
+        List[nx.Graph]:
+            A list of graphs each indicating connected sarcomeres (myofibrils)
+
+        Notes
+        -----
+        - For a detailed description of the Trackpy package check:
+          http://soft-matter.github.io/trackpy/v0.5.0/tutorial.html
+
+        - For a detailed description of the OPTICS algorithm check:
+          https://scikit-learn.org/stable/modules/generated/sklearn.cluster.OPTICS.html
+
+        See Also
+        --------
+        :func:`sarcgraph.sg.SarcGraph.zdisc_segmentation`
+
+        :func:`sarcgraph.sg.SarcGraph.zdisc_tracking`
+        """
+        if tracked_zdiscs is None:
+            tracked_zdiscs = self.zdisc_tracking(
+                file_path,
+                raw_frames,
+                segmented_zdiscs,
+                sigma,
+                min_length,
+                tp_depth,
+                full_track_ratio,
+                skip_merging,
+                save_output,
+            )
+
+        zdiscs_clusters = (
+            tracked_zdiscs.groupby("particle")
+            .mean()
+            .reset_index()[["x", "y", "particle"]]
+            .to_numpy()
+        )
+        G = self._zdisc_to_graph(zdiscs_clusters)
+        G = self._score_graph(G, c_avg_length, c_angle, c_diff_length, l_avg)
+        G = self._prune_graph(G, score_threshold, angle_threshold)
+
+        myofibrils = [G.subgraph(c).copy() for c in nx.connected_components(G)]
+
+        sarcs = []
+        num_frames = tracked_zdiscs.frame.max() + 1
+        z0 = pd.DataFrame(np.arange(0, num_frames, 1), columns=["frame"])
+        for i, edge in enumerate(G.edges):
+            p1 = int(G.nodes[edge[0]]["particle_id"])
+            p2 = int(G.nodes[edge[1]]["particle_id"])
+            z1 = tracked_zdiscs[tracked_zdiscs.particle == p1]
+            z2 = tracked_zdiscs[tracked_zdiscs.particle == p2]
+            z1.columns = np.insert(z2.columns.values[1:] + "_p1", 0, "frame")
+            z2.columns = np.insert(z2.columns.values[1:] + "_p2", 0, "frame")
+
+            sarc = pd.merge(z0, z1, how="outer", on="frame")
+            sarc = pd.merge(sarc, z2, how="outer", on="frame")
+
+            sarc["sarc_id"] = i
+            sarc["zdiscs"] = ",".join(
+                map(str, sorted((p1, p2)))
+            )  # list(map(float, sarc.zdiscs[0].split(',')))
+            sarc["x"] = (sarc.x_p1 + sarc.x_p2) / 2
+            sarc["y"] = (sarc.y_p1 + sarc.y_p2) / 2
+            length = np.sqrt(
+                (sarc.x_p1 - sarc.x_p2) ** 2 + (sarc.y_p1 - sarc.y_p2) ** 2
+            )
+            sarc["length"] = length
+            width1 = np.sqrt(
+                (sarc.p1_x_p1 - sarc.p2_x_p1) ** 2
+                + (sarc.p1_y_p1 - sarc.p2_y_p1) ** 2
+            )
+            width2 = np.sqrt(
+                (sarc.p1_x_p2 - sarc.p2_x_p2) ** 2
+                + (sarc.p1_y_p2 - sarc.p2_y_p2) ** 2
+            )
+            sarc["width"] = (width1 + width2) / 2
+            angle = np.arctan2(sarc.x_p2 - sarc.x_p1, sarc.y_p2 - sarc.y_p1)
+            angle[angle < 0] += np.pi
+            sarc["angle"] = angle
+            sarcs.append(
+                sarc[
+                    [
+                        "frame",
+                        "sarc_id",
+                        "x",
+                        "y",
+                        "length",
+                        "width",
+                        "angle",
+                        "zdiscs",
+                    ]
+                ]
+            )
+        sarcs = pd.concat(sarcs).reset_index().drop("index", axis=1)
+
+        if save_output:
+            self._save_dataframe(sarcs, "sarcomeres")
+
+        return sarcs, myofibrils
```

### Comparing `sarcgraph-0.1.1/sarcgraph/sg_tools.py` & `sarcgraph-0.2.1/sarcgraph/sg_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1563 +1,1633 @@
-import numpy as np
-import matplotlib.pyplot as plt
-import pandas as pd
-import networkx as nx
-import pickle
-import imageio
-import shutil
-import json
-import os
-
-from scipy import signal
-from scipy.signal import find_peaks
-from scipy.linalg import polar
-from sklearn.gaussian_process import GaussianProcessRegressor
-from sklearn.gaussian_process.kernels import RBF, WhiteKernel
-from scipy.spatial.distance import pdist, squareform
-from scipy.cluster.hierarchy import linkage, dendrogram
-from pathlib import Path
-from typing import Tuple  # List, Union
-
-from warnings import simplefilter
-from sklearn.exceptions import ConvergenceWarning
-
-from sarcgraph.sg import SarcGraph
-
-simplefilter("ignore", category=ConvergenceWarning)
-
-
-class SarcGraphTools:
-    def __init__(
-        self,
-        input_dir: str = "test-run",
-        quality: int = 300,
-        include_eps: bool = False,
-        save_results: bool = True,
-    ):
-        """Tools for post processing analysis on detected sarcomeres.
-
-        Parameters
-        ----------
-        input_dir : str
-            Should be the same as the `output_dir` in sarcgraph.sg.Sarcgraph(),
-             by default "test-run"
-        quality : int
-            dpi of saved figures in png format, by default 300
-        include_eps : bool
-            save eps format of figures, by default False
-        save_results : bool
-            save the results of post processing analysis, by default True
-        """
-        if not os.path.exists(input_dir):
-            raise FileNotFoundError(f"{input_dir}/ directory was not found!")
-
-        self.input_dir = input_dir
-        self.output_dir = input_dir
-        self.quality = quality
-        self.include_eps = include_eps
-        self.save_results = save_results
-        self.visualization = self.Visualization(self)
-        self.time_series = self.TimeSeries(self)
-        self.analysis = self.Analysis(self)
-
-    ###########################################################
-    #                    Time Series Class                    #
-    ###########################################################
-    class TimeSeries:
-        def __init__(self, sg_tools):
-            """Provides the tools to apply Gaussian Process Regression (GPR) on
-            timeseries of detected sarcomere
-            """
-            self.sg_tools = sg_tools
-
-        def _dtw_distance(self, s1: np.ndarray, s2: np.ndarray) -> np.ndarray:
-            """Compute distance based on dynamic time warping (DTW) between
-            two 1D signals s1 and s2.
-
-            Parameters
-            ----------
-            s1 : np.ndarray
-                1D signal
-            s2 : np.ndarray
-                1D signal
-
-            Returns
-            -------
-            np.ndarray
-                DTW distance between s1 and s2 based on euclidean distance.
-            """
-            if (not isinstance(s1, np.ndarray)) or (
-                not isinstance(s2, np.ndarray)
-            ):
-                raise TypeError("s1 and s2 must be 1D numpy arrays.")
-            if s1.ndim == 1 and s2.ndim == 1:
-                n = len(s1)
-                m = len(s2)
-                dtw = np.inf * np.ones((n + 1, m + 1))
-                dtw[0, 0] = 0
-                dist = (s1.reshape(-1, 1) - s2.reshape(1, -1)) ** 2
-                for i in range(1, n + 1):
-                    for j in range(1, m + 1):
-                        dtw[i, j] = dist[i - 1, j - 1] + min(
-                            dtw[i - 1, j], dtw[i, j - 1], dtw[i - 1, j - 1]
-                        )
-                return np.sqrt(dtw[-1, -1])
-            else:
-                raise ValueError("s1 and s2 must be 1D numpy arrays.")
-
-        def _gpr(self, s: np.ndarray) -> np.ndarray:
-            """Applies Gaussian Process Regression (GPR) on a 1D signal
-
-            Parameters
-            ----------
-            s : np.ndarray
-
-            Returns
-            -------
-            np.ndarray
-
-            Notes
-            -----
-            For more information on GPR check:
-            https://scikit-learn.org/stable/modules/gaussian_process.html
-            """
-            num_frames = len(s)
-
-            kernel = 1.0 * RBF(
-                length_scale=1.0, length_scale_bounds=(1e-5, 1e1)
-            ) + 1.0 * WhiteKernel(
-                noise_level=1.0, noise_level_bounds=(1e-5, 1e1)
-            )
-            model = GaussianProcessRegressor(kernel=kernel, normalize_y=True)
-            xdata = np.arange(num_frames).reshape(-1, 1)
-            xhat = xdata
-            ydata = s.reshape(-1, 1)
-
-            remove_indices = np.where(np.isnan(ydata.reshape(-1)))[0]
-            xdata = np.delete(xdata, remove_indices, axis=0)
-            ydata = np.delete(ydata, remove_indices, axis=0)
-
-            model.fit(xdata, ydata)
-            yhat = model.predict(xhat)
-
-            return yhat.reshape(-1)
-
-        def _sarcomeres_length_normalize(
-            self, sarcomeres: pd.DataFrame
-        ) -> pd.DataFrame:
-            groupby_sarc_id = sarcomeres.groupby("sarc_id")
-            mean_length = groupby_sarc_id.length.transform("mean")
-            sarcomeres["length_norm"] = (
-                sarcomeres.length - mean_length
-            ) / mean_length
-            return sarcomeres
-
-        def sarcomeres_gpr(self) -> pd.DataFrame:
-            """Applies Gaussian Process Regression (GPR) on the output of the
-            sarcomere detection algorithm to reduce the noise and fill in
-            missing data.
-
-            Returns
-            -------
-            pd.DataFrame
-
-            Notes
-            -----
-            For more information on GPR check
-            https://scikit-learn.org/stable/modules/gaussian_process.html
-
-            See Also
-            --------
-            :func:`sarcgraph.sg.SarcGraph.sarcomere_detection`
-            """
-            sarcomeres = self.sg_tools._load_sarcomeres()
-            cols = [
-                "x",
-                "y",
-                "length",
-                "angle",
-                "width",
-            ]
-
-            num_sarcs = sarcomeres.sarc_id.max() + 1
-            for info_type in cols:
-                for sarc_num in range(num_sarcs):
-                    row_mask = sarcomeres.sarc_id == sarc_num
-                    s = sarcomeres.loc[row_mask, info_type].to_numpy()
-                    sarcomeres.loc[row_mask, info_type] = self._gpr(s)
-            sarcomeres = self._sarcomeres_length_normalize(sarcomeres)
-            if self.sg_tools.save_results:
-                sarcomeres.to_csv(
-                    f"./{self.sg_tools.output_dir}/sarcomeres_gpr.csv"
-                )
-            return sarcomeres
-
-    #############################################################
-    #                    Visualization Class                    #
-    #############################################################
-    class Visualization:
-        def __init__(self, sg_tools):
-            """Provides tools to visualize the results of post-processing
-            analysis on detected sarcomeres.
-            """
-            self.sg_tools = sg_tools
-
-        def zdiscs_and_sarcs(self, frame_num: int = 0):
-            """Visualize and save the plot of segmented zdiscs and detected
-            sarcomeres in the chosen frame
-
-            Parameters
-            ----------
-            frame_num : int, by default 0
-            """
-            raw_frame = self.sg_tools._load_raw_frames()[frame_num]
-            contours = self.sg_tools._load_contours()[frame_num]
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            sarcs_x = sarcomeres[sarcomeres.frame == frame_num].x
-            sarcs_y = sarcomeres[sarcomeres.frame == frame_num].y
-
-            ax = plt.axes()
-            ax.set_aspect("equal")
-            ax.imshow(raw_frame[:, :, 0], cmap=plt.cm.gray)
-            ax.set_title(
-                f"{len(contours)} z-disks and {len(sarcs_x)} sarcomeres\n"
-                f"found in frame {frame_num}"
-            )
-            for contour in contours:
-                ax.plot(contour[:, 1], contour[:, 0], "#0000cc", linewidth=1)
-            ax.plot(sarcs_y, sarcs_x, "*", color="#cc0000", markersize=3)
-            ax.set_xticks([])
-            ax.set_yticks([])
-
-            output_file = (
-                f"{self.sg_tools.output_dir}/zdiscs-sarcs-frame-{frame_num}"
-            )
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
-
-        def contraction(self):
-            """Visualize all detected sarcomeres in every frame according to
-            normalized fraction length and save as a gif file.
-            """
-            raw_frames = self.sg_tools._load_raw_frames()
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            num_frames = sarcomeres.frame.max() + 1
-            frames = sarcomeres.frame.to_numpy()
-            sarcs_x = sarcomeres.x.to_numpy()
-            sarcs_y = sarcomeres.y.to_numpy()
-            sarcs_length_norm = sarcomeres.length_norm.to_numpy()
-
-            img_list = []
-            Path("tmp").mkdir(parents=True, exist_ok=True)
-            for frame_num in range(num_frames):
-                indices = frames == frame_num
-                raw_frame = raw_frames[frame_num, :, :, 0]
-
-                plt.figure()
-                plt.imshow(raw_frame, cmap=plt.cm.gray)
-                y = sarcs_x[indices]
-                x = sarcs_y[indices]
-                length = np.abs(sarcs_length_norm[indices])
-                colors = np.piecewise(
-                    length,
-                    [length < 0.2, length >= 0.2],
-                    [lambda x: 2.5 * x + 0.5, lambda x: x],
-                )
-                for p_x, p_y, p_col in zip(x, y, colors):
-                    col = (1 - p_col, 0, p_col)
-                    plt.scatter(p_x, p_y, s=15, color=col, marker="o")
-
-                ax = plt.gca()
-                ax.set_xticks([])
-                ax.set_yticks([])
-                plt.savefig(
-                    f"tmp/frame-{frame_num}.png",
-                    dpi=self.sg_tools.quality,
-                    bbox_inches="tight",
-                )
-                plt.close()
-                img_list.append(imageio.imread(f"tmp/frame-{frame_num}.png"))
-            shutil.rmtree("tmp")
-            if num_frames > 1:
-                imageio.mimsave(
-                    f"{self.sg_tools.output_dir}/contract_anim.gif", img_list
-                )
-            print(
-                f"GIF saved as '{self.sg_tools.output_dir}/contract_anim.gif'!"
-            )
-
-        def normalized_sarcs_length(self):
-            """Plot normalized length of all detected sarcomeres vs frame
-            number.
-            """
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            num_sarcs = sarcomeres.sarc_id.max() + 1
-            sarc_ids = sarcomeres.sarc_id.to_numpy()
-            sarcs_length_norm = sarcomeres.length_norm.to_numpy()
-            groupby_frame = sarcomeres.groupby("frame")
-            sarcs_length_norm_median = groupby_frame.length_norm.median()
-            sarcs_length_norm_mean = groupby_frame.length_norm.mean()
-
-            for sarc_id in range(num_sarcs):
-                indices = sarc_ids == sarc_id
-                plt.plot(sarcs_length_norm[indices], linewidth=0.25)
-            plt.plot(
-                sarcs_length_norm_median,
-                "k-",
-                linewidth=3,
-                label="median curve",
-            )
-            plt.plot(
-                sarcs_length_norm_mean,
-                "--",
-                color=(0.5, 0.5, 0.5),
-                linewidth=3,
-                label="mean curve",
-            )
-            plt.xlabel("frame")
-            plt.ylabel("normalized length")
-            plt.title(
-                f"timeseries data, tracked and normalized, {num_sarcs} "
-                "sarcomeres"
-            )
-            plt.ylim((-0.1, 0.1))
-            plt.legend()
-            plt.tight_layout()
-            output_file = (
-                f"{self.sg_tools.output_dir}/normalized_sarcomeres_length"
-            )
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
-
-        def OOP(self):
-            """Plot recovered Orientational Order Parameter."""
-            OOP = self.sg_tools._load_recovered_info("OOP")
-
-            plt.figure(figsize=(5, 5))
-            plt.subplot(1, 1, 1)
-            plt.plot(OOP, "k-", label="OOP recovered")
-            plt.legend()
-            plt.title("recovered Orientational Order Parameter")
-            plt.xlabel("frames")
-
-            output_file = f"{self.sg_tools.output_dir}/recovered_OOP"
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
-
-        def F(self):
-            """Plot recovered deformation gradient."""
-            F = self.sg_tools._load_recovered_info("F")
-
-            plt.figure(figsize=(5, 5))
-            plt.subplot(1, 1, 1)
-            plt.plot(F[:, 0, 0] - 1, "r--", linewidth=5, label="F11 recovered")
-            plt.plot(F[:, 1, 1] - 1, "g--", linewidth=4, label="F22 recovered")
-            plt.plot(F[:, 0, 1], "c:", label="F12 recovered")
-            plt.plot(F[:, 1, 0], "b:", label="F21 recovered")
-            plt.legend()
-            plt.title("recovered deformation gradient")
-            plt.xlabel("frames")
-            output_file = f"{self.sg_tools.output_dir}/recovered_F"
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
-
-        def J(self):
-            """Plot recovered deformation jacobian."""
-            J = self.sg_tools._load_recovered_info("J")
-            frames = np.arange(len(J))
-
-            # compute the parameters of the timeseries
-            plt.figure(figsize=(5, 5))
-            plt.plot(J, "k-")
-
-            J_med = signal.medfilt(J, 5)
-            J_deriv = np.gradient(J, frames)
-            count_C = 0
-            count_R = 0
-            count_F = 0
-            thresh_flat = 0.01 * (np.max(J) - np.min(J))
-
-            for frame_num in range(len(frames)):
-                if J_deriv[frame_num] > thresh_flat:
-                    count_R += 1
-                    plt.plot(
-                        frames[frame_num],
-                        J[frame_num],
-                        "o",
-                        color=(0.5, 0.5, 0.5),
-                    )
-                elif J_deriv[frame_num] < -1.0 * thresh_flat:
-                    count_C += 1
-                    plt.plot(
-                        frames[frame_num], J[frame_num], "o", color=(0.5, 0, 0)
-                    )
-                else:
-                    count_F += 1
-                    plt.plot(
-                        frames[frame_num], J[frame_num], "o", color=(0, 0, 0.5)
-                    )
-
-            # detect peaks and valleys
-            # peaks_U, _ = find_peaks(data_med, threshold=th, distance=di,
-            # width=wi)
-            peaks_L, _ = find_peaks(
-                -1.0 * J_med, threshold=0.0, distance=10, width=5
-            )
-            plt.grid()
-            # plt.plot(x[peaks_U],data[peaks_U],'rx',markersize=10)
-            plt.plot(frames[peaks_L], J[peaks_L], "rx", markersize=13)
-            plt.title(
-                f"frames contract: {count_C}, relax: {count_R}, flat: "
-                f"{count_F}"
-            )
-            plt.xlabel("frame number")
-            plt.ylabel("determinate of average F")
-            plt.tight_layout()
-
-            output_file = f"{self.sg_tools.output_dir}/recovered_J"
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
-
-        def F_eigenval_animation(self):
-            """Visualize the eigenvalues of F over all frames"""
-            raw_frames = self.sg_tools._load_raw_frames()[:, :, :, 0]
-            F_all = self.sg_tools._load_recovered_info("F")
-            J_all = self.sg_tools._load_recovered_info("J")
-            OOP_all = self.sg_tools._load_recovered_info("OOP")
-            OOP_vec_all = self.sg_tools._load_recovered_info("OOP_vector")
-
-            num_frames = len(J_all)
-            frames = np.arange(num_frames)
-
-            R_all = np.zeros((num_frames, 2, 2))
-            U_all = np.zeros((num_frames, 2, 2))
-            lambda_1 = np.zeros(num_frames)
-            lambda_2 = np.zeros(num_frames)
-            vec_1 = np.zeros((num_frames, 2))
-            vec_2 = np.zeros((num_frames, 2))
-            for frame_num, f in enumerate(F_all):
-                R, U = polar(f)
-                R_all[frame_num] = R
-                U_all[frame_num] = U
-                w, v = np.linalg.eig(U)
-                lambda_1[frame_num] = np.min(w)
-                lambda_2[frame_num] = np.max(w)
-                v = R.dot(v)
-                vec_1[frame_num] = v[:, np.argmin(w)]
-                vec_2[frame_num] = v[:, np.argmax(w)]
-
-            img_list = []
-            Path("tmp").mkdir(parents=True, exist_ok=True)
-            radius = 0.2 * np.min(raw_frames.shape[1:])
-            th = np.linspace(0, 2.0 * np.pi, 100)
-            v = np.array([radius * np.cos(th), radius * np.sin(th)]).T
-            center = np.array(raw_frames.shape[1:]).reshape(-1) / 2
-            vec_circ = v + center
-            p1_1 = center - radius * vec_1
-            p1_2 = center + radius * vec_1
-            p2_1 = center - radius * vec_2
-            p2_2 = center + radius * vec_2
-            for frame_num, raw_img in enumerate(raw_frames):
-                plt.figure(figsize=(10, 5))
-                plt.subplot(1, 2, 1)
-                plt.imshow(raw_img, cmap=plt.cm.gray)
-                plt.plot(
-                    [p1_1[frame_num][1], p1_2[frame_num][1]],
-                    [p1_1[frame_num][0], p1_2[frame_num][0]],
-                    "-",
-                    color=(255 / 255, 204 / 255, 203 / 255),
-                    linewidth=0.3,
-                )
-                plt.plot(
-                    [p2_1[frame_num][1], p2_2[frame_num][1]],
-                    [p2_1[frame_num][0], p2_2[frame_num][0]],
-                    "-",
-                    color=(0.5, 0.5, 0.5),
-                    linewidth=0.3,
-                )
-                # add in eigenvector directions
-                f = F_all[frame_num]
-                v_def = v.dot(np.linalg.matrix_power(f, 9))
-                vec_inner_circ = v_def + center
-
-                plt.plot(
-                    vec_circ[:, 1],
-                    vec_circ[:, 0],
-                    "-",
-                    color=(255 / 255, 204 / 255, 203 / 255),
-                    linewidth=0.3,
-                )
-                plt.plot(
-                    vec_inner_circ[:, 1],
-                    vec_inner_circ[:, 0],
-                    "-",
-                    color=(255 / 255, 204 / 255, 203 / 255),
-                    linewidth=1.0,
-                )
-
-                OOP_vec = OOP_vec_all[frame_num]
-                OOP_rad = radius * OOP_all[frame_num]
-                plt.plot(
-                    [
-                        center[1] - OOP_vec[1] * OOP_rad,
-                        center[1] + OOP_vec[1] * OOP_rad,
-                    ],
-                    [
-                        center[0] - OOP_vec[0] * OOP_rad,
-                        center[0] + OOP_vec[0] * OOP_rad,
-                    ],
-                    "r-",
-                    linewidth=5,
-                )
-
-                ax = plt.gca()
-                ax.set_xticks([])
-                ax.set_yticks([])
-
-                plt.subplot(1, 2, 2)
-                plt.plot(
-                    frames, lambda_1, "-", color="k", linewidth=1, label="λ1"
-                )
-                plt.plot(
-                    frames,
-                    lambda_2,
-                    "-",
-                    color="#7F7F7F",
-                    linewidth=1,
-                    label="λ2",
-                )
-                plt.plot(
-                    frame_num,
-                    lambda_1[frame_num],
-                    "o",
-                    mfc="#B30000",
-                    mec="k",
-                    markersize=7,
-                )
-                plt.plot(
-                    frame_num,
-                    lambda_2[frame_num],
-                    "o",
-                    mfc="#B30000",
-                    mec="#7F7F7F",
-                    markersize=7,
-                )
-                plt.xlabel("frame number")
-                plt.legend()
-                plt.tight_layout()
-                plt.savefig(
-                    f"tmp/frame-{frame_num}.png",
-                    dpi=self.sg_tools.quality,
-                    bbox_inches="tight",
-                )
-                plt.close()
-                img_list.append(imageio.imread(f"tmp/frame-{frame_num}.png"))
-            shutil.rmtree("tmp")
-
-            if self.sg_tools.save_results:
-                with open(
-                    f"{self.sg_tools.output_dir}/recovered_lambda.npy", "wb"
-                ) as file:
-                    np.save(file, np.array([lambda_1, lambda_2]))
-            if num_frames > 1:
-                imageio.mimsave(
-                    f"{self.sg_tools.output_dir}/F_anim.gif", img_list
-                )
-
-        def timeseries_params(self):
-            """Visualize time series parameters."""
-            ts_params = self.sg_tools._load_ts_params()
-
-            plt.figure(figsize=(7, 7))
-
-            med = np.median(ts_params["mean_contraction_time"])
-            plt.subplot(2, 2, 1)
-            plt.hist(ts_params["mean_contraction_time"])
-            plt.plot([med, med], [0, 10], "r--")
-            plt.xlabel("frames")
-            plt.title(f"median_contract: {med:.2f}")
-            plt.tight_layout()
-
-            med = np.median(ts_params["mean_relax_time"])
-            plt.subplot(2, 2, 2)
-            plt.hist(ts_params["mean_relax_time"])
-            plt.plot([med, med], [0, 10], "r--")
-            plt.xlabel("frames")
-            plt.title(f"median_relax: {med:.2f}")
-            plt.tight_layout()
-
-            med = np.median(ts_params["mean_flat_time"])
-            plt.subplot(2, 2, 3)
-            plt.hist(ts_params["mean_flat_time"])
-            plt.plot([med, med], [0, 10], "r--")
-            plt.xlabel("frames")
-            plt.title(f"median_flat: {med:.2f}")
-            plt.tight_layout()
-
-            med = np.median(ts_params["mean_period_len"])
-            plt.subplot(2, 2, 4)
-            plt.hist(ts_params["mean_period_len"])
-            plt.plot([med, med], [0, 10], "r--")
-            plt.xlabel("frames")
-            plt.title(f"median_period: {med:.2f}")
-            plt.tight_layout()
-
-            out_file = f"{self.sg_tools.output_dir}/histogram_time_constants"
-            plt.savefig(
-                f"{out_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{out_file}.eps")
-
-        def dendrogram(self, dist_func: str = "dtw"):
-            """Cluster timeseries and plot a dendrogram that shows clusters.
-
-            Parameters
-            ----------
-            dist_func : str, optional, by default "dtw"
-                Choose between "euclidean" or "dtw"
-            """
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            num_frames = sarcomeres.frame.max() + 1
-            num_sarcs = sarcomeres.sarc_id.max() + 1
-            length = sarcomeres.length_norm.to_numpy().reshape(-1, num_frames)
-
-            if dist_func == "dtw":
-                dtw_dist = self.sg_tools.time_series._dtw_distance
-                dist_mat = np.zeros((num_sarcs, num_sarcs))
-                for sarc_1_id in range(num_sarcs):
-                    for sarc_2_id in range(sarc_1_id + 1, num_sarcs):
-                        dist = dtw_dist(
-                            length[sarc_1_id, :],
-                            length[sarc_2_id, :],
-                        )
-                        dist_mat[sarc_1_id, sarc_2_id] = dist
-                        dist_mat[sarc_2_id, sarc_1_id] = dist
-            if dist_func == "euclidean":
-                dist_mat = squareform(pdist(length, "euclidean"))
-
-            dist_v = squareform(dist_mat)
-            Z = linkage(dist_v, method="ward", metric="euclidean")
-
-            # --> plot dendrogram
-            plt.figure(figsize=(9, 30), frameon=False)
-            plt.subplot(1, 2, 1)
-            # dendrogram
-            dn1 = dendrogram(
-                Z,
-                orientation="left",
-                color_threshold=0,
-                above_threshold_color="k",
-            )
-            ordered = dn1["leaves"]  # from bottom to top
-
-            ax = plt.gca()
-            ax.xaxis.set_visible(False)
-            plt.subplot(1, 2, 2)
-            ax = plt.gca()
-
-            for kk in range(len(ordered)):
-                ix = ordered[kk]
-                col = (
-                    1 - kk / len(ordered),
-                    kk / len(ordered),
-                    1 - kk / len(ordered),
-                )
-                plt.plot(length[ix, :] + kk * 0.3, c=col)
-
-            plt.tight_layout()
-            plt.ylim((-0.4, kk * 0.3 + 0.35))
-            plt.axis("off")
-
-            output_file = f"{self.sg_tools.output_dir}/dendrogram_{dist_func}"
-            plt.savefig(f"{output_file}.pdf")
-
-        def spatial_graph(self):
-            """Visualizes the spatial graph
-
-            See Also
-            --------
-            :func:`sarcgraph.sg_tools.SarcGraphTools.Analysis.create_spatial_graph`
-            """
-            G = nx.read_gpickle(
-                f"{self.sg_tools.output_dir}/spatial-graph.pkl"
-            )
-
-            with open(
-                f"{self.sg_tools.output_dir}/spatial-graph-pos.pkl", "rb"
-            ) as file:
-                pos = pickle.load(file)
-
-            for node_1, node_2 in G.edges:
-                pos_1 = np.array(
-                    [G.nodes[node_1]["y_pos"], -G.nodes[node_1]["x_pos"]]
-                )
-                pos_2 = np.array(
-                    [G.nodes[node_2]["y_pos"], -G.nodes[node_2]["x_pos"]]
-                )
-                ang = 1 / np.sqrt(
-                    np.sum(((pos_1 - pos_2) / (pos_1[0] - pos_2[0])) ** 2)
-                )
-                G[node_1][node_2]["weight"] = ang
-
-            node_scores = []
-            for node in G.nodes:
-                edge_list = list(G.edges(node))
-                counter = 0
-                value = 0
-                for i in range(len(edge_list)):
-                    node_1 = edge_list[i][0]
-                    node_2 = edge_list[i][1]
-
-                    pos_1 = np.array(
-                        [G.nodes[node_1]["y_pos"], -G.nodes[node_1]["x_pos"]]
-                    )
-                    pos_2 = np.array(
-                        [G.nodes[node_2]["y_pos"], -G.nodes[node_2]["x_pos"]]
-                    )
-
-                    vec_1 = (pos_1 - pos_2) / np.linalg.norm(pos_1 - pos_2, 2)
-                    for j in range(i + 1, len(edge_list)):
-                        node_1 = edge_list[j][0]
-                        node_2 = edge_list[j][1]
-
-                        pos_1 = np.array(
-                            [
-                                G.nodes[node_1]["y_pos"],
-                                -G.nodes[node_1]["x_pos"],
-                            ]
-                        )
-                        pos_2 = np.array(
-                            [
-                                G.nodes[node_2]["y_pos"],
-                                -G.nodes[node_2]["x_pos"],
-                            ]
-                        )
-
-                        vec_2 = (pos_1 - pos_2) / np.linalg.norm(
-                            pos_1 - pos_2, 2
-                        )
-
-                        value += np.abs(np.dot(vec_1, vec_2))
-                        counter += 1
-
-                if counter:
-                    node_scores.append(value / counter)
-                else:
-                    node_scores.append(0)
-
-            plt.figure(figsize=(5, 5))
-            plt.axis("equal")
-            edges, weights = zip(*nx.get_edge_attributes(G, "weight").items())
-            nx.draw(
-                G,
-                pos,
-                node_color="k",
-                node_size=10,
-                width=2,
-                edge_color=weights,
-                edge_cmap=plt.cm.rainbow,
-            )
-
-            mi = np.min(node_scores)
-            ma = np.max(node_scores)
-            for node, node_score in zip(G.nodes, node_scores):
-                pos = np.array(
-                    [G.nodes[node]["y_pos"], -G.nodes[node]["x_pos"]]
-                )
-                color_val = 1 - (0.75 * (node_score - mi) / (ma - mi) + 0.25)
-                color = (color_val, color_val, color_val)
-                if node_score > 0.9:
-                    plt.plot(pos[0], pos[1], ".", color=color, ms=10)
-                if node_score > 0.75:
-                    plt.plot(pos[0], pos[1], ".", color=color, ms=7.5)
-                else:
-                    plt.plot(pos[0], pos[1], ".", color=color, ms=5)
-
-            output_file = f"./{self.sg_tools.output_dir}/spatial-graph"
-            plt.savefig(
-                f"./{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"./{output_file}.eps")
-
-        def tracked_vs_untracked(
-            self,
-            file_path: str,
-            start_frame: int = 0,
-            stop_frame: int = np.inf,
-        ):
-            """Visualize metrics to compare the effect of tracking sarcomeres
-            in a video vs only detecting sarcomeres in each frame without
-            tracking
-
-            Parameters
-            ----------
-            file_path: str
-                address to the original video file
-            start_frame : int, optional, by default 0
-            stop_frame : int, optional, by default np.inf
-            """
-            # process the whole video and detect and track sarcomeres
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            total_frames = sarcomeres.frame.max() + 1
-            stop_frame = min(stop_frame, total_frames)
-            start_frame = min(start_frame, stop_frame - 1)
-            num_frames = stop_frame - start_frame
-
-            sarcomeres = sarcomeres[
-                sarcomeres.frame.between(start_frame, stop_frame)
-            ]
-            num_tracked = sarcomeres.sarc_id.max() + 1
-
-            # process the video frame by frame - no tracking
-            sg_video = SarcGraph(self.sg_tools.input_dir)
-            segmented_zdiscs = sg_video.zdisc_segmentation(file_path)
-
-            length_all_frames = []
-            width_all_frames = []
-            angle_all_frames = []
-            median_length_all_frames = []
-            sarc_num_all_frames = []
-            sg_image = SarcGraph(self.sg_tools.input_dir, "image")
-            for frame in range(start_frame, stop_frame):
-                segmented_zdiscs_frame = segmented_zdiscs.loc[
-                    segmented_zdiscs.frame == frame
-                ].copy()
-                segmented_zdiscs_frame.loc[:, "frame"] = 0.0
-                tracked_zdiscs_frame = sg_image.zdisc_tracking(
-                    segmented_zdiscs=segmented_zdiscs_frame
-                )
-                sarcomeres_frame, _ = sg_image.sarcomere_detection(
-                    tracked_zdiscs=tracked_zdiscs_frame
-                )
-                length_all_frames.append(sarcomeres_frame.length.to_numpy())
-                width_all_frames.append(sarcomeres_frame.width.to_numpy())
-                angle_all_frames.append(sarcomeres_frame.angle.to_numpy())
-                median_length_all_frames.append(
-                    np.median(length_all_frames[-1])
-                )
-                sarc_num_all_frames.append(sarcomeres_frame.sarc_id.max() + 1)
-
-            # compute average number of not tracked sarcomeres in each frame
-            num_not_tracked = np.mean(sarc_num_all_frames)
-
-            len_diff_mean = []
-            sarcs_length_grouped = sarcomeres.groupby("frame").length
-            for untracked_len, tracked_len in zip(
-                length_all_frames, sarcs_length_grouped
-            ):
-                tracked_len = tracked_len[1].to_numpy()
-                tracked_len_mean = np.mean(tracked_len)
-                len_diff_mean.append(
-                    self.sg_tools.analysis._sampler(
-                        untracked_len,
-                        tracked_len_mean,
-                        num_tracked,
-                        num_run=1000,
-                    )
-                )
-
-            plt.figure(figsize=(np.clip(int(num_frames * 0.3), 10, 25), 5))
-            plt.boxplot(
-                len_diff_mean, positions=range(start_frame, stop_frame)
-            )
-            plt.plot([start_frame, stop_frame - 1], [-0.5, -0.5], "k--")
-            plt.plot([start_frame, stop_frame - 1], [0.5, 0.5], "k--")
-            plt.title(
-                f"Comparison of length in pixels, approx {num_not_tracked:.2f}"
-                f" untracked, {num_tracked} tracked"
-            )
-            plt.xlabel("frame number")
-            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
-            output_file = f"{self.sg_tools.output_dir}/length-comparison"
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps")
-
-            wid_diff_mean = []
-            sarcs_width_grouped = sarcomeres.groupby("frame").width
-            for untracked_wid, tracked_wid in zip(
-                width_all_frames, sarcs_width_grouped
-            ):
-                tracked_wid = tracked_wid[1].to_numpy()
-                tracked_wid_mean = np.mean(tracked_wid)
-                wid_diff_mean.append(
-                    self.sg_tools.analysis._sampler(
-                        untracked_wid,
-                        tracked_wid_mean,
-                        num_tracked,
-                        num_run=1000,
-                    )
-                )
-
-            plt.figure(figsize=(np.clip(int(num_frames * 0.3), 10, 25), 5))
-            plt.boxplot(
-                wid_diff_mean, positions=range(start_frame, stop_frame)
-            )
-            plt.plot([start_frame, stop_frame - 1], [-0.5, -0.5], "k--")
-            plt.plot([start_frame, stop_frame - 1], [0.5, 0.5], "k--")
-            plt.title(
-                f"Comparison of Width in pixels, approx {num_not_tracked:.2f} "
-                f"untracked, {num_tracked} tracked"
-            )
-            plt.xlabel("frame number")
-            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
-            output_file = f"{self.sg_tools.output_dir}/width-comparison"
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps")
-
-            ang_diff_mean = []
-            rad_diff_mean = []
-            sarcs_angle_grouped = sarcomeres.groupby("frame").angle
-            for untracked_ang, tracked_ang in zip(
-                angle_all_frames, sarcs_angle_grouped
-            ):
-                tracked_ang = tracked_ang[1].to_numpy()
-                out = self.sg_tools.analysis._angular_mean(tracked_ang)
-                tracked_ang_mean = out[0]
-                tracked_rad_mean = out[1]
-                ang_diff, rad_diff = self.sg_tools.analysis._angular_sampler(
-                    untracked_ang,
-                    tracked_ang_mean,
-                    tracked_rad_mean,
-                    num_tracked,
-                    num_run=1000,
-                )
-                ang_diff_mean.append(ang_diff)
-                rad_diff_mean.append(rad_diff)
-
-            plt.figure(figsize=(np.clip(int(num_frames * 0.3), 10, 25), 10))
-            plt.subplot(2, 1, 1)
-            plt.boxplot(
-                ang_diff_mean, positions=range(start_frame, stop_frame)
-            )
-            plt.plot(
-                [start_frame, stop_frame - 1], [-np.pi / 8, -np.pi / 8], "k--"
-            )
-            plt.plot(
-                [start_frame, stop_frame - 1], [np.pi / 8, np.pi / 8], "k--"
-            )
-            plt.title(
-                f"Comparison of angle in radians, approx {num_not_tracked:.2f}"
-                f" untracked, {num_tracked} tracked"
-            )
-            plt.xlabel("frame number")
-            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
-            plt.subplot(2, 1, 2)
-            plt.boxplot(
-                rad_diff_mean, positions=range(start_frame, stop_frame)
-            )
-            plt.plot(
-                [start_frame, stop_frame - 1], [0, 0], "r--", label="uniform"
-            )
-            plt.plot(
-                [start_frame, stop_frame - 1], [1, 1], "k--", label="oriented"
-            )
-            plt.title(
-                "Comparison of angle radius in pixels, approx "
-                f"{num_not_tracked:.2f} untracked, {num_tracked} tracked"
-            )
-            plt.xlabel("frame number")
-            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
-            plt.legend()
-            output_file = f"{self.sg_tools.output_dir}/angle-comparison"
-            plt.savefig(
-                f"{output_file}.png",
-                dpi=self.sg_tools.quality,
-                bbox_inches="tight",
-            )
-            if self.sg_tools.include_eps:
-                plt.savefig(f"{output_file}.eps")
-
-    ##########################################################
-    #                     Analysis Class                     #
-    ##########################################################
-    class Analysis:
-        def __init__(self, sg_tools):
-            """Provides tools for post processing analysis of detected
-            sarcomeres.
-            """
-            self.sg_tools = sg_tools
-
-        def _sampler(
-            self,
-            signal: np.ndarray,
-            mu: float,
-            tracked_num: int,
-            num_run: int = 1000,
-        ) -> np.ndarray:
-            """Random sampler
-
-            Parameters
-            ----------
-            signal : np.ndarray
-            mu : float
-            tracked_num : int
-            num_run : int, optional
-            """
-            samples = np.zeros(num_run)
-            for run in range(num_run):
-                ids = np.random.randint(0, len(signal), size=(tracked_num))
-                samples[run] = mu - np.mean(signal[ids])
-            return samples
-
-        def _angular_mean(self, signal: np.ndarray) -> Tuple[float, float]:
-            """Angular signal averaging
-
-            Parameters
-            ----------
-            signal : np.ndarray
-
-            Returns
-            -------
-            Tuple[float, float]
-                angle and radius of averaged signal
-            """
-            x_mean = np.nanmean(np.cos(signal))
-            y_mean = np.nanmean(np.sin(signal))
-
-            mean_angle = np.arctan2(y_mean, x_mean)
-            mean_rad = np.linalg.norm([x_mean, y_mean], 2)
-
-            return mean_angle, mean_rad
-
-        def _angular_sampler(
-            self,
-            signal: np.ndarray,
-            mu_ang: float,
-            mu_rad: float,
-            tracked_num: int,
-            num_run: int = 1000,
-        ) -> Tuple[np.ndarray, np.ndarray]:
-            """Angular random sampler
-
-            Parameters
-            ----------
-            signal : np.ndarray
-            mu_ang : float
-            mu_rad : float
-            tracked_num : int
-            num_run : int, by default 1000, optional
-
-            Returns
-            -------
-            Tuple[np.ndarray, np.ndarray]
-            """
-            ang_samples = np.zeros(num_run)
-            rad_samples = np.zeros(num_run)
-            for run in range(num_run):
-                ids = np.random.randint(0, len(signal), size=(tracked_num))
-                ang_mean, rad_mean = self.sg_tools.analysis._angular_mean(
-                    signal[ids]
-                )
-                ang_samples[run] = mu_ang - ang_mean
-                rad_samples[run] = mu_rad - rad_mean
-
-            return ang_samples, rad_samples
-
-        def compute_F_J(
-            self, adjust_reference: bool = False
-        ) -> Tuple[np.ndarray, np.ndarray]:
-            """Compute the average deformation gradient (F) and its jacobian
-            (J) for the whole movie.
-
-            Parameters
-            ----------
-            adjust_reference : bool, by default False
-                The refrence frame by default is the first frame of the movie,
-                if this variable is set to ``True`` the function will run twice
-                and the refrence frame on the second run will be the most
-                contracted frame
-
-            Returns
-            -------
-            Tuple(np.ndarray, np.ndarray)
-                The average deformation gradient (F), shape=(num_frames, 2, 2)
-                The jacobian of F, shape=(num_frames)
-            """
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            sarcs_x = sarcomeres.x.to_numpy()
-            sarcs_y = sarcomeres.y.to_numpy()
-
-            # compute Lambda from x_pos and y_pos
-            num_frames = sarcomeres.frame.max() + 1
-            num_sarcs = sarcomeres.sarc_id.max() + 1
-            n = int(num_sarcs * (num_sarcs - 1) / 2)
-
-            Lambda_list = []
-            for frame_num in range(num_frames):
-                ids = sarcomeres.frame == frame_num
-                x_vec = sarcs_x[ids]
-                y_vec = sarcs_y[ids]
-
-                Lambda = np.zeros((2, n))
-                x_vec_tile = np.tile(x_vec, (num_sarcs, 1))
-                v_x = x_vec_tile.T - x_vec_tile
-                y_vec_tile = np.tile(y_vec, (num_sarcs, 1))
-                v_y = y_vec_tile.T - y_vec_tile
-
-                indices = np.triu_indices(num_sarcs, 1)
-                Lambda[0, :] = v_x[indices]
-                Lambda[1, :] = v_y[indices]
-
-                Lambda_list.append(Lambda)
-
-            F_all = np.zeros((num_frames, 2, 2))
-            J_all = np.zeros(num_frames)
-            num_iter = 2 if adjust_reference else 1
-            for iter in range(num_iter):
-                ref_frame = np.argmax(J_all)
-                for target_frame in range(num_frames):
-                    Lambda_i = Lambda_list[ref_frame]
-                    Lambda_t = Lambda_list[target_frame]
-                    term_1 = np.dot(Lambda_t, Lambda_i.T)
-                    term_2 = np.linalg.inv(np.dot(Lambda_i, Lambda_i.T))
-                    F = np.dot(term_1, term_2)
-                    F_all[target_frame] = F
-                    J_all[target_frame] = np.linalg.det(F)
-
-            if self.sg_tools.save_results:
-                np.save(f"{self.sg_tools.output_dir}/recovered_F.npy", F_all)
-                np.save(f"{self.sg_tools.output_dir}/recovered_J.npy", J_all)
-
-            return F_all, J_all
-
-        def compute_OOP(self) -> Tuple[np.ndarray, np.ndarray]:
-            """Computes Orientation Order Parameter (OOP) for the whole movie.
-
-            Returns
-            -------
-            Tuple[np.ndarray, np.ndarray]
-                OOP for all frames, shape=(num_frames)
-                OOP vector for all frames, shape=(num_frames, 2)
-            """
-
-            def f(data):
-                rxx = np.cos(data) ** 2
-                rxy = np.cos(data) * np.sin(data)
-                ryy = np.sin(data) ** 2
-                n = np.array([[rxx, rxy], [rxy, ryy]])
-                t = 2 * n - np.eye(2).reshape(2, 2, 1)
-                return np.mean(t, axis=2)
-
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-            num_frames = sarcomeres.frame.max() + 1
-
-            T = sarcomeres.groupby("frame")["angle"].apply(lambda x: f(x))
-            OOP_all = np.zeros(num_frames)
-            OOP_vec_all = np.zeros((num_frames, 2))
-            for frame in range(num_frames):
-                u, v = np.linalg.eig(T[frame])
-                OOP_all[frame] = np.max(u)
-                OOP_vec_all[frame, :] = v[:, np.argmax(u)]
-
-            if self.sg_tools.save_results:
-                np.save(
-                    f"{self.sg_tools.output_dir}/recovered_OOP.npy", OOP_all
-                )
-                np.save(
-                    f"{self.sg_tools.output_dir}/recovered_OOP_vector.npy",
-                    OOP_vec_all,
-                )
-
-            return OOP_all, OOP_vec_all
-
-        def compute_metrics(self, frame: int = None) -> dict:
-            """This function computes the following metrics as defind in the
-            paper: {OOP, C_iso, C_OOP, s_til, s_avg}.
-
-            Parameters
-            ----------
-            frame : int, optional
-                By default is set to the frame with maximum contraction
-
-            Notes
-            -----
-            See the paper for more information:
-            https://arxiv.org/abs/2102.02412
-
-            Returns
-            -------
-            dict
-            """
-
-            def f(data):
-                return (np.max(data) - np.min(data)) / (np.max(data) + 1)
-
-            F_all = self.sg_tools._load_recovered_info("F")
-            J_all = self.sg_tools._load_recovered_info("J")
-            OOP_all = self.sg_tools._load_recovered_info("OOP")
-            OOP_vec_all = self.sg_tools._load_recovered_info("OOP_vector")
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-
-            if frame is None:
-                frame = np.argmin(J_all)
-            OOP = OOP_all[frame]
-            OOP_vec = OOP_vec_all[frame]
-            F = F_all[frame]
-            J = J_all[frame]
-
-            v = OOP_vec
-            v_abs = np.linalg.norm(v, 2)
-            v0 = np.dot(np.linalg.inv(F), v)
-            v0_abs = np.linalg.norm(v0, 2)
-            avg_contract = 1 - np.sqrt(J)
-            avg_aligned_contract = (v0_abs - v_abs) / v0_abs
-
-            sarcs_groupby_sarc_id = sarcomeres.groupby("sarc_id").length_norm
-            sarcs_groupby_frame = sarcomeres.groupby("frame").length_norm
-
-            s_til = sarcs_groupby_sarc_id.apply(lambda x: f(x)).median()
-            s_avg = f(sarcs_groupby_frame.mean())
-
-            info_dict = {
-                "OOP": OOP,
-                "C_iso": avg_contract,
-                "C_OOP": avg_aligned_contract,
-                "s_til": s_til,
-                "s_avg": s_avg,
-            }
-
-            if self.sg_tools.save_results:
-                with open(
-                    f"{self.sg_tools.output_dir}/recovered_metrics.json", "w"
-                ) as file:
-                    json.dump(info_dict, file)
-
-            return info_dict
-
-        def compute_ts_params(self) -> pd.DataFrame:
-            """Compute and save timeseries time constants (contraction time,
-            relaxation time, flat time, period, offset, etc.).
-
-            Returns
-            -------
-            pd.DataFrame
-            """
-            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
-            num_sarcs = sarcomeres.sarc_id.max() + 1
-            num_frames = sarcomeres.frame.max() + 1
-
-            sarcs_length = sarcomeres.groupby("sarc_id").length
-            sarcs_length_norm = sarcomeres.groupby("sarc_id").length_norm
-
-            signal_th = 0
-            signal_dist = 10
-            signal_width = 5
-
-            frames = np.arange(0, num_frames, 1)
-            sarc_ids = np.arange(0, num_sarcs, 1)
-            pix_length_median = np.zeros(num_sarcs)
-            pix_length_mean = np.zeros(num_sarcs)
-            pix_length_min = np.zeros(num_sarcs)
-            pix_length_max = np.zeros(num_sarcs)
-            pix_percent_shortening = np.zeros(num_sarcs)
-            mean_contraction_time = np.zeros(num_sarcs)
-            mean_relax_time = np.zeros(num_sarcs)
-            mean_flat_time = np.zeros(num_sarcs)
-            mean_period_len = np.zeros(num_sarcs)
-            frames_to_first_peak = np.zeros(num_sarcs)
-            peaks_count = np.zeros(num_sarcs)
-            for length, length_norm in zip(sarcs_length, sarcs_length_norm):
-                sarc_id = length[0]
-                sarc_length = length[1].to_numpy()
-                sarc_length_norm = length_norm[1].to_numpy()
-
-                sarc_length_med = signal.medfilt(sarc_length_norm, 5)
-                sarc_length_deriv = np.gradient(sarc_length_norm, frames)
-
-                thresh_flat = 0.025 * (
-                    np.max(sarc_length_med) - np.min(sarc_length_med)
-                )
-                count_R = np.sum(sarc_length_deriv > thresh_flat)
-                count_C = np.sum(sarc_length_deriv < -thresh_flat)
-                count_F = num_frames - count_R - count_C
-
-                # detect valleys
-                peaks_L, _ = signal.find_peaks(
-                    -sarc_length_med,
-                    threshold=signal_th,
-                    distance=signal_dist,
-                    width=signal_width,
-                )
-
-                num_peaks = np.sum(
-                    sarc_length_med[peaks_L]
-                    < np.mean(sarc_length_med) - thresh_flat
-                )
-                if num_peaks == 0:
-                    num_peaks = np.inf
-
-                mean_contraction_time[sarc_id] = count_C / num_peaks
-                mean_relax_time[sarc_id] = count_R / num_peaks
-                mean_flat_time[sarc_id] = count_F / num_peaks
-
-                min_sarc_length = np.min(sarc_length)
-                max_sarc_length = np.max(sarc_length)
-                pix_length_median[sarc_id] = np.median(sarc_length)
-                pix_length_mean[sarc_id] = np.mean(sarc_length)
-                pix_length_min[sarc_id] = min_sarc_length
-                pix_length_max[sarc_id] = max_sarc_length
-                pix_percent_shortening[sarc_id] = (
-                    100 * (max_sarc_length - min_sarc_length) / max_sarc_length
-                )
-
-                if peaks_L.size:
-                    frames_to_first_peak[sarc_id] = peaks_L[0]
-                else:
-                    frames_to_first_peak[sarc_id] = 0
-
-                mean_period_len[sarc_id] = num_frames / num_peaks
-                peaks_count[sarc_id] = num_peaks
-
-            # import data to a dataframe
-            data = np.vstack(
-                (
-                    sarc_ids,
-                    pix_length_median,
-                    pix_length_mean,
-                    pix_length_min,
-                    pix_length_max,
-                    pix_percent_shortening,
-                    mean_contraction_time,
-                    mean_relax_time,
-                    mean_flat_time,
-                    mean_period_len,
-                    frames_to_first_peak,
-                    peaks_count,
-                )
-            )
-
-            cols = [
-                "sarc_ids",
-                "pix_length_median",
-                "pix_length_mean",
-                "pix_length_min",
-                "pix_length_max",
-                "pix_percent_shortening",
-                "mean_contraction_time",
-                "mean_relax_time",
-                "mean_flat_time",
-                "mean_period_len",
-                "frames_to_first_peak",
-                "peaks_count",
-            ]
-
-            df = pd.DataFrame(data.T, columns=cols)
-
-            if self.sg_tools.save_results:
-                df.to_csv(
-                    f"./{self.sg_tools.output_dir}/timeseries_params.csv"
-                )
-
-            return df
-
-        def create_spatial_graph(
-            self,
-            file_path: str = None,
-            tracked_zdiscs: pd.DataFrame = None,
-        ):
-            """Generates and saves a spatial graph of tracked zdiscs where
-            edges indicate sarcomeres and edge weights indicates the ratio of
-            the frames in which that sarcomere is detected
-
-            Parameters
-            ----------
-            file_path : str
-                The address of an image or a video file to be loaded
-            tracked_zdiscs : pd.DataFrame
-                Information of all detected and tracked zdiscs in every frame.
-            """
-            sg_video = SarcGraph(file_type="video")
-
-            # load tracked zdiscs:
-            if tracked_zdiscs is None:
-                if file_path is None:
-                    raise ValueError(
-                        "either file_path or "
-                        + "tracked_zdiscs should be specified."
-                    )
-                tracked_zdiscs = sg_video.zdisc_tracking(
-                    file_path, save_output=False
-                )
-
-            # initiate the graph:
-            G = nx.Graph()
-
-            pos = {}
-            for particle in tracked_zdiscs.particle.unique():
-                x_pos = tracked_zdiscs[tracked_zdiscs.particle == particle][
-                    "x"
-                ].mean()
-                y_pos = tracked_zdiscs[tracked_zdiscs.particle == particle][
-                    "y"
-                ].mean()
-                G.add_node(particle, x_pos=x_pos, y_pos=y_pos)
-                pos.update({particle: (y_pos, -x_pos)})
-
-            # SarcGraph object that work with single frames
-            sg_image = SarcGraph(file_type="image")
-
-            # frame by frame sarcomere detection, add graph edges and weigts:
-            for frame in tracked_zdiscs.frame.unique():
-                tracked_zdiscs_frame = tracked_zdiscs[
-                    tracked_zdiscs.frame == frame
-                ]
-                tracked_zdiscs_frame.loc[:]["frame"] = 0
-                _, myofibrils = sg_image.sarcomere_detection(
-                    tracked_zdiscs=tracked_zdiscs_frame, save_output=False
-                )
-                for myo in myofibrils:
-                    for edge in myo.edges:
-                        disc_1 = myo.nodes[edge[0]]["particle_id"]
-                        disc_2 = myo.nodes[edge[1]]["particle_id"]
-                        if G.has_edge(disc_1, disc_2):
-                            G[disc_1][disc_2]["weight"] += 1
-                        else:
-                            G.add_edge(disc_1, disc_2, weight=1)
-
-            # graph pruning based on minimum weight threshold
-            num_frames = tracked_zdiscs.frame.max() + 1
-            weight_cutoff = np.floor(0.1 * num_frames)
-            edges, weights = zip(*nx.get_edge_attributes(G, "weight").items())
-            for edge in edges:
-                if G[edge[0]][edge[1]]["weight"] < weight_cutoff:
-                    G.remove_edge(edge[0], edge[1])
-
-            # isolated nodes removal
-            isolated_nodes = list(nx.isolates(G))
-            G.remove_nodes_from(isolated_nodes)
-
-            # save the graph
-            output_file = f"{self.sg_tools.output_dir}/spatial-graph"
-            nx.write_gpickle(G, path=f"{output_file}.pkl")
-            with open(f"{output_file}-pos.pkl", "wb") as file:
-                pickle.dump(pos, file)
-
-    ###########################################################
-    #                    Utility Functions                    #
-    ###########################################################
-    def _run_all(self, file_path: str = None):
-        """Runs all functions in the Analysis class and saves outputs.
-
-        Parameters
-        ----------
-        file_path : str
-            Path to the input video or image file.
-        """
-        self.analysis.compute_F_J()
-        self.analysis.compute_OOP()
-        self.analysis.compute_metrics()
-        self.analysis.compute_ts_params()
-        self.analysis.create_spatial_graph(file_path)
-
-    def _load_raw_frames(self):
-        try:
-            raw_frames = np.load(f"{self.input_dir}/raw-frames.npy")
-        except Exception:
-            self._raise_sarcgraph_data_not_found("raw-frames.npy")
-        return raw_frames
-
-    def _load_contours(self):
-        try:
-            contours = np.load(
-                f"{self.input_dir}/contours.npy",
-                allow_pickle=True,
-            )
-        except Exception:
-            self._raise_sarcgraph_data_not_found("contours.npy")
-        return contours
-
-    def _load_sarcomeres(self):
-        try:
-            sarcomeres = pd.read_csv(
-                f"{self.input_dir}/sarcomeres.csv", index_col=[0]
-            )
-        except Exception:
-            self._raise_sarcgraph_data_not_found("sarcomeres.csv")
-        return sarcomeres
-
-    def _load_sarcomeres_gpr(self):
-        try:
-            sarcomeres = pd.read_csv(
-                f"{self.input_dir}/sarcomeres_gpr.csv",
-                index_col=[0],
-            )
-        except Exception:
-            self._raise_data_not_found("sarcomeres_gpr.csv")
-        return sarcomeres
-
-    def _load_recovered_info(self, info_type: str):
-        try:
-            OOP = np.load(f"{self.input_dir}/recovered_{info_type}.npy")
-        except Exception:
-            self._raise_data_not_found(f"recovered_{info_type}.npy")
-        return OOP
-
-    def _load_ts_params(self):
-        try:
-            ts_params = pd.read_csv(
-                f"{self.input_dir}/timeseries_params.csv",
-                index_col=[0],
-            )
-        except FileNotFoundError:
-            self._raise_data_not_found("timeseries_params.csv")
-        return ts_params
-
-    def _raise_sarcgraph_data_not_found(self, data_file: str):
-        raise FileNotFoundError(
-            f"{data_file} was not found in {self.input_dir}/. Run "
-            "SarcGraph().sarcomeres_detection(save_output=True) first."
-        )
-
-    def _raise_data_not_found(self, data_file: str):
-        raise FileNotFoundError(
-            f"{data_file} was not found in {self.input_dir}/. Run "
-            "SarcGraphTools()._run_all() first."
-        )
+import numpy as np
+import matplotlib.pyplot as plt
+import pandas as pd
+import networkx as nx
+import pickle
+import imageio
+import shutil
+import json
+import os
+
+from matplotlib.lines import Line2D
+from scipy import signal
+from scipy.signal import find_peaks
+from scipy.linalg import polar
+from sklearn.gaussian_process import GaussianProcessRegressor
+from sklearn.gaussian_process.kernels import RBF, WhiteKernel
+from scipy.spatial.distance import pdist, squareform
+from scipy.cluster.hierarchy import linkage, dendrogram
+from pathlib import Path
+from typing import Tuple  # List, Union
+
+from warnings import simplefilter
+from sklearn.exceptions import ConvergenceWarning
+
+from sarcgraph.sg import SarcGraph
+
+simplefilter("ignore", category=ConvergenceWarning)
+
+
+class SarcGraphTools:
+    def __init__(
+        self,
+        input_dir: str = "test-run",
+        quality: int = 300,
+        include_eps: bool = False,
+        save_results: bool = True,
+    ):
+        """Tools for post processing analysis on detected sarcomeres.
+
+        Parameters
+        ----------
+        input_dir : str
+            Should be the same as the `output_dir` in sarcgraph.sg.Sarcgraph(),
+             by default "test-run"
+        quality : int
+            dpi of saved figures in png format, by default 300
+        include_eps : bool
+            save eps format of figures, by default False
+        save_results : bool
+            save the results of post processing analysis, by default True
+        """
+        if not os.path.exists(input_dir):
+            raise FileNotFoundError(f"{input_dir}/ directory was not found!")
+
+        self.input_dir = input_dir
+        self.output_dir = input_dir
+        self.quality = quality
+        self.include_eps = include_eps
+        self.save_results = save_results
+        self.visualization = self.Visualization(self)
+        self.time_series = self.TimeSeries(self)
+        self.analysis = self.Analysis(self)
+
+    ###########################################################
+    #                    Time Series Class                    #
+    ###########################################################
+    class TimeSeries:
+        def __init__(self, sg_tools):
+            """Provides the tools to apply Gaussian Process Regression (GPR) on
+            timeseries of detected sarcomere
+            """
+            self.sg_tools = sg_tools
+
+        def _dtw_distance(self, s1: np.ndarray, s2: np.ndarray) -> np.ndarray:
+            """Compute distance based on dynamic time warping (DTW) between
+            two 1D signals s1 and s2.
+
+            Parameters
+            ----------
+            s1 : np.ndarray
+                1D signal
+            s2 : np.ndarray
+                1D signal
+
+            Returns
+            -------
+            np.ndarray
+                DTW distance between s1 and s2 based on euclidean distance.
+            """
+            if (not isinstance(s1, np.ndarray)) or (
+                not isinstance(s2, np.ndarray)
+            ):
+                raise TypeError("s1 and s2 must be 1D numpy arrays.")
+            if s1.ndim == 1 and s2.ndim == 1:
+                n = len(s1)
+                m = len(s2)
+                dtw = np.inf * np.ones((n + 1, m + 1))
+                dtw[0, 0] = 0
+                dist = (s1.reshape(-1, 1) - s2.reshape(1, -1)) ** 2
+                for i in range(1, n + 1):
+                    for j in range(1, m + 1):
+                        dtw[i, j] = dist[i - 1, j - 1] + min(
+                            dtw[i - 1, j], dtw[i, j - 1], dtw[i - 1, j - 1]
+                        )
+                return np.sqrt(dtw[-1, -1])
+            else:
+                raise ValueError("s1 and s2 must be 1D numpy arrays.")
+
+        def _gpr(self, s: np.ndarray) -> np.ndarray:
+            """Applies Gaussian Process Regression (GPR) on a 1D signal
+
+            Parameters
+            ----------
+            s : np.ndarray
+
+            Returns
+            -------
+            np.ndarray
+
+            Notes
+            -----
+            For more information on GPR check:
+            https://scikit-learn.org/stable/modules/gaussian_process.html
+            """
+            num_frames = len(s)
+
+            kernel = 1.0 * RBF(
+                length_scale=1.0, length_scale_bounds=(1e-5, 1e1)
+            ) + 1.0 * WhiteKernel(
+                noise_level=1.0, noise_level_bounds=(1e-5, 1e1)
+            )
+            model = GaussianProcessRegressor(kernel=kernel, normalize_y=True)
+            xdata = np.arange(num_frames).reshape(-1, 1)
+            xhat = xdata
+            ydata = s.reshape(-1, 1)
+
+            remove_indices = np.where(np.isnan(ydata.reshape(-1)))[0]
+            xdata = np.delete(xdata, remove_indices, axis=0)
+            ydata = np.delete(ydata, remove_indices, axis=0)
+
+            model.fit(xdata, ydata)
+            yhat = model.predict(xhat)
+
+            return yhat.reshape(-1)
+
+        def _sarcomeres_length_normalize(
+            self, sarcomeres: pd.DataFrame
+        ) -> pd.DataFrame:
+            groupby_sarc_id = sarcomeres.groupby("sarc_id")
+            mean_length = groupby_sarc_id.length.transform("mean")
+            sarcomeres["length_norm"] = (
+                sarcomeres.length - mean_length
+            ) / mean_length
+            return sarcomeres
+
+        def sarcomeres_gpr(self) -> pd.DataFrame:
+            """Applies Gaussian Process Regression (GPR) on the output of the
+            sarcomere detection algorithm to reduce the noise and fill in
+            missing data.
+
+            Returns
+            -------
+            pd.DataFrame
+
+            Notes
+            -----
+            For more information on GPR check
+            https://scikit-learn.org/stable/modules/gaussian_process.html
+
+            See Also
+            --------
+            :func:`sarcgraph.sg.SarcGraph.sarcomere_detection`
+            """
+            sarcomeres = self.sg_tools._load_sarcomeres()
+            cols = [
+                "x",
+                "y",
+                "length",
+                "angle",
+                "width",
+            ]
+
+            num_sarcs = sarcomeres.sarc_id.max() + 1
+            for info_type in cols:
+                for sarc_num in range(num_sarcs):
+                    row_mask = sarcomeres.sarc_id == sarc_num
+                    s = sarcomeres.loc[row_mask, info_type].to_numpy()
+                    sarcomeres.loc[row_mask, info_type] = self._gpr(s)
+            sarcomeres = self._sarcomeres_length_normalize(sarcomeres)
+            if self.sg_tools.save_results:
+                sarcomeres.to_csv(
+                    f"./{self.sg_tools.output_dir}/sarcomeres_gpr.csv"
+                )
+            return sarcomeres
+
+    #############################################################
+    #                    Visualization Class                    #
+    #############################################################
+    class Visualization:
+        def __init__(self, sg_tools):
+            """Provides tools to visualize the results of post-processing
+            analysis on detected sarcomeres.
+            """
+            self.sg_tools = sg_tools
+
+        def zdiscs_and_sarcs(self, frame_num: int = 0):
+            """Visualize and save the plot of segmented zdiscs and detected
+            sarcomeres in the chosen frame
+
+            Parameters
+            ----------
+            frame_num : int, by default 0
+            """
+            raw_frame = self.sg_tools._load_raw_frames()[frame_num]
+            contours = self.sg_tools._load_contours()[frame_num]
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            sarcs_x = sarcomeres[sarcomeres.frame == frame_num].x
+            sarcs_y = sarcomeres[sarcomeres.frame == frame_num].y
+
+            ax = plt.axes()
+            ax.set_aspect("equal")
+            ax.imshow(raw_frame[:, :, 0], cmap=plt.cm.gray)
+            ax.set_title(
+                f"{len(contours)} z-disks and {len(sarcs_x)} sarcomeres "
+                f"in frame {frame_num+1}"
+            )
+            for contour in contours:
+                ax.plot(contour[:, 1], contour[:, 0], "#0000cc", linewidth=1)
+            ax.plot(sarcs_y, sarcs_x, "*", color="#cc0000", markersize=3)
+            ax.set_xticks([])
+            ax.set_yticks([])
+
+            # Create legend
+            legend_elements = [
+                Line2D([0], [0], color="#0000cc", lw=4, label="Z-disc"),
+                Line2D(
+                    [0],
+                    [0],
+                    marker="*",
+                    color="#cc0000",
+                    markersize=8,
+                    linestyle="None",
+                    label="Sarcomere",
+                ),
+            ]
+
+            ax.legend(handles=legend_elements)
+
+            output_file = (
+                f"{self.sg_tools.output_dir}/zdiscs-sarcs-frame-{frame_num}"
+            )
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
+
+            plt.show()
+
+        def contraction(self):
+            """Visualize all detected sarcomeres in every frame according to
+            normalized fraction length and save as a gif file.
+            """
+            raw_frames = self.sg_tools._load_raw_frames()
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            num_frames = sarcomeres.frame.max() + 1
+            frames = sarcomeres.frame.to_numpy()
+            sarcs_x = sarcomeres.x.to_numpy()
+            sarcs_y = sarcomeres.y.to_numpy()
+            sarcs_length_norm = sarcomeres.length_norm.to_numpy()
+
+            img_list = []
+            Path("tmp").mkdir(parents=True, exist_ok=True)
+            for frame_num in range(num_frames):
+                indices = frames == frame_num
+                raw_frame = raw_frames[frame_num, :, :, 0]
+
+                plt.figure()
+                plt.imshow(raw_frame, cmap=plt.cm.gray)
+                y = sarcs_x[indices]
+                x = sarcs_y[indices]
+                length = np.abs(sarcs_length_norm[indices])
+                colors = np.piecewise(
+                    length,
+                    [length < 0.2, length >= 0.2],
+                    [lambda x: 2.5 * x + 0.5, lambda x: x],
+                )
+                for p_x, p_y, p_col in zip(x, y, colors):
+                    col = (1 - p_col, 0, p_col)
+                    plt.scatter(p_x, p_y, s=15, color=col, marker="o")
+
+                ax = plt.gca()
+                ax.set_xticks([])
+                ax.set_yticks([])
+                plt.savefig(
+                    f"tmp/frame-{frame_num}.png",
+                    dpi=self.sg_tools.quality,
+                    bbox_inches="tight",
+                )
+                plt.close()
+                img_list.append(imageio.imread(f"tmp/frame-{frame_num}.png"))
+            shutil.rmtree("tmp")
+            if num_frames > 1:
+                imageio.mimsave(
+                    f"{self.sg_tools.output_dir}/contract_anim.gif", img_list
+                )
+            print(
+                f"GIF saved as '{self.sg_tools.output_dir}/contract_anim.gif'!"
+            )
+
+        def normalized_sarcs_length(self):
+            """Plot normalized length of all detected sarcomeres vs frame
+            number.
+            """
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            num_sarcs = sarcomeres.sarc_id.max() + 1
+            sarc_ids = sarcomeres.sarc_id.to_numpy()
+            sarcs_length_norm = sarcomeres.length_norm.to_numpy()
+            groupby_frame = sarcomeres.groupby("frame")
+            sarcs_length_norm_median = groupby_frame.length_norm.median()
+            sarcs_length_norm_mean = groupby_frame.length_norm.mean()
+
+            _, ax = plt.subplots(figsize=(5, 5))
+            ax.grid("on")
+            for sarc_id in range(num_sarcs):
+                indices = sarc_ids == sarc_id
+                plt.plot(
+                    sarcs_length_norm[indices],
+                    linewidth=0.25,
+                    color=(0.545, 0.106, 0.086),
+                    alpha=0.1,
+                )
+            plt.plot(
+                sarcs_length_norm_mean,
+                "k-",
+                linewidth=2,
+                label="mean curve",
+            )
+            plt.plot(
+                sarcs_length_norm_median,
+                "--",
+                color=(0.5, 0.5, 0.5),
+                linewidth=2,
+                label="median curve",
+            )
+            plt.xlabel("frame")
+            plt.ylabel("normalized length")
+            plt.title(
+                f"timeseries data, tracked and normalized, {num_sarcs} "
+                "sarcomeres"
+            )
+            plt.ylim((-0.1, 0.1))
+            plt.legend()
+            plt.tight_layout()
+            output_file = (
+                f"{self.sg_tools.output_dir}/normalized_sarcomeres_length"
+            )
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
+
+            plt.show()
+
+        def OOP(self):
+            """Plot recovered Orientational Order Parameter."""
+            OOP = self.sg_tools._load_recovered_info("OOP")
+
+            plt.figure(figsize=(5, 5))
+            plt.subplot(1, 1, 1)
+            plt.plot(OOP, "k-", label="OOP recovered")
+            plt.legend()
+            plt.title("recovered Orientational Order Parameter")
+            plt.xlabel("frames")
+
+            output_file = f"{self.sg_tools.output_dir}/recovered_OOP"
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
+
+            plt.show()
+
+        def F(self):
+            """Plot recovered deformation gradient."""
+            F = self.sg_tools._load_recovered_info("F")
+
+            _, ax = plt.subplots(figsize=(5, 5))
+            ax.grid("on")
+            plt.plot(
+                F[:, 0, 0] - 1,
+                "--",
+                color=(0.078, 0.118, 0.594),
+                linewidth=5,
+                label="F11 recovered",
+            )
+            plt.plot(
+                F[:, 1, 1] - 1,
+                "--",
+                color=(0.545, 0.106, 0.086),
+                linewidth=4,
+                label="F22 recovered",
+            )
+            plt.plot(
+                F[:, 0, 1],
+                ":",
+                color=(0.078, 0.118, 0.594),
+                label="F12 recovered",
+            )
+            plt.plot(
+                F[:, 1, 0],
+                ":",
+                color=(0.545, 0.106, 0.086),
+                label="F21 recovered",
+            )
+            plt.legend()
+            plt.title("recovered deformation gradient")
+            plt.xlabel("frames")
+            plt.ylabel("value")
+            output_file = f"{self.sg_tools.output_dir}/recovered_F"
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
+
+            plt.show()
+
+        def J(self):
+            """Plot recovered deformation jacobian."""
+            J = self.sg_tools._load_recovered_info("J")
+            frames = np.arange(len(J))
+
+            # compute the parameters of the timeseries
+            plt.figure(figsize=(5, 5))
+            plt.plot(J, "k-")
+
+            J_med = signal.medfilt(J, 5)
+            J_deriv = np.gradient(J, frames)
+            count_C = 0
+            count_R = 0
+            count_F = 0
+            thresh_flat = 0.01 * (np.max(J) - np.min(J))
+
+            for frame_num in range(len(frames)):
+                if J_deriv[frame_num] > thresh_flat:
+                    count_R += 1
+                    plt.plot(
+                        frames[frame_num],
+                        J[frame_num],
+                        "o",
+                        color=(0.5, 0.5, 0.5),
+                    )
+                elif J_deriv[frame_num] < -1.0 * thresh_flat:
+                    count_C += 1
+                    plt.plot(
+                        frames[frame_num], J[frame_num], "o", color=(0.5, 0, 0)
+                    )
+                else:
+                    count_F += 1
+                    plt.plot(
+                        frames[frame_num], J[frame_num], "o", color=(0, 0, 0.5)
+                    )
+
+            # detect peaks and valleys
+            # peaks_U, _ = find_peaks(data_med, threshold=th, distance=di,
+            # width=wi)
+            peaks_L, _ = find_peaks(
+                -1.0 * J_med, threshold=0.0, distance=10, width=5
+            )
+            plt.grid()
+            # plt.plot(x[peaks_U],data[peaks_U],'rx',markersize=10)
+            plt.plot(frames[peaks_L], J[peaks_L], "rx", markersize=13)
+            plt.title(
+                f"frames contract: {count_C}, relax: {count_R}, flat: "
+                f"{count_F}"
+            )
+            plt.xlabel("frame number")
+            plt.ylabel("determinate of average F")
+            plt.tight_layout()
+
+            output_file = f"{self.sg_tools.output_dir}/recovered_J"
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps", bbox_inches="tight")
+
+            plt.show()
+
+        def F_eigenval_animation(self, no_anim=False):
+            """Visualize the eigenvalues of F over all frames"""
+            F_all = self.sg_tools._load_recovered_info("F")
+            J_all = self.sg_tools._load_recovered_info("J")
+
+            num_frames = len(J_all)
+            frames = np.arange(num_frames)
+
+            R_all = np.zeros((num_frames, 2, 2))
+            U_all = np.zeros((num_frames, 2, 2))
+            lambda_1 = np.zeros(num_frames)
+            lambda_2 = np.zeros(num_frames)
+            vec_1 = np.zeros((num_frames, 2))
+            vec_2 = np.zeros((num_frames, 2))
+            for frame_num, f in enumerate(F_all):
+                R, U = polar(f)
+                R_all[frame_num] = R
+                U_all[frame_num] = U
+                w, v = np.linalg.eig(U)
+                lambda_1[frame_num] = np.min(w)
+                lambda_2[frame_num] = np.max(w)
+                v = R.dot(v)
+                vec_1[frame_num] = v[:, np.argmin(w)]
+                vec_2[frame_num] = v[:, np.argmax(w)]
+
+            if no_anim:
+                return np.array([lambda_1, lambda_2])
+
+            raw_frames = self.sg_tools._load_raw_frames()[:, :, :, 0]
+            OOP_all = self.sg_tools._load_recovered_info("OOP")
+            OOP_vec_all = self.sg_tools._load_recovered_info("OOP_vector")
+
+            if self.sg_tools.save_results:
+                with open(
+                    f"{self.sg_tools.output_dir}/recovered_lambda.npy", "wb"
+                ) as file:
+                    np.save(file, np.array([lambda_1, lambda_2]))
+
+            img_list = []
+            Path("tmp").mkdir(parents=True, exist_ok=True)
+            radius = 0.2 * np.min(raw_frames.shape[1:])
+            th = np.linspace(0, 2.0 * np.pi, 100)
+            v = np.array([radius * np.cos(th), radius * np.sin(th)]).T
+            center = np.array(raw_frames.shape[1:]).reshape(-1) / 2
+            vec_circ = v + center
+            p1_1 = center - radius * vec_1
+            p1_2 = center + radius * vec_1
+            p2_1 = center - radius * vec_2
+            p2_2 = center + radius * vec_2
+            for frame_num, raw_img in enumerate(raw_frames):
+                plt.figure(figsize=(10, 5))
+                plt.subplot(1, 2, 1)
+                plt.imshow(raw_img, cmap=plt.cm.gray)
+                plt.plot(
+                    [p1_1[frame_num][1], p1_2[frame_num][1]],
+                    [p1_1[frame_num][0], p1_2[frame_num][0]],
+                    "-",
+                    color=(255 / 255, 204 / 255, 203 / 255),
+                    linewidth=0.3,
+                )
+                plt.plot(
+                    [p2_1[frame_num][1], p2_2[frame_num][1]],
+                    [p2_1[frame_num][0], p2_2[frame_num][0]],
+                    "-",
+                    color=(0.5, 0.5, 0.5),
+                    linewidth=0.3,
+                )
+                # add in eigenvector directions
+                f = F_all[frame_num]
+                v_def = v.dot(np.linalg.matrix_power(f, 9))
+                vec_inner_circ = v_def + center
+
+                plt.plot(
+                    vec_circ[:, 1],
+                    vec_circ[:, 0],
+                    "-",
+                    color=(255 / 255, 204 / 255, 203 / 255),
+                    linewidth=0.3,
+                )
+                plt.plot(
+                    vec_inner_circ[:, 1],
+                    vec_inner_circ[:, 0],
+                    "-",
+                    color=(255 / 255, 204 / 255, 203 / 255),
+                    linewidth=1.0,
+                )
+
+                OOP_vec = OOP_vec_all[frame_num]
+                OOP_rad = radius * OOP_all[frame_num]
+                plt.plot(
+                    [
+                        center[1] - OOP_vec[1] * OOP_rad,
+                        center[1] + OOP_vec[1] * OOP_rad,
+                    ],
+                    [
+                        center[0] - OOP_vec[0] * OOP_rad,
+                        center[0] + OOP_vec[0] * OOP_rad,
+                    ],
+                    "r-",
+                    linewidth=5,
+                )
+
+                ax = plt.gca()
+                ax.set_xticks([])
+                ax.set_yticks([])
+
+                plt.subplot(1, 2, 2)
+                plt.plot(
+                    frames, lambda_1, "-", color="k", linewidth=1, label="λ1"
+                )
+                plt.plot(
+                    frames,
+                    lambda_2,
+                    "-",
+                    color="#7F7F7F",
+                    linewidth=1,
+                    label="λ2",
+                )
+                plt.plot(
+                    frame_num,
+                    lambda_1[frame_num],
+                    "o",
+                    mfc="#B30000",
+                    mec="k",
+                    markersize=7,
+                )
+                plt.plot(
+                    frame_num,
+                    lambda_2[frame_num],
+                    "o",
+                    mfc="#B30000",
+                    mec="#7F7F7F",
+                    markersize=7,
+                )
+                plt.xlabel("frame number")
+                plt.legend()
+                plt.tight_layout()
+                plt.savefig(
+                    f"tmp/frame-{frame_num}.png",
+                    dpi=self.sg_tools.quality,
+                    bbox_inches="tight",
+                )
+                plt.close()
+                img_list.append(imageio.imread(f"tmp/frame-{frame_num}.png"))
+            shutil.rmtree("tmp")
+
+            if num_frames > 1:
+                imageio.mimsave(
+                    f"{self.sg_tools.output_dir}/F_anim.gif", img_list
+                )
+
+        def timeseries_params(self):
+            """Visualize time series parameters."""
+            ts_params = self.sg_tools._load_ts_params()
+
+            plt.figure(figsize=(7, 7))
+
+            med = np.median(ts_params["mean_contraction_time"])
+            plt.subplot(2, 2, 1)
+            plt.hist(ts_params["mean_contraction_time"])
+            plt.plot([med, med], [0, 10], "r--")
+            plt.xlabel("frames")
+            plt.title(f"median_contract: {med:.2f}")
+            plt.tight_layout()
+
+            med = np.median(ts_params["mean_relax_time"])
+            plt.subplot(2, 2, 2)
+            plt.hist(ts_params["mean_relax_time"])
+            plt.plot([med, med], [0, 10], "r--")
+            plt.xlabel("frames")
+            plt.title(f"median_relax: {med:.2f}")
+            plt.tight_layout()
+
+            med = np.median(ts_params["mean_flat_time"])
+            plt.subplot(2, 2, 3)
+            plt.hist(ts_params["mean_flat_time"])
+            plt.plot([med, med], [0, 10], "r--")
+            plt.xlabel("frames")
+            plt.title(f"median_flat: {med:.2f}")
+            plt.tight_layout()
+
+            med = np.median(ts_params["mean_period_len"])
+            plt.subplot(2, 2, 4)
+            plt.hist(ts_params["mean_period_len"])
+            plt.plot([med, med], [0, 10], "r--")
+            plt.xlabel("frames")
+            plt.title(f"median_period: {med:.2f}")
+            plt.tight_layout()
+
+            out_file = f"{self.sg_tools.output_dir}/histogram_time_constants"
+            plt.savefig(
+                f"{out_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{out_file}.eps")
+
+            plt.show()
+
+        def dendrogram(self, dist_func: str = "dtw"):
+            """Cluster timeseries and plot a dendrogram that shows clusters.
+
+            Parameters
+            ----------
+            dist_func : str, optional, by default "dtw"
+                Choose between "euclidean" or "dtw"
+            """
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            num_frames = sarcomeres.frame.max() + 1
+            num_sarcs = sarcomeres.sarc_id.max() + 1
+            length = sarcomeres.length_norm.to_numpy().reshape(-1, num_frames)
+
+            if dist_func == "dtw":
+                dtw_dist = self.sg_tools.time_series._dtw_distance
+                dist_mat = np.zeros((num_sarcs, num_sarcs))
+                for sarc_1_id in range(num_sarcs):
+                    for sarc_2_id in range(sarc_1_id + 1, num_sarcs):
+                        dist = dtw_dist(
+                            length[sarc_1_id, :],
+                            length[sarc_2_id, :],
+                        )
+                        dist_mat[sarc_1_id, sarc_2_id] = dist
+                        dist_mat[sarc_2_id, sarc_1_id] = dist
+            if dist_func == "euclidean":
+                dist_mat = squareform(pdist(length, "euclidean"))
+
+            dist_v = squareform(dist_mat)
+            Z = linkage(dist_v, method="ward", metric="euclidean")
+
+            # --> plot dendrogram
+            plt.figure(figsize=(9, 30), frameon=False)
+            plt.subplot(1, 2, 1)
+            # dendrogram
+            dn1 = dendrogram(
+                Z,
+                orientation="left",
+                color_threshold=0,
+                above_threshold_color="k",
+            )
+            ordered = dn1["leaves"]  # from bottom to top
+
+            ax = plt.gca()
+            ax.xaxis.set_visible(False)
+            plt.subplot(1, 2, 2)
+            ax = plt.gca()
+
+            for kk in range(len(ordered)):
+                ix = ordered[kk]
+                col = (
+                    1 - kk / len(ordered),
+                    kk / len(ordered),
+                    1 - kk / len(ordered),
+                )
+                plt.plot(length[ix, :] + kk * 0.3, c=col)
+
+            plt.tight_layout()
+            plt.ylim((-0.4, kk * 0.3 + 0.35))
+            plt.axis("off")
+
+            output_file = f"{self.sg_tools.output_dir}/dendrogram_{dist_func}"
+            plt.savefig(f"{output_file}.pdf")
+
+            plt.show()
+
+        def spatial_graph(self):
+            """Visualizes the spatial graph
+
+            See Also
+            --------
+            :func:`sarcgraph.sg_tools.SarcGraphTools.Analysis.create_spatial_graph`
+            """
+            G = nx.read_gpickle(
+                f"{self.sg_tools.output_dir}/spatial-graph.pkl"
+            )
+
+            with open(
+                f"{self.sg_tools.output_dir}/spatial-graph-pos.pkl", "rb"
+            ) as file:
+                pos = pickle.load(file)
+
+            for node_1, node_2 in G.edges:
+                pos_1 = np.array(
+                    [G.nodes[node_1]["y_pos"], -G.nodes[node_1]["x_pos"]]
+                )
+                pos_2 = np.array(
+                    [G.nodes[node_2]["y_pos"], -G.nodes[node_2]["x_pos"]]
+                )
+                ang = 1 / np.sqrt(
+                    np.sum(((pos_1 - pos_2) / (pos_1[0] - pos_2[0])) ** 2)
+                )
+                G[node_1][node_2]["weight"] = ang
+
+            node_scores = []
+            for node in G.nodes:
+                edge_list = list(G.edges(node))
+                counter = 0
+                value = 0
+                for i in range(len(edge_list)):
+                    node_1 = edge_list[i][0]
+                    node_2 = edge_list[i][1]
+
+                    pos_1 = np.array(
+                        [G.nodes[node_1]["y_pos"], -G.nodes[node_1]["x_pos"]]
+                    )
+                    pos_2 = np.array(
+                        [G.nodes[node_2]["y_pos"], -G.nodes[node_2]["x_pos"]]
+                    )
+
+                    vec_1 = (pos_1 - pos_2) / np.linalg.norm(pos_1 - pos_2, 2)
+                    for j in range(i + 1, len(edge_list)):
+                        node_1 = edge_list[j][0]
+                        node_2 = edge_list[j][1]
+
+                        pos_1 = np.array(
+                            [
+                                G.nodes[node_1]["y_pos"],
+                                -G.nodes[node_1]["x_pos"],
+                            ]
+                        )
+                        pos_2 = np.array(
+                            [
+                                G.nodes[node_2]["y_pos"],
+                                -G.nodes[node_2]["x_pos"],
+                            ]
+                        )
+
+                        vec_2 = (pos_1 - pos_2) / np.linalg.norm(
+                            pos_1 - pos_2, 2
+                        )
+
+                        value += np.abs(np.dot(vec_1, vec_2))
+                        counter += 1
+
+                if counter:
+                    node_scores.append(value / counter)
+                else:
+                    node_scores.append(0)
+
+            plt.figure(figsize=(5, 5))
+            plt.axis("equal")
+            edges, weights = zip(*nx.get_edge_attributes(G, "weight").items())
+            nx.draw(
+                G,
+                pos,
+                node_color="k",
+                node_size=10,
+                width=2,
+                edge_color=weights,
+                edge_cmap=plt.cm.rainbow,
+            )
+
+            mi = np.min(node_scores)
+            ma = np.max(node_scores)
+            for node, node_score in zip(G.nodes, node_scores):
+                pos = np.array(
+                    [G.nodes[node]["y_pos"], -G.nodes[node]["x_pos"]]
+                )
+                color_val = 1 - (0.75 * (node_score - mi) / (ma - mi) + 0.25)
+                color = (color_val, color_val, color_val)
+                if node_score > 0.9:
+                    plt.plot(pos[0], pos[1], ".", color=color, ms=10)
+                if node_score > 0.75:
+                    plt.plot(pos[0], pos[1], ".", color=color, ms=7.5)
+                else:
+                    plt.plot(pos[0], pos[1], ".", color=color, ms=5)
+
+            output_file = f"./{self.sg_tools.output_dir}/spatial-graph"
+            plt.savefig(
+                f"./{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"./{output_file}.eps")
+
+            plt.show()
+
+        def tracked_vs_untracked(
+            self,
+            file_path: str,
+            start_frame: int = 0,
+            stop_frame: int = np.inf,
+        ):
+            """Visualize metrics to compare the effect of tracking sarcomeres
+            in a video vs only detecting sarcomeres in each frame without
+            tracking
+
+            Parameters
+            ----------
+            file_path: str
+                address to the original video file
+            start_frame : int, optional, by default 0
+            stop_frame : int, optional, by default np.inf
+            """
+            # process the whole video and detect and track sarcomeres
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            total_frames = sarcomeres.frame.max() + 1
+            stop_frame = min(stop_frame, total_frames)
+            start_frame = min(start_frame, stop_frame - 1)
+            num_frames = stop_frame - start_frame
+
+            sarcomeres = sarcomeres[
+                sarcomeres.frame.between(start_frame, stop_frame)
+            ]
+            num_tracked = sarcomeres.sarc_id.max() + 1
+
+            # process the video frame by frame - no tracking
+            sg_video = SarcGraph(self.sg_tools.input_dir)
+            segmented_zdiscs = sg_video.zdisc_segmentation(file_path)
+
+            length_all_frames = []
+            width_all_frames = []
+            angle_all_frames = []
+            median_length_all_frames = []
+            sarc_num_all_frames = []
+            sg_image = SarcGraph(self.sg_tools.input_dir, "image")
+            for frame in range(start_frame, stop_frame):
+                segmented_zdiscs_frame = segmented_zdiscs.loc[
+                    segmented_zdiscs.frame == frame
+                ].copy()
+                segmented_zdiscs_frame.loc[:, "frame"] = 0.0
+                tracked_zdiscs_frame = sg_image.zdisc_tracking(
+                    segmented_zdiscs=segmented_zdiscs_frame
+                )
+                sarcomeres_frame, _ = sg_image.sarcomere_detection(
+                    tracked_zdiscs=tracked_zdiscs_frame
+                )
+                length_all_frames.append(sarcomeres_frame.length.to_numpy())
+                width_all_frames.append(sarcomeres_frame.width.to_numpy())
+                angle_all_frames.append(sarcomeres_frame.angle.to_numpy())
+                median_length_all_frames.append(
+                    np.median(length_all_frames[-1])
+                )
+                sarc_num_all_frames.append(sarcomeres_frame.sarc_id.max() + 1)
+
+            # compute average number of not tracked sarcomeres in each frame
+            num_not_tracked = np.mean(sarc_num_all_frames)
+
+            len_diff_mean = []
+            sarcs_length_grouped = sarcomeres.groupby("frame").length
+            for untracked_len, tracked_len in zip(
+                length_all_frames, sarcs_length_grouped
+            ):
+                tracked_len = tracked_len[1].to_numpy()
+                tracked_len_mean = np.mean(tracked_len)
+                len_diff_mean.append(
+                    self.sg_tools.analysis._sampler(
+                        untracked_len,
+                        tracked_len_mean,
+                        num_tracked,
+                        num_run=1000,
+                    )
+                )
+
+            plt.figure(figsize=(np.clip(int(num_frames * 0.3), 10, 25), 5))
+            plt.boxplot(
+                len_diff_mean, positions=range(start_frame, stop_frame)
+            )
+            plt.plot([start_frame, stop_frame - 1], [-0.5, -0.5], "k--")
+            plt.plot([start_frame, stop_frame - 1], [0.5, 0.5], "k--")
+            plt.title(
+                f"Comparison of length in pixels, approx {num_not_tracked:.2f}"
+                f" untracked, {num_tracked} tracked"
+            )
+            plt.xlabel("frame number")
+            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
+            output_file = f"{self.sg_tools.output_dir}/length-comparison"
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps")
+
+            wid_diff_mean = []
+            sarcs_width_grouped = sarcomeres.groupby("frame").width
+            for untracked_wid, tracked_wid in zip(
+                width_all_frames, sarcs_width_grouped
+            ):
+                tracked_wid = tracked_wid[1].to_numpy()
+                tracked_wid_mean = np.mean(tracked_wid)
+                wid_diff_mean.append(
+                    self.sg_tools.analysis._sampler(
+                        untracked_wid,
+                        tracked_wid_mean,
+                        num_tracked,
+                        num_run=1000,
+                    )
+                )
+
+            plt.figure(figsize=(np.clip(int(num_frames * 0.3), 10, 25), 5))
+            plt.boxplot(
+                wid_diff_mean, positions=range(start_frame, stop_frame)
+            )
+            plt.plot([start_frame, stop_frame - 1], [-0.5, -0.5], "k--")
+            plt.plot([start_frame, stop_frame - 1], [0.5, 0.5], "k--")
+            plt.title(
+                f"Comparison of Width in pixels, approx {num_not_tracked:.2f} "
+                f"untracked, {num_tracked} tracked"
+            )
+            plt.xlabel("frame number")
+            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
+            output_file = f"{self.sg_tools.output_dir}/width-comparison"
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps")
+
+            ang_diff_mean = []
+            rad_diff_mean = []
+            sarcs_angle_grouped = sarcomeres.groupby("frame").angle
+            for untracked_ang, tracked_ang in zip(
+                angle_all_frames, sarcs_angle_grouped
+            ):
+                tracked_ang = tracked_ang[1].to_numpy()
+                out = self.sg_tools.analysis._angular_mean(tracked_ang)
+                tracked_ang_mean = out[0]
+                tracked_rad_mean = out[1]
+                ang_diff, rad_diff = self.sg_tools.analysis._angular_sampler(
+                    untracked_ang,
+                    tracked_ang_mean,
+                    tracked_rad_mean,
+                    num_tracked,
+                    num_run=1000,
+                )
+                ang_diff_mean.append(ang_diff)
+                rad_diff_mean.append(rad_diff)
+
+            plt.figure(figsize=(np.clip(int(num_frames * 0.3), 10, 25), 10))
+            plt.subplot(2, 1, 1)
+            plt.boxplot(
+                ang_diff_mean, positions=range(start_frame, stop_frame)
+            )
+            plt.plot(
+                [start_frame, stop_frame - 1], [-np.pi / 8, -np.pi / 8], "k--"
+            )
+            plt.plot(
+                [start_frame, stop_frame - 1], [np.pi / 8, np.pi / 8], "k--"
+            )
+            plt.title(
+                f"Comparison of angle in radians, approx {num_not_tracked:.2f}"
+                f" untracked, {num_tracked} tracked"
+            )
+            plt.xlabel("frame number")
+            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
+            plt.subplot(2, 1, 2)
+            plt.boxplot(
+                rad_diff_mean, positions=range(start_frame, stop_frame)
+            )
+            plt.plot(
+                [start_frame, stop_frame - 1], [0, 0], "r--", label="uniform"
+            )
+            plt.plot(
+                [start_frame, stop_frame - 1], [1, 1], "k--", label="oriented"
+            )
+            plt.title(
+                "Comparison of angle radius in pixels, approx "
+                f"{num_not_tracked:.2f} untracked, {num_tracked} tracked"
+            )
+            plt.xlabel("frame number")
+            plt.ylabel(r"$\mu_{track}-\mu_{all}$")
+            plt.legend()
+            output_file = f"{self.sg_tools.output_dir}/angle-comparison"
+            plt.savefig(
+                f"{output_file}.png",
+                dpi=self.sg_tools.quality,
+                bbox_inches="tight",
+            )
+            if self.sg_tools.include_eps:
+                plt.savefig(f"{output_file}.eps")
+
+            plt.show()
+
+    ##########################################################
+    #                     Analysis Class                     #
+    ##########################################################
+    class Analysis:
+        def __init__(self, sg_tools):
+            """Provides tools for post processing analysis of detected
+            sarcomeres.
+            """
+            self.sg_tools = sg_tools
+
+        def _sampler(
+            self,
+            signal: np.ndarray,
+            mu: float,
+            tracked_num: int,
+            num_run: int = 1000,
+        ) -> np.ndarray:
+            """Random sampler
+
+            Parameters
+            ----------
+            signal : np.ndarray
+            mu : float
+            tracked_num : int
+            num_run : int, optional
+            """
+            samples = np.zeros(num_run)
+            for run in range(num_run):
+                ids = np.random.randint(0, len(signal), size=(tracked_num))
+                samples[run] = mu - np.mean(signal[ids])
+            return samples
+
+        def _angular_mean(self, signal: np.ndarray) -> Tuple[float, float]:
+            """Angular signal averaging
+
+            Parameters
+            ----------
+            signal : np.ndarray
+
+            Returns
+            -------
+            Tuple[float, float]
+                angle and radius of averaged signal
+            """
+            x_mean = np.nanmean(np.cos(signal))
+            y_mean = np.nanmean(np.sin(signal))
+
+            mean_angle = np.arctan2(y_mean, x_mean)
+            mean_rad = np.linalg.norm([x_mean, y_mean], 2)
+
+            return mean_angle, mean_rad
+
+        def _angular_sampler(
+            self,
+            signal: np.ndarray,
+            mu_ang: float,
+            mu_rad: float,
+            tracked_num: int,
+            num_run: int = 1000,
+        ) -> Tuple[np.ndarray, np.ndarray]:
+            """Angular random sampler
+
+            Parameters
+            ----------
+            signal : np.ndarray
+            mu_ang : float
+            mu_rad : float
+            tracked_num : int
+            num_run : int, by default 1000, optional
+
+            Returns
+            -------
+            Tuple[np.ndarray, np.ndarray]
+            """
+            ang_samples = np.zeros(num_run)
+            rad_samples = np.zeros(num_run)
+            for run in range(num_run):
+                ids = np.random.randint(0, len(signal), size=(tracked_num))
+                ang_mean, rad_mean = self.sg_tools.analysis._angular_mean(
+                    signal[ids]
+                )
+                ang_samples[run] = mu_ang - ang_mean
+                rad_samples[run] = mu_rad - rad_mean
+
+            return ang_samples, rad_samples
+
+        def compute_F_J(
+            self, adjust_reference: bool = False
+        ) -> Tuple[np.ndarray, np.ndarray]:
+            """Compute the average deformation gradient (F) and its jacobian
+            (J) for the whole movie.
+
+            Parameters
+            ----------
+            adjust_reference : bool, by default False
+                The refrence frame by default is the first frame of the movie,
+                if this variable is set to ``True`` the function will run twice
+                and the refrence frame on the second run will be the most
+                contracted frame
+
+            Returns
+            -------
+            Tuple(np.ndarray, np.ndarray)
+                The average deformation gradient (F), shape=(num_frames, 2, 2)
+                The jacobian of F, shape=(num_frames)
+            """
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            sarcs_x = sarcomeres.x.to_numpy()
+            sarcs_y = sarcomeres.y.to_numpy()
+
+            # compute Lambda from x_pos and y_pos
+            num_frames = sarcomeres.frame.max() + 1
+            num_sarcs = sarcomeres.sarc_id.max() + 1
+            n = int(num_sarcs * (num_sarcs - 1) / 2)
+
+            Lambda_list = []
+            for frame_num in range(num_frames):
+                ids = sarcomeres.frame == frame_num
+                x_vec = sarcs_x[ids]
+                y_vec = sarcs_y[ids]
+
+                Lambda = np.zeros((2, n))
+                x_vec_tile = np.tile(x_vec, (num_sarcs, 1))
+                v_x = x_vec_tile.T - x_vec_tile
+                y_vec_tile = np.tile(y_vec, (num_sarcs, 1))
+                v_y = y_vec_tile.T - y_vec_tile
+
+                indices = np.triu_indices(num_sarcs, 1)
+                Lambda[0, :] = v_x[indices]
+                Lambda[1, :] = v_y[indices]
+
+                Lambda_list.append(Lambda)
+
+            F_all = np.zeros((num_frames, 2, 2))
+            J_all = np.zeros(num_frames)
+            num_iter = 2 if adjust_reference else 1
+            for iter in range(num_iter):
+                ref_frame = np.argmax(J_all)
+                for target_frame in range(num_frames):
+                    Lambda_i = Lambda_list[ref_frame]
+                    Lambda_t = Lambda_list[target_frame]
+                    term_1 = np.dot(Lambda_t, Lambda_i.T)
+                    term_2 = np.linalg.inv(np.dot(Lambda_i, Lambda_i.T))
+                    F = np.dot(term_1, term_2)
+                    F_all[target_frame] = F
+                    J_all[target_frame] = np.linalg.det(F)
+
+            if self.sg_tools.save_results:
+                np.save(f"{self.sg_tools.output_dir}/recovered_F.npy", F_all)
+                np.save(f"{self.sg_tools.output_dir}/recovered_J.npy", J_all)
+
+            return F_all, J_all
+
+        def compute_OOP(self) -> Tuple[np.ndarray, np.ndarray]:
+            """Computes Orientation Order Parameter (OOP) for the whole movie.
+
+            Returns
+            -------
+            Tuple[np.ndarray, np.ndarray]
+                OOP for all frames, shape=(num_frames)
+                OOP vector for all frames, shape=(num_frames, 2)
+            """
+
+            def f(data):
+                rxx = np.cos(data) ** 2
+                rxy = np.cos(data) * np.sin(data)
+                ryy = np.sin(data) ** 2
+                n = np.array([[rxx, rxy], [rxy, ryy]])
+                t = 2 * n - np.eye(2).reshape(2, 2, 1)
+                return np.mean(t, axis=2)
+
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+            num_frames = sarcomeres.frame.max() + 1
+
+            T = sarcomeres.groupby("frame")["angle"].apply(lambda x: f(x))
+            OOP_all = np.zeros(num_frames)
+            OOP_vec_all = np.zeros((num_frames, 2))
+            for frame in range(num_frames):
+                u, v = np.linalg.eig(T[frame])
+                OOP_all[frame] = np.max(u)
+                OOP_vec_all[frame, :] = v[:, np.argmax(u)]
+
+            if self.sg_tools.save_results:
+                np.save(
+                    f"{self.sg_tools.output_dir}/recovered_OOP.npy", OOP_all
+                )
+                np.save(
+                    f"{self.sg_tools.output_dir}/recovered_OOP_vector.npy",
+                    OOP_vec_all,
+                )
+
+            return OOP_all, OOP_vec_all
+
+        def compute_metrics(self, frame: int = None) -> dict:
+            """This function computes the following metrics as defind in the
+            paper: {OOP, C_iso, C_OOP, s_til, s_avg}.
+
+            Parameters
+            ----------
+            frame : int, optional
+                By default is set to the frame with maximum contraction
+
+            Notes
+            -----
+            See the paper for more information:
+            https://arxiv.org/abs/2102.02412
+
+            Returns
+            -------
+            dict
+            """
+
+            def f(data):
+                return (np.max(data) - np.min(data)) / (np.max(data) + 1)
+
+            F_all = self.sg_tools._load_recovered_info("F")
+            J_all = self.sg_tools._load_recovered_info("J")
+            OOP_all = self.sg_tools._load_recovered_info("OOP")
+            OOP_vec_all = self.sg_tools._load_recovered_info("OOP_vector")
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+
+            if frame is None:
+                frame = np.argmin(J_all)
+            OOP = OOP_all[frame]
+            OOP_vec = OOP_vec_all[frame]
+            F = F_all[frame]
+            J = J_all[frame]
+
+            v = OOP_vec
+            v_abs = np.linalg.norm(v, 2)
+            v0 = np.dot(np.linalg.inv(F), v)
+            v0_abs = np.linalg.norm(v0, 2)
+            avg_contract = 1 - np.sqrt(J)
+            avg_aligned_contract = (v0_abs - v_abs) / v0_abs
+
+            sarcs_groupby_sarc_id = sarcomeres.groupby("sarc_id").length_norm
+            sarcs_groupby_frame = sarcomeres.groupby("frame").length_norm
+
+            s_til = sarcs_groupby_sarc_id.apply(lambda x: f(x)).median()
+            s_avg = f(sarcs_groupby_frame.mean())
+
+            info_dict = {
+                "OOP": OOP,
+                "C_iso": avg_contract,
+                "C_OOP": avg_aligned_contract,
+                "s_til": s_til,
+                "s_avg": s_avg,
+            }
+
+            if self.sg_tools.save_results:
+                with open(
+                    f"{self.sg_tools.output_dir}/recovered_metrics.json", "w"
+                ) as file:
+                    json.dump(info_dict, file)
+
+            return info_dict
+
+        def compute_ts_params(self) -> pd.DataFrame:
+            """Compute and save timeseries time constants (contraction time,
+            relaxation time, flat time, period, offset, etc.).
+
+            Returns
+            -------
+            pd.DataFrame
+            """
+            sarcomeres = self.sg_tools._load_sarcomeres_gpr()
+            num_sarcs = sarcomeres.sarc_id.max() + 1
+            num_frames = sarcomeres.frame.max() + 1
+
+            sarcs_length = sarcomeres.groupby("sarc_id").length
+            sarcs_length_norm = sarcomeres.groupby("sarc_id").length_norm
+
+            signal_th = 0
+            signal_dist = 10
+            signal_width = 5
+
+            frames = np.arange(0, num_frames, 1)
+            sarc_ids = np.arange(0, num_sarcs, 1)
+            pix_length_median = np.zeros(num_sarcs)
+            pix_length_mean = np.zeros(num_sarcs)
+            pix_length_min = np.zeros(num_sarcs)
+            pix_length_max = np.zeros(num_sarcs)
+            pix_percent_shortening = np.zeros(num_sarcs)
+            mean_contraction_time = np.zeros(num_sarcs)
+            mean_relax_time = np.zeros(num_sarcs)
+            mean_flat_time = np.zeros(num_sarcs)
+            mean_period_len = np.zeros(num_sarcs)
+            frames_to_first_peak = np.zeros(num_sarcs)
+            peaks_count = np.zeros(num_sarcs)
+            for length, length_norm in zip(sarcs_length, sarcs_length_norm):
+                sarc_id = length[0]
+                sarc_length = length[1].to_numpy()
+                sarc_length_norm = length_norm[1].to_numpy()
+
+                sarc_length_med = signal.medfilt(sarc_length_norm, 5)
+                sarc_length_deriv = np.gradient(sarc_length_norm, frames)
+
+                thresh_flat = 0.025 * (
+                    np.max(sarc_length_med) - np.min(sarc_length_med)
+                )
+                count_R = np.sum(sarc_length_deriv > thresh_flat)
+                count_C = np.sum(sarc_length_deriv < -thresh_flat)
+                count_F = num_frames - count_R - count_C
+
+                # detect valleys
+                peaks_L, _ = signal.find_peaks(
+                    -sarc_length_med,
+                    threshold=signal_th,
+                    distance=signal_dist,
+                    width=signal_width,
+                )
+
+                num_peaks = np.sum(
+                    sarc_length_med[peaks_L]
+                    < np.mean(sarc_length_med) - thresh_flat
+                )
+                if num_peaks == 0:
+                    num_peaks = np.inf
+
+                mean_contraction_time[sarc_id] = count_C / num_peaks
+                mean_relax_time[sarc_id] = count_R / num_peaks
+                mean_flat_time[sarc_id] = count_F / num_peaks
+
+                min_sarc_length = np.min(sarc_length)
+                max_sarc_length = np.max(sarc_length)
+                pix_length_median[sarc_id] = np.median(sarc_length)
+                pix_length_mean[sarc_id] = np.mean(sarc_length)
+                pix_length_min[sarc_id] = min_sarc_length
+                pix_length_max[sarc_id] = max_sarc_length
+                pix_percent_shortening[sarc_id] = (
+                    100 * (max_sarc_length - min_sarc_length) / max_sarc_length
+                )
+
+                if peaks_L.size:
+                    frames_to_first_peak[sarc_id] = peaks_L[0]
+                else:
+                    frames_to_first_peak[sarc_id] = 0
+
+                mean_period_len[sarc_id] = num_frames / num_peaks
+                peaks_count[sarc_id] = num_peaks
+
+            # import data to a dataframe
+            data = np.vstack(
+                (
+                    sarc_ids,
+                    pix_length_median,
+                    pix_length_mean,
+                    pix_length_min,
+                    pix_length_max,
+                    pix_percent_shortening,
+                    mean_contraction_time,
+                    mean_relax_time,
+                    mean_flat_time,
+                    mean_period_len,
+                    frames_to_first_peak,
+                    peaks_count,
+                )
+            )
+
+            cols = [
+                "sarc_ids",
+                "pix_length_median",
+                "pix_length_mean",
+                "pix_length_min",
+                "pix_length_max",
+                "pix_percent_shortening",
+                "mean_contraction_time",
+                "mean_relax_time",
+                "mean_flat_time",
+                "mean_period_len",
+                "frames_to_first_peak",
+                "peaks_count",
+            ]
+
+            df = pd.DataFrame(data.T, columns=cols)
+
+            if self.sg_tools.save_results:
+                df.to_csv(
+                    f"./{self.sg_tools.output_dir}/timeseries_params.csv"
+                )
+
+            return df
+
+        def create_spatial_graph(
+            self,
+            file_path: str = None,
+            tracked_zdiscs: pd.DataFrame = None,
+        ):
+            """Generates and saves a spatial graph of tracked zdiscs where
+            edges indicate sarcomeres and edge weights indicates the ratio of
+            the frames in which that sarcomere is detected
+
+            Parameters
+            ----------
+            file_path : str
+                The address of an image or a video file to be loaded
+            tracked_zdiscs : pd.DataFrame
+                Information of all detected and tracked zdiscs in every frame.
+            """
+            sg_video = SarcGraph(file_type="video")
+
+            # load tracked zdiscs:
+            if tracked_zdiscs is None:
+                if file_path is None:
+                    raise ValueError(
+                        "either file_path or "
+                        + "tracked_zdiscs should be specified."
+                    )
+                tracked_zdiscs = sg_video.zdisc_tracking(
+                    file_path, save_output=False
+                )
+
+            # initiate the graph:
+            G = nx.Graph()
+
+            pos = {}
+            for particle in tracked_zdiscs.particle.unique():
+                x_pos = tracked_zdiscs[tracked_zdiscs.particle == particle][
+                    "x"
+                ].mean()
+                y_pos = tracked_zdiscs[tracked_zdiscs.particle == particle][
+                    "y"
+                ].mean()
+                G.add_node(particle, x_pos=x_pos, y_pos=y_pos)
+                pos.update({particle: (y_pos, -x_pos)})
+
+            # SarcGraph object that work with single frames
+            sg_image = SarcGraph(file_type="image")
+
+            # frame by frame sarcomere detection, add graph edges and weigts:
+            for frame in tracked_zdiscs.frame.unique():
+                tracked_zdiscs_frame = tracked_zdiscs[
+                    tracked_zdiscs.frame == frame
+                ]
+                tracked_zdiscs_frame.loc[:]["frame"] = 0
+                _, myofibrils = sg_image.sarcomere_detection(
+                    tracked_zdiscs=tracked_zdiscs_frame, save_output=False
+                )
+                for myo in myofibrils:
+                    for edge in myo.edges:
+                        disc_1 = myo.nodes[edge[0]]["particle_id"]
+                        disc_2 = myo.nodes[edge[1]]["particle_id"]
+                        if G.has_edge(disc_1, disc_2):
+                            G[disc_1][disc_2]["weight"] += 1
+                        else:
+                            G.add_edge(disc_1, disc_2, weight=1)
+
+            # graph pruning based on minimum weight threshold
+            num_frames = tracked_zdiscs.frame.max() + 1
+            weight_cutoff = np.floor(0.1 * num_frames)
+            edges, weights = zip(*nx.get_edge_attributes(G, "weight").items())
+            for edge in edges:
+                if G[edge[0]][edge[1]]["weight"] < weight_cutoff:
+                    G.remove_edge(edge[0], edge[1])
+
+            # isolated nodes removal
+            isolated_nodes = list(nx.isolates(G))
+            G.remove_nodes_from(isolated_nodes)
+
+            # save the graph
+            output_file = f"{self.sg_tools.output_dir}/spatial-graph"
+            nx.write_gpickle(G, path=f"{output_file}.pkl")
+            with open(f"{output_file}-pos.pkl", "wb") as file:
+                pickle.dump(pos, file)
+
+    ###########################################################
+    #                    Utility Functions                    #
+    ###########################################################
+    def _run_all(self, file_path: str = None):
+        """Runs all functions in the Analysis class and saves outputs.
+
+        Parameters
+        ----------
+        file_path : str
+            Path to the input video or image file.
+        """
+        self.analysis.compute_F_J()
+        self.analysis.compute_OOP()
+        self.analysis.compute_metrics()
+        self.analysis.compute_ts_params()
+        self.analysis.create_spatial_graph(file_path)
+
+    def _load_raw_frames(self):
+        try:
+            raw_frames = np.load(f"{self.input_dir}/raw-frames.npy")
+        except Exception:
+            self._raise_sarcgraph_data_not_found("raw-frames.npy")
+        return raw_frames
+
+    def _load_contours(self):
+        try:
+            contours = np.load(
+                f"{self.input_dir}/contours.npy",
+                allow_pickle=True,
+            )
+        except Exception:
+            self._raise_sarcgraph_data_not_found("contours.npy")
+        return contours
+
+    def _load_sarcomeres(self):
+        try:
+            sarcomeres = pd.read_csv(
+                f"{self.input_dir}/sarcomeres.csv", index_col=[0]
+            )
+        except Exception:
+            self._raise_sarcgraph_data_not_found("sarcomeres.csv")
+        return sarcomeres
+
+    def _load_sarcomeres_gpr(self):
+        try:
+            sarcomeres = pd.read_csv(
+                f"{self.input_dir}/sarcomeres_gpr.csv",
+                index_col=[0],
+            )
+        except Exception:
+            self._raise_data_not_found("sarcomeres_gpr.csv")
+        return sarcomeres
+
+    def _load_recovered_info(self, info_type: str):
+        try:
+            OOP = np.load(f"{self.input_dir}/recovered_{info_type}.npy")
+        except Exception:
+            self._raise_data_not_found(f"recovered_{info_type}.npy")
+        return OOP
+
+    def _load_ts_params(self):
+        try:
+            ts_params = pd.read_csv(
+                f"{self.input_dir}/timeseries_params.csv",
+                index_col=[0],
+            )
+        except FileNotFoundError:
+            self._raise_data_not_found("timeseries_params.csv")
+        return ts_params
+
+    def _raise_sarcgraph_data_not_found(self, data_file: str):
+        raise FileNotFoundError(
+            f"{data_file} was not found in {self.input_dir}/. Run "
+            "SarcGraph().sarcomeres_detection(save_output=True) first."
+        )
+
+    def _raise_data_not_found(self, data_file: str):
+        raise FileNotFoundError(
+            f"{data_file} was not found in {self.input_dir}/. Run "
+            "SarcGraphTools()._run_all() first."
+        )
```

### Comparing `sarcgraph-0.1.1/sarcgraph.egg-info/PKG-INFO` & `sarcgraph-0.2.1/sarcgraph.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,200 +1,229 @@
-Metadata-Version: 2.1
-Name: sarcgraph
-Version: 0.1.1
-Summary: A software for sarcomere detection and tracking
-Home-page: https://pypi.org/project/sarcgraph/
-Author: Saeed Mohammadzadeh
-Author-email: saeedmhz@bu.edu
-Maintainer: [('Saeed Mohammadzadeh', 'saeedmhz@bu.edu'), ('Emma Lejeune', 'elejeune@bu.edu')]
-License: MIT
-Project-URL: Source, https://github.com/Sarc-Graph/sarcgraph
-Project-URL: Documentation, https://sarc-graph.readthedocs.io/en/latest/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **SarcGraph**
-
-[![python](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/) ![os](https://img.shields.io/badge/os-ubuntu%20|%20macos%20|%20windows-blue.svg) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Sarc-Graph/sarcgraph#license)
-
-[![flake8](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml/badge.svg)](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml) [![codecov](https://codecov.io/gh/Sarc-Graph/sarcgraph/branch/main/graph/badge.svg?token=XNE85EJ4GX)](https://codecov.io/gh/Sarc-Graph/sarcgraph) [![Documentation Status](https://readthedocs.org/projects/sarc-graph/badge/?version=latest)](https://sarc-graph.readthedocs.io/en/latest/?badge=latest)
-
-## **Table of Contents**
-* [Project Summary](#summary)
-* [Installation Instructions](#install)
-* [Contents](#contents)
-* [Tutorial](#tutorial) - [Notebooks](https://github.com/Sarc-Graph/sarcgraph/tree/main/tutorials)
-* [Validation](#validation)
-* [References to Related Work](#references)
-* [Contact Information](#contact)
-* [Acknowledgements](#acknowledge)
-
-## **Project Summary** <a name="summary"></a>
-
-**SarcGraph** is a tool for automatic detection, tracking and analysis of
-z-discs and sarcomeres in movies of beating *human induced pluripotent stem
-cell-derived cardiomyocytes (hiPSC-CMs)*.
-
-<br />
-<center><img src="figures/intro.png" width=30%></center>
-<br />
-
-SarcGraph was initially introduced in [Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443).
-This package is created to make SarcGraph more accessible to the broader
-research community.
-
-**For more information visit [SarcGraph documentation](https://sarc-graph.readthedocs.io/en/latest/).**
-
-## **Installation Instructions** <a name="install"></a>
-
-### **Get a copy of the [SarcGraph repository](https://github.com/Sarc-Graph/sarcgraph) on your local machine**
-
-You can do this by clicking the green ``<> code`` button and selecting ``Download Zip`` or by running the following command in terminal:
-
-```bash
-git clone https://github.com/Sarc-Graph/sarcgraph.git
-```
-
-### **Create and activate a conda virtual environment**
-
-1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
-
-2. Open a terminal and move to the directory of the ``sarcgraph`` repository. Then, type the following command in terminal to create a virtual envirnoment and install the required packages:
-
-```bash
-cd sarcgraph
-conda env create --file=environment.yml
-```
-
-3. Activate your virtual environment.
-
-```bash
-conda activate sarcgraph
-```
-
-### **Install SarcGraph**
-
-SarcGraph can be installed using ``pip``:
-
-```bash
-pip install sarcgraph
-```
-
-## **Contents** <a name="contents"></a>
-
-```bash
-|___ sarcgraph
-|        |___ docs/
-|        |___ figures/
-|                |___ *.png
-|        |___ samples/
-|        |___ sarcgraph/
-|                |___ __init__.py
-|                |___ sg.py
-|                |___ sg_tools.py
-|        |___ tests/
-|        |___ tutorials/
-|                |___ *.ipynb
-```
-
-## **Tutorial** <a name="tutorial"></a>
-
-This GitHub repository contains a folder called ``tutorials`` that contains demos to extensively show how this package can be used to analyze videos or images of hiPSC-CMs.
-
-### **Package Contents** <a name="whats-in-package"></a>
-
-The package contains two seperate modules: `sg` for sarcomere detection and tracking and `sg_tools` for running further analysis and visualizations.
-
-#### **sarcgraph.sg** <a name="sarcgraph.py"></a>
-`sarcgraph.sg` module takes a video/image file as input (more details in tutorials). This module then processes the input file to detect and track z-discs and sarcomeres through running 3 tasks:
-
- - Z-disc Segmentation,
- - Z-disc Tracking,
- - Sarcomere Detection.
-
-Here is a list of functions developed for each task:
-
-- `zdisc_segmentation`: Detect z-discs in each frame of the input video/image and saves the following information into a pandas `DataFrame`:
-
-> - `frame`: (frame number) 
-> - `x` and `y`: (X and Y position of the center of a z-disc)
-> - `p1_x`, `p1_y` and `p2_x`, `p2_y`: (X and Y position of both ends of a z-disc)
-
-- `zdisc_tracking`: Tracks detected z-discs in the input video over all frames and adds the following information to the pandas `DataFrame`:
-
-> - `particle`: (z-disc id)
-> - `freq`: (number of frames in which a z-discs is tracked)
-frame,sarc_id,x,y,length,width,angle,z-discs
-
-- `sarcomere_detection`: Detects sarcomeres in the input video/image using tracked z-discs `DataFrame` and saves the following information into a new pandas `DataFrame`:
-
-> - `frame`: (frame number)
-> - `sarc_id`: (sarcomere id)
-> - `x` and `y`: (X and Y position of the center of a sarcomere)
-> - `length`: (sarcomere length)
-> - `width`: (sarcomere width)
-> - `angle`: (sarcomere angle)
-> - `zdiscs`: (ids of the two z-discs forming a sarcomere)
-
-
-#### **sarcgraph.sg_tools** <a name="sarcgraph_tools.py"></a>
-
-`sarcgraph.sg_tools` module consists of 3 subclasses:
-
-- `TimeSeries`: Process timeseries of detected and tracked sarcomeres
-
-> - `sarcomeres_gpr()`: Applies Gaussian Process Regression (GPR) on each recovered timeseries characteristic of all detected sarcomeres to reduce the noise and fill in the missing data
-
-- `Analysis`: Extract more information from detected sarcomeres characteristics timeseries
-
-> - `compute_F_J`: Computes the average deformation gradient (F) and its jacobian (J)
-> - `compute_OOP`: Computes the Orientation Order Parameter (OOP)
-> - `compute_metrics`: Computes {OOP, C_iso, C_OOP, s_til, s_avg} as defined in the [SarcGraph paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443)
-> - `compute_ts_params`: Computes timeseries constants (contraction time, relaxation time, flat time, period, offset)
-> - `create_spatial_graph`: Generates a spatial graph of tracked z-discs where edges indicate sarcomeres and edge weights indicate the ratio of the frames in which each sarcomere is detected
-
-- `Visualization`: Visualize detected sarcomeres information
-
-> - `zdiscs_and_sarcs`: Visualizes detected z-discs and sarcomeres in the chosen frame
-> - `contraction`:Visualizes detected sarcomeres in every frame as a gif file
-> - `normalized_sarcs_length`: Plots normalized length of all detected sarcomeres vs frame number
-> - `OOP`: Plots recovered Orientational Order Parameter
-> - `F`: Plots recovered deformation gradient
-> - `J`: Plots recovered deformation jacobian
-> - `F_eigenval_animation`: Visualizes the eigenvalues of F vs frame number
-> - `timeseries_params`: Visualizes time series parameters
-> - `dendrogram`: Clusters timeseries and plots as a dendrogram of the clusters
-> - `spatial_graph`: Visualizes the spatial graph
-> - `tracked_vs_untracked`: Visualizes metrics that compare the effect of tracking sarcomeres in a video vs only detecting sarcomeres in each frame without tracking
-
-To use this module an object of the class `SarcGraphTools` should be created by setting the `input_dir` to the folder that contains the output saved from running full sarcomere detection and timeseries processing on the input data.
-
-## Validation <a name="validation"></a>
-
-To validate our methods and ensure correct implementation, we generated challenging synthetic videos with characteristics similar to beating hiPSC-CMs. We used these videos to evaluate the sarcomere detection algorithm by comparing recovered metrics to their known ground truth. The figure shows this process for one of many tested validation examples.
-
-<br />
-<center><img src="figures/validation.png" width=75%></center>
-<br />
-
-## References to Related Work <a name="references"></a>
-
-* Zhao, B., Zhang, K., Chen, C. S., & Lejeune, E. (2021). Sarc-graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Computational Biology, 17(10), e1009443.
-
-* Allan, D. B., Caswell, T., Keim, N. C., Wel, C. M. van der, & Verweij, R. W. (2023). Soft-matter/trackpy: v0.6.1 (Version v0.6.1). Zenodo. https://doi.org/10.5281/zenodo.7670439
-
-* Toepfer, C. N., Sharma, A., Cicconet, M., Garfinkel, A. C., MÃ¼cke, M., Neyazi, M., Willcox, J. A., Agarwal, R., Schmid, M., Rao, J., & others. (2019). SarcTrack: An adaptable software tool for efficient large-scale analysis of sarcomere function in hiPSC-cardiomyocytes. Circulation Research, 124(8), 1172â€“1183.
-
-* Morris, T. A., Naik, 94 J., Fibben, K. S., Kong, X., Kiyono, T., Yokomori, K., & Grosberg, A. (2020). Striated myocyte structural integrity: Automated analysis of sarcomeric z-discs. PLoS Computational Biology, 16(3), e1007676.
-
-* Pasqualin, C., Gannier, F., Yu, A., MalÃ©cot, C. O., Bredeloux, P., & Maupoil, V. (2016). SarcOptiM for ImageJ: High-frequency online sarcomere length computing on stimulated cardiomyocytes. American Journal of Physiology-Cell Physiology, 311(2), C277â€“C283.
-
-* Ribeiro, A. J. S., Schwab, O., Mandegar, M. A., Ang, Y.-S., Conklin, B. R., Srivastava, D., & Pruitt, B. L. (2017). Multi-imaging method to assay the contractile mechanical output of micropatterned human iPSC-derived cardiac myocytes. Circulation Research, 120(10), 1572â€“1583. https://doi.org/10.1161/CIRCRESAHA.116.310363
-
-## Contact Information <a name="contact"></a>
-
-For information about this software, please get in touch with [Saeed Mohammadzadeh](mailto:saeedmhz@bu.edu) or [Emma Lejeune](mailto:elejeune@bu.edu).
-
-## Acknowledgements <a name="acknowledge"></a>
+Metadata-Version: 2.1
+Name: sarcgraph
+Version: 0.2.1
+Summary: A software for sarcomere detection and tracking
+Home-page: https://pypi.org/project/sarcgraph/
+Author: Saeed Mohammadzadeh
+Author-email: saeedmhz@bu.edu
+Maintainer: [('Saeed Mohammadzadeh', 'saeedmhz@bu.edu'), ('Emma Lejeune', 'elejeune@bu.edu')]
+License: MIT
+Project-URL: Source, https://github.com/Sarc-Graph/sarcgraph
+Project-URL: Documentation, https://sarc-graph.readthedocs.io/en/latest/
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **SarcGraph**
+
+[![python](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/) ![os](https://img.shields.io/badge/os-ubuntu%20|%20macos%20|%20windows-blue.svg) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Sarc-Graph/sarcgraph#license)
+
+[![flake8](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml/badge.svg)](https://github.com/Sarc-Graph/sarcgraph/actions/workflows/black_flake8.yml) [![codecov](https://codecov.io/gh/Sarc-Graph/sarcgraph/branch/main/graph/badge.svg?token=XNE85EJ4GX)](https://codecov.io/gh/Sarc-Graph/sarcgraph) [![Documentation Status](https://readthedocs.org/projects/sarc-graph/badge/?version=latest)](https://sarc-graph.readthedocs.io/en/latest/?badge=latest)
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Sarc-Graph/sarcgraph/main)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7963553.svg)](https://doi.org/10.5281/zenodo.7963553)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05322/status.svg)](https://doi.org/10.21105/joss.05322)
+
+## **Table of Contents**
+* [Project Summary](#summary)
+* [Installation Instructions](#install)
+* [Contents](#contents)
+* [Tutorial](#tutorial) - [Notebooks](https://github.com/Sarc-Graph/sarcgraph/tree/main/tutorials)
+* [Validation](#validation)
+* [References to Related Work](#references)
+* [Contact Information](#contact)
+* [Acknowledgements](#acknowledge)
+
+## **Project Summary** <a name="summary"></a>
+
+**SarcGraph** is a tool for automatic detection, tracking and analysis of
+z-discs and sarcomeres in movies of beating *human induced pluripotent stem
+cell-derived cardiomyocytes (hiPSC-CMs)*.
+
+<br />
+<center><img src="figures/intro.png" width=30%></center>
+<br />
+
+SarcGraph was initially introduced in [Sarc-Graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443).
+This package is created to make SarcGraph more accessible to the broader
+research community.
+
+**For more information visit [SarcGraph documentation](https://sarc-graph.readthedocs.io/en/latest/).**
+
+## **Installation Instructions** <a name="install"></a>
+
+### **Stable Version** <a name="install-stable"></a>
+
+#### From Conda
+
+Follow the instructions to install [Anaconda](https://www.anaconda.com/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
+
+Create a new Conda envirnoment and install sarcgraph.
+
+```bash
+conda create --name sarcgraph-env -c conda-forge -c saeedmhz sarcgraph
+```
+
+**Note:** Type ``y`` and press ``Enter`` when prompted.
+
+Activate the environment.
+
+```bash
+conda activate sarcgraph-env
+```
+#### From PyPI
+
+Please check the [Getting Started](https://sarc-graph.readthedocs.io/en/latest/installation.html) section in the documentation.
+
+### **Developer's Version** <a name="install-dev"></a>
+
+#### **Get a copy of the [SarcGraph repository](https://github.com/Sarc-Graph/sarcgraph) on your local machine**
+
+You can do this by clicking the green ``<> code`` button and selecting ``Download Zip`` or by running the following command in terminal and move to the directory of the ``sarcgraph`` repository.:
+
+```bash
+git clone https://github.com/Sarc-Graph/sarcgraph.git
+cd sarcgraph
+```
+
+#### **Create and activate a conda virtual environment**
+
+1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) on your local machine.
+
+2. Type the following command in terminal to create a virtual envirnoment and install the required packages:
+
+```bash
+conda env create --file=environment.yml
+```
+
+3. Activate your virtual environment.
+
+```bash
+conda activate sarcgraph
+```
+
+#### **Install SarcGraph**
+
+Install SarcGraph in editable mode:
+
+```bash
+pip install -e .
+```
+
+## **Contents** <a name="contents"></a>
+
+```bash
+|___ sarcgraph
+|        |___ docs/
+|        |___ figures/
+|                |___ *.png
+|        |___ samples/
+|        |___ sarcgraph/
+|                |___ __init__.py
+|                |___ sg.py
+|                |___ sg_tools.py
+|        |___ tests/
+|        |___ tutorials/
+|                |___ *.ipynb
+```
+
+## **Tutorial** <a name="tutorial"></a>
+
+This GitHub repository contains a folder called ``tutorials`` that contains demos to extensively show how this package can be used to analyze videos or images of hiPSC-CMs.
+
+### **Package Contents** <a name="whats-in-package"></a>
+
+The package contains two seperate modules: `sg` for sarcomere detection and tracking and `sg_tools` for running further analysis and visualizations.
+
+#### **sarcgraph.sg** <a name="sarcgraph.py"></a>
+`sarcgraph.sg` module takes a video/image file as input (more details in tutorials). This module then processes the input file to detect and track z-discs and sarcomeres through running 3 tasks:
+
+ - Z-disc Segmentation,
+ - Z-disc Tracking,
+ - Sarcomere Detection.
+
+Here is a list of functions developed for each task:
+
+- `zdisc_segmentation`: Detect z-discs in each frame of the input video/image and saves the following information into a pandas `DataFrame`:
+
+> - `frame`: (frame number) 
+> - `x` and `y`: (X and Y position of the center of a z-disc)
+> - `p1_x`, `p1_y` and `p2_x`, `p2_y`: (X and Y position of both ends of a z-disc)
+
+- `zdisc_tracking`: Tracks detected z-discs in the input video over all frames and adds the following information to the pandas `DataFrame`:
+
+> - `particle`: (z-disc id)
+> - `freq`: (number of frames in which a z-discs is tracked)
+frame,sarc_id,x,y,length,width,angle,z-discs
+
+- `sarcomere_detection`: Detects sarcomeres in the input video/image using tracked z-discs `DataFrame` and saves the following information into a new pandas `DataFrame`:
+
+> - `frame`: (frame number)
+> - `sarc_id`: (sarcomere id)
+> - `x` and `y`: (X and Y position of the center of a sarcomere)
+> - `length`: (sarcomere length)
+> - `width`: (sarcomere width)
+> - `angle`: (sarcomere angle)
+> - `zdiscs`: (ids of the two z-discs forming a sarcomere)
+
+
+#### **sarcgraph.sg_tools** <a name="sarcgraph_tools.py"></a>
+
+`sarcgraph.sg_tools` module consists of 3 subclasses:
+
+- `TimeSeries`: Process timeseries of detected and tracked sarcomeres
+
+> - `sarcomeres_gpr()`: Applies Gaussian Process Regression (GPR) on each recovered timeseries characteristic of all detected sarcomeres to reduce the noise and fill in the missing data
+
+- `Analysis`: Extract more information from detected sarcomeres characteristics timeseries
+
+> - `compute_F_J`: Computes the average deformation gradient (F) and its jacobian (J)
+> - `compute_OOP`: Computes the Orientation Order Parameter (OOP)
+> - `compute_metrics`: Computes {OOP, C_iso, C_OOP, s_til, s_avg} as defined in the [SarcGraph paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009443)
+> - `compute_ts_params`: Computes timeseries constants (contraction time, relaxation time, flat time, period, offset)
+> - `create_spatial_graph`: Generates a spatial graph of tracked z-discs where edges indicate sarcomeres and edge weights indicate the ratio of the frames in which each sarcomere is detected
+
+- `Visualization`: Visualize detected sarcomeres information
+
+> - `zdiscs_and_sarcs`: Visualizes detected z-discs and sarcomeres in the chosen frame
+> - `contraction`:Visualizes detected sarcomeres in every frame as a gif file
+> - `normalized_sarcs_length`: Plots normalized length of all detected sarcomeres vs frame number
+> - `OOP`: Plots recovered Orientational Order Parameter
+> - `F`: Plots recovered deformation gradient
+> - `J`: Plots recovered deformation jacobian
+> - `F_eigenval_animation`: Visualizes the eigenvalues of F vs frame number
+> - `timeseries_params`: Visualizes time series parameters
+> - `dendrogram`: Clusters timeseries and plots as a dendrogram of the clusters
+> - `spatial_graph`: Visualizes the spatial graph
+> - `tracked_vs_untracked`: Visualizes metrics that compare the effect of tracking sarcomeres in a video vs only detecting sarcomeres in each frame without tracking
+
+To use this module an object of the class `SarcGraphTools` should be created by setting the `input_dir` to the folder that contains the output saved from running full sarcomere detection and timeseries processing on the input data.
+
+## Validation <a name="validation"></a>
+
+To validate our methods and ensure correct implementation, we generated challenging synthetic videos with characteristics similar to beating hiPSC-CMs. We used these videos to evaluate the sarcomere detection algorithm by comparing recovered metrics to their known ground truth. The figure shows this process for one of many tested validation examples.
+
+<br />
+<center><img src="figures/validation.png" width=75%></center>
+<br />
+
+## References to Related Work <a name="references"></a>
+
+* Zhao, B., Zhang, K., Chen, C. S., & Lejeune, E. (2021). Sarc-graph: Automated segmentation, tracking, and analysis of sarcomeres in hiPSC-derived cardiomyocytes. PLoS Computational Biology, 17(10), e1009443.
+
+* Allan, D. B., Caswell, T., Keim, N. C., Wel, C. M. van der, & Verweij, R. W. (2023). Soft-matter/trackpy: v0.6.1 (Version v0.6.1). Zenodo. https://doi.org/10.5281/zenodo.7670439
+
+* Toepfer, C. N., Sharma, A., Cicconet, M., Garfinkel, A. C., Mücke, M., Neyazi, M., Willcox, J. A., Agarwal, R., Schmid, M., Rao, J., & others. (2019). SarcTrack: An adaptable software tool for efficient large-scale analysis of sarcomere function in hiPSC-cardiomyocytes. Circulation Research, 124(8), 1172–1183.
+
+* Morris, T. A., Naik, 94 J., Fibben, K. S., Kong, X., Kiyono, T., Yokomori, K., & Grosberg, A. (2020). Striated myocyte structural integrity: Automated analysis of sarcomeric z-discs. PLoS Computational Biology, 16(3), e1007676.
+
+* Pasqualin, C., Gannier, F., Yu, A., Malécot, C. O., Bredeloux, P., & Maupoil, V. (2016). SarcOptiM for ImageJ: High-frequency online sarcomere length computing on stimulated cardiomyocytes. American Journal of Physiology-Cell Physiology, 311(2), C277–C283.
+
+* Ribeiro, A. J. S., Schwab, O., Mandegar, M. A., Ang, Y.-S., Conklin, B. R., Srivastava, D., & Pruitt, B. L. (2017). Multi-imaging method to assay the contractile mechanical output of micropatterned human iPSC-derived cardiac myocytes. Circulation Research, 120(10), 1572–1583. https://doi.org/10.1161/CIRCRESAHA.116.310363
+
+## Contact Information <a name="contact"></a>
+
+For information about this software, please get in touch with [Saeed Mohammadzadeh](mailto:saeedmhz@bu.edu) or [Emma Lejeune](mailto:elejeune@bu.edu).
+
+## Acknowledgements <a name="acknowledge"></a>
```

