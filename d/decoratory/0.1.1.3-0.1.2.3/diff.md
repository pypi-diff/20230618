# Comparing `tmp/decoratory-0.1.1.3.tar.gz` & `tmp/decoratory-0.1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.1.3.tar", last modified: Fri Jun 16 18:02:15 2023, max compression
+gzip compressed data, was "decoratory-0.1.2.3.tar", last modified: Sun Jun 18 17:23:04 2023, max compression
```

## Comparing `decoratory-0.1.1.3.tar` & `decoratory-0.1.2.3.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.974894 decoratory-0.1.1.3/
--rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.1.3/License.txt
--rw-rw-rw-   0        0        0    39099 2023-06-16 18:02:15.974894 decoratory-0.1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    37474 2023-06-16 17:55:52.000000 decoratory-0.1.1.3/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.1.3/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.924897 decoratory-0.1.1.3/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.964893 decoratory-0.1.1.3/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.1.3/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     4621 2023-06-16 18:01:41.000000 decoratory-0.1.1.3/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     4855 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    16033 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    40070 2023-06-16 17:56:14.000000 decoratory-0.1.1.3/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     9128 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    13933 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.964893 decoratory-0.1.1.3/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    39099 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 18:02:15.974894 decoratory-0.1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     4017 2023-06-16 18:01:41.000000 decoratory-0.1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.2.3/License.txt
+-rw-rw-rw-   0        0        0    43195 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    41570 2023-06-18 17:20:31.000000 decoratory-0.1.2.3/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.2.3/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.902316 decoratory-0.1.2.3/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.940058 decoratory-0.1.2.3/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.2.3/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     5466 2023-06-18 17:22:40.000000 decoratory-0.1.2.3/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5490 2023-06-18 11:48:18.000000 decoratory-0.1.2.3/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-17 09:30:05.000000 decoratory-0.1.2.3/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    11946 2023-06-17 11:25:08.000000 decoratory-0.1.2.3/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    38712 2023-06-18 17:18:51.000000 decoratory-0.1.2.3/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7319 2023-06-17 11:25:08.000000 decoratory-0.1.2.3/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0     9932 2023-06-17 11:25:08.000000 decoratory-0.1.2.3/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.940058 decoratory-0.1.2.3/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    43195 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/Unittest/
+-rw-rw-rw-   0        0        0    24268 2023-06-18 11:03:38.000000 decoratory-0.1.2.3/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    21811 2023-06-18 10:51:44.000000 decoratory-0.1.2.3/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    42465 2023-06-18 08:46:05.000000 decoratory-0.1.2.3/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10504 2023-06-18 13:26:28.000000 decoratory-0.1.2.3/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0     9069 2023-06-18 11:03:38.000000 decoratory-0.1.2.3/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     4446 2023-06-18 17:22:40.000000 decoratory-0.1.2.3/setup.py
```

### Comparing `decoratory-0.1.1.3/License.txt` & `decoratory-0.1.2.3/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.1.3/PKG-INFO` & `decoratory-0.1.2.3/Readme.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,7 @@
-Metadata-Version: 2.1
-Name: decoratory
-Version: 0.1.1.3
-Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
-Home-page: http://evation.eu
-Download-URL: http://evation.eu
-Author: Martin Abel
-Author-email: Martin Abel <python@evation.eu>
-Maintainer: Martin Abel
-Maintainer-email: Martin Abel <python@evation.eu>
-License: PSF
-Project-URL: Projekt, http://evation.eu
-Project-URL: Release Notes, http://evation.eu
-Project-URL: Download, http://evation.eu
-Keywords: decorator singleton multiton observer observable wrapper
-Platform: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation
-Classifier: License :: OSI Approved :: Python Software Foundation License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: License.txt
-
 
 .. _top:
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
@@ -60,27 +21,32 @@
     pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
+In particular, there is a *comprehensive unit test* for each module, which 
+can be executed from the command line using the ``--test`` option. ::
+
+    python -m decoratory --test
+
 .. _toc:
 
 **Package Contents**
 
 The *decoratory package* available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_ 
 
-This is an open list that possibly will grow over time.
+This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, a simple as well as a
 more complex example is presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
@@ -130,14 +96,16 @@
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Teddy')
     print(f"b = {b}")               # b = Animal('Teddy')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
+.. _dynamic-decoration:
+
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
 code is used, additional parameters can be passed to the decorator for
 passing to the class constructor.
 
 .. code-block:: python
 
@@ -348,15 +316,15 @@
                                     #  True:  Animal('cat', 'Molly')}
 
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
-.. warning::
+.. hint::
 
     Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory, i.e. the directory may then be
     corrupted by such modifications.
 
     Therefore, **never change key related values of classified objects**!
@@ -496,20 +464,21 @@
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
-.. note::
+.. hint::
 
     Decorations to ``@staticmethod`` or ``@classmethod`` can be done
     analogously to the function decorations above, since they already exist
     at compile time. Instance methods, on the other hand, do not exist until
-    an object instance is created and must be handled differently.
+    an object instance is created and must be decorated dynamically as an 
+    instance (e.g. see  `Instance Decoration`_ below).
 
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
@@ -541,16 +510,16 @@
 observed object (observable, publisher, subject).
 
 This implementation provides several ways to decorate a function or class
 as an observable or observer.
 
 * `Observable Decoration`_
 * `Observer Decoration`_
-* `Static Class Decoration`_
-* `Dynamic Class Decoration`_ 
+* `Class Decoration`_
+* `Instance Decoration`_ 
 
 
 Observable Decoration
 ---------------------
 
 The simplest and at the same time the most Pythonic variant of decoration
 is to decorate only the *observed* entities.
@@ -668,17 +637,17 @@
 And again, cat acts before person because of the order of the observer
 list.
 
 
 Observer Decoration 
 -------------------
 
-In this reverse decoration, the observer decorator collects its observables.
-Because an observer decoration uses observable methods, all observable(s)
-must always be declared before their observer(s).
+In this reversed decoration scheme, the observer decorator collects its 
+observables. Because an observer decoration uses observable methods, all 
+observable(s) must always be declared before their observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
 Thus, the initial example ``Case 1`` from above is as follows:
 
 .. code-block:: python
 
@@ -738,15 +707,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Here, the *observed cat* observes the dog, reacts and triggers the person 
-observing the *orignal cat*. This situation reflects the ``Case 2`` from above.
+observing the *original cat*. This situation reflects the ``Case 2`` from above.
 
 To reproduce ``Case 3`` above, simply swap the order of the decorations at the 
 cat and the person then looks at the *observed cat*.
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
@@ -777,20 +746,20 @@
 
 Note the difference: in ``Case 2``, the cat ends up as an ``Observer``, not as 
 an ``Observable``. So the person observes the *original cat*. Whereas in 
 ``case 3``, the cat actually ends up as an ``Observable`` and person can observe 
 the *observed cat*.
 
 
-Static Class Decoration 
------------------------
+Class Decoration 
+----------------
 
-Both techniques, observable and observer decoration, are static, in the sense, 
-decorations are done in @-notation evaluated at compile time. They are applied 
-to *static functions*.
+Both above techniques, `Observable Decoration`_ and `Observer Decoration`_, 
+are static, in the sense, decorations are done e.g. in @-notation evaluated 
+at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the 
 *class constructor*, this means
 
 .. code-block:: python
 
     @Observable
@@ -803,118 +772,200 @@
 .. code-block:: python
 
     class Dog:
         @Observable
         def __init__(self):
             pass                    # Some code ...
 
-But this behavior is insidious.
+But this behavior is insidious, e.g.
+
+.. code-block:: python
+
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+    @Observable(observers=Person)
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 1: Dog is an observable to Person
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe arrived.
+
+The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
 .. warning::
 
     Calling **__init__()** results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
     in not any case this is the desired action...
 
-These previous two techniques can be used to decorate ``@staticmethod`` and 
-``@classmethod`` that are declared and available at compile time. Things are 
-different for instance methods, because instances are not available at 
-compile time. They are not available until class instantiation. Therefore, 
-instance methods are best decorated dynamically in the class constructor.
+So the decoration should not address a class but one (or more) target 
+functions. As already mentioned, this is easy if this callback function 
+is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Hello?"):
+            print(f"Person says {act}")
 
-    class Agent:
         @classmethod
-        def inform(cls, value):
-            print(f"Informed value is: {value}")
+        def action2(cls, act: str = "What's up?"):
+            print(f"Person says {act}")
 
-        def report(self, value):
-            print(f"Reported value is: {value}")
+    @Observable(observers=[Person.action1, Person.action2])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              # Dynamic decoration, static data
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')])(self.modify)
+    # Case 2: Dog is an observable to Person.action
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Person says Hello?
+                                    # Person says What's up?
 
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
+This way, *one action* of ``Dog`` triggers *many actions* at one ``Person``
+(or on each ``Person``).
 
-Each ``Actor`` instance defines its ``modify`` method as an observable, which 
-informs about each change of ``self.a`` both the class method ``Agent.inform`` 
-and the ``Agent().report`` instance method. But at the time of execution of 
-``__init__()`` no (current) values or data are available yet, so only static 
-reporting is possible in this way.
+But often an instance method is more interesting as a callback function.
+If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
+is meant, a decoration like ``@Observable(observers=prs.action)`` 
+can be applied to ``Dog``. And for *any instance* 
+``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
+structures would be possible to submit different parameters.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
 
-    # Case 1: Dynamic decoration, static data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: unknown
-                                    # Reported value is: undefined
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        def action(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
 
-However, the problem can be tackled i.e. adding the attribute
-``activate=Activation.NONE`` to the ``Observable`` definition in 
-``__init__()`` to switch off default ``Activation.AFTER`` and add an 
-individualized dispatch within the ``modify`` method
+    prs1 = Person()                 # Jane Doe arrived.
+    prs2 = Person("John Doe")       # John Doe arrived.
+
+    @Observable(observers=[prs1.action, F(prs2.action, "What's up?")])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 3: Dog is an observable to actions of various person instances.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe says Hello?
+                                    # John Doe says What's up?
+
+This way, *one action* of ``Dog`` triggers *one or many actions* at each 
+of the selected ``Person`` instances. In such situations, a late 
+`dynamic decoration <#dynamic-decoration>`_ of Dog could be a good idea.
+Additionally, in all these cases, for the sake of code clarity, an optional 
+empty decoration ``@Oberserver class Person`` or ``@Oberserver() class Person`` 
+is recommended.
+
+So far, instantiating ``Dog`` resulted in an information with the following 
+action at ``Person``. If ``Dog`` has its own actions that need to be 
+selectively monitored, each of the selected actions can of course be decorated 
+individually as an ``Observable``. For the sake of a better overview, this 
+can also be done on the class itself.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')],
-            # (1) Switch off default activation
-                activate=Activation.NONE)(self.modify)
-
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
-            # (2) Add individual dispatch
-            self.modify.observable.dispatch(value=self.a)
-    
-    # Case 2: Dynamic decoration, dynamic data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: 14
-                                    # Reported value is: 14
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        @classmethod
+        def actionA(cls, act: str = "Hello?"):
+            print(f"Person says {act}")
+
+        def actionB(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
+
+    @Observable(methods=["action1", "action2"],
+                observers=[Person.actionA, Person("Any Doe").actionB])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            self.name = name
+            print(f"Dog {name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Woof!"):
+            print(f"Dog acts {act}")
+
+        def action2(self, act: str = "Brrr!"):
+            print(f"{self.name} acts {act}")
+
+    # Case 4: Dog is an observable with selected actions.
+                                    # Any Doe arrived.
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
     
+    dog.action1()                   # Dog acts Woof!        (@staticmethod)
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+    Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+This last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
+first argument. This works because implicitly the *class method* ``Dog.action2`` 
+was registered. Therefore the call ``dog.action2`` fails because this 
+*instance method* was not registered. But, if this is what is to be achieved, 
+an instance method must first be created and registered, as above.
+
 
-Dynamic Class Decoration 
-------------------------
+Instance Decoration 
+-------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
 ``unregister`` methods that an observable exports. This way, information can 
 be given to the right recipients at the right places in the code. For this, 
-the classes are not decorated. The dynamic decoration comes into play. 
+the classes are not decorated. The `dynamic decoration <#dynamic-decoration>`_ 
+comes into play. 
 
 For this, the classes remain undecorated. Dynamic decoration is used, often 
 also in connection with getter/setter/property constructions, since data 
 changes take place meaningfully over these methods.
 
 Let's start with the simple classes:
 
 .. code-block:: python
 
-    # *** example_observer.py - daynamic class decoration
+    # *** example_observer.py - instance decoration
+
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
         def __init__(self, a=0):
             self._a = a
@@ -926,15 +977,18 @@
             self._a = value
         a = property(get_a, set_a)
 
 Well, some typical actions might be:
 
 .. code-block:: python
 
-    # *** example_observer.py - daynamic class decoration
+    # *** example_observer.py - instance decoration
+
+    from decoratory.observer import Observable
+    from decoratory.basic import F
 
     # (1) Setup instances
     nti = Note()                    # Note instance
     thg = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     thg.inc = Observable(thg.inc)           # Late method decoration   
@@ -958,20 +1012,35 @@
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
     thg.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
     # Case 5: Print the current value of thg.a
     print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
 
-
+    # Case 6: Print list of all observers
+    print(thg.inc.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}   
+    print(thg.set_a.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
+
+    # Case 7: Unregister nti.info from thg
+    thg.inc.observable.unregister(nti.info)
+    print(thg.inc.observable.observers(classbased=True))    # {}
+    
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.2.*, Build: 2023-06-18**
+
+- Intergration of unit tests for modules singleton, multiton and wrapper
+- An overall unit test for the package decoratory
+- Documentation enhancements for module observer, t.b.c.
+
 **Version: 0.1.1.*, Build: 2023-06-16**
 
 - Initial version of the observer, incl. documentation
 
 **Version: 0.1.0.3, Build: 2023-06-15**
 
 - accessible parameter for singleton and multiton, incl. documentation
@@ -982,14 +1051,16 @@
 - Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with singleton, multiton and wrapper
 
 
+~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
```

### Comparing `decoratory-0.1.1.3/Readme.rst` & `decoratory-0.1.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+Metadata-Version: 2.1
+Name: decoratory
+Version: 0.1.2.3
+Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
+Home-page: http://evation.eu
+Download-URL: http://evation.eu
+Author: Martin Abel
+Author-email: Martin Abel <python@evation.eu>
+Maintainer: Martin Abel
+Maintainer-email: Martin Abel <python@evation.eu>
+License: PSF
+Project-URL: Projekt, http://evation.eu
+Project-URL: Release Notes, http://evation.eu
+Project-URL: Download, http://evation.eu
+Keywords: decorator singleton multiton observer observable wrapper
+Platform: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation
+Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: License.txt
+
 
 .. _top:
 
 ==============================================================================
 Decoratory
 ==============================================================================
 
@@ -21,27 +60,32 @@
     pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
+In particular, there is a *comprehensive unit test* for each module, which 
+can be executed from the command line using the ``--test`` option. ::
+
+    python -m decoratory --test
+
 .. _toc:
 
 **Package Contents**
 
 The *decoratory package* available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_ 
 
-This is an open list that possibly will grow over time.
+This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, a simple as well as a
 more complex example is presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
@@ -91,14 +135,16 @@
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Teddy')
     print(f"b = {b}")               # b = Animal('Teddy')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
+.. _dynamic-decoration:
+
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
 code is used, additional parameters can be passed to the decorator for
 passing to the class constructor.
 
 .. code-block:: python
 
@@ -309,15 +355,15 @@
                                     #  True:  Animal('cat', 'Molly')}
 
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
-.. warning::
+.. hint::
 
     Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory, i.e. the directory may then be
     corrupted by such modifications.
 
     Therefore, **never change key related values of classified objects**!
@@ -457,20 +503,21 @@
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
-.. note::
+.. hint::
 
     Decorations to ``@staticmethod`` or ``@classmethod`` can be done
     analogously to the function decorations above, since they already exist
     at compile time. Instance methods, on the other hand, do not exist until
-    an object instance is created and must be handled differently.
+    an object instance is created and must be decorated dynamically as an 
+    instance (e.g. see  `Instance Decoration`_ below).
 
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
@@ -502,16 +549,16 @@
 observed object (observable, publisher, subject).
 
 This implementation provides several ways to decorate a function or class
 as an observable or observer.
 
 * `Observable Decoration`_
 * `Observer Decoration`_
-* `Static Class Decoration`_
-* `Dynamic Class Decoration`_ 
+* `Class Decoration`_
+* `Instance Decoration`_ 
 
 
 Observable Decoration
 ---------------------
 
 The simplest and at the same time the most Pythonic variant of decoration
 is to decorate only the *observed* entities.
@@ -629,17 +676,17 @@
 And again, cat acts before person because of the order of the observer
 list.
 
 
 Observer Decoration 
 -------------------
 
-In this reverse decoration, the observer decorator collects its observables.
-Because an observer decoration uses observable methods, all observable(s)
-must always be declared before their observer(s).
+In this reversed decoration scheme, the observer decorator collects its 
+observables. Because an observer decoration uses observable methods, all 
+observable(s) must always be declared before their observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
 Thus, the initial example ``Case 1`` from above is as follows:
 
 .. code-block:: python
 
@@ -699,15 +746,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Here, the *observed cat* observes the dog, reacts and triggers the person 
-observing the *orignal cat*. This situation reflects the ``Case 2`` from above.
+observing the *original cat*. This situation reflects the ``Case 2`` from above.
 
 To reproduce ``Case 3`` above, simply swap the order of the decorations at the 
 cat and the person then looks at the *observed cat*.
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
@@ -738,20 +785,20 @@
 
 Note the difference: in ``Case 2``, the cat ends up as an ``Observer``, not as 
 an ``Observable``. So the person observes the *original cat*. Whereas in 
 ``case 3``, the cat actually ends up as an ``Observable`` and person can observe 
 the *observed cat*.
 
 
-Static Class Decoration 
------------------------
+Class Decoration 
+----------------
 
-Both techniques, observable and observer decoration, are static, in the sense, 
-decorations are done in @-notation evaluated at compile time. They are applied 
-to *static functions*.
+Both above techniques, `Observable Decoration`_ and `Observer Decoration`_, 
+are static, in the sense, decorations are done e.g. in @-notation evaluated 
+at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the 
 *class constructor*, this means
 
 .. code-block:: python
 
     @Observable
@@ -764,118 +811,200 @@
 .. code-block:: python
 
     class Dog:
         @Observable
         def __init__(self):
             pass                    # Some code ...
 
-But this behavior is insidious.
+But this behavior is insidious, e.g.
+
+.. code-block:: python
+
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+    @Observable(observers=Person)
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 1: Dog is an observable to Person
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe arrived.
+
+The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
 .. warning::
 
     Calling **__init__()** results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
     in not any case this is the desired action...
 
-These previous two techniques can be used to decorate ``@staticmethod`` and 
-``@classmethod`` that are declared and available at compile time. Things are 
-different for instance methods, because instances are not available at 
-compile time. They are not available until class instantiation. Therefore, 
-instance methods are best decorated dynamically in the class constructor.
+So the decoration should not address a class but one (or more) target 
+functions. As already mentioned, this is easy if this callback function 
+is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Hello?"):
+            print(f"Person says {act}")
 
-    class Agent:
         @classmethod
-        def inform(cls, value):
-            print(f"Informed value is: {value}")
+        def action2(cls, act: str = "What's up?"):
+            print(f"Person says {act}")
 
-        def report(self, value):
-            print(f"Reported value is: {value}")
+    @Observable(observers=[Person.action1, Person.action2])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              # Dynamic decoration, static data
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')])(self.modify)
+    # Case 2: Dog is an observable to Person.action
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Person says Hello?
+                                    # Person says What's up?
 
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
+This way, *one action* of ``Dog`` triggers *many actions* at one ``Person``
+(or on each ``Person``).
 
-Each ``Actor`` instance defines its ``modify`` method as an observable, which 
-informs about each change of ``self.a`` both the class method ``Agent.inform`` 
-and the ``Agent().report`` instance method. But at the time of execution of 
-``__init__()`` no (current) values or data are available yet, so only static 
-reporting is possible in this way.
+But often an instance method is more interesting as a callback function.
+If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
+is meant, a decoration like ``@Observable(observers=prs.action)`` 
+can be applied to ``Dog``. And for *any instance* 
+``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
+structures would be possible to submit different parameters.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
 
-    # Case 1: Dynamic decoration, static data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: unknown
-                                    # Reported value is: undefined
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        def action(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
 
-However, the problem can be tackled i.e. adding the attribute
-``activate=Activation.NONE`` to the ``Observable`` definition in 
-``__init__()`` to switch off default ``Activation.AFTER`` and add an 
-individualized dispatch within the ``modify`` method
+    prs1 = Person()                 # Jane Doe arrived.
+    prs2 = Person("John Doe")       # John Doe arrived.
+
+    @Observable(observers=[prs1.action, F(prs2.action, "What's up?")])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 3: Dog is an observable to actions of various person instances.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe says Hello?
+                                    # John Doe says What's up?
+
+This way, *one action* of ``Dog`` triggers *one or many actions* at each 
+of the selected ``Person`` instances. In such situations, a late 
+`dynamic decoration <#dynamic-decoration>`_ of Dog could be a good idea.
+Additionally, in all these cases, for the sake of code clarity, an optional 
+empty decoration ``@Oberserver class Person`` or ``@Oberserver() class Person`` 
+is recommended.
+
+So far, instantiating ``Dog`` resulted in an information with the following 
+action at ``Person``. If ``Dog`` has its own actions that need to be 
+selectively monitored, each of the selected actions can of course be decorated 
+individually as an ``Observable``. For the sake of a better overview, this 
+can also be done on the class itself.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')],
-            # (1) Switch off default activation
-                activate=Activation.NONE)(self.modify)
-
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
-            # (2) Add individual dispatch
-            self.modify.observable.dispatch(value=self.a)
-    
-    # Case 2: Dynamic decoration, dynamic data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: 14
-                                    # Reported value is: 14
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        @classmethod
+        def actionA(cls, act: str = "Hello?"):
+            print(f"Person says {act}")
+
+        def actionB(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
+
+    @Observable(methods=["action1", "action2"],
+                observers=[Person.actionA, Person("Any Doe").actionB])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            self.name = name
+            print(f"Dog {name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Woof!"):
+            print(f"Dog acts {act}")
+
+        def action2(self, act: str = "Brrr!"):
+            print(f"{self.name} acts {act}")
+
+    # Case 4: Dog is an observable with selected actions.
+                                    # Any Doe arrived.
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
     
+    dog.action1()                   # Dog acts Woof!        (@staticmethod)
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+    Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+This last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
+first argument. This works because implicitly the *class method* ``Dog.action2`` 
+was registered. Therefore the call ``dog.action2`` fails because this 
+*instance method* was not registered. But, if this is what is to be achieved, 
+an instance method must first be created and registered, as above.
+
 
-Dynamic Class Decoration 
-------------------------
+Instance Decoration 
+-------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
 ``unregister`` methods that an observable exports. This way, information can 
 be given to the right recipients at the right places in the code. For this, 
-the classes are not decorated. The dynamic decoration comes into play. 
+the classes are not decorated. The `dynamic decoration <#dynamic-decoration>`_ 
+comes into play. 
 
 For this, the classes remain undecorated. Dynamic decoration is used, often 
 also in connection with getter/setter/property constructions, since data 
 changes take place meaningfully over these methods.
 
 Let's start with the simple classes:
 
 .. code-block:: python
 
-    # *** example_observer.py - daynamic class decoration
+    # *** example_observer.py - instance decoration
+
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
         def __init__(self, a=0):
             self._a = a
@@ -887,15 +1016,18 @@
             self._a = value
         a = property(get_a, set_a)
 
 Well, some typical actions might be:
 
 .. code-block:: python
 
-    # *** example_observer.py - daynamic class decoration
+    # *** example_observer.py - instance decoration
+
+    from decoratory.observer import Observable
+    from decoratory.basic import F
 
     # (1) Setup instances
     nti = Note()                    # Note instance
     thg = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     thg.inc = Observable(thg.inc)           # Late method decoration   
@@ -919,20 +1051,35 @@
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
     thg.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
     # Case 5: Print the current value of thg.a
     print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
 
-
+    # Case 6: Print list of all observers
+    print(thg.inc.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}   
+    print(thg.set_a.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
+
+    # Case 7: Unregister nti.info from thg
+    thg.inc.observable.unregister(nti.info)
+    print(thg.inc.observable.observers(classbased=True))    # {}
+    
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.2.*, Build: 2023-06-18**
+
+- Intergration of unit tests for modules singleton, multiton and wrapper
+- An overall unit test for the package decoratory
+- Documentation enhancements for module observer, t.b.c.
+
 **Version: 0.1.1.*, Build: 2023-06-16**
 
 - Initial version of the observer, incl. documentation
 
 **Version: 0.1.0.3, Build: 2023-06-15**
 
 - accessible parameter for singleton and multiton, incl. documentation
@@ -943,14 +1090,16 @@
 - Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with singleton, multiton and wrapper
 
 
+~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
```

### Comparing `decoratory-0.1.1.3/Sources/decoratory/__main__.py` & `decoratory-0.1.2.3/Sources/decoratory/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,26 +13,30 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.1.3"
-__date__ = "2023-06-16"
-__time__ = "20:01:41"
+__version__ = "0.1.2.3"
+__date__ = "2023-06-18"
+__time__ = "19:22:40"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
+import unittest
+
 from sys import argv
-from os.path import dirname, join
+from os.path import dirname, join, basename
+from glob import glob
+from importlib import import_module
 
 # -----------------------------------------------------------------------------
 # Parameters
 module = __title__.lower()
 name = __title__.capitalize()
 
 
@@ -55,14 +59,28 @@
                       "r") as f:
                 txt = f.read()
             print("\n" + txt)
         except (FileNotFoundError, Exception):
             print("*** No additional data accessible. "
                   f"Please look for file 'License.txt' ***".center(79, " "))
         print(f"{'-' * 79}")
+    elif arg in "--test":
+        try:
+            print(f"\n{'-' * 70}")
+            print(f" Running unit tests for all modules ".center(70, '-'))
+            print(f"{'-' * 70}\n")
+            loader = unittest.TestLoader().loadTestsFromModule
+            for mdl in glob(join(dirname(__file__), "tests", "test_*.py")):
+                mdl = basename(mdl)[:-3].lower()
+                print(f"\n{' ' + mdl + ' ' :-^70s}\n")
+                mdl = import_module(f"decoratory.tests.{mdl}")
+                suite = loader(mdl)
+                unittest.TextTestRunner(verbosity=2).run(suite)
+        except (ModuleNotFoundError, ImportError, Exception) as ex:
+            print(ex)
     elif arg in "--information":
         print(f"\nPeople and contact information for package {module}:\n")
         print(f"Author    : {__author__}")
         print(f"Maintainer: {__maintainer__}")
         print(f"Company   : {__company__}")
         print(f"Email     : {__email__}")
         print(f"Web       : {__url__}")
@@ -100,14 +118,15 @@
 Possible options are:
 
   -h, --help            show this help message
   -v, --version         show {module}[.module] version information      
   -c, --copyright       show {module}[.module] copyright statement
   -l, --license         show {module}[.module] license statement (License.txt)
       --licence         an alias to --license
+  -t, --test            run unit tests for {module}[.module]
   -i, --info            people and contact information
 
 Example: Display license statement for the multiton module:
 
 {'python -m decoratory.multiton --license': ^79s}
          
 -------------------------------------------------------------------------------
```

### Comparing `decoratory-0.1.1.3/Sources/decoratory/banner.py` & `decoratory-0.1.2.3/Sources/decoratory/banner.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.1.1"
-__date__ = "2023-06-16"
-__time__ = "09:40:57"
+__version__ = "0.1.2.21"
+__date__ = "2023-06-18"
+__time__ = "13:48:16"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
+import unittest
+
 from sys import argv
 from os.path import dirname, join
+from importlib import import_module
 
 
 # -----------------------------------------------------------------------------
 # Banner Display
 def __banner(title, version, date, time, docs,
              author: str = __author__,
              maintainer: str = __maintainer__,
@@ -78,14 +81,25 @@
     elif arg in "--information":
         print(f"\nPeople and contact information for module {module}:\n")
         print(f"Author    : {author}")
         print(f"Maintainer: {maintainer}")
         print(f"Company   : {company}")
         print(f"Email     : {email}")
         print(f"Web       : {url}")
+    elif arg in "--test":
+        try:
+            print(f"\n{'-' * 70}")
+            print(f" Running unit test for module: {module} ".center(70, '-'))
+            print(f"{'-' * 70}\n")
+            loader = unittest.TestLoader().loadTestsFromModule
+            mdl = import_module(f"decoratory.tests.test_{module.lower()}")
+            suite = loader(mdl)
+            unittest.TextTestRunner(verbosity=2).run(suite)
+        except (ModuleNotFoundError, ImportError, Exception) as ex:
+            print(ex)
     else:
         print(f"""
 -------------------------------------------------------------------------------
 {title.upper(): ^79}
 -------------------------------------------------------------------------------
 
 {module} is a Python module you cannot execute directly from command line.
@@ -107,14 +121,15 @@
 
   -h, --help            show this help message
   -v, --version         show module {module} version information      
   -c, --copyright       show module {module} copyright statement
   -l, --license         show module {module} license statement (License.txt)
       --licence         an alias to --license
   -d, --documentation   display selected module code documentation
+  -t, --test            run unit test for module {module}
   -i, --info            people and contact information
 
 -------------------------------------------------------------------------------
 {copyright: <69s}{date: >10s}
 -------------------------------------------------------------------------------
 """)
```

### Comparing `decoratory-0.1.1.3/Sources/decoratory/basic.py` & `decoratory-0.1.2.3/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.1.1"
-__date__ = "2023-06-16"
-__time__ = "09:40:57"
+__version__ = "0.1.2.1"
+__date__ = "2023-06-17"
+__time__ = "11:30:04"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.1.3/Sources/decoratory/observer.py` & `decoratory-0.1.2.3/Sources/decoratory/observer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 #!/usr/bin/env python
 # -*- coding=UTF-8 -*-
 # vim: fileencoding=UTF-8 tabstop=8 expandtab shiftwidth=4 softtabstop=4
 # -----------------------------------------------------------------------------
 # Document Description
-"""**Observer Pattern**
+"""**Observer**
 
     The observer pattern is generally used to inform one or more registered
     objects (observers, subscribers, objects) about selected actions of an
     observed object (observable, publisher, subject).
 
     This implementation provides several ways to decorate a function or class
     as an Observable or Observer.
 
     Attributes
     ----------
-        None.
-
-    Methods
-    -------
-    seal(self):
-        Seal multiton.
+    Observer (class):                           (uses BaseObserver)
+        Creates an observer instance as a callable object.
 
-    unseal(self):
-        Unseal multiton.
+    Observable (class):                         (uses BaseObservable)
+        Creates an observable callable object exposing the pattern interface.
 
-    issealed(self):
-        Multiton sealing state
+    BaseObserver (class):                       (for inheritance, only)
+        A base implementation of the (abstract) observer base class.
 
-    get_instance():
-        Return the singleton instance.  (if accessible=True)
+    BaseObservable (class):                     (for inheritance, only)
+        A base implementation of the (abstract) observable base class.
 
-    reset():
-        Resets the singleton instance.  (if resettable=True)
-
-    Example
+    Methods
     -------
+        None.
+
+    Examples
+    --------
 
     A) Observable Decoration
 
     The simplest and at the same time the most Pythonic variant of decoration
     is to decorate only the *observed* entities. This is possible because all
     observer pattern functionalities are concentrated in the BaseClass
     (=BaseObservable) of the observable decorator, while the BaseClass
@@ -191,15 +188,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
     Here, the observed cat observes the dog, reacts and triggers the person
-    observing the orignal cat. This situation reflects the Case 2 from above.
+    observing the original cat. This situation reflects the Case 2 from above.
 
     To reproduce Case 3 above, simply swap the order of the decorations at the
     cat and the person then looks at the observed cat.
 
     @Observable                     # 2. Rule: dog before cat, person
     def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
         print(f"{dog.__name__} acts '{act}'")
@@ -259,14 +256,17 @@
 
     These previous two techniques can be used to decorate @staticmethod and
     @classmethod that are declared and available at compile time. Things are
     different for instance methods, because instances are not available at
     compile time. They are not available until class instantiation. Therefore,
     instance methods are best decorated dynamically in the class constructor.
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     class Agent:
         @classmethod
         def inform(cls, value):
             print(f"Informed value is: {value}")
 
         def report(self, value):
             print(f"Reported value is: {value}")
@@ -296,14 +296,17 @@
                                     # Reported value is: undefined
 
     However, the problem can be tackled i.e. adding the attribute
     activate=Activation.NONE to the Observable definition in __init__ to
     switch off default Activation.AFTER and add an individualized dispatch
     within the modify method
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F, Activation
+
     class Actor:
         def __init__(self):
             self.a = 1
             print(f"Initialization: a = {self.a}")
             self.modify = Observable(observers=[
                 F(Agent.inform, 'unknown'),
                 F(Agent().report, 'undefined')],
@@ -350,14 +353,17 @@
             return self._a
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
     Well, some typical actions might be:
 
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
     # (1) Setup instances
     nti = Note()                    # Note instance
     thg = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     thg.inc = Observable(thg.inc)           # Late method decoration
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration
@@ -379,31 +385,41 @@
 
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
     thg.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
     # Case 5: Print the current value of thg.a
     print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
+
+    # Case 6: Print list of all observers
+    print(thg.inc.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}
+    print(thg.set_a.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
+
+    # Case 7: Unregister nti.info from thg
+    thg.inc.observable.unregister(nti.info)
+    print(thg.inc.observable.observers(classbased=True))    # {}
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Observer"
 __module__ = "observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.1.2"
-__date__ = "2023-06-16"
-__time__ = "19:56:14"
+__version__ = "0.1.2.11"
+__date__ = "2023-06-18"
+__time__ = "19:18:48"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -411,15 +427,15 @@
 from typing import Union
 from decoratory.basic import Activation, F, Parser, X
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class BaseObservable:
-    """**Observable Base Class**
+    """**BaseObservable**
 
     A base implementation of the (abstract) observable base class. It manages
     (abstract) observers (of F-type) within a private dictionary using the
     methods:
 
     register  : Register an observer for callback
     unregister: Unregister an observer
@@ -520,16 +536,21 @@
             if observer_args or observer_kwargs:
                 F(observer.callee, *observer_args, **observer_kwargs).eval()
             else:
                 observer.eval()
         elif callable(observer):
             # Dynamic call using current arguments, no extra eval obj!
             F(observer, *observer_args, **observer_kwargs).eval()
-        elif isinstance(observer, str):
-            pass  # todo: str???
+        elif observer in self.__observers:
+            # Try to resolve the string or something else...
+            observer = self.__observers.get(observer)
+            if observer_args or observer_kwargs:
+                F(observer.callee, *observer_args, **observer_kwargs).eval()
+            else:
+                observer.eval()
         else:
             raise TypeError(f"'{observer}' cannot be dispatched.")
 
     def observers(self, classbased=False) -> dict:
         """Listing of all observers.
 
         Observers are collected in a dict, which is returned by default with
@@ -542,29 +563,49 @@
         Returns:
             observers (dict): Dictionary of all observers
         """
         if bool(classbased):
             result = dict()
             for obs in self.__observers.values():
                 *skip, cls, mtd = obs.callee.__qualname__.split(".")
-                result.setdefault(cls, []).append(obs)
+                result.setdefault(cls, []).append(repr(obs))
             return result
         else:
             return self.__observers  # Has to be the default (without params)!
 
 
 class Observable:
     """**Observable** (Publisher, Subject)
 
     Creating an observable instantiates a callable object which exposes the
     four basic observable pattern methods register, unregister, dispatch and
     observers via an observable attribute for an instance of BaseClass
     (default = BaseObservable) as well as the original decorator arguments,
     if present, like the callable to be substituted, observers, methods and
     activation point in time.
+
+    Observable(substitute, *args, observers, methods, activate, **kwargs)
+
+    Attributes
+    ----------
+    substitute (callable|type):
+        A type to be made an observable
+
+    observers (list|F|callable|str):
+        (List of) callable(s) of observers
+
+    methods (list|F|callable|str):
+        (List of) callable(s) of as method name strings
+
+    activate (Activation):
+        Dispatch activation point in time
+
+    Methods
+    -------
+        None.
     """
 
     BaseClass = BaseObservable
 
     def __init__(self,
                  substitute: Union[callable, type] = None,
                  *args: object,
@@ -723,15 +764,15 @@
         self.__activate = activate if isinstance(
             activate, Activation) else Activation.NONE
 
     activate = property(__get__activate, __set__activate)
 
 
 class BaseObserver:
-    """**Observer Base Class**
+    """**BaseObserver**
 
     A base implementation of the (abstract) observer base class.
 
     As long as this class, just like here, is an empty dummy, decoration of a
     callable as an observer is optional. If BaseObserver is overwritten and
     assigned to the observers BaseClass attribute all non captured decorator
     args & kwargs will be submitted to be used in customized class
@@ -745,31 +786,51 @@
 
 class Observer:
     """**Observer** (Subscriber, Object)
 
     Creating an observer instantiates a callable object which exposes the
     original decorator arguments, if present, like the callable to be
     substituted, observables and methods.
+
+    Observer(substitute, *args, observables, methods, **kwargs)
+
+    Attributes
+    ----------
+    substitute (callable|type):
+        A type to be made an observer
+
+    observables (list|X|callable|str):
+        (List of) callable(s) of observables
+
+    methods (list|X|callable|str):
+        (List of) callable(s) of as method name strings
+
+    Methods
+    -------
+        None.
    """
 
     BaseClass = BaseObserver
 
     def __init__(self,
                  substitute: Union[callable, type] = None,
                  *args: object,
                  observables: Union[list, X, callable, str] = None,
                  methods: Union[list, X, callable, str] = None,
                  **kwargs: object) -> None:
         """**Observer** (Subscriber, Object)
 
-        @param substitute: The callable or type to be made an observable
-        @param observables: (List of) callable(s) of observables
-        @param methods: (List of) callable(s) of method strings
-        @rtype: NoneType
-            """
+        Parameters:
+            substitute (callable|type: Callable|Type to be made an observable
+            observables (list|X|callable|str): (List of) callable(s) of observables
+            methods (list|X|callable|str): (List of) callable(s) of as strings
+
+        Returns:
+            None.
+        """
         self.__set__substitute(substitute)
         self.__set__observables(observables)
         self.__set__methods(methods)
 
         # --- Decorator Arguments Pattern (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
@@ -898,125 +959,22 @@
     observer = property(__get__observer)
 
 
 # -----------------------------------------------------------------------------
 # Simple example
 if __name__ == '__main__':
     from decoratory.banner import __banner as banner
+    import decoratory.observer as module
 
     banner(title=__title__,
            version=__version__,
            date=__date__,
            time=__time__,
-           docs=(BaseObserver, Observer, BaseObservable, Observable),
+           docs=(module, Observer, Observable, BaseObserver, BaseObservable),
            author=__author__,
            maintainer=__maintainer__,
            company=__company__,
            email=__email__,
            url=__url__,
            copyright=__copyright__,
            state=__state__,
            license=__license__)
-
-
-    #
-    # def __test03():
-    #     # ---------------------------------------------------------------------
-    #     # Class decoration (dynamic)
-    #     class DftFormatter:
-    #         """Default Formatter"""
-    #
-    #         def __init__(self, name):
-    #             self.name = name
-    #             self._data = 0
-    #             print(f"{self.__class__.__name__}: "
-    #                   f"{self.name} has data {self._data}")
-    #
-    #         def __str__(self):
-    #             return f"{self.__class__.__name__}({self.name}, {self._data})"
-    #
-    #         def get_data(self):
-    #             """Getter"""
-    #             return self._data
-    #
-    #         def set_data(self, value):
-    #             self._data = value
-    #
-    #         data = property(get_data, set_data)
-    #
-    #     class HexFormatter(DftFormatter):
-    #         """Hex Formatter"""
-    #
-    #         def notify(self, resource):
-    #             """Notifier"""
-    #             value = hex(resource.data)
-    #             print(f"{self.__class__.__name__}: "
-    #                   f"{resource.name} has data {value}")
-    #
-    #     class BinFormatter(DftFormatter):
-    #         """Binary Formatter"""
-    #
-    #         def notify(self, resource):
-    #             """Notifier"""
-    #             value = bin(resource.data)
-    #             print(f"{self.__class__.__name__}: "
-    #                   f"{resource.name} has data {value}")
-    #
-    #     # Instances
-    #     print("Instantiation:")
-    #     df = DftFormatter('Dfter')
-    #     hf = HexFormatter('Hexer')
-    #     bf = BinFormatter('Biner')
-    #
-    #     # Setup Observable for a property
-    #     DftFormatter.set_data = Observable(DftFormatter.set_data)
-    #     DftFormatter.data = property(DftFormatter.get_data,
-    #                                  DftFormatter.set_data)
-    #
-    #     hf.notify = Observer(hf.notify)  # Optional
-    #     bf.notify = Observer(bf.notify)  # Optional
-    #
-    #     # noinspection PyTypeHints
-    #     df.set_data: Observable
-    #
-    #     # Register Observer with default resource argument
-    #     df.set_data.observable.register(F(hf.notify, df))
-    #     df.set_data.observable.register(F(bf.notify, resource=df))
-    #
-    #     # Change data using the property
-    #     print("\nChange data: 2")
-    #     df.data = 2
-    #
-    #     # Some additional dispatches
-    #     print("\nAdditional dispatches: df, bf, all(2)")
-    #     df.set_data.observable.dispatch(hf.notify, df)
-    #     df.set_data.observable.dispatch(BinFormatter.notify, bf, df)
-    #     print()
-    #     df.set_data.observable.dispatch(resource=df)
-    #
-    #     # List all observers
-    #     print("\nList all observers:")
-    #     print(df.set_data.observable.observers())
-    #     print(df.set_data.observable.observers(classbased=True))
-    #
-    #     # Unregister bf
-    #     print("\nUnregister bf:")
-    #     df.set_data.observable.unregister(bf.notify)
-    #     print(df.set_data.observable.observers())
-    #
-    #     # Unregister all
-    #     print("\nUnregister all:")
-    #     df.set_data.observable.unregister()
-    #     print(df.set_data.observable.observers())
-    #
-    #
-    # # -------------------------------------------------------------------------
-    # # Apply tests
-    # print("----------")
-    # __test01()
-
-    # print("----------")
-    # __test02()
-    # print("----------")
-    # __test03()
-    # print("----------")
-
```

### Comparing `decoratory-0.1.1.3/Sources/decoratory/wrapper.py` & `decoratory-0.1.2.3/Sources/decoratory/wrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,37 +14,28 @@
 
      - (optional) replace call functionality.
 
     All three decorator parameters, before, after and replace, can be combined
     with each other and support both single callables and (nested) lists of
     F-types (imported from module decoratory.basic, see below for details).
     In addition, replace supports passing results from successive replacement
-    calls through an optional keyword argument named result (defaut value is
+    calls through an optional keyword argument named result (default value is
     None).
 
     Attributes
     ----------
-    substitute: object (getter property)
-        A type to be made a multiton.
-
-    before: callable or list (getter property)
-        (List of) callable(s) to be executed before substitute.
-
-    replace: callable or list (getter property)
-        (List of) callable(s) replacing the substitute.
-
-    after: callable or list (getter property)
-        (List of) callable(s) to be executed after substitute.
+    Wrapper (class):
+        Creates a wrapper instance as a callable object.
 
     Methods
     -------
         None.
 
-    Example
-    -------
+    Examples
+    --------
 
     from decoratory.wrapper import Wrapper
     from decoratory.basic import F
 
     # Case 1: Dynamic decoration with decorator arguments, only
     def some_function(value: str = "original"):
         print(f"value = '{value}'")
@@ -125,17 +116,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.1.1"
-__date__ = "2023-06-16"
-__time__ = "09:40:57"
+__version__ = "0.1.2.5"
+__date__ = "2023-06-17"
+__time__ = "13:25:04"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -144,124 +135,33 @@
 
 
 # -----------------------------------------------------------------------------
 # Classes
 class Wrapper:
     """**Wrapper**
 
-    A wrapper encloses the original function with an
-
-     - (optional) before call functionality, and/or
-     - (optional) after  call functionality, and/or
-
-    substitutes the original functionality with an
-
-     - (optional) replace call functionality.
-
-    All three decorator parameters, before, after and replace, can be combined
-    with each other and support both single callables and (nested) lists of
-    F-types (imported from module decoratory.basic, see below for details).
-    In addition, replace supports passing results from successive replacement
-    calls through an optional keyword argument named result (defaut value is
-    None).
+    Wrapper(substitute, *args, before, replace, after, **kwargs)
 
     Attributes
     ----------
-    substitute: object (getter property)
-        A type to be made a multiton.
+    substitute (callable|type):
+        A type to be made a wrapper
 
-    before: callable or list (getter property)
-        (List of) callable(s) to be executed before substitute.
+    before (callable|list):
+        (List of) callable(s) to be executed before substitute
 
-    replace: callable or list (getter property)
-        (List of) callable(s) replacing the substitute.
+    replace (callable|list):
+        (List of) callable(s) replacing the substitute
 
-    after: callable or list (getter property)
-        (List of) callable(s) to be executed after substitute.
+    after (callable|list):
+        (List of) callable(s) to be executed after substitute
 
     Methods
     -------
         None.
-
-    Example
-    -------
-
-    from decoratory.wrapper import Wrapper
-    from decoratory.basic import F
-
-    # Case 1: Dynamic decoration with decorator arguments, only
-    def some_function(value: str = "original"):
-        print(f"value = '{value}'")
-
-    some_function()                 # value = 'original'
-    some_function = Wrapper(some_function, value="changed")
-    some_function()                 # value = 'changed'
-
-    # Case 2: Static decoration with before and after functionalities
-    def print_message(message: str = "ENTER"):
-        print(message)
-
-    @Wrapper(before=print_message, after=F(print_message, "LEAVE"))
-    def some_function(value: str = "original"):
-        print(f"value = '{value}'")
-
-    # Function call with decoration: before and after
-    some_function()                 # ENTER
-                                    # value = 'original'
-                                    # LEAVE
-
-    # Case 3: Decoration with before, after and multiple replacements
-    def print_message(message: str = "BEFORE"):
-        print(message)
-
-    def replacement_printer(add: int = 1, *, result=None):
-        result += add if isinstance(result, int) else 0
-        print(f"result = {result}")
-        return result
-
-    @Wrapper(before=F(print_message, "ENTER"),
-             replace=[F(replacement_printer, 1, result=0),
-                      F(replacement_printer, 3),
-                      F(replacement_printer, 5)],
-             after=F(print_message, "LEAVE"))
-    def default_printer(message: str = "DEFAULT"):
-        print(message)
-
-    # Function call with decoration: before, after and replacement
-    default_printer()               # ENTER         (before)
-                                    # result = 1    (replacement_printer, 1)
-                                    # result = 4    (replacement_printer, 3)
-                                    # result = 9    (replacement_printer, 5)
-                                    # LEAVE         (after)
-                                    # 9             (output default_printer)
-
-    # Case 4: Decoration of a class always refers to __init__
-    @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
-    class Animal:
-        def __init__(self, name):
-            self.name = name
-            print("RUNNING init")
-
-    a = Animal(name='Teddy')        # BEFORE init
-                                    # RUNNING init
-                                    # AFTER init
-
-    # Case 5: Define a private wrapper library
-    before_wrapper = Wrapper(before=F(print, "BEFORE"))
-    after_wrapper = Wrapper(after=F(print, "AFTER"))
-
-    # Multiple decorations for specialized functionality encapsulation
-    @before_wrapper
-    @after_wrapper
-    def some_function(value: str = "original"):
-        print(f"value = '{value}'")
-
-    some_function()                 # BEFORE
-                                    # value = 'original'
-                                    # AFTER
     """
 
     def __init__(self,
                  substitute: callable or type = None,
                  *args: object,
                  before: callable or list = None,
                  replace: callable or list = None,
@@ -367,21 +267,22 @@
 
     after = property(__get__after)
 
 
 # -----------------------------------------------------------------------------
 # Simple example
 if __name__ == '__main__':
+    import decoratory.wrapper as module
     from decoratory.banner import __banner as banner
 
     banner(title=__title__,
            version=__version__,
            date=__date__,
            time=__time__,
-           docs=(Wrapper,),
+           docs=(module, Wrapper),
            author=__author__,
            maintainer=__maintainer__,
            company=__company__,
            email=__email__,
            url=__url__,
            copyright=__copyright__,
            state=__state__,
```

### Comparing `decoratory-0.1.1.3/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.1.2.3/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.1.3
+Version: 0.1.2.3
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -60,27 +60,32 @@
     pip install --upgrade decoratory
 
 After installation, basic information about the package, the individual
 modules and their methods is also available from the command line. ::
 
     python -m decoratory --help
 
+In particular, there is a *comprehensive unit test* for each module, which 
+can be executed from the command line using the ``--test`` option. ::
+
+    python -m decoratory --test
+
 .. _toc:
 
 **Package Contents**
 
 The *decoratory package* available here includes some classic decorators
 implemented and functionally extended with this concept, e.g.
 
 * `Singleton`_
 * `Multiton`_
 * `Wrapper`_
 * `Observer`_ 
 
-This is an open list that possibly will grow over time.
+This is an open list of modules that possibly will grow over time.
 
 
 **Description**
 
 To illustrate the functionality of each module, a simple as well as a
 more complex example is presented. Even if only one particular module
 is needed, it is recommended to view the preceding examples as well. For even
@@ -130,14 +135,16 @@
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     print(f"a = {a}")               # a = Animal('Teddy')
     print(f"b = {b}")               # b = Animal('Teddy')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
+.. _dynamic-decoration:
+
 If instead of the above *static decoration* using pie-notation, i.e. with
 @-notation at the class declaration, the *dynamic decoration* within Python
 code is used, additional parameters can be passed to the decorator for
 passing to the class constructor.
 
 .. code-block:: python
 
@@ -348,15 +355,15 @@
                                     #  True:  Animal('cat', 'Molly')}
 
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
 
-.. warning::
+.. hint::
 
     Classifications into the multiton directory are done only once on
     initial key data. Subsequent changes affecting a key value are not
     reflected in the multiton directory, i.e. the directory may then be
     corrupted by such modifications.
 
     Therefore, **never change key related values of classified objects**!
@@ -496,20 +503,21 @@
     a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
 
 For all other methods applies:
 
-.. note::
+.. hint::
 
     Decorations to ``@staticmethod`` or ``@classmethod`` can be done
     analogously to the function decorations above, since they already exist
     at compile time. Instance methods, on the other hand, do not exist until
-    an object instance is created and must be handled differently.
+    an object instance is created and must be decorated dynamically as an 
+    instance (e.g. see  `Instance Decoration`_ below).
 
 With ``Wrapper`` and custom service functions, a *private wrapper library*
 can be built and reused.
 
 .. code-block:: python
 
     # *** example_wrapper.py - private wrapper library
@@ -541,16 +549,16 @@
 observed object (observable, publisher, subject).
 
 This implementation provides several ways to decorate a function or class
 as an observable or observer.
 
 * `Observable Decoration`_
 * `Observer Decoration`_
-* `Static Class Decoration`_
-* `Dynamic Class Decoration`_ 
+* `Class Decoration`_
+* `Instance Decoration`_ 
 
 
 Observable Decoration
 ---------------------
 
 The simplest and at the same time the most Pythonic variant of decoration
 is to decorate only the *observed* entities.
@@ -668,17 +676,17 @@
 And again, cat acts before person because of the order of the observer
 list.
 
 
 Observer Decoration 
 -------------------
 
-In this reverse decoration, the observer decorator collects its observables.
-Because an observer decoration uses observable methods, all observable(s)
-must always be declared before their observer(s).
+In this reversed decoration scheme, the observer decorator collects its 
+observables. Because an observer decoration uses observable methods, all 
+observable(s) must always be declared before their observer(s).
 
     **1. Rule:** Declare *Observables before Observers*
 
 Thus, the initial example ``Case 1`` from above is as follows:
 
 .. code-block:: python
 
@@ -738,15 +746,15 @@
 
     dog()                           # dog acts 'Woof!'        (dog acting)
                                     # cat acts 'Roar!'        (observer to dog)
                                     # person says 'Hey, cat!' (observer to cat)
                                     # person says 'Hey, dog!' (observer to dog)
 
 Here, the *observed cat* observes the dog, reacts and triggers the person 
-observing the *orignal cat*. This situation reflects the ``Case 2`` from above.
+observing the *original cat*. This situation reflects the ``Case 2`` from above.
 
 To reproduce ``Case 3`` above, simply swap the order of the decorations at the 
 cat and the person then looks at the *observed cat*.
 
 .. code-block:: python
 
     # *** example_observer.py - observer decoration
@@ -777,20 +785,20 @@
 
 Note the difference: in ``Case 2``, the cat ends up as an ``Observer``, not as 
 an ``Observable``. So the person observes the *original cat*. Whereas in 
 ``case 3``, the cat actually ends up as an ``Observable`` and person can observe 
 the *observed cat*.
 
 
-Static Class Decoration 
------------------------
+Class Decoration 
+----------------
 
-Both techniques, observable and observer decoration, are static, in the sense, 
-decorations are done in @-notation evaluated at compile time. They are applied 
-to *static functions*.
+Both above techniques, `Observable Decoration`_ and `Observer Decoration`_, 
+are static, in the sense, decorations are done e.g. in @-notation evaluated 
+at compile time. They are applied to *static functions*.
 
 *Decoration of a class* by default addresses decoration of the 
 *class constructor*, this means
 
 .. code-block:: python
 
     @Observable
@@ -803,118 +811,200 @@
 .. code-block:: python
 
     class Dog:
         @Observable
         def __init__(self):
             pass                    # Some code ...
 
-But this behavior is insidious.
+But this behavior is insidious, e.g.
+
+.. code-block:: python
+
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+    @Observable(observers=Person)
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 1: Dog is an observable to Person
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe arrived.
+
+The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
 .. warning::
 
     Calling **__init__()** results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
     in not any case this is the desired action...
 
-These previous two techniques can be used to decorate ``@staticmethod`` and 
-``@classmethod`` that are declared and available at compile time. Things are 
-different for instance methods, because instances are not available at 
-compile time. They are not available until class instantiation. Therefore, 
-instance methods are best decorated dynamically in the class constructor.
+So the decoration should not address a class but one (or more) target 
+functions. As already mentioned, this is easy if this callback function 
+is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            print(f"{name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Hello?"):
+            print(f"Person says {act}")
 
-    class Agent:
         @classmethod
-        def inform(cls, value):
-            print(f"Informed value is: {value}")
+        def action2(cls, act: str = "What's up?"):
+            print(f"Person says {act}")
 
-        def report(self, value):
-            print(f"Reported value is: {value}")
+    @Observable(observers=[Person.action1, Person.action2])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              # Dynamic decoration, static data
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')])(self.modify)
+    # Case 2: Dog is an observable to Person.action
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Person says Hello?
+                                    # Person says What's up?
 
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
+This way, *one action* of ``Dog`` triggers *many actions* at one ``Person``
+(or on each ``Person``).
 
-Each ``Actor`` instance defines its ``modify`` method as an observable, which 
-informs about each change of ``self.a`` both the class method ``Agent.inform`` 
-and the ``Agent().report`` instance method. But at the time of execution of 
-``__init__()`` no (current) values or data are available yet, so only static 
-reporting is possible in this way.
+But often an instance method is more interesting as a callback function.
+If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
+is meant, a decoration like ``@Observable(observers=prs.action)`` 
+can be applied to ``Dog``. And for *any instance* 
+``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
+structures would be possible to submit different parameters.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
+
+    from decoratory.observer import Observable
+    from decoratory.basic import F
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        def action(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
 
-    # Case 1: Dynamic decoration, static data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: unknown
-                                    # Reported value is: undefined
+    prs1 = Person()                 # Jane Doe arrived.
+    prs2 = Person("John Doe")       # John Doe arrived.
 
-However, the problem can be tackled i.e. adding the attribute
-``activate=Activation.NONE`` to the ``Observable`` definition in 
-``__init__()`` to switch off default ``Activation.AFTER`` and add an 
-individualized dispatch within the ``modify`` method
+    @Observable(observers=[prs1.action, F(prs2.action, "What's up?")])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            print(f"Dog {name} arrived.")
+
+    # Case 3: Dog is an observable to actions of various person instances.
+    dog = Dog()                     # Dog Teddy arrived.
+                                    # Jane Doe says Hello?
+                                    # John Doe says What's up?
+
+This way, *one action* of ``Dog`` triggers *one or many actions* at each 
+of the selected ``Person`` instances. In such situations, a late 
+`dynamic decoration <#dynamic-decoration>`_ of Dog could be a good idea.
+Additionally, in all these cases, for the sake of code clarity, an optional 
+empty decoration ``@Oberserver class Person`` or ``@Oberserver() class Person`` 
+is recommended.
+
+So far, instantiating ``Dog`` resulted in an information with the following 
+action at ``Person``. If ``Dog`` has its own actions that need to be 
+selectively monitored, each of the selected actions can of course be decorated 
+individually as an ``Observable``. For the sake of a better overview, this 
+can also be done on the class itself.
 
 .. code-block:: python
 
-    # *** example_observer.py - static class decoration
+    # *** example_observer.py - class decoration
 
-    class Actor:
-        def __init__(self):
-            self.a = 1              
-            print(f"Initialization: a = {self.a}")
-            self.modify = Observable(observers=[
-                F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undefined')],
-            # (1) Switch off default activation
-                activate=Activation.NONE)(self.modify)
-
-        def modify(self, value=1):
-            self.a += value
-            print(f"Modification  : a = {self.a}")
-            # (2) Add individual dispatch
-            self.modify.observable.dispatch(value=self.a)
-    
-    # Case 2: Dynamic decoration, dynamic data
-    a = Actor()                     # Initialization: a = 1
-    a.modify(13)                    # Modification  : a = 14
-                                    # Informed value is: 14
-                                    # Reported value is: 14
+    from decoratory.observer import Observable
+
+    class Person:
+        def __init__(self, name: str = "Jane Doe"):
+            self.name = name
+            print(f"{name} arrived.")
+
+        @classmethod
+        def actionA(cls, act: str = "Hello?"):
+            print(f"Person says {act}")
+
+        def actionB(self, act: str = "Hello?"):
+            print(f"{self.name} says {act}")
+
+    @Observable(methods=["action1", "action2"],
+                observers=[Person.actionA, Person("Any Doe").actionB])
+    class Dog:
+        def __init__(self, name: str = "Teddy"):
+            self.name = name
+            print(f"Dog {name} arrived.")
+
+        @staticmethod
+        def action1(act: str = "Woof!"):
+            print(f"Dog acts {act}")
+
+        def action2(self, act: str = "Brrr!"):
+            print(f"{self.name} acts {act}")
+
+    # Case 4: Dog is an observable with selected actions.
+                                    # Any Doe arrived.
+    prs = Person()                  # Jane Doe arrived.
+    dog = Dog()                     # Dog Teddy arrived.
     
+    dog.action1()                   # Dog acts Woof!        (@staticmethod)
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+    Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
+                                    # Person says Hello?    (@classmethod)
+                                    # Any Doe says Hello?   (Instance 'Any')
+
+This last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
+first argument. This works because implicitly the *class method* ``Dog.action2`` 
+was registered. Therefore the call ``dog.action2`` fails because this 
+*instance method* was not registered. But, if this is what is to be achieved, 
+an instance method must first be created and registered, as above.
+
 
-Dynamic Class Decoration 
-------------------------
+Instance Decoration 
+-------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
 ``unregister`` methods that an observable exports. This way, information can 
 be given to the right recipients at the right places in the code. For this, 
-the classes are not decorated. The dynamic decoration comes into play. 
+the classes are not decorated. The `dynamic decoration <#dynamic-decoration>`_ 
+comes into play. 
 
 For this, the classes remain undecorated. Dynamic decoration is used, often 
 also in connection with getter/setter/property constructions, since data 
 changes take place meaningfully over these methods.
 
 Let's start with the simple classes:
 
 .. code-block:: python
 
-    # *** example_observer.py - daynamic class decoration
+    # *** example_observer.py - instance decoration
+
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
         def __init__(self, a=0):
             self._a = a
@@ -926,15 +1016,18 @@
             self._a = value
         a = property(get_a, set_a)
 
 Well, some typical actions might be:
 
 .. code-block:: python
 
-    # *** example_observer.py - daynamic class decoration
+    # *** example_observer.py - instance decoration
+
+    from decoratory.observer import Observable
+    from decoratory.basic import F
 
     # (1) Setup instances
     nti = Note()                    # Note instance
     thg = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
     thg.inc = Observable(thg.inc)           # Late method decoration   
@@ -958,20 +1051,35 @@
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
     thg.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
     # Case 5: Print the current value of thg.a
     print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
 
-
+    # Case 6: Print list of all observers
+    print(thg.inc.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}   
+    print(thg.set_a.observable.observers(classbased=True))
+    # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
+
+    # Case 7: Unregister nti.info from thg
+    thg.inc.observable.unregister(nti.info)
+    print(thg.inc.observable.observers(classbased=True))    # {}
+    
 
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.2.*, Build: 2023-06-18**
+
+- Intergration of unit tests for modules singleton, multiton and wrapper
+- An overall unit test for the package decoratory
+- Documentation enhancements for module observer, t.b.c.
+
 **Version: 0.1.1.*, Build: 2023-06-16**
 
 - Initial version of the observer, incl. documentation
 
 **Version: 0.1.0.3, Build: 2023-06-15**
 
 - accessible parameter for singleton and multiton, incl. documentation
@@ -982,14 +1090,16 @@
 - Documentation enhancements for for singleton, multiton and wrapper
 
 **Version: 0.1.0.1, Build: 2023-06-12**
 
 - Initial version with singleton, multiton and wrapper
 
 
+~~~ `contents <#toc>`_ ~~~ `singleton`_ ~~~ `multiton`_ ~~~ `wrapper`_ ~~~ `observer`_ ~~~
+
 .. ===========================================================================
 .. _project homepage: http://evation.eu
 .. _singleton pattern: https://en.wikipedia.org/wiki/Singleton_pattern
 .. _multiton pattern: https://en.wikipedia.org/wiki/Multiton_pattern
 .. _observer pattern: https://en.wikipedia.org/wiki/Observer_pattern
 .. _Decorator Arguments Pattern: http://evation.eu
```

### Comparing `decoratory-0.1.1.3/setup.py` & `decoratory-0.1.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.1.3"
-__date__ = "2023-06-16"
-__time__ = "20:01:41"
+__version__ = "0.1.2.3"
+__date__ = "2023-06-18"
+__time__ = "19:22:40"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -37,20 +37,23 @@
 
 with open("Requirements.txt", "r") as f:
     requirements = [str(req) for req in f.read().splitlines() if req]
 
 
 def version_check():
     """Keep versions in sync"""
-    # noinspection PyProtectedMember
-    from Sources.decoratory.__main__ import __version__ as version
-    assert version == __version__, (
-        f"\n\n{'':=^79s}\n"
-        f"{' Version mismatch: __main__.version != setup.version ':=^79s}\n"
-        f"{'':=^79s}")
+    try:
+        # noinspection PyProtectedMember
+        from Sources.decoratory.__main__ import __version__ as version
+        assert version == __version__, (
+            f"\n\n{'':=^79s}\n"
+            f"{' Version mismatch: __main__.version != setup.version ':=^79s}\n"
+            f"{'':=^79s}")
+    except (ModuleNotFoundError, ImportError):
+        pass  # Let the AssertionError pass...
 
 
 # -----------------------------------------------------------------------------
 # Excecute
 setupargs = dict(
     # General
     name=__title__,
@@ -96,15 +99,21 @@
     # Modules, Files and Data
     # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#finding-simple-packages
     packages=find_packages(where=src),
     package_dir={"": src},
     package_data={},
     py_modules=[],
     data_files=[(f"./lib/site-packages/{__title__}/data",
-                 ["License.txt", "Readme.rst", "Requirements.txt"])],
+                 ["License.txt", "Readme.rst", "Requirements.txt"]),
+                (f"./lib/site-packages/{__title__}/tests",
+                 ["Unittest/test_basic.py",
+                  "Unittest/test_singleton.py",
+                  "Unittest/test_multiton.py",
+                  "Unittest/test_wrapper.py",
+                  "Unittest/test_observer.py"])],
     entry_points={},
     # Dependencies
     python_requires='>=3.7',
     setup_requires=[],
     install_requires=requirements,
     # Post install
     # cmdclass={'install': CustomInstall},
```

