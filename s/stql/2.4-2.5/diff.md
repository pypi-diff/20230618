# Comparing `tmp/stql-2.4.tar.gz` & `tmp/stql-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stql-2.4.tar", last modified: Sun Jun 18 16:43:14 2023, max compression
+gzip compressed data, was "stql-2.5.tar", last modified: Sun Jun 18 17:27:42 2023, max compression
```

## Comparing `stql-2.4.tar` & `stql-2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:43:14.283736 stql-2.4/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:43:14.283736 stql-2.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-18 16:43:14.299374 stql-2.4/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-06-18 16:42:54.000000 stql-2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:43:14.275224 stql-2.4/stql/
--rw-rw-rw-   0        0        0    18549 2023-06-18 16:42:42.000000 stql-2.4/stql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:43:14.283736 stql-2.4/stql.egg-info/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:27:42.235479 stql-2.5/
+-rw-rw-rw-   0        0        0      101 2023-06-18 17:27:42.236475 stql-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:27:42.238479 stql-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      210 2023-06-18 17:27:26.000000 stql-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:27:42.218338 stql-2.5/stql/
+-rw-rw-rw-   0        0        0    27556 2023-06-18 17:27:13.000000 stql-2.5/stql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:27:42.232476 stql-2.5/stql.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-06-18 17:27:42.000000 stql-2.5/stql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-18 17:27:42.000000 stql-2.5/stql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:27:42.000000 stql-2.5/stql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 17:27:42.000000 stql-2.5/stql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2023-06-18 17:27:42.000000 stql-2.5/stql.egg-info/top_level.txt
```

### Comparing `stql-2.4/stql/__init__.py` & `stql-2.5/stql/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -367,31 +367,304 @@
     ord4 = Order('Игрушка', '2021-01-01')
     print(ord1.date)
     orders = [ord1,ord2,ord3,ord4]
     print(orders)
     Order.quick_sort(orders)
     print(orders)
     '''
+    z22 = '''
+    class Node:
+        def __init__(self, data):
+          self.data = data
+          self.left = None
+          self.right = None        
+    
+    class BinaryTree:
+        def __init__(self):
+            self.root = None
+    
+        def insert(self, data):
+            new_node = Node(data)
+            if self.root is None:
+                self.root = new_node
+            else:
+                current = self.root
+                while True:
+                    if data < current.data:
+                        if current.left is None:
+                            current.left = new_node
+                            break
+                        else:
+                            current = current.left
+                    else:
+                        if current.right is None:
+                            current.right = new_node
+                            break
+                        else:
+                            current = current.right
+    
+        def search(self, data):
+            current = self.root
+            while current is not None:
+                if data == current.data:
+                    return True
+                elif data < current.data:
+                    current = current.left
+                else:
+                    current = current.right
+            return False
+    
+        def delete(self, data):
+            if self.root is not None:
+                self.root = self._delete(data, self.root)
+    
+        def _delete(self, data, node):
+            if node is None:
+                return node
+    
+            if data < node.data:
+                node.left = self._delete(data, node.left)
+            elif data > node.data:
+                node.right = self._delete(data, node.right)
+            else:
+                if node.left is None:
+                    return node.right
+                elif node.right is None:
+                    return node.left
+    
+                temp = self._find_min_node(node.right)
+                node.data = temp.data
+                node.right = self._delete(temp.data, node.right)
+    
+            return node
+    
+        def _find_min_node(self, node):
+            while node.left is not None:
+                node = node.left
+            return node
+    
+        def _display(self, node, level=0):
+          if node is not None:
+            self._display(node.right, level+1)
+            print("\t" * level, "->", node.data)
+            self._display(node.left, level+1)
+    
+        def display(self):
+          self._display(self.root)
+    
+        def find_largest_smaller_than(self, data):
+            current = self.root
+            largest_smaller = None
+            while current is not None:
+              if current.data < data:
+                if largest_smaller is None or current.data > largest_smaller:
+                    largest_smaller = current.data
+                current = current.right
+              else:
+                  current = current.left
+            return largest_smaller
+    
+    bt = BinaryTree()
+    bt.insert(5)
+    bt.insert(2)
+    bt.insert(8)
+    bt.insert(1)
+    bt.insert(3)
+    bt.insert(1)
+    bt.insert(2)
+    bt.insert(16)
+    bt.insert(7)
+    bt.display()
+    #bt.find_largest_smaller_than(5)
+    '''
+    z23 = '''
+    class Node:
+        def __init__(self, data):
+          self.data = data
+          self.left = None
+          self.right = None        
+    
+    class BinaryTree:
+        def __init__(self):
+            self.root = None
+    
+        def insert(self, data):
+            new_node = Node(data)
+            if self.root is None:
+                self.root = new_node
+            else:
+                current = self.root
+                while True:
+                    if data < current.data:
+                        if current.left is None:
+                            current.left = new_node
+                            break
+                        else:
+                            current = current.left
+                    else:
+                        if current.right is None:
+                            current.right = new_node
+                            break
+                        else:
+                            current = current.right
+    
+        def search(self, data):
+            current = self.root
+            while current is not None:
+                if data == current.data:
+                    return True
+                elif data < current.data:
+                    current = current.left
+                else:
+                    current = current.right
+            return False
+    
+        def delete(self, data):
+            if self.root is not None:
+                self.root = self._delete(data, self.root)
+    
+        def _delete(self, data, node):
+            if node is None:
+                return node
+    
+            if data < node.data:
+                node.left = self._delete(data, node.left)
+            elif data > node.data:
+                node.right = self._delete(data, node.right)
+            else:
+                if node.left is None:
+                    return node.right
+                elif node.right is None:
+                    return node.left
+    
+                temp = self._find_min_node(node.right)
+                node.data = temp.data
+                node.right = self._delete(temp.data, node.right)
+    
+            return node
+    
+        def _find_min_node(self, node):
+            while node.left is not None:
+                node = node.left
+            return node
+    
+        def _display(self, node, level=0):
+          if node is not None:
+            self._display(node.right, level+1)
+            print("\t" * level, "->", node.data)
+            self._display(node.left, level+1)
+    
+        def display(self):
+          self._display(self.root)
+    
+        def height(self, node):
+            if node is None:
+                return 0
+            else:
+                left_height = self.height(node.left)
+                right_height = self.height(node.right)
+                return max(left_height, right_height) + 1
+    
+        def get_height(self):
+            return self.height(self.root)
+    
+    bt = BinaryTree()
+    bt.insert(5)
+    bt.insert(2)
+    bt.insert(8)
+    bt.insert(1)
+    bt.insert(3)
+    bt.insert(1)
+    bt.insert(2)
+    bt.insert(16)
+    bt.insert(7)
+    bt.get_height()
+    '''
+    z25 = '''
+    class Book:
+        def __init__(self, title, author, year):
+            self.title = title
+            self.author = author
+            self.year = year
+        def __str__(self):
+          return f'Название {self.title}, автор: {self.author}, год: {self.year}'
+    class HashTable:
+        def __init__(self, size):
+            self.size = size
+            self.table = [[] for _ in range(self.size)]
+    
+        def hash_function(self, key):
+            return hash(key) % self.size
+    
+        def insert(self, book):
+            slot = self.hash_function(book.author)
+            for pair in self.table[slot]:
+                if pair[0] == book.author:
+                    pair[1].append(book)
+                    return
+            self.table[slot].append((book.author, [book]))
+    
+        def find(self, author):
+            slot = self.hash_function(author)
+            for pair in self.table[slot]:
+                if pair[0] == author:
+                    return pair[1]
+            return None
+    
+    ht = HashTable(10)
+    book1 = Book("Преступление и наказание", "Федор Достоевский", 1866)
+    book2 = Book("Война и мир", "Лев Толстой", 1869)
+    book3 = Book("Идиот", "Федор Достоевский", 1869)
+    ht.insert(book1)
+    ht.insert(book2)
+    ht.insert(book3)
+    for book in (ht.find('Федор Достоевский')):
+      print(book)
+
+    '''
     d = {'стек': stack,
     'очередь': queue, 
     'двусвязный список': dll, 
     'вставками': ins_s, 
     'пузырьком': b_s,
     'быстрая': q_s, 
     'выбором': sel_s,
     'метод класса заказ': z21,
     'список чисел вставками': z20,
     'метод класса клиент': z19,
     'список строк выбором': z18,
     'список дат пузырьком': z17,
     'метод класса товар': z16,
     'список слов вставками': z15,
+    'наибольший дерево': z22,
+    'высота дерева': z23,
+    'хеш-таблица': z25
          }
     print(d[key])
 
+def info():
+    d = {'стек': 1,
+         'очередь': 2,
+         'двусвязный список': 3,
+         'вставками': 4,
+         'пузырьком': 5,
+         'быстрая': 6,
+         'выбором': 7,
+         'метод класса заказ': 8,
+         'список чисел вставками': 9,
+         'метод класса клиент': 10,
+         'список строк выбором': 11,
+         'список дат пузырьком': 12,
+         'метод класса товар': 13,
+         'список слов вставками': 14,
+        'наибольший дерево': 15,
+        'высота дерева': 16,
+        'хеш-таблица': 17
+         }
+    print(d.keys())
 
 def choice2(key):
     anagram = '''
     lst = ['парк', 'карп', 'среда', 'антон', 'андрей', 'адрес', 'топор', 'грот', 'торг', 'ропот', 'повтор']
     a = set()
     f = lambda x, y: all((x.count(i) == y.count(i) and len(x) == len(y)) for i in x)
     for i in range(0, len(lst) - 1):
```

