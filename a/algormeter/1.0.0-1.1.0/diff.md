# Comparing `tmp/algormeter-1.0.0.tar.gz` & `tmp/algormeter-1.1.0.tar.gz`

## Comparing `algormeter-1.0.0.tar` & `algormeter-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
--rw-r--r--   0        0        0   717816 2020-02-02 00:00:00.000000 algormeter-1.0.0/ProblemsLib.pdf
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 algormeter-1.0.0/algorMeter.ipynb
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 algormeter-1.0.0/example1.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 algormeter-1.0.0/example2.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 algormeter-1.0.0/example3.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 algormeter-1.0.0/example4.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 algormeter-1.0.0/example5.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 algormeter-1.0.0/example6.py
--rwxr-xr-x   0        0        0     5152 2020-02-02 00:00:00.000000 algormeter-1.0.0/viewer.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algormeter-1.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algormeter-1.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algormeter-1.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algormeter-1.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/__init__.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/algormeter.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/perfprof.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/algorithms/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/algorithms/algorithms.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/kernel/__init__.py
--rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/kernel/kernel.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/libs/DCJBKMLib.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/libs/__init__.py
--rw-r--r--   0        0        0    26636 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/libs/data.py
--rw-r--r--   0        0        0    16569 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/libs/probLib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/tools/__init__.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/tools/counter.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 algormeter-1.0.0/algormeter/tools/dbx.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 algormeter-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 algormeter-1.0.0/tests/test_algoMeter.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 algormeter-1.0.0/tests/test_counter.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 algormeter-1.0.0/tests/test_kernel.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 algormeter-1.0.0/tests/test_minimize.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 algormeter-1.0.0/.gitignore
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 algormeter-1.0.0/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 algormeter-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12376 2020-02-02 00:00:00.000000 algormeter-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0   717816 2020-02-02 00:00:00.000000 algormeter-1.1.0/ProblemsLib.pdf
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 algormeter-1.1.0/algorMeter.ipynb
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 algormeter-1.1.0/example1.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 algormeter-1.1.0/example2.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 algormeter-1.1.0/example3.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 algormeter-1.1.0/example4.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 algormeter-1.1.0/example5.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 algormeter-1.1.0/example6.py
+-rwxr-xr-x   0        0        0     5114 2020-02-02 00:00:00.000000 algormeter-1.1.0/viewer.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/__init__.py
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/algormeter.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/perfprof.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/algorithms/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/algorithms/algorithms.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/kernel/__init__.py
+-rw-r--r--   0        0        0    12967 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/kernel/kernel.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/libs/DCJBKMLib.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/libs/__init__.py
+-rw-r--r--   0        0        0    26636 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/libs/data.py
+-rw-r--r--   0        0        0    16569 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/libs/probLib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/tools/__init__.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/tools/counter.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 algormeter-1.1.0/algormeter/tools/dbx.py
+-rw-r--r--   0        0        0   129937 2020-02-02 00:00:00.000000 algormeter-1.1.0/figs/dataframe.png
+-rw-r--r--   0        0        0    54851 2020-02-02 00:00:00.000000 algormeter-1.1.0/figs/perfprof.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 algormeter-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 algormeter-1.1.0/tests/test_algoMeter.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 algormeter-1.1.0/tests/test_counter.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 algormeter-1.1.0/tests/test_kernel.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 algormeter-1.1.0/tests/test_minimize.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 algormeter-1.1.0/.gitignore
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 algormeter-1.1.0/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 algormeter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12786 2020-02-02 00:00:00.000000 algormeter-1.1.0/PKG-INFO
```

### Comparing `algormeter-1.0.0/ProblemsLib.pdf` & `algormeter-1.1.0/ProblemsLib.pdf`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/algorMeter.ipynb` & `algormeter-1.1.0/algorMeter.ipynb`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/example2.py` & `algormeter-1.1.0/example2.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
         [Elizabeth D. Dolan · Jorge J. More ́ Benchmarking Optimization Software with Performance Profiles]]
 '''
 import pandas as pd
 import matplotlib.pyplot as plt
 from algormeter import *
 from algormeter.algorithms import *
 
-algorithms = [
+algorithms :Algorithms = [
                 harmonicGradient,
                 sqrtGradient,
                 logGradient,
                 polyak
         ]
```

### Comparing `algormeter-1.0.0/example3.py` & `algormeter-1.1.0/example3.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/example4.py` & `algormeter-1.1.0/example4.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # tuneParams: algorithm parameters tuning
 import pandas as pd
 
 from algormeter import *
 import algormeter.algorithms as alg
 
-Param.alpha = 1. # type: ignore
-Param.beta = 1. # type: ignore
+alpha = 1. 
+beta = 1. 
 
 def gradient(p, **kwargs):
     for k in p.loop():
-        p.Xkp1 = p.Xk - Param.alpha/(k+1) * p.gfXk / np.linalg.norm(p.gfXk) # type: ignore
+        p.Xkp1 = p.Xk - alpha/(k+1) * p.gfXk / np.linalg.norm(p.gfXk) # type: ignore
+    # print (alpha,beta)
 
-tpar = [ # [name, [values list]]
-    ('Param.alpha', [1. + i for i in np.arange(.05,.9,.05)]),
-    # ('Param.beta', [1., 2., 3.]),
+
+tpar : TuneParameters = [ # [name, [values list]]
+    ('alpha', [1. + i for i in np.arange(.05,.9,.05)]),
+    ('beta', [1., 2., 3.]),
 ]
 
-problems = [
+problems : Problems = [
             (Parab,[2,4,6]),
             (ParAbs,[2]),
             (Acad,[2]),
         ]
 
-algorithms = [
+algorithms : Algorithms = [
                 gradient,
         ]
 
 dff, pv = algorMeter(algorithms = algorithms, problems = problems, iterations = 3000,
                     tuneParameters=tpar, 
                      )
 
 print('\n', dff)
 print('\n', pv)
 
 
 
 df = dff[dff.Status == 'Success']
-# df = df[ df.Param.str.contains("alpha': 0.3") ]
+# df = df[ df.TuneParams.str.contains("alpha': 0.3") ]
 
-df = df.groupby(['Param','Status',]).agg({'Status':'count','f1':'sum'})
+df = df.groupby(['TuneParams','Status',]).agg({'Status':'count','f1':'sum'})
 df.rename(columns={'Status': 'count'}, inplace=True)
 df = df.sort_values(['count','f1'],ascending=[False, True])
 
 pd.options.display.max_rows = 2000
 pd.options.display.max_colwidth = 1000
 
 print(df)
```

### Comparing `algormeter-1.0.0/example5.py` & `algormeter-1.1.0/example5.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/example6.py` & `algormeter-1.1.0/example6.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/viewer.py` & `algormeter-1.1.0/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,18 @@
         data = np.load(filename)
         x = data[:,0]
         y = data[:,1]
     else:
         raise ValueError('File not found')
     return q,data,x,y
 
-def contour(funcname, rect = None):
+def contour(funcname):
     f, data, x, y = loadData(funcname)
 
-    if rect is None:
-        rect, mM = plotRect(f, data)
+    rect, mM = plotRect(f, data)
     xlist = np.linspace(rect[0][0], rect[1][0],levels)
     ylist = np.linspace(rect[0][1], rect[1][1],levels)
     X,Y = np.meshgrid(xlist, ylist)
     
     start  = abs(mM[0])
     ln = mM[1] - mM[0]
     levs = np.geomspace(.1,start+ln,levels) + mM[0]
```

### Comparing `algormeter-1.0.0/algormeter/algormeter.py` & `algormeter-1.1.0/algormeter/algormeter.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,75 +5,85 @@
 
 @author: Pietro D'Alessandro
 
 '''
 __all__ = ['algorMeter']
 __author__ = "Pietro d'Alessandro"
 
+import sys
+# from importlib import import_module
 import pandas as pd
 import numpy as np
 from typing import Optional, Callable
 import datetime
 import os
 import __main__
 from algormeter.tools import counter, dbx
-class Param:
-    ...
 
+from typing import Optional, Callable, Any, List, Tuple, Type, Dict, TypeVar
+from .kernel import Kernel, sign
 
-def algorMeter(algorithms : list[Callable], problems : list[tuple[Callable,list[int]]],  iterations : int = 500, timeout : int = 180, 
-    tuneParameters : Optional[list] = None,
-    runs : int = 1, trace : bool = False, dbprint : bool = False, 
+Problem = Type[Kernel]
+Problems = List[Tuple[Problem,List[int]]]
+Algorithm = Callable[[Problem], None]
+Algorithms = List[Algorithm]
+TuneParameters = Optional[List[Tuple[str,List[Any]]]]
+
+def algorMeter(algorithms : Algorithms, problems : Problems,  iterations : int = 500, timeout : int = 180, 
+    tuneParameters : TuneParameters = None,
+    runs : int = 1, 
+    trace : bool = False, dbprint : bool = False, 
     csv : bool = True, savedata : bool = False,
-    absTol : float =1.E-4, relTol : float = 1.E-5,  **kwargs) -> tuple[pd.DataFrame ,pd.DataFrame | np.ndarray] : 
-    '''Benchmark environment for Optimizer algorithms
+    absTol : float =1.E-4, relTol : float = 1.E-5,  **kwargs) -> Tuple[pd.DataFrame ,pd.DataFrame | np.ndarray] : 
+    '''Benchmark for Optimizer algorithms
         - algorithms: algorithms list. *(algoList_simple is available )* 
-        - problems: problem list. See problems list in example4.py for syntax.   *(probList_base, probList_covx, probList_DCJBKM are available)*
-        - tuneParameters = None: see tuneParameters section 
+        - problems: problems list.   *(probList_base, probList_covx, probList_DCJBKM are available)*
+        - tuneParameters = None: see README tuneParameters section 
         - iterations = 500: max iterations number 
         - timeout = 180: time out in seconds
-        - runs = 1: see random section 
-        - trace = False: see trace section 
-        - dbprint= False: see dbprint section 
+        - runs = 1: see README random section 
+        - trace = False: see README trace section 
+        - dbprint= False: see README dbprint section 
         - csv = True: write a report in csv format in csv folder
         - savedata = False: save data in data folder
         - absTol =1.E-4, relTol = 1.E-5: tolerance used in numpy allClose and isClose
         - **kwargs: python kwargs propagated to algorithms
     '''
 
     def algoRun (algorithm, experiment, exceptionOn = False, **kwargs ):
         def checkTunePar(ls):
             if not ls:
                 return
             for varName, l in ls:
-                if  'Param' not in varName:
-                    raise ValueError(f'{varName} invalid name. Must be Param.<someparam>')
+                if  type(varName) is not str:
+                    raise ValueError(f'{varName} invalid name. Must be str')
                 if   not len(l):
                     raise ValueError(f'{varName}: empty value list {l}')
 
-        def scanParams(list):
-            def paramStatus():
-                vs = {}
-                for k,e  in vars(Param).items():
-                    if not k.startswith('__'):
-                        vs[k] = e
-                return vs
+        params = {}
+        # algModule = import_module(algorithm.__module__)
+        algModule = sys.modules[algorithm.__module__]
 
+        def scanParams(list):
             if list:
                 varName, ls = list[0]
                 for v in ls:
                     try:
-                        exec(f'{varName}=round({v},5)')
+                        val=round(v,5)
+                        setattr(algModule,varName, val)
+                        params[varName] = val
                     except Exception as e: 
-                        raise ValueError(f'parameter {varName}:',e)
+                        raise ValueError(f'scanning {varName}:',e)
                     yield from scanParams(list[1:])
             else:
-                yield paramStatus()
+                yield params
         
         def prettyAlgo():
+            if algorithm.__module__ == algorithm.__name__:
+                return algorithm.__name__
             str = algorithm.__module__ + '.' + algorithm.__name__
             t = str.split('.')
             if len(t)>2:
                 str = t[-2] + '.' + t[-1]
             return str.replace('__main__.','')
 
         iter = 0
@@ -108,15 +118,15 @@
                     except (ArithmeticError, Exception) as e:
                         excp = e
                         counter.log (str(e), 'Error')
                         if (exceptionOn or dbprint or trace) and excp :
                             raise e
                     finally:
                         if tuneParameters:
-                            counter.log (str(varStat), 'Param')
+                            counter.log (str(varStat), 'TuneParams')
                         st = p.stats()
                         if excp: st['Status'] = 'Error'
                         stats.append(st)
                         iter = p.K
 
             usedtime = datetime.datetime.now() - ts  
             msg = ': ' + str(excp) if excp else ''
@@ -143,15 +153,16 @@
 
     if not dfl:
         print('Empty result')
         exit()
         
     df = pd.concat(dfl).sort_values(by=['Problem','Dim','Algorithm']) if len(dfl) > 1 else dfl[0]
     df = df.reset_index(drop=True)
-    df['Delta'] = pd.to_numeric(df['Delta'])
+    df = df.astype({'Dim':int, 'Delta':float}) 
+
 
     if csv:
         if hasattr(__main__, '__file__'):
             expName = __main__.__file__.split('/')[-1].split('.')[0]
         else:
             expName = 'jupyter'
         now  = datetime.datetime.now().strftime('%Y%m%d-%H%M%S')
```

### Comparing `algormeter-1.0.0/algormeter/perfprof.py` & `algormeter-1.1.0/algormeter/perfprof.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,17 +91,20 @@
         for solver, xy in solvers.items():
             ax[i].step(xy[0], xy[1], where='post', label=solver, alpha=.5)
         ax[i].set_xlabel('τ',fontsize=fontsize)
         ax[i].set_ylabel(r'$P(r_{p,s} \leq \tau: \, 1 \leq s \leq n_s)$',fontsize=fontsize)
         ax[i].set_xscale('log')
         ax[i].set_title(c,fontsize=fontsize)
         ax[i].legend(fontsize=fontsize)
-        fig.tight_layout()
+        ax[i].tick_params(axis='both', which='major', labelsize=fontsize)
+        ax[i].tick_params(axis='both', which='minor', labelsize=fontsize)
+
     for i in range(cl,nr*nc):
         ax[i].axis('off')
+    fig.tight_layout()
 
 
 if __name__ == '__main__':
 
     dfr = pd.read_pickle('perfprof.pickle')
     # dfr = pd.read_csv('aaa.csv')
```

### Comparing `algormeter-1.0.0/algormeter/algorithms/algorithms.py` & `algormeter-1.1.0/algormeter/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/algormeter/kernel/kernel.py` & `algormeter-1.1.0/algormeter/kernel/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,18 @@
         return r, flags # flags is None if x not exist in cache
 
 ## problem interface
     def __init__ (self, dimension : int , iterations : int =500, timeout : int = 180, trace : bool = False, savedata : bool = False,
                 csv :bool = False, relTol : float = 1.E-5, absTol : float = 1.E-8, **kwargs) :
         self.dimension = dimension 
         self.initCache(dimension)
+        self.isTimeout = False
         self.isRandomRun = False
+        self.startTime = tm.default_timer()
+
         self.__inizialize__(dimension)
         '''configure with default value'''
         self.trace = trace
         self.csv = csv
         self.timeout = timeout
         self.maxiterations = iterations
         self.relTol = relTol 
@@ -93,14 +96,15 @@
         self.Xk = self.XStart
 
         self.randomSet() # default random run param
         self.label = ''
         self.isf1_only = 'Kernel' in self._f2.__qualname__ and 'Kernel' in self._gf2.__qualname__
         self.K = -1
         self.Xk = self.XStart
+        self.XStar = np.empty(dimension)
         self.Xprev = self.Xk
         self.fXkPrev = math.inf
         if self.savedata is True:
             self.data = np.zeros([Kernel.SAVEDATABUFFERSIZE,self.dimension+1]) # +1 per fx
             self.X = self.data[:,:-1] 
             self.Y = self.data[:,-1] 
         self.clearCache()
@@ -128,15 +132,15 @@
 
         if self.savedata is True:
             self.data = np.zeros([Kernel.SAVEDATABUFFERSIZE,self.dimension+1]) # +1 per fx
             self.X = self.data[:,:-1] 
             self.Y = self.data[:,-1] 
     
     def isMinimum(self, x : np.ndarray) -> bool:
-        return bool(abs(self._f(x) - self.optimumValue) < self.absTol)
+        return math.isclose(self._f(x),self.optimumValue, rel_tol = self.relTol, abs_tol = self.absTol)
 
     def f (self, x : np.ndarray) -> np.ndarray :
         return self.f1(x) - self.f2(x)
     def gf (self, x : np.ndarray) -> np.ndarray :
         return self.gf1(x) - self.gf2(x)   
     def _f (self, x : np.ndarray) -> np.ndarray :
         return self._f1(x) - self._f2(x)
@@ -293,25 +297,25 @@
         counter.disable()
         stat = {"Problem" : str(self),
                 "Dim": self.dimension,
                 "Status":expStatus(),
                 "Iterations": int(self.K),
                 "f(XStar)": f'{float(self.f(self.XStar)):.7G}',
                 "f(BKXStar)":  f'{self.optimumValue:.7G}',
-                'Delta': f'{(abs(self.optimumValue-float(self.f(self.XStar)))):.2E}',
+                'Delta': f'{(abs(self.optimumValue-float(self.f(self.XStar)))):.1E}',
                 "Seconds" :f'{(tm.default_timer() - self.startTime):.4f}',
                 "XStar": self._pp(self.XStar),
                 "BKXStar":  self._pp(self.optimumPoint),
                 "Start point": self._pp(self.XStart),
             }
         stat.update(counter.report())
         counter.enable()
         return stat
 
-    def minimize(self,algorithm : Callable, iterations : int = 500, trace : bool = False, **kargs) -> tuple[bool, np.ndarray , np.ndarray]:
+    def minimize(self,algorithm : Callable, iterations : int = 500, trace : bool = False, dbprint: bool = False, **kargs) -> tuple[bool, np.ndarray , np.ndarray]:
         '''Find  minimum of a problem/function by applying an algorithm developed with algormeter.
             returns (Success, X, f(X))
         '''
         self.maxiterations = iterations
         self.trace = trace
         algorithm(self,**kargs)
         return self.isFound, self.Xk, self.fXk
```

### Comparing `algormeter-1.0.0/algormeter/libs/DCJBKMLib.py` & `algormeter-1.1.0/algormeter/libs/DCJBKMLib.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/algormeter/libs/data.py` & `algormeter-1.1.0/algormeter/libs/data.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/algormeter/libs/probLib.py` & `algormeter-1.1.0/algormeter/libs/probLib.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/algormeter/tools/counter.py` & `algormeter-1.1.0/algormeter/tools/counter.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/tests/test_counter.py` & `algormeter-1.1.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/tests/test_kernel.py` & `algormeter-1.1.0/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/tests/test_minimize.py` & `algormeter-1.1.0/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `algormeter-1.0.0/README.md` & `algormeter-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 AlgorMeter is a python implementation of an  environment for develop, test, measure, report and  compare optimization algorithms. 
 Having a common platform that simplifies developing, testing and exchange of optimization algorithms allows for better collaboration and sharing of resources among researchers in the field. This can lead to more efficient development and testing of new algorithms, as well as faster progress in the field overall.
 AlgorMeter produces comparative measures among algorithms  in csv format with effective test function call count.  
 It embeds a specific feature devoted to optimize the number of function calls, so that multiple function  calls at the same point are accounted for just once, without storing intermediate results, with benefit in terms of algorithm coding.  
 AlgorMeter contains a standard library of 10 DC problems and 7 convex problems for testing algorithms. More problem collections can be easily added.  
 AlgorMeter provide integrated performance profiles graphics, as developed by E. D. Dolan and J. J. More. They are a powerful standard tool, within the optimization community, to assess the performance of optimization software. 
 
+<img src="figs/perfprof.png" alt="Performance profiles" width="800px" height="391px"/>
+
 ## problems + algorithms = experiments
 
 - A problem is a function f where f: R(n) -> R with n called dimension.  
 - f = f1() - f2() difference of convex function where f1, f2: R(n) -> R. 
 - 'problems' is a list of problem
 - 'algorithm' is a code that try to find problem local minima
 - 'experiment' is an algorMeter run with a list of problems and a list of algorithms that produce a result report
@@ -50,15 +52,20 @@
 ...and run it:
 
 ```python
 df, pv = algorMeter(algorithms = [gradient], problems = probList_covx, iterations = 500, absTol=1E-2)
 print('\n', pv,'\n', df)
 ```
 
-pv and df are pandas dataframe with run result. A .csv file with result is also created in csv folder. 
+pv and df are pandas dataframe with run result. 
+
+<img src="figs/dataframe.png" alt="dataframe result" width="720px" height="230px"/>
+
+A .csv file with result is also created in csv folder. 
+
 
 *(see example\*.py)*
 
 ## AlgorMeter interface
 
 ```python
 def algorMeter(algorithms, problems, tuneParameters = None, iterations = 500, timeout = 180
@@ -119,15 +126,15 @@
         return status 
         ...
 
     p.stop = stop
     p.isSuccess = stop
 
 ```
-Another maybe simplet way is to call statement break in main loop.  
+Another maybe more simple way is to call statement break in main loop.  
 See example3.py
 ## Problems function call optimization
 
 AlgorMeter embeds a specific feature devoted to optimize the number of function calls, so that multiple function  calls at the same point are accounted for just once, without storing intermediate results, with benefit in terms of algorithm coding.  So in algorithm implementation is not necessary to store the previous result in variables to reduce f1, f2, gf1, gf2 function calls. AlgorMeter cache 128 previous calls to obtain such automatic optimization.  
 
 ## Problems ready to use
 
@@ -152,15 +159,15 @@
 is used to count events in code, summerized in statistics at the end of experiment as a column, available in dataframe returned by call to algorMeter and in final csv.
 For the code above a column with count of counter.up calls and head 'qp.lb>0' is produced.  
 Also are automatically available columns 'f1', 'f2', 'gf1', 'gf1' with effective calls to f1, f2, gf1, gf2  
 See example3.py
 
 ### dbprint = True
 
-Instruction dbx.print produce print out only if algorMeter call ha option dbprint == True
+Instruction dbx.print produce print out only if algorMeter call has option dbprint == True
 > dbx.print('t:',t, 'Xprev:',Xprev, 'f(Xprev):',p.f(Xprev) ).  
 
 See example3.py  
 NB: If dbprint = True python exceptions are not handled and raised.
 
 ### Trace == True
 
@@ -172,26 +179,26 @@
 These lines represent the path followed by the algorithm for the specific problem.  
 NB: If trace = True python exceptions are not handled and raised.  
 See example3.py
 
 ### tuneParameters
 Some time is necessary tune some parameter combinations.  Procede as follow (See example4.py):
 
-- Use numeric parameters with Param as domain name, like Param.alpha in your algo code.
+- Define and use module, non locals parameters in your algo code.
 - Define a list of lists with possible values of tuning parameters as follows:
 
 ```python
 tpar = [ # [name, [values list]]
-    ('Param.alpha', [1. + i for i in np.arange(.05,.9,.05)]),
-    # ('Param.beta', [1. + i for i in np.arange(.05,.9,.05)]),
+    ('alpha', [1. + i for i in np.arange(.05,.9,.05)]),
+    # ('beta', [1. + i for i in np.arange(.05,.9,.05)]),
 ]
 ```
 
 - call algorMeter with csv = True and tuneParameters=<list of parameters values> like tuneParameters=tpar.
-- open csv file produced and analyze the performance of parameters combinations by looking column '# tunePar'. Useful is a pivot table on such column.
+- open csv file produced and analyze the performance of parameters combinations by looking column '# TuneParams'. Useful is a pivot table on such columns.
 See example4.py
 ## Random start point 
 
 If algorMeter parameter run is set with a number greater than 1, each algorithm is repeated on the same problem with random start point in range -1 to 1 for all dimensions.
 By the method setRandom(center, size) random X can be set in [center-size, center+size] interval.  
 See example5.py
 
@@ -207,20 +214,28 @@
 
 ## Performance Profile
 Performance profiles graphics, as developed by E. D. Dolan and J. J. More, are a powerful tool to assess the performance of optimization software. For this reason they are standard accepted within the optimization community. See example2.py
 
 ```python
     df, pv = algorMeter(algorithms = algorithms, ...)
 
-    perfProf(df, cost= ['f1','Iterations'] ) 
+    perfProf(df, costs= ['f1','Iterations'] ) 
     # df: first pandas dataframe output of algormeter call
     # costs: list of column labels in df
 
     plt.show(block=True)
 ```
+It is possible to graph performance profiles by preparing a pandas data frame using a spreadsheet with the mandatory columns 'Problem','Dim','Algorithm','Status' and the columns costs that you want to draw
+```python
+    df = pd.read_excel(r'Path of Excel file\File name.xlsx', sheet_name='your Excel sheet name')
+
+    perfProf(df, costs= ['cost1','cost2'] ) 
+
+    plt.show(block=True)
+```
 ## Minimize
 
 In case you need to find the minimum of a problem/function by applying an algorithm developed with algormeter, the minimize method is available. (See example6.py):
 
 ```python
     p = MyProb(K) 
     found, x, y = p.minimize(myAlgo)
@@ -236,18 +251,14 @@
 - example2.py: Dolan, More performance profile
 - example3.py: dbx.print, trace,counter.up, counter.log, override stop, break  example
 - example4.py: algorithm parameters tuning 
 - example5.py: multiple run of each problem with random start point
 - example6.py: minimize new problem with algometer algorithm
 
 
-# Acknowledgment
-
-Algormeter was inspired and suggested by prof. Manlio Gaudioso of the University of Calabria and made with him.
-
 # Contributing
 
 You can download or fork the repository freely.  
 https://github.com/xedla/algormeter  
 If you see a mistake you can send me a mail at pietrodalessandro@gmail.com 
 If you open up a ticket, please make sure it describes the problem or feature request fully.  
 Any suggestion are welcome.
```

### Comparing `algormeter-1.0.0/pyproject.toml` & `algormeter-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "algormeter"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Pietro d Alessandro", email="pietrodalessandro@gmail.com" },
 ]
 description = "Tool for developing, testing and measuring optimizers algorithms"
 keywords = ["convex-optimization", "optimization-algorithms","difference-convex-function"]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `algormeter-1.0.0/PKG-INFO` & `algormeter-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algormeter
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tool for developing, testing and measuring optimizers algorithms
 Project-URL: Homepage, https://github.com/xedla/algormeter.git
 Project-URL: Bug Tracker, https://github.com/xedla/algormeter/issues
 Author-email: Pietro d Alessandro <pietrodalessandro@gmail.com>
 Keywords: convex-optimization,difference-convex-function,optimization-algorithms
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,16 @@
 AlgorMeter is a python implementation of an  environment for develop, test, measure, report and  compare optimization algorithms. 
 Having a common platform that simplifies developing, testing and exchange of optimization algorithms allows for better collaboration and sharing of resources among researchers in the field. This can lead to more efficient development and testing of new algorithms, as well as faster progress in the field overall.
 AlgorMeter produces comparative measures among algorithms  in csv format with effective test function call count.  
 It embeds a specific feature devoted to optimize the number of function calls, so that multiple function  calls at the same point are accounted for just once, without storing intermediate results, with benefit in terms of algorithm coding.  
 AlgorMeter contains a standard library of 10 DC problems and 7 convex problems for testing algorithms. More problem collections can be easily added.  
 AlgorMeter provide integrated performance profiles graphics, as developed by E. D. Dolan and J. J. More. They are a powerful standard tool, within the optimization community, to assess the performance of optimization software. 
 
+<img src="figs/perfprof.png" alt="Performance profiles" width="800px" height="391px"/>
+
 ## problems + algorithms = experiments
 
 - A problem is a function f where f: R(n) -> R with n called dimension.  
 - f = f1() - f2() difference of convex function where f1, f2: R(n) -> R. 
 - 'problems' is a list of problem
 - 'algorithm' is a code that try to find problem local minima
 - 'experiment' is an algorMeter run with a list of problems and a list of algorithms that produce a result report
@@ -68,15 +70,20 @@
 ...and run it:
 
 ```python
 df, pv = algorMeter(algorithms = [gradient], problems = probList_covx, iterations = 500, absTol=1E-2)
 print('\n', pv,'\n', df)
 ```
 
-pv and df are pandas dataframe with run result. A .csv file with result is also created in csv folder. 
+pv and df are pandas dataframe with run result. 
+
+<img src="figs/dataframe.png" alt="dataframe result" width="720px" height="230px"/>
+
+A .csv file with result is also created in csv folder. 
+
 
 *(see example\*.py)*
 
 ## AlgorMeter interface
 
 ```python
 def algorMeter(algorithms, problems, tuneParameters = None, iterations = 500, timeout = 180
@@ -137,15 +144,15 @@
         return status 
         ...
 
     p.stop = stop
     p.isSuccess = stop
 
 ```
-Another maybe simplet way is to call statement break in main loop.  
+Another maybe more simple way is to call statement break in main loop.  
 See example3.py
 ## Problems function call optimization
 
 AlgorMeter embeds a specific feature devoted to optimize the number of function calls, so that multiple function  calls at the same point are accounted for just once, without storing intermediate results, with benefit in terms of algorithm coding.  So in algorithm implementation is not necessary to store the previous result in variables to reduce f1, f2, gf1, gf2 function calls. AlgorMeter cache 128 previous calls to obtain such automatic optimization.  
 
 ## Problems ready to use
 
@@ -170,15 +177,15 @@
 is used to count events in code, summerized in statistics at the end of experiment as a column, available in dataframe returned by call to algorMeter and in final csv.
 For the code above a column with count of counter.up calls and head 'qp.lb>0' is produced.  
 Also are automatically available columns 'f1', 'f2', 'gf1', 'gf1' with effective calls to f1, f2, gf1, gf2  
 See example3.py
 
 ### dbprint = True
 
-Instruction dbx.print produce print out only if algorMeter call ha option dbprint == True
+Instruction dbx.print produce print out only if algorMeter call has option dbprint == True
 > dbx.print('t:',t, 'Xprev:',Xprev, 'f(Xprev):',p.f(Xprev) ).  
 
 See example3.py  
 NB: If dbprint = True python exceptions are not handled and raised.
 
 ### Trace == True
 
@@ -190,26 +197,26 @@
 These lines represent the path followed by the algorithm for the specific problem.  
 NB: If trace = True python exceptions are not handled and raised.  
 See example3.py
 
 ### tuneParameters
 Some time is necessary tune some parameter combinations.  Procede as follow (See example4.py):
 
-- Use numeric parameters with Param as domain name, like Param.alpha in your algo code.
+- Define and use module, non locals parameters in your algo code.
 - Define a list of lists with possible values of tuning parameters as follows:
 
 ```python
 tpar = [ # [name, [values list]]
-    ('Param.alpha', [1. + i for i in np.arange(.05,.9,.05)]),
-    # ('Param.beta', [1. + i for i in np.arange(.05,.9,.05)]),
+    ('alpha', [1. + i for i in np.arange(.05,.9,.05)]),
+    # ('beta', [1. + i for i in np.arange(.05,.9,.05)]),
 ]
 ```
 
 - call algorMeter with csv = True and tuneParameters=<list of parameters values> like tuneParameters=tpar.
-- open csv file produced and analyze the performance of parameters combinations by looking column '# tunePar'. Useful is a pivot table on such column.
+- open csv file produced and analyze the performance of parameters combinations by looking column '# TuneParams'. Useful is a pivot table on such columns.
 See example4.py
 ## Random start point 
 
 If algorMeter parameter run is set with a number greater than 1, each algorithm is repeated on the same problem with random start point in range -1 to 1 for all dimensions.
 By the method setRandom(center, size) random X can be set in [center-size, center+size] interval.  
 See example5.py
 
@@ -225,20 +232,28 @@
 
 ## Performance Profile
 Performance profiles graphics, as developed by E. D. Dolan and J. J. More, are a powerful tool to assess the performance of optimization software. For this reason they are standard accepted within the optimization community. See example2.py
 
 ```python
     df, pv = algorMeter(algorithms = algorithms, ...)
 
-    perfProf(df, cost= ['f1','Iterations'] ) 
+    perfProf(df, costs= ['f1','Iterations'] ) 
     # df: first pandas dataframe output of algormeter call
     # costs: list of column labels in df
 
     plt.show(block=True)
 ```
+It is possible to graph performance profiles by preparing a pandas data frame using a spreadsheet with the mandatory columns 'Problem','Dim','Algorithm','Status' and the columns costs that you want to draw
+```python
+    df = pd.read_excel(r'Path of Excel file\File name.xlsx', sheet_name='your Excel sheet name')
+
+    perfProf(df, costs= ['cost1','cost2'] ) 
+
+    plt.show(block=True)
+```
 ## Minimize
 
 In case you need to find the minimum of a problem/function by applying an algorithm developed with algormeter, the minimize method is available. (See example6.py):
 
 ```python
     p = MyProb(K) 
     found, x, y = p.minimize(myAlgo)
@@ -254,18 +269,14 @@
 - example2.py: Dolan, More performance profile
 - example3.py: dbx.print, trace,counter.up, counter.log, override stop, break  example
 - example4.py: algorithm parameters tuning 
 - example5.py: multiple run of each problem with random start point
 - example6.py: minimize new problem with algometer algorithm
 
 
-# Acknowledgment
-
-Algormeter was inspired and suggested by prof. Manlio Gaudioso of the University of Calabria and made with him.
-
 # Contributing
 
 You can download or fork the repository freely.  
 https://github.com/xedla/algormeter  
 If you see a mistake you can send me a mail at pietrodalessandro@gmail.com 
 If you open up a ticket, please make sure it describes the problem or feature request fully.  
 Any suggestion are welcome.
```

