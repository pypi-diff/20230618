# Comparing `tmp/bfgdealer-0.0.5.tar.gz` & `tmp/bfgdealer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgdealer-0.0.5.tar", last modified: Thu May 11 08:39:16 2023, max compression
+gzip compressed data, was "bfgdealer-0.0.6.tar", last modified: Sun Jun 18 12:51:47 2023, max compression
```

## Comparing `bfgdealer-0.0.5.tar` & `bfgdealer-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.063919 bfgdealer-0.0.5/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.5/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      980 2023-05-11 08:39:16.063919 bfgdealer-0.0.5/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.5/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.057252 bfgdealer-0.0.5/bfgdealer/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.5/bfgdealer/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-11 08:37:22.000000 bfgdealer-0.0.5/bfgdealer/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.060586 bfgdealer-0.0.5/bfgdealer/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.5/bfgdealer/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    20266 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10586 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/dealer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    27456 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/dealer_duo.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.5/bfgdealer/source/dealer_engine.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14324 2023-05-05 16:12:36.000000 bfgdealer-0.0.5/bfgdealer/source/dealer_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:39:16.060586 bfgdealer-0.0.5/bfgdealer.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      980 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-11 08:39:15.000000 bfgdealer-0.0.5/bfgdealer.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-11 08:39:16.063919 bfgdealer-0.0.5/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.5/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.6/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1028 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.6/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.983348 bfgdealer-0.0.6/bfgdealer/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.6/bfgdealer/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-18 12:50:16.000000 bfgdealer-0.0.6/bfgdealer/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/bfgdealer/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.6/bfgdealer/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    20266 2023-05-05 16:12:36.000000 bfgdealer-0.0.6/bfgdealer/source/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    10586 2023-05-05 16:12:36.000000 bfgdealer-0.0.6/bfgdealer/source/dealer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    27873 2023-06-18 12:50:16.000000 bfgdealer-0.0.6/bfgdealer/source/dealer_duo.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.6/bfgdealer/source/dealer_engine.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14324 2023-05-05 16:12:36.000000 bfgdealer-0.0.6/bfgdealer/source/dealer_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.983348 bfgdealer-0.0.6/bfgdealer.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1028 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.6/setup.py
```

### Comparing `bfgdealer-0.0.5/LICENSE.txt` & `bfgdealer-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.5/PKG-INFO` & `bfgdealer-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.5
+Version: 0.0.6
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.6 18 Jun 2023
+
+1. Multi-2D
+
+------
+
 
 Version 0.0.5 11 May 2023
 
 1. Change __init__ to reflect set hand defn__
 
 ------
 Version 0.0.4 05 May 2023
```

### Comparing `bfgdealer-0.0.5/bfgdealer/__init__.py` & `bfgdealer-0.0.6/bfgdealer/__init__.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.5/bfgdealer/source/board.py` & `bfgdealer-0.0.6/bfgdealer/source/board.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.5/bfgdealer/source/dealer.py` & `bfgdealer-0.0.6/bfgdealer/source/dealer.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.5/bfgdealer/source/dealer_duo.py` & `bfgdealer-0.0.6/bfgdealer/source/dealer_duo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from termcolor import cprint
 
 from .dealer import Dealer as DealerBase
 from bridgeobjects import SEATS, BALANCED_SHAPES, SUITS, SHAPES
 
 MODULE_COLOUR = 'red'
 
+
 class Dealer(DealerBase):
     """Generate deals for Duo stages."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.set_hands = [
@@ -106,15 +107,15 @@
     def _get_benji_hand(self):
         selection = random.randint(0, 2)
         hand = None
         if selection == 2:
             return self.generate_hand([19, 20], BALANCED_SHAPES)
 
         while True:
-            hand = self.generate_hand([16,22], self.WEAK_TWO_SHAPES)
+            hand = self.generate_hand([16, 22], self.WEAK_TWO_SHAPES)
             if hand.suit_points(hand.longest_suit) >= 9:
                 if (hand.shape[0] != 6 and hand.aces < 2):
                     return hand
 
     def slam_potential_hand(self):
         """Deal a hand with slam potential."""
         found = False
@@ -651,30 +652,39 @@
                 }
             board = self.create_board(hands)
             board.dealer = self._dealer
             auction = self._generate_auction_calls(board)
 
             # Check first bid is valid
             if check_bid:
-                if auction[0].name  != 'P':
+                if auction[0].name != 'P':
                     continue
             if auction[check_bid].is_minor:
                 suit = auction[check_bid].denomination.name
                 if responders_hand.suit_holding[suit] >= 4:
                     found = True
         return board
 
     def multi_two_diamond(self):
-        # TODO ...
-        hand = self.generate_hand([20, 35])
+        """Return 19-20 balanced or weak 5/4."""
+        choice = random.randint(0, 1)
+        if choice == 0:
+            hand = self.generate_hand([19, 20], BALANCED_SHAPES)
+        else:
+            found = False
+            hand = None
+            while not found:
+                hand = self.generate_hand([6, 10])
+                if hand.spades >= 5 or hand.hearts >= 5:
+                    if hand.shape[0] == 5 and hand.shape[1] == 4:
+                        found = True
         hands = {self._first_seat(): hand}
         board = self.create_board(hands)
         return board
 
-
     def _opener_given_dealer(self, ns_opener):
         """Return the seat indices given dealer and opener orientation."""
         # E.g if we want N or S to bid and E is dealer then the opener will be S.
         # If on the other hand W is dealer, the opener will be N.
 
         # check_bid returns True (1) if N/S are to be opener and E/W are dealer
         # or if E/W are to be opener and N/S are dealer
```

### Comparing `bfgdealer-0.0.5/bfgdealer/source/dealer_engine.py` & `bfgdealer-0.0.6/bfgdealer/source/dealer_engine.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.5/bfgdealer/source/dealer_solo.py` & `bfgdealer-0.0.6/bfgdealer/source/dealer_solo.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.5/bfgdealer.egg-info/PKG-INFO` & `bfgdealer-0.0.6/bfgdealer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.5
+Version: 0.0.6
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.6 18 Jun 2023
+
+1. Multi-2D
+
+------
+
 
 Version 0.0.5 11 May 2023
 
 1. Change __init__ to reflect set hand defn__
 
 ------
 Version 0.0.4 05 May 2023
```

### Comparing `bfgdealer-0.0.5/setup.py` & `bfgdealer-0.0.6/setup.py`

 * *Files identical despite different names*

