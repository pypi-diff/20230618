# Comparing `tmp/stql-2.1.tar.gz` & `tmp/stql-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stql-2.1.tar", last modified: Sun Jun 18 16:23:59 2023, max compression
+gzip compressed data, was "stql-2.2.tar", last modified: Sun Jun 18 16:26:51 2023, max compression
```

## Comparing `stql-2.1.tar` & `stql-2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:23:59.484702 stql-2.1/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:23:59.484702 stql-2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-18 16:23:59.484702 stql-2.1/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-06-18 16:23:56.000000 stql-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:23:59.462895 stql-2.1/stql/
--rw-rw-rw-   0        0        0     9923 2023-06-18 16:23:32.000000 stql-2.1/stql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:23:59.484702 stql-2.1/stql.egg-info/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 16:26:51.277155 stql-2.2/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:26:51.277155 stql-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:26:51.277155 stql-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      210 2023-06-18 16:26:24.000000 stql-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:26:51.251314 stql-2.2/stql/
+-rw-rw-rw-   0        0        0     9923 2023-06-18 16:26:36.000000 stql-2.2/stql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:26:51.273645 stql-2.2/stql.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:26:51.000000 stql-2.2/stql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-18 16:26:51.000000 stql-2.2/stql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:26:51.000000 stql-2.2/stql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 16:26:51.000000 stql-2.2/stql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2023-06-18 16:26:51.000000 stql-2.2/stql.egg-info/top_level.txt
```

### Comparing `stql-2.1/stql/__init__.py` & `stql-2.2/stql/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,14 @@
             arr[i], arr[min_idx] = arr[min_idx], arr[i]
         return arr
     '''
     d = {'стек': stack, 'очередь': queue, 'двусвязный список': dll, 'вставками': ins_s, 'пузырьком': b_s, 'быстрая': q_s, 'выбором': sel_s}
     print(d[key])
   
 def choice2(key):
-    d = {'анаграммы':anagram, 'isprime': isprime, 'сумма квадратов': kv_sum, 'гласные': glasnie, 'капрекара': capr, 'армстронга': armstrong, 'кармайкл': carm}
     anagram = '''
     lst = ['парк', 'карп', 'среда', 'антон', 'андрей', 'адрес', 'топор', 'грот', 'торг', 'ропот', 'повтор']
     a = set()
     f = lambda x, y: all((x.count(i) == y.count(i) and len(x) == len(y)) for i in x)
     for i in range(0, len(lst) - 1):
       for j in range(i+1, len(lst)):
         if f(lst[i],lst[j]):
@@ -249,14 +248,15 @@
         for a in range(2, n):
             if math.gcd(a, n) == 1 and pow(a, n-1, n) != 1:
                 return False
         return True
     carmichael_numbers = sorted(list(filter(lambda x: is_carmichael(x), lst)))
     print(f"Числа Кармайкла: {carmichael_numbers}")
     '''
+    d = {'анаграммы':anagram, 'isprime': isprime, 'сумма квадратов': kv_sum, 'гласные': glasnie, 'капрекара': capr, 'армстронга': armstrong, 'кармайкл': carm}
     print(d[key]) 
     
 def leonov():
     a = '''
     lst = ['парк', 'карп', 'среда', 'антон', 'андрей', 'адрес', 'топор', 'грот', 'торг', 'ропот', 'повтор']
     a = set()
     f = lambda x, y: all((x.count(i) == y.count(i) and len(x) == len(y)) for i in x)
```

