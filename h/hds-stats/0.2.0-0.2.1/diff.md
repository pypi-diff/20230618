# Comparing `tmp/hds-stats-0.2.0.tar.gz` & `tmp/hds-stats-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.2.0.tar", last modified: Sat Apr 15 14:53:25 2023, max compression
+gzip compressed data, was "hds-stats-0.2.1.tar", last modified: Sun Jun 18 15:52:49 2023, max compression
```

## Comparing `hds-stats-0.2.0.tar` & `hds-stats-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:53:25.182725 hds-stats-0.2.0/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.0/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-15 14:53:25.182486 hds-stats-0.2.0/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.0/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:53:25.180718 hds-stats-0.2.0/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.0/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11840 2023-04-15 14:49:49.000000 hds-stats-0.2.0/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27199 2023-04-15 14:49:49.000000 hds-stats-0.2.0/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:53:25.182141 hds-stats-0.2.0/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.0/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-15 14:53:25.182807 hds-stats-0.2.0/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-04-15 14:52:36.000000 hds-stats-0.2.0/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 15:52:49.941866 hds-stats-0.2.1/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.1/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 15:52:49.941619 hds-stats-0.2.1/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.1/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 15:52:49.939485 hds-stats-0.2.1/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.1/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-04-25 11:45:11.000000 hds-stats-0.2.1/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27158 2023-06-18 15:48:20.000000 hds-stats-0.2.1/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-06-18 15:52:49.941243 hds-stats-0.2.1/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-06-18 15:52:49.000000 hds-stats-0.2.1/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.1/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-06-18 15:52:49.941953 hds-stats-0.2.1/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-04-25 11:50:37.000000 hds-stats-0.2.1/setup.py
```

### Comparing `hds-stats-0.2.0/LICENSE` & `hds-stats-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.2.0/PKG-INFO` & `hds-stats-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.2.0/hds_stats/plot.py` & `hds-stats-0.2.1/hds_stats/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         y: 연속형 변수명을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -49,29 +49,30 @@
     
     plt.axhline(
         y = data[y].mean(), 
         color = 'red', 
         linestyle = '--'
     )
     
-    plt.title(label = f'{x} 범주별 {y}의 평균 비교');
+    plt.title(label = f'{x} 범주별 {y}의 평균 비교')
+    plt.show()
 
 
 # 두 연속형 변수로 산점도를 그리는 함수
 def scatter(data, x: str, y: str, color: str = '0.3') -> None:
     '''
     이 함수는 두 연속형 변수의 산점도를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 원인이 되는 연속형 변수명을 문자열로 지정합니다.
         y: 결과가 되는 연속형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.(기본값: '0.3')
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -79,30 +80,31 @@
     sns.scatterplot(
         data = data, 
         x = x, 
         y = y, 
         color = color
     )
     
-    plt.title(label = f'{x}와(과) {y}의 관계');
+    plt.title(label = f'{x}와(과) {y}의 관계')
+    plt.show()
 
 
 # 두 연속형 변수로 산점도와 회귀직선을 그리는 함수
 def regline(data, x: str, y: str, color: str = '0.3', size: int = 15) -> None:
     '''
     이 함수는 두 연속형 변수의 산점도에 회귀직선을 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 원인이 되는 연속형 변수명을 문자열로 지정합니다.
         y: 결과가 되는 연속형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.(기본값: '0.3')
         size: 점의 크기를 정수로 지정합니다.(기본값: 15)
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -120,33 +122,33 @@
         },
         line_kws = {
             'color': 'red', 
             'linewidth': 1.5
         }
     )
     
-    plt.title(label = f'{x}와(과) {y}의 관계')
-    
     # x_min = data[x].min()
     # x_max = data[x].max()
-    # plt.xlim(x_min * 0.9, x_max * 1.1);
+    # plt.xlim(x_min * 0.9, x_max * 1.1)
+    plt.title(label = f'{x}와(과) {y}의 관계')
+    plt.show()
 
 
 # 범주형 변수의 빈도수로 막대 그래프를 그리는 함수
 def bar_freq(data, x: str, color: str = None, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수의 빈도수를 내림차순 정렬한 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -169,30 +171,31 @@
             y = v + space, 
             s = v, 
             ha = 'center', 
             va = 'bottom', 
             c = 'black'
         )
     
+    plt.ylim(0, v_max * 1.2)
     plt.title(label = '목표변수의 범주별 빈도수 비교')
-    plt.ylim(0, v_max * 1.2);
+    plt.show()
 
 
 # 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그리는 함수
 def bar_dodge_freq(data, x: str, group: str, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -219,32 +222,33 @@
             x = i, 
             y = v + space, 
             s = v, 
             ha = 'center', 
             va = 'bottom'
         )
     
-    plt.title(label = f'{x}의 범주별 {group}의 빈도수 비교')
     plt.ylim(0, v_max * 1.2)
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
+    plt.title(label = f'{x}의 범주별 {group}의 빈도수 비교')
+    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5))
+    plt.show();
 
 
 # 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_freq(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         kind: 막대 그래프의 종류를 'bar' 또는 'barh'로 지정합니다.(기본값: 'bar')
         pal: 팔레트를 리스트로 지정합니다.
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -297,30 +301,31 @@
                     y = i, 
                     s = v2, 
                     ha = 'center', 
                     va = 'center', 
                     c = 'black'
                 )
 
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
+    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5))
+    plt.show()
 
 
 # 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_prop(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그립니다.
     
     매개변수:
         data: 데이터프레임을 지정합니다.
         x: 범주형 변수명을 문자열로 지정합니다.
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         kind: 막대 그래프의 종류를 'bar' 또는 'barh'로 지정합니다.(기본값: 'bar')
         pal: 팔레트를 리스트로 지정합니다.
     
-    반환:
+    반환값:
         그래프 외에 반환하는 객체는 없습니다.
     '''
     import numpy as np
     import pandas as pd
     from scipy import stats
     import seaborn as sns
     import matplotlib.pyplot as plt
@@ -378,11 +383,12 @@
                     y = i, 
                     s = v3, 
                     ha = 'center', 
                     va = 'center', 
                     c = 'black'
                 )
     
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
+    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5))
+    plt.show()
 
 
 ## End of Document
```

### Comparing `hds-stats-0.2.0/hds_stats/stat.py` & `hds-stats-0.2.1/hds_stats/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,36 +502,32 @@
         index = ['Statistic', 'P-Value', 'F-Value', 'F P-Value']
     ).T
     
     return result
 
 
 # 분산 팽창 지수
-def vif(X):
+def vif(model):
     '''
     이 함수는 입력변수 행렬의 분산 팽창 지수를 계산합니다.
     
     매개변수:
-         X: 입력변수 행렬을 pd.DataFrame으로 지정합니다.
+         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         입력변수 행렬의 열별 분산 팽창 지수를 반환합니다.
     '''
     import numpy as np
     import pandas as pd
     import statsmodels.stats.outliers_influence as oi
     
-    X2 = X.copy()
-    if 'const' not in X2.columns:
-        X2.insert(loc = 0, column = 'const', value = 1)
-    
     func = oi.variance_inflation_factor
-    ncol = X2.shape[1]
-    vifs = [func(exog = X2.values, exog_idx = i) for i in range(1, ncol)]
-    result = pd.DataFrame(data = vifs, index = X2.columns[1:]).T
+    ncol = len(model.model.exog_names)
+    vifs = [func(exog = model.model.exog, exog_idx = i) for i in range(1, ncol)]
+    result = pd.DataFrame(data = vifs, index = model.model.exog_names[1:]).T
     
     return result
 
 
 # 회귀모형의 회귀계수
 def coefs(model):
     '''
```

### Comparing `hds-stats-0.2.0/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.2.1/hds_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.2.0
+Version: 0.2.1
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.2.0/setup.py` & `hds-stats-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 from setuptools import setup
 from setuptools import find_packages
 
-with open(file = 'README.md', mode = 'r', encoding = 'utf-8') as file:
+with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.2.0',
+    version = '0.2.1',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

