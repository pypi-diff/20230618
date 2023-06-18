# Comparing `tmp/stql-2.0.tar.gz` & `tmp/stql-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stql-2.0.tar", last modified: Sun Jun 18 16:19:41 2023, max compression
+gzip compressed data, was "stql-2.1.tar", last modified: Sun Jun 18 16:23:59 2023, max compression
```

## Comparing `stql-2.0.tar` & `stql-2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:19:41.923390 stql-2.0/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:19:41.923390 stql-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-18 16:19:41.923390 stql-2.0/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-06-18 16:19:20.000000 stql-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:19:41.907147 stql-2.0/stql/
--rw-rw-rw-   0        0        0     9924 2023-06-18 16:18:39.000000 stql-2.0/stql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:19:41.923390 stql-2.0/stql.egg-info/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 16:23:59.484702 stql-2.1/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:23:59.484702 stql-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:23:59.484702 stql-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      210 2023-06-18 16:23:56.000000 stql-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:23:59.462895 stql-2.1/stql/
+-rw-rw-rw-   0        0        0     9923 2023-06-18 16:23:32.000000 stql-2.1/stql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:23:59.484702 stql-2.1/stql.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2023-06-18 16:23:59.000000 stql-2.1/stql.egg-info/top_level.txt
```

### Comparing `stql-2.0/stql/__init__.py` & `stql-2.1/stql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                         min_idx = j
             arr[i], arr[min_idx] = arr[min_idx], arr[i]
         return arr
     '''
     d = {'стек': stack, 'очередь': queue, 'двусвязный список': dll, 'вставками': ins_s, 'пузырьком': b_s, 'быстрая': q_s, 'выбором': sel_s}
     print(d[key])
   
- def choice2(key):
+def choice2(key):
     d = {'анаграммы':anagram, 'isprime': isprime, 'сумма квадратов': kv_sum, 'гласные': glasnie, 'капрекара': capr, 'армстронга': armstrong, 'кармайкл': carm}
     anagram = '''
     lst = ['парк', 'карп', 'среда', 'антон', 'андрей', 'адрес', 'топор', 'грот', 'торг', 'ропот', 'повтор']
     a = set()
     f = lambda x, y: all((x.count(i) == y.count(i) and len(x) == len(y)) for i in x)
     for i in range(0, len(lst) - 1):
       for j in range(i+1, len(lst)):
@@ -210,24 +210,21 @@
           a.add(lst[i])
           a.add(lst[j])
     print(a)
     '''
     isprime = '''
     isprime = lambda x: x > 0 and all(x % i for i in range(2, int(x ** 0.5) + 1))
     '''
-    
     kv_sum = '''
     result_list = list(filter(lambda x: any(x == a*a + b*b for a in range(0, x) for b in range(0, x)), range(1, 50+1)))
     '''
-    
     glasnie = '''
     gl = list('ауоыиэяюёе')
     print(sorted(lst, key = lambda x : sum(1 for i in x if i in gl)))
     '''
-    
     capr = '''
     def chisla(element):
       s = str(element ** 2)
       for i in range(0, len(s)):
         a = s[:i+1]
         b = s[i+1:]
         ch = 0
@@ -238,33 +235,32 @@
             break
           else:
             ch = a + b
             if ch == element:
               return True
     print(list(filter(lambda x: chisla(x), lst)))
     '''
-    
     armstrong = '''
     armstrong_nums = list(filter(lambda n: sum(int(digit)**len(str(n)) for digit in str(n)) == n, lst))
     '''
-    
     carm = '''
     import math
     lst = [561, 256, 8911, 1729, 2465, 147, 6601,12,31]
     def is_carmichael(n):
         for a in range(2, n):
             if math.gcd(a, n) == 1 and pow(a, n-1, n) != 1:
                 return False
         return True
     carmichael_numbers = sorted(list(filter(lambda x: is_carmichael(x), lst)))
     print(f"Числа Кармайкла: {carmichael_numbers}")
     '''
+    print(d[key]) 
     
- def leonov():
-    return '''
+def leonov():
+    a = '''
     lst = ['парк', 'карп', 'среда', 'антон', 'андрей', 'адрес', 'топор', 'грот', 'торг', 'ропот', 'повтор']
     a = set()
     f = lambda x, y: all((x.count(i) == y.count(i) and len(x) == len(y)) for i in x)
     for i in range(0, len(lst) - 1):
       for j in range(i+1, len(lst)):
         if f(lst[i],lst[j]):
           a.add(lst[i])
@@ -300,8 +296,9 @@
         return True
       return False 
     def is_carm(n):
         for a in range(2, n):
             if math.gcd(a, n) == 1 and pow(a, n-1, n) != 1:
                 return False
         return True
-    '''
+    '''
+    print(a)
```

