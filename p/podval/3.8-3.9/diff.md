# Comparing `tmp/podval-3.8.tar.gz` & `tmp/podval-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-3.8.tar", last modified: Fri Jun 16 21:35:06 2023, max compression
+gzip compressed data, was "dist\podval-3.9.tar", last modified: Sun Jun 18 11:45:16 2023, max compression
```

## Comparing `podval-3.8.tar` & `podval-3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:06.000000 podval-3.8/
--rw-rw-rw-   0        0        0      188 2023-06-16 21:35:06.000000 podval-3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:06.000000 podval-3.8/podval/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.8/podval/__init__.py
--rw-rw-rw-   0        0        0    97495 2023-06-16 21:32:51.000000 podval-3.8/podval/exam.py
--rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.8/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-16 21:35:06.000000 podval-3.8/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.8/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-16 21:35:05.000000 podval-3.8/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 21:35:06.000000 podval-3.8/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-16 21:32:57.000000 podval-3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:45:16.000000 podval-3.9/
+-rw-rw-rw-   0        0        0      188 2023-06-18 11:45:16.000000 podval-3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 11:45:16.000000 podval-3.9/podval/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:57:54.000000 podval-3.9/podval/__init__.py
+-rw-rw-rw-   0        0        0    99871 2023-06-18 11:43:41.000000 podval-3.9/podval/exam.py
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-3.9/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:45:16.000000 podval-3.9/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-18 11:45:14.000000 podval-3.9/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-06-18 11:45:15.000000 podval-3.9/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:45:14.000000 podval-3.9/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-3.9/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-18 11:45:14.000000 podval-3.9/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:45:16.000000 podval-3.9/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-18 11:44:26.000000 podval-3.9/setup.py
```

### Comparing `podval-3.8/podval/exam.py` & `podval-3.9/podval/exam.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,74 @@
 1) Лямбда-функции: fchyaks, bstsk, lpschsi, isusd, nipsu, pyaksz, chsrchd, pavzs, lpssszva, lpschsz, evpks, lichsz, nipchd, chpyaks, rvbts, ndnin, tstsks, chspvch, tnzks, kchyaks, achyaks, akvpn, lpschts, lpschz, pivia, lichsz, lpssszvch     
 2) Сортировки: kkemi, skvbg, chpobd, skdup, kkevv, skvzi, applv
 3) Классы (с дочерними): Автомобиль - khzsap, Фильм - rivgz, Продукт - sitszs, Животное - oipzs, Студент - dtibs
 4) Классы: Банк - fuvko, Круг - tstsirr, Студент - vvisv, Recipe - dtiyai, Animal - zhtsups, Student - suknf, Книга - igpkd, BankAccount - sokvv, Movie - fzhups, Прямоугольник - pppds
 5) Двусвязный список: nneei, nsitn, sdvev, sdvem, sieui, sivii, sdvek
 6) Стэк: sedkya, sepdya, chchyank
 7) Бинарное дерево поиска: pdbvn, pdbvz
-8) Очередь вар: ddnot, ddnot, upobd
+8) Очередь: ddnot, ddnot, upobd
 9) Хеш-таблица: tyaovkh, tyaovkhdoa
-10) Квик сорт: sbapsd
-11) Бабл сорт: psaps
-12) Инсершн сорт: vsapsa''')
+10) Быстрая сорт: sbapsd
+11) Пузырьком сорт: psaps
+12) Вставками сорт: vsapsa, vsapsu
+13) Выбором сорт: vsapss
+
+Интересные методы:
+1) a.lower() - преобразует строку в нижний регистр
+2) a.isdigit() - проверка на цифру
+3) a.isupper() - проверка на большие буквы
+4) isinstance(obj, class) принадлежит ли объект определенному типу или нет''')
+
+#Допка
+def HashTable():
+    print('''
+class HashTable:
+    def __init__(self):
+        self.size = 10
+        self.table = [[] for _ in range(self.size)]
+
+    def _hash_func(self, key):
+        return hash(key) % self.size
+
+    def insert(self, key, value):
+        hash_key = self._hash_func(key)
+        for idx, kv in enumerate(self.table[hash_key]):
+            k, v = kv
+            if key == k:
+                self.table[hash_key][idx] = (key, value)
+                break
+        else:
+            self.table[hash_key].append((key, value))
+
+    def search(self, key):
+        hash_key = self._hash_func(key)
+        for k, v in self.table[hash_key]:
+            if key == k:
+                return v
+        raise KeyError(key)
+
+    def delete(self, key):
+        hash_key = self._hash_func(key)
+        for idx, kv in enumerate(self.table[hash_key]):
+            k, v = kv
+            if key == k:
+                del self.table[hash_key][idx]
+                return
+        raise KeyError(key)
 
+    def display(self):
+        print("{:<15} {}".format("Key", "Value"))
+        print("---------------")
+        for bucket in self.table:
+            for k, v in bucket:
+                print("{:<15} {}".format(k, v))
+
+
+Метод `display` выводит все ключи и значения на экран, отформатированные в виде таблицы с двумя столбцами. Он проходит по каждой корзинке хэш-таблицы и для каждой пары ключ-значение выводит строку в формате `"{:<15} {}"`, где `'{:<15}'` означает, что первый столбец должен занимать 15 символов и быть выровнен по левому краю, а `{}` - это второй столбец со значением.''')
+    
 #1
 def fchyaks():
     print('''#Используя лямбда-функцию, найдите все числа в заданном списке, которые являются числами Фибоначчи.
 
 is_fibo = (lambda a: lambda v,fib=0,n=1: a(a,v,fib,n))(lambda f,value,fib,n: f(f,value,fib+n,fib) if fib < value else fib==value)
 
 # Заданный список чисел
@@ -1541,20 +1595,22 @@
 #приготовления блюда, и свойство, позволяющее установить тип кухни
 #(например, итальянская, японская и т. д.).
 class Recipe:
     def __init__(self, name, ingredients, steps):
         self.name = name
         self.ingredients = ingredients
         self.steps = steps
-        self._cuisine_type = ""
+        self._cuisine_type = None
 
     def display_recipe(self):
         print(f"{self.name}\nIngredients: {self.ingredients}\nSteps:")
         for i, step in enumerate(self.steps, start=1):
             print(f"{i}. {step}")
+        if self.cuisine_type:
+            print(f"Тип кухни: {self.cuisine_type}\n")
 
     def check_ingredients(self, available_ingredients):
         for ingredient in self.ingredients:
             if ingredient not in available_ingredients:
                 return False
         return True
```

### Comparing `podval-3.8/podval/podval.py` & `podval-3.9/podval/podval.py`

 * *Files identical despite different names*

