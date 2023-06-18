# Comparing `tmp/lifeactuary-1.2.1.tar.gz` & `tmp/lifeactuary-1.3.tar.gz`

## Comparing `lifeactuary-1.2.1.tar` & `lifeactuary-1.3.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/about.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/pyproject_ver_0.1.8.toml.txt
--rw-r--r--   0        0        0   610030 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/info/lifeActuary_v1_2.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/__init__.py
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/annuities.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/annuities_certain.py
--rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/commutation_table.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/commutation_table_frac.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/mortality_table.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/lifeActuary/read_soa_table_xml.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/197982PortugalFemale.xml
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/197982PortugalMale.xml
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/AF80.xml
--rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/AM80.xml
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/CSO_1941.xml
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/GRF95.xml
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/GRM80.xml
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/GRM95.xml
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/IA8590F.xml
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/IA8590M.xml
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/PFL80.xml
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/PML80.xml
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/SIF91.xml
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/SIM91.xml
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/TV7377.xml
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/TV8890.xml
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/WL80.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/__init__.py
--rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/soa_tables/tables_manual.xlsx
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/LICENSE
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/README.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 lifeactuary-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 lifeactuary-1.3/about.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lifeactuary-1.3/desktop.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/__init__.py
+-rw-r--r--   0        0        0    15749 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/annuities.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/annuities_certain.py
+-rw-r--r--   0        0        0    31661 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/commutation_table.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/commutation_table_frac.py
+-rw-r--r--   0        0        0    35439 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/life_2heads.py
+-rw-r--r--   0        0        0    26647 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/mortality_insurance.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/mortality_table.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 lifeactuary-1.3/lifeActuary/mortality_table_2heads.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/197982PortugalFemale.xml
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/197982PortugalMale.xml
+-rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/AF80.xml
+-rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/AM80.xml
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/CSO_1941.xml
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/GRF95.xml
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/GRM80.xml
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/GRM95.xml
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/IA8590F.xml
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/IA8590M.xml
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/PFL80.xml
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/PML80.xml
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/SIF91.xml
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/SIM91.xml
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/TV7377.xml
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/TV8890.xml
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/WL80.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/read_soa_table_xml.py
+-rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 lifeactuary-1.3/soa_tables/tables_manual.xlsx
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 lifeactuary-1.3/LICENSE
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 lifeactuary-1.3/README.md
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 lifeactuary-1.3/pyproject.toml
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 lifeactuary-1.3/PKG-INFO
```

### Comparing `lifeactuary-1.2.1/pyproject_ver_0.1.8.toml.txt` & `lifeactuary-1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifeactuary"
-version = "1.2"
+version = "1.3"
 authors = [
   { name="Pedro Corte Real", email="parcr@fct.unl.pt" },
 { name="Gracinda R. Guerreiro", email="grg@fct.unl.pt" },
 ]
 
 maintainers=[
   { name="Pedro Corte Real", email="parcr@fct.unl.pt" },
@@ -22,9 +22,9 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/parcr/lifeactuary_1.2"
-"Bug Tracker" = "https://github.com/parcr/lifeactuary_1.2/issues"
+"Homepage" = "https://github.com/parcr/lifeactuary_1.3"
+"Bug Tracker" = "https://github.com/parcr/lifeactuary_1.3/issues"
```

### Comparing `lifeactuary-1.2.1/lifeActuary/annuities_certain.py` & `lifeactuary-1.3/lifeActuary/annuities_certain.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
     def __new__(cls, interest_rate, m):
         if interest_rate < 0 or m < 0 or int(m) != m:
             print(f"We need a rate of interest non negative and a positive integer frequency")
             return None
         return object.__new__(cls)
 
     def __init__(self, interest_rate, m=1):
-        '''
+        """
         This class instantiates the methods for the computation of financial annuities, for a given
         interest rate and a chosen frequency of payments m (in each period of the interest rate)
 
         :param interest_rate: interest rate, in percentage (e.g. use 5 for 5%)
         :param m: frequency of payments, in each period of the interest rate
 
         :return: several methods and annuities for the interest rate and frequency.
-        '''
+        """
         self.interest_rate = interest_rate / 100.
         self.frequency = m
 
         self.v = 1 / (1 + self.interest_rate)
         self.im = self.frequency * (np.power(1 + self.interest_rate, 1 / self.frequency) - 1)
         self.vm = np.power((1 + self.im / self.frequency), -1)
         self.dm = self.im * self.vm
@@ -47,182 +47,182 @@
 
         return func_wrapper
 
     # Constant Term Financial Annuities
 
     @check_terms
     def an(self, terms):
-        '''
+        """
         Returns the present value of an immediate n-term financial annuity with payments equal to 1.
         Payments are made in the end of the periods. In fractional annuities, payments of 1/m are made
         m times per year at the end of the periods.
 
         :param terms: number of years
 
         :return: Expected Present Value (EPV) of an immediate n-term financial annuity
-        '''
+        """
         if not terms:
             return 1 / self.im
         return (1 - np.power(self.vm, terms * self.frequency)) / self.im
 
     @check_terms
     def aan(self, terms):
-        '''
+        """
         Returns the present value of a due n-term financial annuity with payments equal to 1.
         Payments are made in the end of the periods. In fractional annuities, payments of 1/m are made
         m times per year at the end of the periods.
 
         :param terms: number of years
 
         :return: Expected Present Value (EPV) of a due n-term financial annuity
-        '''
+        """
         if not terms:
             return 1 / self.dm
         return (1 - np.power(self.vm, terms * self.frequency)) / self.dm
 
     # Variable Terms Financial Annuities
     @check_terms
     def Ian(self, terms, payment=1, increase=1):
-        '''
+        """
         Returns the present value of an immediate $n$ term financial annuity with payments
         increasing/decreasing arithmetically. Payments are made in the end of the periods.
         First payment and increase amount may differ.
         In fractional annuities, payments level within each interest period and increase/decrease from one
         interest period to the next.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param increase: increase amount of payments (positive for increasing annuities and negative for decreasing annuities)
 
         :return: Expected Present Value (EPV) of an immediate arithmetically increasing/decreasing financial annuity. Payments level within each interest period and increase/decrease from one interest period to the next.
-        '''
+        """
         if payment + increase * terms < 0:
             return np.nan
         # (payment - increase) * self.an(terms) + increase * (self.aan(terms) - terms * self.v ** terms) / self.im
         return payment * self.an(terms) + increase / self.im * (
                     (1 - self.v ** terms) / self.interest_rate - terms * self.v ** terms)
 
     @check_terms
     def Iaan(self, terms, payment=1, increase=1):
-        '''
+        """
         Returns the present value of a due $n$ term financial annuity with payments increasing/decreasing arithmetically. Payments are made in the beginning of the periods.
         First payment and increase amount may differ.
         In fractional annuities, payments level within each interest period and increase/decrease from one
         interest period to the next.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param increase: increase amount of payments (positive for increasing annuities and negative for decreasing annuities)
 
         :return: Expected Present Value (EPV) of a due arithmetically increasing/decreasing financial annuity. Payments level within each interest period and increase/decrease from one interest period to the next
-        '''
+        """
         return self.Ian(terms, payment, increase) / self.vm
 
     @check_terms
     def Iman(self, terms, payment=1, increase=1):
-        '''
+        """
         Returns the present value of an immediate $n$-term financial annuity with payments
         increasing/decreasing arithmetically.
         Payments are made in the end of the periods.
         First payment and increase amount may differ.
         In fractional annuities, payments increase in each payment period.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param increase: increase amount of payments (positive for increasing annuities and negative for decreasing annuities)
 
         :return: Expected Present Value (EPV) of an arithmetically increasing/decreasing financial annuity.
         Payments increase in each payment period and are paid in the end of periods.
-        '''
+        """
         if payment + increase * terms < 0:
             return np.nan
 
         return (payment - increase) * self.an(terms) \
                + increase * self.v \
                * (self.v ** terms * ((terms * self.frequency) * (self.vm - 1) - 1) + 1) \
                / (self.frequency * self.v ** ((self.frequency - 1) / self.frequency) * (self.vm - 1) ** 2)
 
     @check_terms
     def Imaan(self, terms, payment=1, increase=1):
-        '''
+        """
         Returns the present value of an immediate $n$-term financial annuity with payments
         increasing/decreasing arithmetically.
         Payments are made in the beginning of the periods.
         First payment and increase amount may differ.
         In fractional annuities, payments increase in each payment period.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param increase: increase amount of payments (positive for increasing annuities and negative for decreasing annuities)
 
         :return: Expected Present Value (EPV) of an arithmetically increasing/decreasing financial annuity.
         Payments increase in each payment period and are paid in the beginning of periods.
-        '''
+        """
 
         return self.Iman(terms, payment, increase) / self.vm
 
     @check_grow
     def Gan(self, terms, payment=1, grow=0):
-        '''
+        """
         Returns the present value of an immediate $n$ term financial annuity with payments increasing/decreasing geometrically. Payments are made in the end of the periods. In fractional annuities, payments level within each interest period and increase/decrease from one interest period to the next.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param grow: growth rate from one year to the other
 
         :return: Expected Present Value (EPV) of an arithmetically increasing/decreasing financial annuity. Payments increase in each year.
-        '''
+        """
 
         v = (1 + grow / 100) * self.v
         if self.interest_rate == grow / 100:
             return payment * terms * self.frequency * self.vm / self.frequency
         return payment / (1 + grow / 100) ** (1 / self.frequency) * (1 - v ** terms) / \
                (1 - v ** (1 / self.frequency)) * v ** (1 / self.frequency) / self.frequency
 
     @check_grow
     def Gaan(self, terms, payment=1, grow=0):
-        '''
+        """
         Returns the present value of a due $n$ term financial annuity with payments increasing/decreasing geometrically. Payments are made in the beginning of the periods. In fractional annuities, payments level within each interest period and increase/decrease from one interest period to the next.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param grow: growth rate from one year to the other
 
         :return: Present Value of an arithmetically increasing/decreasing financial annuity. Payments increase in each year.
-        '''
+        """
         v = (1 + grow / 100) * self.v
         return self.Gan(terms, payment, grow) / v ** (1 / self.frequency)
 
     @check_grow
     def Gman(self, terms, payment=1, grow=0):
-        '''
+        """
         Returns the present value of an immediate $n$ term financial annuity with payments increasing/decreasing geometrically. Payments are made in the end of the periods. In fractional annuities, payments increase in each payment period.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param grow: rate of growing of payments, in percentage
 
         :return: Present Value of an arithmetically increasing/decreasing financial annuity with terms paid in the end of periods.
         Payments increase in each payment period.
-        '''
+        """
         a1 = (1 - self.v) / self.im
         if self.interest_rate == grow / 100:
             return a1 * terms
         ig = (self.interest_rate - grow / 100) / (1 + grow / 100)
         vg = 1 / (1 + ig)
         a2 = (1 - vg ** terms) / (1 - vg)
         return payment * a1 * a2
 
     @check_grow
     def Gmaan(self, terms, payment=1, grow=0):
-        '''
+        """
         Returns the present value of an immediate $n$ term financial annuity with payments increasing/decreasing geometrically. Payments are made in the beginning of the periods. In fractional annuities, payments increase in each payment period.
 
         :param terms: number of years
         :param payment: amount of the first payment
         :param grow: rate of growing of payments, in percentage
 
         :return: Present Value of an arithmetically increasing/decreasing financial annuity with terms paid in the beginning of periods.
         Payments increase in each payment period.
-        '''
+        """
         v = (1 + grow / 100) * self.v
         return self.Gman(terms, payment, grow) / v ** (1 / self.frequency)
```

### Comparing `lifeactuary-1.2.1/lifeActuary/commutation_table.py` & `lifeactuary-1.3/lifeActuary/commutation_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
     def __repr__(self):
         return f"{self.__class__.__name__}{self.i, self.g, self.data_type, self.mt, self.perc, self.app_cont}"
 
     # getters and setters
     @property
     def i(self):
-        return self.__i*100
+        return self.__i * 100
 
     @property
     def g(self):
-        return self.__g*100
+        return self.__g * 100
 
     @property
     def v(self):
         return self.__v
 
     @property
     def d(self):
@@ -93,15 +93,14 @@
     def Mx(self):
         return self.__Mx
 
     @property
     def Rx(self):
         return self.__Rx
 
-
     def df_commutation_table(self):
         data = {'Dx': self.__Dx, 'Nx': self.__Nx, 'Sx': self.__Sx, 'Cx': self.__Cx, 'Mx': self.__Mx, 'Rx': self.__Rx}
         df = pd.DataFrame(data)
         data_lf = self.df_life_table()
         df = pd.concat([data_lf, df], axis=1, sort=False)
         return df
 
@@ -350,18 +349,18 @@
 
         if first_amount + (n - 1) * increase_amount < 0:
             return np.nan
         if x + n + defer > self.w:
             return .0
 
         term1 = first_amount * self.t_naax(x=x, n=n, m=m, defer=defer)
-        list_increases = [increase_amount * self.t_nax(x=x + defer, n=n-j, m=m, defer=defer + j - 1)
+        list_increases = [increase_amount * self.t_nax(x=x + defer, n=n - j, m=m, defer=defer + j - 1)
                           for j in range(1, n)]
 
-        return term1+sum(list_increases)
+        return term1 + sum(list_increases)
 
     # Present Value of a series of cash-flows
     def present_value(self, probs, age, spot_rates, capital):
         """
         Computes the expected present value of a cash-flows, that can be contingent on some probabilities.
         Payments are considered at the end of the period.
 
@@ -377,22 +376,27 @@
         probs_ = None
         if probs is None:
             if age is None:
                 return np.nan
             else:
                 probs_ = [self.npx(age, n + 1) for n in range(len(capital))]
 
+        if isinstance(probs, list):
+            if len(probs) == len(spot_rates):
+                probs_ = probs
+            else:
+                return np.nan
+
         if isinstance(probs, (float, int)):
             probs_ = [probs] * len(capital)
         discount = 1 + np.array(spot_rates) / 100.
         discount = np.cumprod(1 / discount)
 
         return sum([p * capital[idx_p] * discount[idx_p] for idx_p, p in enumerate(probs_)])
 
-
     ### Life Insurances
 
     ## Pure Endowment / Actuarial Present Value
 
     def nEx(self, x, n):
         """
         Actuarial Present Value of a Pure endowment or Deferred capital
@@ -661,15 +665,15 @@
 
         :return: net single premium of a Term Life Insurance with capitals increasing arithmetically, with first capital
         equal to the rate of progression (the increase amount). The payment is made at the moment of death.
         """
         if x < 0:
             return np.nan
         if x > self.w:
-            return self.__v ** 0.5 # it will die before year's end, because already attained age>w
+            return self.__v ** 0.5  # it will die before year's end, because already attained age>w
         D_x = self.__Dx[x]
         if self.__app_cont:
             R_x = self.__Rx[x]
         else:
             R_x = self.__Rx[x] * self.__cont
         self.msn.append(f"A_{x}={R_x} / {D_x}")
         return R_x / D_x
@@ -713,30 +717,30 @@
         equal to the rate of progression (the increase amount). The payment is made at the moment of death.
         """
         if x < 0:
             return np.nan
         if n < 0:
             return np.nan
         if x > self.w:
-            return self.__v ** 0.5 # it will die before year's end, because already attained age>w
+            return self.__v ** 0.5  # it will die before year's end, because already attained age>w
         D_x = self.__Dx[x]
         if self.__app_cont:
             M_x_n = self.__Mx[x + n]
             R_x = self.__Rx[x]
             R_x_n = self.__Rx[x + n]
         else:
             M_x_n = self.__Mx[x + n] * self.__cont
             R_x = self.__Rx[x] * self.__cont
             R_x_n = self.__Rx[x + n] * self.__cont
         self.msn.append(f"A_{x}=({R_x}-{R_x_n}-{n}x{M_x_n} / {D_x}")
         return (R_x - R_x_n - n * M_x_n) / D_x
 
     ## Variable Capitals increasing/decreasing arithmetically
 
-    def nIArx(self, x, n, defer=0, first_amount=1, increase_amount=1):
+    def t_nIArx(self, x, n, defer=0, first_amount=1, increase_amount=1):
         """
         Expected Present Value (EPV) of a Term Life Insurance that pays (first_amount + k*increase_amount), at the end of
         the year if death occurs between ages x+k and x+k+1, for k=0,..., n-1.
         Allows the computation of EPV for decreasing capitals.
         The first amount may differ from the increasing/decreasing amount.
 
         :param x: age at the beginning of the contract
@@ -748,21 +752,20 @@
         equal to the rate of progression (the increase amount). The payment is made at the end of the year of death.
         """
 
         if first_amount + (n - 1) * increase_amount < 0:
             return np.nan
 
         term1 = first_amount * self.t_nAx(x=x, n=n, defer=defer)
-        list_increases = [increase_amount * self.t_nAx(x=x + defer, n=n - j, defer=defer + j)
+        list_increases = [increase_amount * self.t_nAx(x=x, n=n - j, defer=defer + j)
                           for j in range(1, n)]
 
         return term1 + sum(list_increases)
 
-
-    def nIArx_(self, x, n, defer=0, first_amount=1, increase_amount=1):
+    def t_nIArx_(self, x, n, defer=0, first_amount=1, increase_amount=1):
         """
         Expected Present Value (EPV) of a Term Life Insurance that pays (first_amount + k*increase_amount), at the moment of death,
         if death occurs between ages x+k and x+k+1, for k=0,..., n-1.
         Allows the computation of EPV for decreasing capitals.
         The first amount may differ from the increasing/decreasing amount.
 
         :param x: age at the beginning of the contract
@@ -774,18 +777,11 @@
         equal to the rate of progression (the increase amount). The payment is made at the moment of death.
         """
 
         if first_amount + (n - 1) * increase_amount < 0:
             return np.nan
 
         term1 = first_amount * self.t_nAx_(x=x, n=n, defer=defer)
-        list_increases = [increase_amount * self.t_nAx_(x=x + defer, n=n - j, defer=defer + j)
+        list_increases = [increase_amount * self.t_nAx_(x=x, n=n - j, defer=defer + j)
                           for j in range(1, n)]
 
         return term1 + sum(list_increases)
-
-
-
-
-
-
-
```

### Comparing `lifeactuary-1.2.1/lifeActuary/commutation_table_frac.py` & `lifeactuary-1.3/lifeActuary/commutation_table_frac.py`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/lifeActuary/mortality_table.py` & `lifeactuary-1.3/lifeActuary/mortality_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
     the first age considered in the table.
     The life table will be complete, that is, from age 0 to age w, that is, the last age where lx>0.
     """
 
     def __init__(self, data_type='q', mt=None, perc=100, last_q=1):
         """
         Initializes the MortalityTable class, so we can construct a mortality table with the usual fields.
-        param data_type: Should be "l" for lx, "p" for px and "q" for qx.
+        :param data_type: Should be "l" for lx, "p" for px and "q" for qx.
         :param mt: Should be "l" for lx, "p" for px and "q" for qx.
         :param perc: The percentage of qx to use, e.g., you should use 50 for 50%.
         :param last_q: The value for qw.
         """
         if data_type not in ('l', 'q', 'p'):
             return
         if not mt:
             return
         self.__data_type = data_type
         self.__methods = ('udd', 'cfm', 'bal')
         self.__mt = mt
-        self.__x0 = np.int(mt[0])
+        self.__x0 = np.int32(mt[0])
         self.__last_q = last_q
         self.__w = 0
         self.__lx = []
         self.__px = []
         self.__qx = []
         self.__dx = []
         self.__ex = []
@@ -120,169 +120,174 @@
         data = {'x': np.arange(self.w + 1), 'lx': self.__lx[:-1], 'dx': self.__dx,
                 'qx': self.__qx, 'px': self.__px, 'exo': self.__ex}
         df = pd.DataFrame(data)
         df = df.astype({'x': 'int16'})
         return df
 
     def lx_udd(self, t):
-        if t > self.w+1:
+        if t > self.w + 1:
             return 0.
         if t < 0:
             return np.nan
-        int_t = np.int(t)
+        int_t = np.int32(t)
         frac_t = t - int_t
         if frac_t == 0:
             return self.__lx[int_t]
         else:
             return self.__lx[int_t] * (1 - frac_t) + self.__lx[int_t + 1] * frac_t
 
     def lx_cfm(self, t):
-        if t > self.w+1:
+        if t > self.w + 1:
             return 0.
         if t < 0:
             return np.nan
-        int_t = np.int(t)
+        int_t = np.int32(t)
         frac_t = t - int_t
         if frac_t == 0:
             return self.__lx[int_t]
         else:
             return self.__lx[int_t] * np.power(self.__lx[int_t + 1] / self.__lx[int_t], frac_t)
 
     def lx_bal(self, t):
-        if t > self.w+1:
+        if t >= self.w:
             return 0.
         if t < 0:
             return np.nan
-        int_t = np.int(t)
+        int_t = np.int32(t)
         frac_t = t - int_t
         if frac_t == 0:
             return self.__lx[int_t]
         else:
             inv_lx = 1 / self.__lx[int_t] - frac_t * (1 / self.__lx[int_t] - 1 / self.__lx[int_t + 1])
             return 1 / inv_lx
 
     def get_lx_method(self, x, method='udd'):
         if method not in self.__methods:
             return np.nan
         if x < 0:
             return np.nan
-        if x > self.w+1:
+        if x > self.w + 1:
             return 0
         if method == 'udd':
             return self.lx_udd(x)
         elif method == 'cfm':
             return self.lx_cfm(x)
         elif method == 'bal':
             return self.lx_bal(x)
         else:
             return np.nan
 
     def get_integral_px_method(self, x, method='udd'):
-        '''
+        """
         This function can be used to approximate the life expectancy between to ages, using the interpolation rules implemented.
         :param x: the value of x, that should be integer
         :param method: the chosen method to approximate px
         :return: the integral of tpx in the interval [0,1] that can be used to approximate life expectancy between ages.
-        '''
+        """
         if method not in self.__methods:
             return np.nan
         if x < 0:
             return np.nan
-        if x > self.w+1:
+        if x > self.w + 1:
             return 0
         if int(x) != x:
             return np.nan
+        x = int(x)
+
         if method == 'udd':
             return 1 - .5 * self.qx[x]
         elif method == 'cfm':
             if self.px[x] == 0:
                 return .0
             return -self.qx[x] / np.log(self.px[x])
         elif method == 'bal':
             if self.px[x] == 0:
                 return .0
             return -self.px[x] / self.qx[x] * np.log(self.px[x])
         else:
             return np.nan
 
     def nqx(self, x, n=1, method='udd'):
-        '''
+        """
         Obtains the probability that a life x dies before x+t
         :param method: the method used to approximate lx for non-integer x's
         :param x: age at beginning
         :param n: period
         :return: probability of x dying before x+t
-        '''
+        """
         if method not in self.__methods:
             return np.nan
         if x < 0:
             return np.nan
         if n <= 0:
             return .0
-        if x + n > self.w+1:
+        if x + n > self.w + 1:
             return self.__qx[-1]
         l_x = self.get_lx_method(x, method)
         l_x_t = self.get_lx_method(x + n, method)
         self.msn.append(f"{n}_q_{x}=1-({l_x_t} / {l_x})")
+        if l_x == 0: return 1.
         return 1 - l_x_t / l_x
 
     def npx(self, x, n=1, method='udd'):
-        '''
+        """
         Obtains the probability that a life x dies before x+t
         :param method: the method used to approximate lx for non-integer x's
         :param x: age at beginning
         :param n: period
         :return: probability of x dying before x+t
-        '''
+        """
         if method not in self.__methods:
             return np.nan
         if x < 0:
             return np.nan
         if n <= 0:
             return 1.
-        if x + n > self.w+1:
+        if x + n > self.w + 1:
             return self.__px[-1]
         l_x = self.get_lx_method(x, method)
         l_x_t = self.get_lx_method(x + n, method)
         self.msn.append(f"{n}_p_{x}={l_x_t} / {l_x}")
+        if l_x == 0: return .0
         return l_x_t / l_x
 
     def t_nqx(self, x, t=1, n=1, method='udd'):
-        '''
+        """
         Obtains the probability that a life x dies survives to age x+t and dies before x+t+n
         :param method: the method used to approximate lx for non-integer x's
         :param x: age at beginning
         :param t: deferment period
         :param n: period
         :return: probability of x dying after age x+t and before x+t+n
-        '''
+        """
         l_x = self.get_lx_method(x, method)
         l_x_t = self.get_lx_method(x + t, method)
         l_x_t_n = self.get_lx_method(x + t + n, method)
         self.msn.append(f"{t}|{n}_q_{x}={t}_p_{x}  {n}_q_{x + t}={l_x_t} / {l_x} ({l_x_t}-{l_x_t_n}) / {l_x_t}")
+        if l_x == 0: return 1.
         return (l_x_t - l_x_t_n) / l_x
 
     def force_qw_0(self):
-        '''
+        """
         forces the last qx to be equal to zero, to state that there are no more decrements after w
         :return: the qx, px and lx adjusted
-        '''
+        """
         self.__qx[-1] = 0
         self.__px[-1] = 1
         self.__lx[-1] = self.__lx[-2:-1][0]
         self.__dx[-1] = 0
 
     def exn(self, x, n, method='udd'):
-        '''
+        """
         Computes the approximated life expectancy between two ages.
         :param x: Initial age.
         :param n: Period to be considered.
         :param method: The method used to interpolate.
         :return: The approximated life span between x and x+n, considering the interpolation methods implemented to approximate the integral of the survival function.
-        '''
+        """
         if method not in self.__methods:
             return np.nan
         if x < 0:
             return np.nan
         if n <= 0:
             return 1.
```

### Comparing `lifeactuary-1.2.1/lifeActuary/read_soa_table_xml.py` & `lifeactuary-1.3/soa_tables/read_soa_table_xml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "PedroCR"
 
 from xml.dom import minidom
 
 http_header = 'https://mort.soa.org/ViewTable.aspx?&TableIdentity='
 
-# todo: correct nan when reading tables from excel with different w's.
+
 class SoaTable:
     def __init__(self, table_name):
         '''
         Reads a previously downloaded life table, from Society of Actuaries, in the xml format and prepares
         all the information to create a life (mortality table).
         :param table_name: The SOA table, in xml format, to be read.
         '''
@@ -20,8 +20,7 @@
         self.contentType = self.xmldoc.getElementsByTagName('ContentType')[0].childNodes[0].data
         self.tableReference = self.xmldoc.getElementsByTagName('TableReference')[0].childNodes[0].data
         self.ages = self.xmldoc.getElementsByTagName('Y')
         self.min_age = int(self.ages[0].attributes['t'].value)
         self.max_age = self.min_age + len(self.ages) - 1
         self.table_qx = [float(age.childNodes[0].data) for age in self.ages]
         self.table_qx.insert(0, self.min_age)
-        # todo: scrap the tables from SOA
```

### Comparing `lifeactuary-1.2.1/soa_tables/197982PortugalFemale.xml` & `lifeactuary-1.3/soa_tables/197982PortugalFemale.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/197982PortugalMale.xml` & `lifeactuary-1.3/soa_tables/197982PortugalMale.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/AF80.xml` & `lifeactuary-1.3/soa_tables/AF80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/AM80.xml` & `lifeactuary-1.3/soa_tables/AM80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/CSO_1941.xml` & `lifeactuary-1.3/soa_tables/CSO_1941.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/GRF95.xml` & `lifeactuary-1.3/soa_tables/GRF95.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/GRM80.xml` & `lifeactuary-1.3/soa_tables/GRM80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/GRM95.xml` & `lifeactuary-1.3/soa_tables/GRM95.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/IA8590F.xml` & `lifeactuary-1.3/soa_tables/IA8590F.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/IA8590M.xml` & `lifeactuary-1.3/soa_tables/IA8590M.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/PFL80.xml` & `lifeactuary-1.3/soa_tables/PFL80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/PML80.xml` & `lifeactuary-1.3/soa_tables/PML80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/SIF91.xml` & `lifeactuary-1.3/soa_tables/SIF91.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/SIM91.xml` & `lifeactuary-1.3/soa_tables/SIM91.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/TV7377.xml` & `lifeactuary-1.3/soa_tables/TV7377.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/TV8890.xml` & `lifeactuary-1.3/soa_tables/TV8890.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/WL80.xml` & `lifeactuary-1.3/soa_tables/WL80.xml`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/soa_tables/tables_manual.xlsx` & `lifeactuary-1.3/soa_tables/tables_manual.xlsx`

 * *Files identical despite different names*

### Comparing `lifeactuary-1.2.1/LICENSE` & `lifeactuary-1.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Pedro Corte Real, Gracinda R. Guerreiro
+Copyright (c) 2023 Pedro Corte Real, Gracinda R. Guerreiro
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

